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
translation-type: ht
source-git-commit: 4983e2e160b5cfb213e249f731e1858fab2cf972
workflow-type: ht
source-wordcount: '1516'
ht-degree: 100%

---


# Questions fréquentes {#frequently-asked-questions}

Les FAQ Brand Portal sont axées sur les questions et problèmes que les utilisateurs finaux peuvent avoir durant l’utilisation de la dernière version d’AEM Assets Brand Portal (la version 6.4.6) ou les versions antérieures.


## FAQ de Brand Portal 6.4.6 {#faqs-bp646}

**Question : Le point d’entrée OAuth hérité existant (`https://legacy-oauth.cloud.adobe.io/login`) ne fonctionne pas. Quelle pourrait en être la raison ?**

**Réponse :** La configuration OAuth héritée est obsolète. Vous devez mettre à niveau les instances d’auteur AEM Assets vers le dernier Service Pack et les configurer à l’aide d’Adobe Developer Console. Voir [Configuration d’AEM Assets avec Brand Portal](configure-aem-assets-with-brand-portal.md) pour plus de détails. Toutefois, pour que la configuration OAuth héritée fonctionne jusqu’à la mise à niveau, mettez à jour le point d’entrée OAuth hérité vers `https://hypnosisprod.ethos11-prod-or1.ethos.adobe.net/`.

<!--
**Ques. I have created a collection using the asset link shared by the administrator. But I am unable to create a share link for my collection. Do I need special permissions to do this?**

**Ans.** The functionality is by design, the viewer users are not permitted to share link for collections as they have limited privileges due to which they cannot add users to create a share link. It is a known issue that the share link for collections is currently visible to the viewer users. This issue will be fixed in the upcoming release, the option to share link for the collections will not be available to the viewer users.    
-->

**Question : Je ne suis pas en mesure de publier les ressources du dossier de contribution depuis Brand Portal vers AEM Assets après la mise à niveau vers Adobe Developer Console. Mon instance d’auteur se trouve sur AEM 6.5.4. Quelle peut en être la raison ?**

**Réponse :** Oui, un problème connu se produit lors de la publication des ressources du dossier de contribution dans AEM Assets sur AEM 6.5.4 via Adobe Developer Console.

Le problème a été corrigé dans AEM 6.5.5. Vous pouvez mettre à niveau votre instance AEM Assets vers le Service Pack le plus récent, AEM 6.5.5, et [mettre à niveau vos configurations](https://docs.adobe.com/content/help/fr-FR/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) sur Adobe Developer Console.

Pour une solution immédiate sur AEM 6.5.4, il est recommandé de [télécharger le correctif](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) et de l’installer sur votre instance d’auteur AEM.

**Question : Je ne vois pas le contenu du dossier de contribution publié sur AEM Assets à partir de Brand Portal. Quelle pourrait en être la raison ?**

**Réponse :** Contactez votre administrateur AEM Assets pour vérifier les configurations et vous assurer que votre client Brand Portal est configuré avec une seule instance d’auteur AEM Assets.

Ce problème peut se produire lorsque vous avez configuré un client Brand Portal sur plusieurs instances d’auteur AEM Assets. Par exemple, l’administrateur configure le même client Brand Portal sur l’instance d’auteur AEM Assets de l’environnement d’évaluation et de production. Dans ce cas, les déclencheurs de publication de ressources dans Brand Portal, mais l’instance d’auteur AEM Assets n’a pas pu importer la ressource, car l’agent de réplication ne reçoit pas le jeton de demande.


**Question : Je ne parviens pas à publier des ressources sur Brand Portal à partir d’AEM Assets. Le journal de réplication indique que la connexion a expiré. Y a-t-il une solution rapide ?**

**Réponse :** En règle générale, la tâche de publication échoue avec une erreur de délai d’expiration si plusieurs requêtes en attente se trouvent dans la file d’attente de réplication. Pour résoudre ce problème, assurez-vous que les agents de réplication sont configurés pour éviter l’expiration.

Effectuez les étapes suivantes pour configurer l’agent de réplication :
1. Connectez-vous à votre instance d’auteur AEM Assets.
1. Dans le panneau **Outils**, accédez à **[!UICONTROL Déploiement]** > **[!UICONTROL Réplication]**.
1. Sur la page Réplication, cliquez sur **[!UICONTROL Agents sur l’auteur]**. Vous voyez les quatre agents de réplication pour votre client Brand Portal.
1. Cliquez sur l’URL de l’agent de réplication pour ouvrir les détails le concernant.
1. Cliquez sur **[!UICONTROL Modifier]** pour modifier les paramètres de l’agent de réplication.
1. Dans Paramètres d’agent, cliquez sur l’onglet **[!UICONTROL Étendu]**.
1. Cochez la case **[!UICONTROL Fermer la connexion]**.
1. Répétez les étapes 4 à 7 pour configurer les quatre agents de réplication.
1. Redémarrez le serveur et vérifiez la connexion.


## FAQ de Brand Portal 6.4.5 {#faqs-bp645}

**Question : Quel changement majeur intervient dans la version 6.4.5 de Brand Portal ?**

**Réponse :** La version 6.4.5 d’AEM Assets Brand Portal dispose d’une fonctionnalité permettant aux utilisateurs Brand Portal de télécharger des contenus depuis l’instance Brand Portal et de republier le dossier Contribution dans AEM Assets sans avoir à demander de droits d’administrateur.
Pour plus d’informations, voir [Approvisionnement des ressources dans Brand Portal](brand-portal-asset-sourcing.md).



**Question : Est-ce que je n’aurai plus accès aux ressources et fonctionnalités existantes ou aux configurations que j’ai créées ?**

**Réponse :** Toutes les fonctionnalités et configurations existantes ne sont pas modifiées. Les utilisateurs finaux ne sont pas affectés. En outre, les contenus restent intacts.



**Question : Quand vais-je passer à la nouvelle version de Brand Portal ?**

**Réponse :** Brand Portal 6.4.5 est sorti en production en octobre 2019. La nouvelle version de Brand Portal devrait être commercialisée au troisième trimestre 2020.
Pour les mises à jour et les changements de versions, il est recommandé de suivre les [Notes de mise à jour](brand-portal-release-notes.md) et les [Nouveautés Brand Portal](whats-new.md).



**Question : Cela aura-t-il une incidence pour mes utilisateurs ?**

**Réponse :** La version 6.4.5 de Brand Portal est uniquement disponible dans cette application. Les utilisateurs finaux ne sont donc pas affectés.



**Question : Dois-je intervenir en tant qu’utilisateur Brand Portal ?**

**Réponse :** La version 6.4.5 de Brand Portal comprend une nouvelle fonctionnalité d’approvisionnement des ressources. L’administrateur AEM doit configurer la fonction d’approvisionnement des ressources dans AEM Assets, afin que les utilisateurs Brand Portal puissent l’activer. Pour plus d’informations, voir [Activation de la fonction d’approvisionnement des ressources](brand-portal-asset-sourcing.md).



**Question : Qui peut créer un dossier Contribution ?**

**Réponse :** Tout utilisateur AEM autorisé à créer un dossier dans AEM Assets peut créer un dossier **Contribution**. Pour créer un dossier **Contribution**, créez un dossier de type **Contribution des ressources**.
Ce dossier est partagé avec les utilisateurs Brand Portal actifs à des fins de contribution.



**Question : Que contient un dossier Contribution ?**

**Réponse : Un dossier** **Contribution** contient deux sous-dossiers, **NEW** et **SHARED**. Au départ, le dossier NEW est vide et le dossier SHARED comprend les contenus de référence (ressources réutilisables) destinés aux utilisateurs Brand Portal.
Ces utilisateurs accèdent au dossier **Contribution** et téléchargent le contenu dans le dossier **NEW**.



**Question :  Puis-je modifier le nom d’un dossier Contribution existant ?**

**Réponse :** **Non**, vous ne pouvez pas modifier le nom d’un dossier **Contribution** existant.



**Question : Quelles sont les exigences de ressources en matière de contribution ?**

**Réponse :** Le document **Brief** joint au dossier **Contribution** et les contenus de référence (ressources réutilisables) téléchargés dans le dossier **SHARED** permettent aux utilisateurs Brand Portal de bien comprendre la nécessité d’apporter leur contribution, ainsi que les attentes à prendre en compte en tant que contributeur. L’expression « exigences de ressources » désigne collectivement tous ces éléments.



**Question : Puis-je télécharger des ressources vers un dossier autorisé ?**

**Réponse :** Tous les dossiers ne sont pas autorisés. Les utilisateurs Brand Portal ne peuvent télécharger des contenus que vers le dossier **Contribution** partagé par l’administrateur AEM ou Brand Portal.



**Question : Comment accéder à un dossier Contribution ?**

**Réponse :** Vous pouvez accéder à un dossier **Contribution** seulement s’il est partagé avec vous. Vous recevez une notification push ou par courrier électronique lorsqu’un dossier Contribution est partagé avec vous. Vous pouvez accéder au dossier Contribution via le lien partagé disponible dans le courrier électronique ou vous connecter à l’instance Brand Portal, puis accéder à l’icône en forme de cloche pour recevoir une notification d’accès à ce dossier.

>[!NOTE]
>
>Si vous n’utilisez pas Brand Portal, demandez à l’administrateur AEM de vous créer un profil d’utilisateur dans la console d’administration AEM et de l’ajouter au fichier de configuration d’utilisateur de la liste d’utilisateurs Brand Portal.

**Question : Quel est le format du fichier CSV utilisé pour importer des utilisateurs ?**

**Réponse :** Ce format est identique à celui pris en charge par Admin Console pour importer des utilisateurs en vrac. Vous devez indiquer vos nom, prénom et adresse email.



**Question : Comment la liste d’utilisateurs (contributeurs Brand Portal) est-elle renseignée dans la liste déroulante d’utilisateurs de contributions des ressources ?**

**Réponse :** La liste d’utilisateurs est renseignée depuis le fichier de configuration d’utilisateur Brand Portal (.csv) téléchargé dans AEM.



**Question : Où consulter le statut des tâches d’importation et de publication ?**

**Réponse :** Dans AEM, vous pouvez consulter le statut des tâches sur la page des tâches **asynchrones**. Dans Brand Portal, vous pouvez consulter le statut d’une tâche de publication dans **[!UICONTROL Outils > Statut de contribution des ressources]**.



**Question : Quelle est la fréquence d’une tâche d’importation s’exécutant régulièrement dans AEM ?**

**Réponse :** Dans AEM, l’interrogation a lieu toutes les 5 minutes.



**Question : La fréquence de publication d’un dossier de Brand Portal vers AEM Assets est-elle limitée ?**

**Réponse :** Non, toutes les ressources du dossier **NEW** sont publiées dans AEM Assets, qu’elles aient ou non déjà été publiées. Lorsqu’un dossier **Contribution** est publié de Brand Portal vers AEM Assets, il remplace le contenu du dossier **NEW**.



**Question : Comment télécharger de nouvelles ressources dans un dossier Contribution ?**

**Réponse :** Voir la documentation détaillée correspondante pour savoir comment [télécharger des ressources vers le dossier Contribution](brand-portal-publish-contribution-folder-to-brand-portal.md).



**Question : Aucun aperçu ou vignette n’apparaît sur les ressources qu’un utilisateur Brand Portal a téléchargées vers le dossier NEW.**

**Réponse :** C’est tout à fait normal, car aucun workflow n’est exécuté au point d’extrémité Brand Portal.



**Question : Que se passe-t-il si un dossier utilisé dans ce processus est publié d’AEM Assets vers Brand Portal ?**

**Réponse :** Dans AEM, les journaux sont mis à jour pour chaque publication d’un dossier dans Brand Portal. Lors de la publication, toutes les ressources non publiées dans Brand Portal sont mises en file d’attente de copie. Les fichiers ajoutés au dossier une fois la tâche de publication déclenchée ne sont pas publiés dans Brand Portal. Lorsque l’utilisateur AEM republie le dossier, seules les ressources non publiées au préalable (et présentes dans la file d’attente de copie) le sont dans Brand Portal.
C’est le cas pour les dossiers publiés d’AEM Assets vers Brand Portal et pour le dossier SHARED d’un dossier Contribution.

**Question : Qui dois-je contacter en cas de questions ?**

**Réponse :** Contactez votre gestionnaire de compte ou le service à la clientèle Adobe.

>[!NOTE]
>
>Le calendrier des nouvelles versions est provisoire et susceptible d’être modifié. Contactez votre gestionnaire de compte ou le service clientèle Adobe pour obtenir le calendrier de version mis à jour.


## Assistance technique et accès au produit (sites à accès limité) {#product-access-and-support-restricted-sites}

Ces sites sont réservés aux clients. Si vous êtes client et avez besoin d’un accès, contactez votre responsable de compte Adobe.

* [](https://daycare.day.com) [Accès aux produits](https://login.marketing.adobe.com)

* [Assistance clientèle d’Adobe](https://helpx.adobe.com/fr/contact.html)
