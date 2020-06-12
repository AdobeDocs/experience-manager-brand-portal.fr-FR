---
title: Questions fréquentes
seo-title: null
description: Découvrez les questions fréquentes sur les ressources Adobe Experience Manager dans Brand Portal.
seo-description: null
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: frequently-asked-questions
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: 5bc5d8db777b31da82b7c68896d881c1fcdaed8f
workflow-type: tm+mt
source-wordcount: '1418'
ht-degree: 88%

---


# Questions fréquentes {#frequently-asked-questions}

Les FAQ Brand Portal sont axées sur les questions et problèmes que les utilisateurs finaux peuvent avoir durant l’utilisation de la dernière version d’AEM Assets Brand Portal (la version 6.4.6) ou les versions antérieures.


## FAQ de Brand Portal 6.4.6 {#faqs-bp646}

**Question Le point d’entrée OAuth hérité existant (`https://legacy-oauth.cloud.adobe.io/login`) ne fonctionne pas. Quelle pourrait en être la raison ?**

**Réponse** La configuration OAuth héritée est obsolète. Vous devez mettre à niveau les instances d’auteur AEM Assets vers le dernier Service Pack et les configurer à l’aide d’Adobe Developer Console. Voir [Configuration d’AEM Assets avec Brand Portal](configure-aem-assets-with-brand-portal.md) pour plus de détails. Toutefois, pour que la configuration OAuth héritée fonctionne jusqu’à la mise à niveau, mettez à jour le point d’entrée OAuth hérité vers `https://hypnosisprod.ethos11-prod-or1.ethos.adobe.net/`.

**Question Je ne suis pas en mesure de publier les ressources du dossier de contribution depuis Brand Portal vers AEM Assets après la mise à niveau vers Adobe Developer Console. Mon instance d’auteur se trouve sur AEM 6.5.4. Quelle peut en être la raison ?**

**Réponse** Oui, un problème connu se produit lors de la publication des ressources du dossier de contribution dans AEM Assets sur AEM 6.5.4 via Adobe Developer Console.

Ce problème a été corrigé dans AEM 6.5.5. Vous pouvez mettre à niveau votre instance AEM Assets vers le Service Pack le plus récent, AEM 6.5.5, et [mettre à niveau vos configurations](https://docs.adobe.com/content/help/fr-FR/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) sur Adobe Developer Console.

Pour une solution immédiate sur AEM 6.5.4, il est recommandé de [télécharger le correctif](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) et de l’installer sur votre instance d’auteur AEM.

**Question Je souhaite activer la fonction d’origine des ressources sur mon instance cloud AEM Assets. Comment puis-je le configurer ?**

**Réponse** Non, la fonction d’origine des ressources n’est actuellement pas prise en charge sur le service cloud AEM Assets.

Restez connecté et regardez les notes de mise à jour pour les notifications sur la disponibilité des fonctionnalités dans les prochaines versions.

**Question Je ne parviens pas à publier les ressources d’AEM Assets sur le portail de marque et le journal de l’agent de réplication lance une exception`java.net.SocketException: Connection timed out`. Y a-t-il une solution rapide ?**

**Réponse** S&#39;il existe un nombre de requêtes en attente dans la file d&#39;attente de réplication, il est possible que l&#39;agent de réplication ne traite pas la demande de publication d&#39;une ressource et lance une exception : `java.net.SocketException: Connection timed out`.

Effectuez les étapes suivantes pour résoudre le problème :

1. Ouvrez l&#39;agent de réplication et cliquez sur **[!UICONTROL Modifier]** pour modifier les paramètres de l&#39;agent de réplication.
1. Dans Paramètres de l&#39;agent, cliquez sur l&#39;onglet **[!UICONTROL Étendu]**.
1. Cochez la case **[!UICONTROL Fermer la connexion]**.
1. Redémarrez le lot de réplication (serveur).

Activez les paramètres sur les quatre agents de réplication pour éviter tout problème avec l&#39;agent de réplication.


## FAQ de Brand Portal 6.4.5 {#faqs-bp645}

**Question Quel changement majeur intervient dans la version 6.4.5 de Brand Portal ?**

**Réponse** La version 6.4.5 d’AEM Assets Brand Portal dispose d&#39;une fonctionnalité permettant aux utilisateurs Brand Portal de télécharger des contenus depuis l’instance Brand Portal et de republier le dossier Contribution dans AEM Assets sans avoir à demander de droits d’administrateur.
Pour plus d’informations, voir [Approvisionnement des ressources dans Brand Portal](brand-portal-asset-sourcing.md).



**Question Est-ce que je n’aurai plus accès aux ressources et fonctionnalités existantes ou aux configurations que j’ai créées ?**

**Réponse** Toutes les fonctionnalités et configurations existantes ne sont pas modifiées. Les utilisateurs finaux ne sont pas affectés. En outre, les contenus restent intacts.



**Question Quand vais-je passer à la nouvelle version de Brand Portal ?**

**Réponse** Brand Portal 6.4.5 est sorti en production en octobre 2019. La nouvelle version de Brand Portal devrait être commercialisée au troisième trimestre 2020.
Pour les mises à jour et les changements de versions, il est recommandé de suivre les [Notes de mise à jour](brand-portal-release-notes.md) et les [Nouveautés Brand Portal](whats-new.md).



**Question Cela aura-t-il une incidence pour mes utilisateurs ?**

**Réponse** La version 6.4.5 de Brand Portal est uniquement disponible dans cette application. Les utilisateurs finaux ne sont donc pas affectés.



**Question Dois-je intervenir en tant qu’utilisateur Brand Portal ?**

**Réponse** La version 6.4.5 de Brand Portal comprend une nouvelle fonctionnalité d&#39;approvisionnement des ressources. L’administrateur AEM doit configurer la fonction d’approvisionnement des ressources dans AEM Assets, afin que les utilisateurs Brand Portal puissent l&#39;activer. Pour plus d’informations, voir [Activation de la fonction d’approvisionnement des ressources](brand-portal-configure-asset-sourcing.md).



**Question Qui peut créer un dossier Contribution ?**

**Réponse** Tout utilisateur AEM autorisé à créer un dossier dans AEM Assets peut créer un dossier **Contribution**. Pour créer un dossier **Contribution**, créez un dossier de type **Contribution des ressources**.
Ce dossier est partagé avec les utilisateurs Brand Portal actifs à des fins de contribution.



**Question Que contient un dossier Contribution ?**

**RéponseUn dossier** **Contribution** contient deux sous-dossiers, **NEW** et **SHARED**. Au départ, le dossier NEW est vide et le dossier SHARED comprend les contenus de référence (ressources réutilisables) destinés aux utilisateurs Brand Portal.
Ces utilisateurs accèdent au dossier **Contribution** et téléchargent le contenu dans le dossier **NEW**.



**Question  Puis-je modifier le nom d’un dossier Contribution existant ?**

**Réponse** **Non**, vous ne pouvez pas modifier le nom d’un dossier **Contribution** existant.



**Question Quelles sont les exigences de ressources en matière de contribution ?**

**Réponse** Le document **Brief** joint au dossier **Contribution** et les contenus de référence (ressources réutilisables) téléchargés dans le dossier **SHARED** permettent aux utilisateurs Brand Portal de bien comprendre la nécessité d&#39;apporter leur contribution, ainsi que les attentes à prendre en compte en tant que contributeur. L’expression « exigences de ressources » désigne collectivement tous ces éléments.



**Question Puis-je télécharger des ressources vers un dossier autorisé ?**

**Réponse** Tous les dossiers ne sont pas autorisés. Les utilisateurs Brand Portal ne peuvent télécharger des contenus que vers le dossier **Contribution** partagé par l’administrateur AEM ou Brand Portal.



**Question Comment accéder à un dossier Contribution ?**

**Réponse** Vous pouvez accéder à un dossier **Contribution** seulement s&#39;il est partagé avec vous. Vous recevez une notification push ou par courrier électronique lorsqu’un dossier Contribution est partagé avec vous. Vous pouvez accéder au dossier Contribution via le lien partagé disponible dans le courrier électronique ou vous connecter à l’instance Brand Portal, puis accéder à l’icône en forme de cloche pour recevoir une notification d’accès à ce dossier.

>[!NOTE]
>
>Si vous n’utilisez pas Brand Portal, demandez à l’administrateur AEM de vous créer un profil d’utilisateur dans la console d’administration AEM et de l’ajouter au fichier de configuration d’utilisateur de la liste d’utilisateurs Brand Portal. Voir [Ajout d’un utilisateur Brand Portal](brand-portal-configure-asset-sourcing.md).




**Question Quel est le format du fichier CSV utilisé pour importer des utilisateurs ?**

**Réponse** Ce format est identique à celui pris en charge par Admin Console pour importer des utilisateurs en vrac. Vous devez indiquer vos nom, prénom et adresse électronique.



**Question Comment la liste d’utilisateurs (contributeurs Brand Portal) est-elle renseignée dans la liste déroulante d’utilisateurs de contributions des ressources ?**

**Réponse** La liste d’utilisateurs est renseignée depuis le fichier de configuration d’utilisateur Brand Portal (.csv) téléchargé dans AEM.



**Question Où consulter le statut des tâches d’importation et de publication ?**

**Réponse** Dans AEM, vous pouvez consulter le statut des tâches sur la page des tâches **asynchrones**. Dans Brand Portal, vous pouvez consulter le statut d&#39;une tâche de publication dans **[!UICONTROL Outils > Statut de contribution des ressources]**.



**Question Quelle est la fréquence d’une tâche d’importation s’exécutant régulièrement dans AEM ?**

**Réponse** Dans AEM, l’interrogation a lieu toutes les 5 minutes.



**Question La fréquence de publication d’un dossier de Brand Portal vers AEM Assets est-elle limitée ?**

**Réponse** Non, toutes les ressources du dossier **NEW** sont publiées dans AEM Assets, qu’elles aient ou non déjà été publiées. Lorsqu&#39;un dossier **Contribution** est publié de Brand Portal vers AEM Assets, il remplace le contenu du dossier **NEW**.



**Question Comment télécharger de nouvelles ressources dans un dossier Contribution ?**

**Réponse** Voir la documentation détaillée correspondante pour savoir comment [télécharger des ressources vers le dossier Contribution](brand-portal-upload-assets-to-contribution-folder.md).



**Question Aucun aperçu ou vignette n’apparaît sur les ressources qu&#39;un utilisateur Brand Portal a téléchargées vers le dossier NEW.**

**Réponse** C’est tout à fait normal, car aucun workflow n’est exécuté au point d’extrémité Brand Portal.



**Question Que se passe-t-il si un dossier utilisé dans ce processus est publié d’AEM Assets vers Brand Portal ?**

**Réponse** Dans AEM, les journaux sont mis à jour pour chaque publication d&#39;un dossier dans Brand Portal. Lors de la publication, toutes les ressources non publiées dans Brand Portal sont mises en file d&#39;attente de copie. Les fichiers ajoutés au dossier une fois la tâche de publication déclenchée ne sont pas publiés dans Brand Portal. Lorsque l’utilisateur AEM republie le dossier, seules les ressources non publiées au préalable (et présentes dans la file d’attente de copie) le sont dans Brand Portal.
C’est le cas pour les dossiers publiés d’AEM Assets vers Brand Portal et pour le dossier SHARED d’un dossier Contribution.



**Question Qui dois-je contacter en cas de questions ?**

**Réponse** Contactez votre gestionnaire de compte ou le service à la clientèle Adobe.


>[!NOTE]
>
>Le calendrier des nouvelles versions est provisoire et susceptible d’être modifié. Contactez votre gestionnaire de compte ou le service clientèle Adobe pour obtenir le calendrier de version mis à jour.




## Assistance technique et accès au produit (sites à accès limité) {#product-access-and-support-restricted-sites}

Ces sites sont réservés aux clients. Si vous êtes client et avez besoin d’un accès, contactez votre responsable de compte Adobe.

* [](https://daycare.day.com) [Accès aux produits](https://login.marketing.adobe.com)

* [Assistance clientèle d’Adobe](https://helpx.adobe.com/fr/contact.html)
