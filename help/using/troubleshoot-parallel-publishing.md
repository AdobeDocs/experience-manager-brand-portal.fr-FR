---
title: Dépannage des problèmes de publication en parallèle sur Brand Portal
seo-title: Dépannage des problèmes de publication en parallèle sur Brand Portal
description: Dépannez la publication en parallèle.
seo-description: Dépannez la publication en parallèle.
uuid: 51 e 45 cca -8 c 96-4 c 69-84 ef -2 ef 34 f 3 bcde 2
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
content-type: référence
topic-tags: brand-portal
discoiquuid: a 4801024-b 509-4 c 51-afd 8-e 337417 e 658 b
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Dépannage des problèmes de publication en parallèle sur Brand Portal {#troubleshoot-issues-in-parallel-publishing-to-brand-portal}

Le portail de marque prend en charge l'intégration à AEM Assets pour que les ressources approuvées soient facilement assimilées (ou publiées) à partir de l'instance d'auteur AEM Assets. Once [integrated](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html), AEM Author uses a replication agent to replicate the selected asset(s) to Brand Portal cloud service for approved usage by Brand Portal users. Les agents de réplication multiples sont utilisés AEM 6.2 SP 1-CFP 5], AEM CFP 6.3.0.2 et à partir de là pour permettre une publication parallèle à haut débit.

>[!NOTE]
>
>Adobe recommande d’effectuer une mise à niveau vers AEM 6.4.1.0 pour s’assurer qu’AEM Assets Brand Portal est correctement intégré à AEM Assets. Une limitation d'AEM 6.4 génère une erreur lors de la configuration de l'intégration avec le portail de marque et la réplication échoue.

Lors de la configuration du service Cloud pour le portail de marque sous [!UICONTROL /etc/cloudservice], tous les utilisateurs et jeton nécessaires sont générés automatiquement et enregistrés dans le référentiel. La configuration du service Cloud est créée, les utilisateurs de services requis pour la réplication et les agents de réplication pour répliquer le contenu sont également créés. Cela crée quatre agents de réplication. Ainsi, lorsque vous publiez plusieurs fichiers d'AEM vers Brand Portal, ceux-ci sont mis en file d'attente et distribués entre ces agents de réplication par le biais de Round Robin.

However, publishing can fail intermittently due to- large sling jobs, increased Network and [!UICONTROL Disk I/O] on AEM Author instance, or slowed performance of AEM Author instance. Il est donc conseillé de tester la connexion avec les agents de réplication avant de commencer la publication.

![](assets/test-connection.png)

## Troubleshoot failures in first time publishing: validating your publish configuration {#troubleshoot-failures-in-first-time-publishing-validating-your-publish-configuration}

Pour valider vos configurations de publication :

1. Vérifiez les journaux des erreurs.
2. Vérifiez si l’agent de réplication est créé.
3. Testez la connexion.

**Journaux de traîne lors de la création du service Cloud**

Vérifiez la fin des journaux. Vérifiez si l’agent de réplication est créé. Si la création de l’agent de réplication échoue, modifiez le service cloud en y apportant des modifications mineures. Validez et vérifiez à nouveau si l'agent de réplication est créé ou non. Si tel n’est pas le cas, modifiez à nouveau le service.

Si, lors de la modification répétée du service Cloud, il n'est pas configuré correctement, signalez un ticket de garderie.

**Test de la connexion aux agents de réplication**

Consultez le journal et si vous trouvez des erreurs dans le journal de réplication :

1. Contactez l'assistance Adobe.

2. Retry [clean-up](../using/troubleshoot-parallel-publishing.md#clean-up-existing-config) and create publish configuration again.

<!--
Comment Type: remark
Last Modified By: Mini Gulati (mgulati)
Last Modified Date: 2018-06-21T22:56:21.256-0400
<p>?? check and compare public key. At times public key is different</p>
<p>?? another thing to check in /useradmin</p>
-->

### Nettoyage des configurations de publication de Portal Portal existantes {#clean-up-existing-config}

Most of the times when publishing is not working, the reason can be that the user who is publishing (for example: [!UICONTROL mac-&lt;tenantid&gt;-replication]) doesn't have the latest private key, and hence publish fails with "401 unauthorized" error and no other error is reported in replication agent logs. Vous pouvez éviter de résoudre les problèmes et créer une nouvelle configuration. Pour que la nouvelle configuration fonctionne correctement, nettoyez les éléments suivants à partir de la configuration de l'auteur AEM :

1. accédez à [!UICONTROL localhost : 4502/crx/de] (si vous utilisez l'instance d'auteur sur [!UICONTROL localhost : 4502]) :\
   i. delete /etc/replication/agents.author/mp_replication *\
   ii. delete /etc/cloudservices/mediaportal/ &lt; nom_ config &gt;

2. accédez à [!UICONTROL localhost : 4502/useradmin]:\
   je recherche l'utilisateur [! UICONTROL Mac-&lt; tenantid &gt;-réplication
ii delete cet utilisateur

Le système est maintenant complètement nettoyé. Vous pouvez à présent essayer de créer une configuration  cloudservice  config and still use the already existing JWT application in [https://legacy-oauth.cloud.adobe.io/](https://legacy-oauth.cloud.adobe.io/). Il n’est pas nécessaire de créer une application ; seule la clé publique doit être mise à jour à partir de la configuration de cloud que vous venez de créer.

## Problème de visibilité des clients d’applications¬JWT sur Developer Connection {#developer-connection-jwt-application-tenant-visibility-issue}

Si, sur [https://legacy-oauth.cloud.adobe.io/](https://legacy-oauth.cloud.adobe.io/), toutes les instances (locataires) pour lesquelles les utilisateurs actuels sont hébergés par l'administrateur système sont répertoriées. Si vous n’y trouvez pas le nom de l’organisation ou si vous ne pouvez pas y créer d’application pour un client requis, vérifiez si vous possédez les droits suffisants (d’administrateur système) pour le faire.

Dans cette interface utilisateur, il existe un problème connu que, pour n'importe quel client, les 10 applications principales sont visibles. Quand vous créez l’application, restez sur cette page et marquez l’URL d’un signet. Il n'est pas nécessaire d'accéder à la page de liste de l'application et de trouver l'application que vous avez créée. Vous pouvez directement accéder à cette URL avec signets et mettre à jour/supprimer l'application chaque fois que cela est nécessaire.

L’application JWT pourrait ne pas être répertoriée convenablement. Il est donc conseillé de noter/marquer d’un signet l’URL lors de la création de l’application JWT.

## La configuration courante cesse de fonctionner {#running-configuration-stops-working}

<!--
Comment Type: draft

<p>If the running configuration stops working, either of the following two possibilities
<g class="gr_ gr_15 gr-alert gr_gramm gr_inline_cards gr_run_anim Grammar multiReplace" data-gr-id="15" id="15" style="font-size: 12px;">
are
</g> there:</p>
<p>1.
<g class="gr_ gr_14 gr-alert gr_gramm gr_inline_cards gr_run_anim Grammar only-ins doubleReplace replaceWithoutSep" data-gr-id="14" id="14">
Connection
</g> has failed, or</p>
<p>2. Publish has failed with permission to dam-replication-service denied, while connection has passed </p>
<p>If the connection has failed [1], the
<g class="gr_ gr_10 gr-alert gr_spell gr_inline_cards gr_run_anim ContextualSpelling ins-del multiReplace" data-gr-id="10" id="10">
fail safe
</g> way to fix it is to <a href="../using/troubleshoot-parallel-publishing.md#main-pars-header-1664955658">clean up</a> the existing Brand Portal publish configuration and recreate a publish configuration. </p>
<p>However, if the
<g class="gr_ gr_18 gr-alert gr_spell gr_inline_cards gr_run_anim ContextualSpelling" data-gr-id="18" id="18">
publish
</g> has failed with
<g class="gr_ gr_16 gr-alert gr_gramm gr_inline_cards gr_run_anim Grammar only-ins doubleReplace replaceWithoutSep" data-gr-id="16" id="16">
permission
</g> denied to dam-replication-service, raise a support ticket.</p>
-->

Si un agent de réplication (qui publiait correctement sur Brand Portal) cesse de traiter les tâches de publication, vérifiez les journaux de réplication. AEM intègre une fonction de réessai automatique qui permet de retenter automatiquement la publication d’une ressource particulière suite à un échec. En cas de problème intermittent comme une erreur réseau, la publication peut réussir lors de la nouvelle tentative.

En cas d'échec de publication et d'échec de la publication en continu, vous devez vérifier **[!UICONTROL la connexion des tests]** et essayer de résoudre les erreurs qui sont rapportées.

En fonction des erreurs, nous vous conseillons de soumettre un ticket d’assistance, de sorte que l’équipe d’ingénierie de Brand Portal puisse vous aider à résoudre les problèmes.
