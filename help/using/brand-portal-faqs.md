---
title: Questions fréquentes
description: Découvrez les questions fréquentes sur les ressources Adobe Experience Manager dans Brand Portal.
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: frequently-asked-questions
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
exl-id: 4a8f7fbd-7485-421d-a8db-755324d2dbef
source-git-commit: 32a67abf466dd3bf635b851b02377ed23591915e
workflow-type: ht
source-wordcount: '1500'
ht-degree: 100%

---

# Questions fréquentes {#frequently-asked-questions}

Les questions fréquentes relatives à Brand Portal sont axées sur les questions et problèmes que les utilisateurs et utilisatrices finaux peuvent avoir durant l’utilisation de la dernière version d’Experience Manager Assets Brand Portal 6.4.6 ou versions antérieures.


## Questions fréquentes relatives à Brand Portal 6.4.6 {#faqs-bp646}

**Question : le point d’entrée OAuth hérité existant (`https://legacy-oauth.cloud.adobe.io/login`) ne fonctionne pas. Quelle pourrait en être la raison ?**

**Réponse :** la configuration OAuth héritée est obsolète. Mettez à niveau les instances de création Experience Manager Assets vers le dernier pack de services et configurez-les à l’aide d’Adobe Developer Console. Voir [Configuration d’Experience Manager Assets avec Brand Portal](configure-aem-assets-with-brand-portal.md) pour plus de détails. Toutefois, pour que la configuration OAuth héritée fonctionne jusqu’à la mise à niveau, mettez à jour le point d’entrée OAuth hérité vers `https://hypnosisprod.ethos11-prod-or1.ethos.adobe.net/`.

**Question : je ne peux pas publier les ressources du dossier de contribution depuis Brand Portal vers Experience Manager Assets après la mise à niveau vers Adobe Developer Console. Mon instance de création se trouve sur Experience Manager Assets 6.5.4. Quelle peut en être la raison ?**

**Réponse :** oui, un problème connu se produit lors de la publication des ressources du dossier de contribution dans Experience Manager Assets 6.5.4 via Adobe Developer Console.

Le problème a été corrigé dans la version 6.5.5 d’Experience Manager Assets. Vous pouvez mettre à niveau votre instance Experience Manager Assets vers le pack de services le plus récent et [mettre à niveau vos configurations](https://experienceleague.adobe.com/fr/docs/experience-manager-65/content/assets/brandportal/configure-aem-assets-with-brand-portal#upgrade-integration-65) sur Adobe Developer Console.


**Question : je ne vois pas le contenu du dossier de contribution publié sur Experience Manager Assets à partir de Brand Portal. Quelle pourrait en être la raison ?**

**Réponse :** contactez votre administrateur ou administratrice Experience Manager Assets pour vérifier les configurations et vous assurer que votre client ou cliente Brand Portal a une configuration avec une seule instance de création Experience Manager Assets.

Ce problème peut se produire lorsque vous avez configuré un client ou une cliente Brand Portal sur plusieurs instances de création Experience Manager Assets. Par exemple, l’administrateur ou l’administratrice configure le même client ou la même cliente Brand Portal sur l’instance de création Experience Manager Assets dans une environnement d’évaluation et de production. Dans ce cas, la publication de ressource se déclenche dans Brand Portal, mais l’instance de création Experience Manager Assets n’a pas pu importer la ressource, car l’agent de réplication ne reçoit pas le jeton de demande.


**Question : je ne parviens pas à publier des ressources sur Brand Portal à partir d’Experience Manager Assets. Le journal de réplication indique que la connexion a expiré. Y a-t-il une solution rapide ?**

**Réponse :** en règle générale, la publication échoue avec une erreur de délai d’expiration si plusieurs requêtes en attente se trouvent dans la file d’attente de réplication. Pour résoudre ce problème, assurez-vous que les agents de réplication sont configurés pour éviter l’expiration.

Effectuez les étapes suivantes pour configurer l’agent de réplication :

1. Connectez-vous à votre instance d’auteur Experience Manager Assets.
1. Dans le panneau **Outils**, accédez à **[!UICONTROL Déploiement]** > **[!UICONTROL Réplication]**.
1. Sur la page Réplication, cliquez sur **[!UICONTROL `Agents on author`]**. Vous voyez les quatre agents de réplication pour votre client Brand Portal.
1. Cliquez sur l’URL de l’agent de réplication pour ouvrir les détails le concernant.
1. Cliquez sur **[!UICONTROL Modifier]** pour modifier les paramètres de l’agent de réplication.
1. Dans les Paramètres d’agent, cliquez sur l’onglet **[!UICONTROL Étendu]**.
1. Cochez la case **[!UICONTROL Fermer la connexion]**.
1. Répétez les étapes 4 à 7 pour configurer les quatre agents de réplication.
1. Redémarrez le serveur et vérifiez la connexion.


## FAQ de Brand Portal 6.4.5  {#faqs-bp645}

**Question : quel changement majeur intervient dans la version 6.4.5 de Brand Portal ?**

**Réponse :** Experience Manager Assets Brand Portal 6.4.5 permet aux utilisateurs et utilisatrices de charger du contenu et de republier le dossier Contribution dans Experience Manager Assets directement depuis Brand Portal, sans avoir besoin de droits d’administration. Pour plus d’informations, consultez [Approvisionnement des ressources dans Brand Portal](brand-portal-asset-sourcing.md).



**Question : ai-je perdu l’accès aux ressources et fonctionnalités existantes ou aux configurations que j’ai créées ?**

**Réponse :** toutes les fonctionnalités et configurations existantes demeurent intactes. Les utilisateurs et utilisatrices finaux ne sont pas affectés. En outre, les contenus restent intacts.



**Question : quand vais-je passer à la nouvelle version de Brand Portal ?**

**Réponse :** la version de Brand Portal 6.4.5 est sortie en production en octobre 2019. La prochaine version de Brand Portal est prévue pour mars 2020.
Pour les mises à jour et les changements de versions, Adobe vous recommande de suivre les [Notes de mise à jour](brand-portal-release-notes.md) et les [Nouveautés de Brand Portal](whats-new.md).



**Question : y a-t-il un impact pour mes utilisateurs et utilisatrices ?**

**Réponse :** la version 6.4.5 de Brand Portal est uniquement disponible dans cette application. Il n’y a donc pas d’impact sur les utilisateurs finaux et les utilisatrices finales.



**Question : dois-je intervenir en tant qu’utilisateur ou utilisatrice Brand Portal ?**

**Réponse :** la version 6.4.5 de Brand Portal comprend une nouvelle fonctionnalité d’approvisionnement des ressources. L’administrateur ou administratrice doit configurer la fonction d’approvisionnement des ressources dans Experience Manager Assets afin d’activer la fonctionnalité pour les utilisateurs et utilisatrices de Brand Portal. Pour plus d’informations, consultez [Activation de la fonction d’approvisionnement des ressources](brand-portal-asset-sourcing.md).



**Question : qui peut créer un dossier Contribution ?**

**Réponse :** tout utilisateur ou toute utilisatrice d’Experience Manager Assets disposant de l’autorisation de créer un dossier dans Experience Manager Assets peut créer un dossier **Contribution**. Pour créer un dossier **Contribution**, créez un dossier de type **Contribution des ressources**.
Ce dossier est partagé avec les utilisateurs et utilisatrices Brand Portal actifs à des fins de contribution.



**Question : que contient un dossier Contribution ?**

**Réponse :** le dossier **Contribution** contient deux sous-dossiers :**NEW** et **SHARED**. Au départ, le dossier NEW est vide et le dossier SHARED comprend les contenus de référence (ressources réutilisables) destinés aux utilisateurs Brand Portal.
Ces utilisateurs accèdent au dossier **Contribution** et téléchargent le contenu dans le dossier **NEW**.



**Question : puis-je modifier le nom d’un dossier Contribution existant ?**

**Réponse :** **non**, vous ne pouvez pas modifier le nom d’un dossier **Contribution** existant.



**Question : quelles sont les exigences de ressources en matière de contribution ?**

**Réponse :** le document **Brief** du dossier **Contribution** et le contenu de référence du dossier **SHARED** aident les utilisateurs et utilisatrices de Brand Portal à comprendre les besoins et les attentes en matière de contribution. Ensemble, ils sont appelés exigences en matière de ressources.

**Question : puis-je charger des ressources vers un dossier autorisé ?**

**Réponse :** pas tous les dossiers autorisés. Un utilisateur et ou une utilisatrice de Brand Portal ne peut charger du contenu que vers le dossier **Contribution** partagé par l’administrateur ou administratrice Experience Manager Assets ou Brand Portal.



**Question : comment accéder à un dossier Contribution ?**

**Réponse :** vous pouvez accéder à un dossier **Contribution** seulement s’il est partagé avec vous. Vous recevez une notification push ou par e-mail lorsqu’un dossier Contribution est partagé avec vous. Vous pouvez accéder au dossier Contribution par le biais du lien partagé dans l’e-mail. Vous pouvez également vous connecter à votre instance Brand Portal et cliquer sur l’icône de cloche des notifications pour accéder au dossier Contribution.

>[!NOTE]
>
>Si vous n’êtes pas un utilisateur ou une utilisatrice de Brand Portal, demandez à l’administrateur ou à l’administratrice d’Experience Manager Assets de créer votre profil dans Admin Console. Ajoutez ensuite votre profil au fichier de configuration utilisateur dans la liste des utilisateurs et utilisatrices de Brand Portal.


**Question : quel est le format du fichier CSV utilisé pour importer des utilisateurs et utilisatrices ?**

**Réponse :** le format correspond à celui pris en charge par Admin Console pour l’import d’utilisateurs et utilisatrices en masse. Vous devez indiquer vos nom, prénom et adresse e-mail.



**Question : comment la liste des utilisateurs et utilisatrices (contributeurs et contributrices Brand Portal) est-elle renseignée dans la liste déroulante des utilisateurs et utilisatrices des contributions des ressources ?**

**Réponse :** la liste des utilisateurs et utilisatrices est renseignée depuis le fichier de configuration utilisateur Brand Portal (.csv) chargé dans Experience Manager Assets.



**Question : où consulter le statut des traitements d’import et de publication ?**

**Réponse :** dans Experience Manager Assets, vous pouvez consulter le statut d’un import sur la page des traitements **asynchrones**. Dans Brand Portal, vous pouvez consulter le statut d’un traitement de publication dans **[!UICONTROL Outils > Statut de contribution des ressources]**.



**Question : quelle est la fréquence d’un traitement d’import s’exécutant régulièrement dans Experience Manager ?**

**Réponse :** dans Experience Manager Assets, l’interrogation a lieu toutes les 5 minutes.



**Question : la fréquence de publication d’un dossier de Brand Portal vers Experience Manager Assets est-elle limitée ?**

**Réponse :** non, toutes les ressources du dossier **NEW** sont publiées dans Experience Manager Assets, qu’elles aient ou non déjà été publiées. Lorsqu’un dossier **Contribution** est publié de Brand Portal vers Experience Manager Assets, il remplace le contenu du dossier **NEW**.



**Question : comment charger de nouvelles ressources dans un dossier Contribution ?**

**Réponse :** consultez la documentation détaillée pour savoir comment [harger des ressources vers le dossier Contribution](brand-portal-publish-contribution-folder-to-brand-portal.md).



**Question : je ne peux pas voir les miniatures ou les prévisualisations des ressources chargées dans le dossier NEW.**

**Réponse :** c’est tout à fait normal, car aucun workflow n’est exécuté au point d’extrémité Brand Portal.



**Question : que se passe-t-il si un dossier en flux est publié d’Experience Manager Assets vers Brand Portal ?**

**Réponse :** dans Experience Manager Assets, les journaux sont mis à jour pour chaque publication d’un dossier dans Brand Portal. Lors de la publication, toutes les ressources non publiées dans Brand Portal sont ajoutées à la file d’attente de réplication. Les fichiers ajoutés au dossier une fois le traitement de publication déclenché ne sont pas publiés dans Brand Portal. Lorsque un utilisateur ou une utilisatrice Experience Manager Assets republie le dossier, seules les ressources non publiées au préalable (et présentes dans la file d’attente de réplication) sont publiées dans Brand Portal. Ce processus s’applique aux dossiers publiés d’Experience Manager Assets vers Brand Portal et pour le dossier SHARED d’un dossier Contribution.

**Question : qui dois-je contacter en cas de questions ?**

**Réponse :** contactez votre gestionnaire de compte Adobe ou le service clientèle.

>[!NOTE]
>
>Le calendrier de publication est provisoire et susceptible d’être modifié. Contactez votre gestionnaire de compte Adobe ou le service clientèle pour obtenir le calendrier de publication mis à jour.


## Assistance technique et accès au produit (sites à accès limité) {#product-access-and-support-restricted-sites}

Ces sites sont réservés aux clientes et clients. Si vous êtes client ou cliente et avez besoin d’un accès, contactez votre gestionnaire de compte Adobe.

<!--
* [](https://daycare.day.com) [Product Access](https://login.marketing.adobe.com)

* [Adobe Customer Support]()
-->
