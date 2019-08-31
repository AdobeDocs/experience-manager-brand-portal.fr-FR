---
title: Accès des invités à Brand Portal
seo-title: Accès des invités à Brand Portal
description: Autorisez l’accès des invités et économisez les efforts d’intégration de nombreux utilisateurs qui n’ont pas besoin d’être authentifiés.
seo-description: Autorisez l’accès des invités et économisez les efforts d’intégration de nombreux utilisateurs qui n’ont pas besoin d’être authentifiés.
uuid: edb 4378 d -1710-44 a 2-97 a 6-594 d 99 f 62 fff
contentOwner: mgulati
topic-tags: introduction
content-type: référence
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
discoiquuid: b 9 e 9 fe 7 b -0373-42 d 1-851 b -7 c 76 b 47657 c 2
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Accès des invités à Brand Portal {#guest-access-to-brand-portal}

AEM Brand Portal permet à des invités d’accéder au portail. Un utilisateur invité n’a pas besoin d’informations d’identification pour accéder au portail et a accès aux ressources (et aux collections) publiques du portail. Users in the guest session can add assets to their lightbox (private collection) and download the same until their session lasts, which is 2 hours from the beginning of the session unless the guest user chooses to [[!UICONTROL End Session]](#exit-guest-session).

Guest access functionality enables organizations to [quickly share approved assets](../using/brand-portal-sharing-folders.md#how-to-share-folders) with the intended audience at scale without having to onboard them. À compter de la version 6.4.2, Brand Portal est capable de servir plusieurs utilisateurs invités simultanés sans dépasser 10 % du nombre total d’utilisateurs par entreprise. L'autorisation d'accès des invités permet de gagner du temps à gérer et à identifier des scores d'utilisateurs qui doivent utiliser des fonctionnalités limitées sur le portail de marque.\
Les organisations peuvent activer (ou désactiver) l'accès aux invités sur le compte de portail de marque de l'organisation à l'aide **[!UICONTROL de l'option Autoriser les]** invités à accéder aux **[!UICONTROL paramètres d'accès]** dans le panneau Outils d'administration.

<!--
Comment Type: annotation
Last Modified By: mgulati
Last Modified Date: 2018-08-17T10:42:59.879-0400
Removed the first para: "AEM Assets Brand Portal allows public users to enter the portal anonymously and have restricted access to the allowed public resources as guests. Organization users with guest role need not seek access and authentication from administrators."
-->

![](assets/enable-guest-access.png)

## Démarrage d’une session d’invité {#begin-guest-session}

Pour accéder à Brand Portal de manière anonyme, sélectionnez **[!UICONTROL Cliquez ici]** en regard de **Accès d’invité ?** sur l'écran de bienvenue de Brand Portal. Les utilisateurs n’ont pas besoin de demander l’accès et d’attendre que l’administrateur les authentifie pour leur accorder l’accès à Brand Portal.

![](assets/bp-login-screen.png)

## Durée d’une session d’invité {#guest-session-duration}

Une session d’utilisateur invité reste active pendant deux heures. This means that the state of the [!UICONTROL Lightbox] is preserved until 1 hour from the session start time, and after 2 hours the current guest session restarts so the Lightbox state is lost.\
Par exemple, un utilisateur invité se connecte à la marque à 1 500 heures et ajoute des ressources à Lightbox en téléchargement à 16:50 heures. If the user doesn't download the [!UICONTROL Lightbox] collection (or its assets) before 17:00 hours, the [!UICONTROL Lightbox] will become empty as the user will have to restart the session at the end of 1 hour (that is 1700 hours).

## Sessions d’invités simultanées permises {#concurrent-guest-sessions-allowed}

Le nombre de sessions d'invités simultanées est limité à 10 % du quota total d'utilisateurs par organisation. Ainsi, pour une organisation disposant du quota d'utilisateurs de 200, 20 utilisateurs invités maximum peuvent travailler simultanément. L'accès à la 21 e utilisateur est refusé et peut accéder en tant qu'invité uniquement si la session de l'un des 20 utilisateurs invités actifs se termine.

## Interaction des utilisateurs invités avec Brand Portal {#guest-user-interaction-with-brand-portal}

### Navigation dans l’IU pour les invités

On entering the Brand Portal as the guest, users can see all the [assets and folders shared](../using/brand-portal-sharing-folders.md#sharefolders) publicly or with guest users exclusively. Réservée au contenu, cette vue affiche les ressources dans les dispositions Carte, Liste ou Colonnes.

![](assets/disabled-folder-hierarchy1.png)

However, the guest users see the folder tree (starting from the root folder) and the shared folders arranged within their respective parent folders on logging in to the Brand Portal, if administrators have enabled [Enable Folder Hierarchy](../using/brand-portal-general-configuration.md#main-pars-header-1621071021) configuration.

Ces dossiers parents sont des dossiers virtuels et ne peuvent faire l’objet d’aucune action. Vous pouvez identifier ces dossiers virtuels grâce à leur icône de verrou.

No action tasks are visible on hovering or selecting them in [!UICONTROL Card View], unlike the shared folders. [!UICONTROL Le] bouton Aperçu s'affiche lors de la sélection d'un dossier virtuel en mode [!UICONTROL Colonnes] et [!UICONTROL Affichage par liste].

>[!NOTE]
>
>Notez que la miniature par défaut des dossiers virtuels est l’image de miniature du premier dossier partagé.

![](assets/enabled-hierarchy1.png) ![](assets/hierarchy1-nonadmin.png) ![](assets/hierarchy-nonadmin.png) ![](assets/hierarchy2-nonadmin.png)

[!UICONTROL L'option Paramètres] d'affichage permet aux utilisateurs invités d'ajuster les tailles de carte dans [!UICONTROL l'Affichage] Carte ou les colonnes à afficher en [!UICONTROL mode Liste].

![](assets/nav-guest-user.png)

The [!UICONTROL Content tree] lets you move through assets hierarchy.

![](assets/guest-login-ui.png)

Brand Portal provides [!UICONTROL Overview] option to guest users to view [!UICONTROL Asset Properties] of selected assets/folders. The [!UICONTROL Overview] option is visible:

* dans la barre d’outils supérieure lors de la sélection d’une ressource/d’un dossier ;
* dans le menu déroulant, lors de la sélection du sélecteur de rail.

On selecting the [!UICONTROL Overview] option while an asset/folder is selected, users can see the title, path, and time of asset creation. Whereas, on asset detail page selecting [!UICONTROL Overview] option lets the users see metadata of the asset.

![](assets/overview-option-1.png)

![](assets/overview-rail-selector-1.png)

**[!UICONTROL L'option de navigation]** dans la barre de navigation gauche permet de naviguer entre les fichiers vers les collections et de revenir à la session d'invités afin que les utilisateurs puissent parcourir les fichiers dans des fichiers ou des collections.

**[!UICONTROL L'option Filtre]** permet aux utilisateurs invités de filtrer les fichiers et dossiers de fichiers à l'aide de prédicats de recherche définis par l'administrateur.

### Fonctions offertes aux utilisateurs invités

Les utilisateurs invités peuvent accéder aux ressources publiques sur Brand Portal et ont également quelques restrictions comme décrit plus loin.

Les utilisateurs invités peuvent :

* accéder à tous les dossiers et collections publics destinés à tous les utilisateurs de Brand Portal ;
* parcourir les membres et la page de détails, et disposer d’une vue complète des ressources des membres de tous les dossiers et collections publics ;
* rechercher des ressources au sein des dossiers et collections publics ;
* ajouter des ressources à la collection Lightbox. Les modifications apportées à la collection persistent pendant la session.
* télécharger des ressources directement ou via la collection Lightbox.

Les utilisateurs invités ne peuvent pas :

* créer des collections et des recherches enregistrées, ni les partager ;
* accéder aux paramètres des dossiers et collections ;
* partager des ressources sous la forme de liens.

### Téléchargement de ressources au cours d’une session d’invité

Les utilisateurs invités peuvent télécharger directement les ressources partagées publiquement ou exclusivement avec les utilisateurs invités sur Brand Portal. Guest users can also add assets to [!UICONTROL Lightbox] (public collection), and download the [!UICONTROL Lightbox] collection before their session expires.

Pour télécharger des fichiers et des collections, utilisez l'icône de téléchargement de :

* miniatures d'action rapide, qui apparaissent lorsque vous passez la souris sur le fichier ou la collection
* la barre d'outils en haut, qui s'affiche lors de la sélection du fichier ou de la collection

![](assets/download-on-guest.png)

Sélectionnez **[!UICONTROL Activer l’accélération des téléchargements]**[!UICONTROL  dans la boîte de dialogue Téléchargement afin d’]améliorer les performances de téléchargement[.](../using/accelerated-download.md)

## Quitter une session d’invité {#exit-guest-session}

To exit a guest session, use **[!UICONTROL End Session]** from the options available in the header. Cependant, si le navigateur utilisé pour la session invité est inactif, la session expire automatiquement après deux heures d'inactivité.

![](assets/end-guest-session.png)

## Surveillance des activités des utilisateurs invités {#monitoring-guest-user-activities}

Les administrateurs peuvent suivre l’interaction des utilisateurs invités avec Brand Portal. Les rapports générés dans Brand Portal peuvent fournir des informations clés sur les activités des utilisateurs invités. Par exemple, le rapport **[!UICONTROL Téléchargement]peut être utilisé pour le suivi du nombre de ressources téléchargées par un utilisateur invité.** **[!UICONTROL Le rapport Connexion]** utilisateur peut informer le dernier utilisateur connecté au portail et la fréquence des connexions d'une durée spécifiée.
