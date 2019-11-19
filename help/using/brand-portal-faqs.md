---
title: Questions fréquentes
seo-title: null
description: Découvrez les questions fréquentes sur le portail des ressources d’Adobe Experience Manager.
seo-description: null
uuid: null
content-type: reference
topic-tags: frequently-asked-questions
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: f8d95ab1e1c17ef2cf86d0206a36134996e4fe07

---


# Questions fréquentes {#frequently-asked-questions}

Les FAQ du portail de marque se concentrent sur les questions et problèmes que les utilisateurs finaux peuvent rencontrer lors de l’utilisation de la dernière version du portail de marque AEM Assets 6.4.5 ou des versions antérieures.



**Question Quel est le changement majeur dans la version 6.4.5 de Brand Portal ?**

**Rép.** AEM Assets Brand Portal 6.4.5 est une version de fonctionnalité qui permet aux utilisateurs du portail de marque de télécharger du contenu depuis l’instance du portail de marque et de publier à nouveau le dossier des contributions dans AEM Assets sans avoir besoin de droits d’administrateur.
Pour plus d’informations, voir [Approvisionnement des ressources dans Brand Portal](brand-portal-asset-sourcing.md).



**Question Est-ce que je n’aurai plus accès aux ressources et fonctionnalités existantes ou aux configurations que j’ai créées ?**

**Rép.** Toutes les fonctionnalités et configurations existantes ne sont pas modifiées. Vos utilisateurs finaux ne sont pas affectés et votre contenu reste intact.



**Question Quand vais-je passer à la nouvelle version de Brand Portal ?**

**Rép.** La version 6.4.5 de Brand Portal a été lancée en octobre 2019. Et la prochaine version du portail de marque devrait être publiée au 3e trimestre 2020.
Pour les mises à jour et les modifications de version, il est recommandé de suivre les Notes [de](brand-portal-release-notes.md) mise à jour et les [Nouveautés du portail](whats-new.md)de marque.



**Ques. Cela aura-t-il une incidence pour mes utilisateurs ?**

**Rép.** La version 6.4.5 de Brand Portal est exclusivement disponible dans Brand Portal, de sorte qu’il n’y a aucun impact pour vos utilisateurs finaux.



**Question Existe-t-il une action requise de ma part en tant qu’utilisateur du portail de marque ?**

**Rép.** La version 6.4.5 de Portal de marque comprend une nouvelle fonctionnalité nommée Ressource des ressources. L’administrateur AEM doit configurer la fonction d’origine des ressources dans AEM Assets pour activer cette fonction pour les utilisateurs du portail de marque. Pour plus d’informations, voir [Activer l’approvisionnement](brand-portal-configure-asset-sourcing.md)des ressources.



**Question Qui peut créer un dossier de contributions ?**

**Rép.** Tous les utilisateurs d’AEM peuvent créer un nouveau dossier dans AEM Assets et affecter la propriété **Asset Contribution**. Le dossier nouvellement créé est appelé dossier de **contribution** .
Ce dossier est ensuite partagé avec les utilisateurs actifs du portail de marque pour contribution.



**Question Que contient un dossier de contributions ?**

**Rép.** Le dossier **Contribution** contient deux sous-dossiers **NOUVEAU** et **PARTAGÉ**. Au départ, le dossier NEW est vide et le dossier SHARED contient le contenu de référence (ressources réutilisables) pour les utilisateurs du portail de marque.
Les utilisateurs du portail de marque accèdent au dossier **Contribution** et téléchargent le contenu dans le dossier **NEW** .



**Question Qu'est-ce que les exigences en matière d'actifs avec la contribution de r.t.**

**Rép.** Le **bref** document joint au dossier **Contribution** et le contenu de référence (ressources réutilisables) téléchargés dans le dossier **PARTAGÉ** aident l’utilisateur du portail de marque à comprendre le besoin de contribution et les attentes en tant que contributeur et est collectivement appelé les exigences en matière de ressources.



**Question Puis-je télécharger des fichiers vers n’importe quel dossier autorisé ?**

**Rép.** Tous les dossiers ne sont pas autorisés. Un utilisateur du portail de marque peut télécharger du contenu uniquement vers le dossier **Contribution** partagé par l’administrateur d’AEM ou du portail de marque.



**Question Comment puis-je accéder à un dossier de contributions ?**

**Rép.** Vous pouvez accéder à un dossier **de contributions** uniquement s’il a été partagé avec vous. Vous recevrez une notification par courrier électronique ou pouls chaque fois qu’un dossier de contribution est partagé avec vous. Vous pouvez accéder au dossier des contributions via le lien partagé dans le courrier électronique ou vous connecter à votre instance du portail de marque et accéder à l’icône représentant une cloche pour obtenir des notifications d’accès au dossier des contributions.

>[!NOTE]
>
>Si vous n’êtes pas un utilisateur existant du portail de marque, demandez à l’administrateur AEM de créer votre utilisateur dans la console d’administration AEM et d’ajouter votre profil au fichier de configuration utilisateur dans la liste des utilisateurs du portail de marque. Reportez-vous à [Ajout d’un utilisateur](brand-portal-configure-asset-sourcing.md)du portail de marque.



**Question Quel est le format du fichier CSV à importer par l’utilisateur ?**

**Rép.** Le format est identique à celui pris en charge par la Console d’administration pour l’importation en masse par l’utilisateur. Le courriel, le prénom et le nom sont obligatoires.



**Question Qu’est-ce qui renseigne la liste des utilisateurs (contributeurs du portail de marque) dans la liste déroulante des utilisateurs des contributions aux ressources ?**

**Rép.** Les utilisateurs de la liste déroulante sont renseignés à partir du fichier de configuration utilisateur du portail de marque (.csv) téléchargé dans AEM.



**Question Où puis-je voir l’état des tâches d’importation et de publication ?**

**Rép.** Dans AEM, vous pouvez voir l’état d’une importation dans la page de travail **asynchrone** . Dans le portail de marque, vous pouvez voir l’état d’une tâche de publication dans **[!UICONTROL Outils &gt; Etat]** de contribution des ressources.



**Question Quelle est la fréquence d’une tâche d’importation qui s’exécute régulièrement dans AEM ?**

**Rép.** Dans AEM, l’interrogation s’effectue toutes les 5 minutes.



**Question Le nombre de fois où un dossier peut être publié de Brand Portal vers AEM Assets est-il limité ?**

**Rép.** Non, toutes les ressources du dossier **NOUVEAU** sont publiées dans AEM Assets, indépendamment du fait qu’elles aient été publiées précédemment. Chaque fois qu’un dossier **de contribution** est publié depuis le portail de marque vers AEM Assets, il remplace le contenu du dossier **NOUVEAU** .



**Question Comment télécharger de nouveaux fichiers dans un dossier de contributions ?**

**Rép.** Reportez-vous à la documentation détaillée pour le [téléchargement de fichiers vers le dossier](brand-portal-upload-assets-to-contribution-folder.md)Contribution.



**Question Je ne vois pas de vignettes/aperçus sur les ressources transférées vers le dossier NEW par un utilisateur du portail de marque ?**

**Rép.** Il est conçu comme prévu, car aucun flux de travail n’est exécuté à la fin du portail de marque.



**Question Que se passe-t-il si un dossier est publié depuis les ressources AEM vers le portail de marque en flux ?**

**Rép.** Dans AEM, les journaux sont conservés chaque fois qu’un dossier est publié sur le portail de marque. Au moment de la publication, toutes les ressources qui ne sont pas publiées sur le portail de marque sont placées dans une file d’attente de réplication. Les fichiers ajoutés au dossier après le déclenchement de la tâche de publication ne sont pas publiés sur le portail de marque. Lorsque l’utilisateur AEM publie à nouveau le dossier, seuls les fichiers qui n’ont pas été publiés précédemment (existants dans la file d’attente de réplication) sont publiés sur le portail de marque.
Cela est vrai pour tout dossier publié à partir des ressources AEM vers le portail de marque et pour le dossier PARTAGÉ dans un dossier de contribution.



**Ques. Qui dois-je contacter en cas de questions ?**

**Rép.** Contactez votre gestionnaire de compte ou le service à la clientèle Adobe.


>[!NOTE]
>
>Le calendrier des nouvelles versions est provisoire et susceptible d’être modifié. Contactez votre gestionnaire de compte ou le service clientèle Adobe pour obtenir le calendrier de version mis à jour.




## Assistance technique et accès au produit (sites à accès limité) {#product-access-and-support-restricted-sites}

Ces sites sont réservés aux clients. Si vous êtes client et avez besoin d’un accès, contactez votre responsable de compte Adobe.

* [](https://daycare.day.com) [Accès aux produits](https://login.marketing.adobe.com)

* [Assistance clientèle d’Adobe](https://helpx.adobe.com/contact.html)
