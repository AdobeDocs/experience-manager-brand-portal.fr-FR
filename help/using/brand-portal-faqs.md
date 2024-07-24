---
title: Questions fréquentes
description: Découvrez les questions fréquentes sur les ressources Adobe Experience Manager dans Brand Portal.
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: frequently-asked-questions
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
exl-id: 4a8f7fbd-7485-421d-a8db-755324d2dbef
source-git-commit: 60104481e8f0b883fbf2cf25c1562e8376882e54
workflow-type: tm+mt
source-wordcount: '1495'
ht-degree: 24%

---

# Questions fréquentes {#frequently-asked-questions}

Les questions fréquentes de Brand Portal se concentrent sur les questions et problèmes que les utilisateurs finaux peuvent rencontrer lorsqu’ils travaillent avec la dernière version de Experience Manager Assets Brand Portal 6.4.6 ou des versions antérieures.


## FAQ de Brand Portal 6.4.6  {#faqs-bp646}

**Question : le point d’entrée OAuth hérité existant (`https://legacy-oauth.cloud.adobe.io/login`) ne fonctionne pas. Quelle pourrait en être la raison ?**

**Réponse :** La configuration OAuth héritée est obsolète. Mettez à niveau les instances d’auteur Experience Manager Assets vers le dernier Service Pack et configurez-les via Adobe Developer Console. Voir [Configuration d’Experience Manager Assets avec Brand Portal](configure-aem-assets-with-brand-portal.md) pour plus de détails. Toutefois, pour que la configuration OAuth héritée fonctionne jusqu’à la mise à niveau, mettez à jour le point d’entrée OAuth hérité vers `https://hypnosisprod.ethos11-prod-or1.ethos.adobe.net/`.

**Question : Je ne suis pas en mesure de publier les ressources du dossier de contribution de Brand Portal vers Experience Manager Assets après la mise à niveau vers Adobe Developer Console. Mon instance d’auteur se trouve sur Experience Manager Assets 6.5.4. Quelle peut en être la raison ?**

**Réponse :** Oui, il existe un problème connu lors de la publication des ressources du dossier de contribution vers Experience Manager Assets 6.5.4 via Adobe Developer Console.

Le problème a été corrigé dans la version 6.5.5 d’Experience Manager Assets. Vous pouvez mettre à niveau votre instance Experience Manager Assets vers le Service Pack le plus récent et [mettre à niveau vos configurations](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/brandportal/configure-aem-assets-with-brand-portal#upgrade-integration-65) sur Adobe Developer Console.


**Question : Je ne vois pas le contenu du dossier de contribution publié à partir de Brand Portal dans Experience Manager Assets. Quelle pourrait en être la raison ?**

**Réponse :** Contactez votre administrateur Experience Manager Assets pour vérifier les configurations et vous assurer que votre client Brand Portal est configuré avec une seule instance d’auteur Experience Manager Assets.

Ce problème peut se produire lorsque vous avez configuré un client Brand Portal sur plusieurs instances d’auteur Experience Manager Assets. Par exemple, l’administrateur configure le même client Brand Portal sur l’instance d’auteur Experience Manager Assets d’un environnement d’évaluation et de production. Dans ce cas, la publication des ressources se déclenche dans Brand Portal, mais l’instance d’auteur Experience Manager Assets ne parvient pas à importer la ressource, car l’agent de réplication ne reçoit pas le jeton de demande.


**Question : Je ne parviens pas à publier des ressources de Experience Manager Assets vers Brand Portal. Le journal de réplication indique que la connexion a expiré. Y a-t-il une solution rapide ?**

**Réponse :** En règle générale, la publication échoue avec une erreur de délai d’expiration si plusieurs requêtes en attente se trouvent dans la file d’attente de réplication. Pour résoudre ce problème, assurez-vous que les agents de réplication sont configurés pour éviter l’expiration.

Effectuez les étapes suivantes pour configurer l’agent de réplication :

1. Connectez-vous à votre instance d’auteur Experience Manager Assets.
1. Dans le panneau **Outils**, accédez à **[!UICONTROL Déploiement]** > **[!UICONTROL Réplication]**.
1. Dans la page Réplication, cliquez sur **[!UICONTROL `Agents on author`]**. Vous voyez les quatre agents de réplication pour votre client Brand Portal.
1. Cliquez sur l’URL de l’agent de réplication pour ouvrir les détails le concernant.
1. Cliquez sur **[!UICONTROL Modifier]** pour modifier les paramètres de l’agent de réplication.
1. Dans les paramètres de l’agent, cliquez sur l’onglet **[!UICONTROL Extended]** .
1. Cochez la case **[!UICONTROL Fermer la connexion]**.
1. Répétez les étapes 4 à 7 pour configurer les quatre agents de réplication.
1. Redémarrez le serveur et vérifiez la connexion.


## FAQ de Brand Portal 6.4.5  {#faqs-bp645}

**Question : Quelle est la modification majeure de la version 6.4.5 de Brand Portal ?**

**Réponse :** Experience Manager Assets Brand Portal 6.4.5 permet aux utilisateurs de charger du contenu et de publier à nouveau le dossier Contribution dans Experience Manager Assets directement depuis Brand Portal, sans avoir à demander de droits d’administrateur. Pour plus d’informations, voir [Approvisionnement des ressources dans Brand Portal](brand-portal-asset-sourcing.md).



**Question : Ai-je perdu l’accès à des ressources, fonctionnalités ou configurations existantes que j’ai créées ?**

**Réponse :** Toutes vos fonctionnalités et configurations existantes restent intactes. Les utilisateurs finaux ne sont pas affectés. En outre, les contenus restent intacts.



**Question : Quand vais-je passer à la nouvelle version de Brand Portal ?**

**Réponse :** Brand Portal 6.4.5 a été publié en production en octobre 2019. La prochaine version de Brand Portal est attendue pour mars 2020.
Pour les mises à jour et les modifications de version, Adobe vous recommande de suivre les [Notes de mise à jour](brand-portal-release-notes.md) et les [Nouveautés de Brand Portal](whats-new.md).



**Question : Mes utilisateurs sont-ils affectés ?**

**Réponse :** La version 6.4.5 de Brand Portal est uniquement disponible dans Brand Portal, de sorte qu’il n’y a aucun impact pour vos utilisateurs finaux.



**Question : Existe-t-il une action requise de ma part en tant qu’utilisateur Brand Portal ?**

**Réponse :** La version 6.4.5 de Brand Portal comprend une nouvelle fonctionnalité d’approvisionnement des ressources. L’administrateur doit configurer la fonctionnalité d’approvisionnement des ressources dans Experience Manager Assets pour l’activer pour les utilisateurs de Brand Portal. Pour plus d’informations, voir [Activation de la fonction d’approvisionnement des ressources](brand-portal-asset-sourcing.md).



**Question : Qui peut créer un dossier Contribution ?**

**Réponse :** Tout utilisateur de Experience Manager Assets autorisé à créer un dossier dans Experience Manager Assets peut créer un dossier **Contribution**. Pour créer un dossier **Contribution**, créez un dossier de type **Contribution des ressources**.
Ce dossier est partagé avec les utilisateurs Brand Portal actifs à des fins de contribution.



**Question : Que contient un dossier Contribution ?**

**Réponse :** **Le dossier Contribution** contient deux sous-dossiers **NEW** et **SHARED**. Au départ, le dossier NEW est vide et le dossier SHARED comprend les contenus de référence (ressources réutilisables) destinés aux utilisateurs Brand Portal.
Ces utilisateurs accèdent au dossier **Contribution** et téléchargent le contenu dans le dossier **NEW**.



**Question : Puis-je modifier le nom d’un dossier Contribution existant ?**

**Réponse :** **Non**, vous ne pouvez pas modifier le nom d’un dossier **Contribution** existant.



**Question : Quelles sont les exigences en matière de ressources avec contribution ?**

**Réponse :** Le document **Brief** du dossier **Contribution** et le contenu de référence du dossier **SHARED** aident les utilisateurs de Brand Portal à comprendre les attentes et les besoins en matière de contribution. Ensemble, elles sont connues sous le nom d’exigences en matière de ressources.

**Question : Puis-je télécharger des ressources dans un dossier autorisé ?**

**Réponse :** Tous les dossiers ne sont pas autorisés. Un utilisateur de Brand Portal peut charger du contenu uniquement vers le dossier **Contribution** partagé par l’administrateur Experience Manager Assets ou Brand Portal.



**Question : Comment puis-je accéder à un dossier Contribution ?**

**Réponse :** Vous ne pouvez accéder à un dossier **Contribution** que s’il a été partagé avec vous. Vous recevez une notification Push/par courrier électronique chaque fois qu’un dossier Contribution est partagé avec vous. Vous pouvez accéder au dossier Contribution au moyen du lien partagé dans le courrier électronique. Vous pouvez également vous connecter à votre instance Brand Portal et accéder à l’icône représentant une cloche pour que les notifications accèdent au dossier Contribution.

>[!NOTE]
>
>Si vous n’êtes pas un utilisateur Brand Portal, demandez à l’administrateur Experience Manager Assets de créer votre utilisateur dans l’Admin Console. Ajoutez ensuite votre profil au fichier de configuration utilisateur de la liste des utilisateurs de Brand Portal.


**Question : Quel est le format du fichier CSV pour l’importation des utilisateurs ?**

**Réponse :** Le format correspond à ce que l’Admin Console prend en charge pour l’importation en masse d’utilisateurs. Vous devez indiquer vos nom, prénom et adresse e-mail.



**Question : Qu’est-ce qui remplit la liste des utilisateurs (contributeurs Brand Portal) dans la liste déroulante des utilisateurs de contribution des ressources ?**

**Réponse :** Les utilisateurs de la liste déroulante sont renseignés à partir du fichier de configuration d’utilisateur Brand Portal (.csv) téléchargé dans Experience Manager Assets.



**Question : Où puis-je voir l’état des tâches d’importation et de publication ?**

**Réponse :** Dans Experience Manager Assets, vous pouvez voir l’état d’un import dans la page de tâche **async**. Dans Brand Portal, vous pouvez consulter le statut d’une tâche de publication dans **[!UICONTROL Outils > Statut de contribution des ressources]**.



**Question : Quelle est la fréquence d&#39;une tâche d&#39;import qui s&#39;exécute régulièrement en Experience Manager ?**

**Réponse :** Dans Experience Manager Assets, l’interrogation a lieu toutes les 5 minutes.



**Question : Existe-t-il un seuil au nombre de fois qu’un dossier peut être publié de Brand Portal vers Experience Manager Assets ?**

**Réponse :** Non, toutes les ressources du dossier **NEW** sont publiées sur Experience Manager Assets, indépendamment du fait qu’elles aient été publiées précédemment. Chaque fois qu’un dossier **Contribution** est publié de Brand Portal vers Experience Manager Assets, il remplace le contenu du dossier **NEW**.



**Question : Comment télécharger de nouvelles ressources dans un dossier Contribution ?**

**Réponse :** Reportez-vous à la documentation détaillée pour [Téléchargement de ressources dans le dossier Contribution](brand-portal-publish-contribution-folder-to-brand-portal.md).



**Question : je ne vois pas de miniatures ni d’aperçus pour les ressources chargées dans le dossier NEW.**

**Réponse :** Il est conçu comme prévu, car aucun workflow n’est exécuté à la fin de Brand Portal.



**Question : Que se passe-t-il si un dossier est publié de Experience Manager Assets vers Brand Portal en flux continu ?**

**Réponse :** Dans Experience Manager Assets, les journaux sont conservés pour chaque publication d’un dossier sur Brand Portal. Au moment de la publication, toutes les ressources qui ne sont pas publiées sur Brand Portal sont ajoutées à une file d’attente de réplication. Les fichiers ajoutés au dossier une fois la tâche de publication déclenchée ne sont pas publiés dans Brand Portal. Lorsqu’un utilisateur Experience Manager Assets republie le dossier, seules les ressources qui n’ont pas été publiées précédemment (qui se trouvent dans la file d’attente de réplication) sont publiées sur Brand Portal. Ce processus s’applique à tous les dossiers publiés de Experience Manager Assets vers Brand Portal et au dossier SHARED d’un dossier Contribution.

**Question : Qui dois-je contacter pour toute question ?**

**Réponse :** Contactez votre gestionnaire de compte d’Adobe ou le service clientèle.

>[!NOTE]
>
>Le calendrier des versions est provisoire et susceptible d’être modifié. Contactez votre gestionnaire de compte d’Adobe ou le service clientèle pour obtenir le calendrier de mise à jour.


## Assistance technique et accès au produit (sites à accès limité) {#product-access-and-support-restricted-sites}

Ces sites sont réservés aux clients. Si vous êtes client et avez besoin d’un accès, contactez votre gestionnaire de compte d’Adobe.

<!--
* [](https://daycare.day.com) [Product Access](https://login.marketing.adobe.com)

* [Adobe Customer Support]()
-->
