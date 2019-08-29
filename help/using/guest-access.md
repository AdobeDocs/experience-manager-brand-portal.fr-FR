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
source-git-commit: 770c353b1143d879280df310012ce9d4d30b40c9

---


# Accès des invités à Brand Portal {#guest-access-to-brand-portal}

[!DNL AEM Brand portal] permet aux invités d'accéder à Portal. Un utilisateur invité n’a pas besoin d’informations d’identification pour accéder au portail et a accès aux ressources (et aux collections) publiques du portail. Users in the guest session can add assets to their lightbox (private collection) and download the same until their session lasts, which is 2 hours from the beginning of the session unless the guest user chooses to [End Session](#exit-guest-session).

Guest access functionality enables organizations to [quickly share approved assets](../using/brand-portal-sharing-folders.md#how-to-share-folders) with the intended audience at scale without having to onboard them. [!DNL Brand Portal]À compter de la version 6.4.2,  est capable de servir plusieurs utilisateurs invités simultanés sans dépasser 10 % du nombre total d’utilisateurs par entreprise. Allowing guest access saves time to manage and on-board scores of users who need to use limited functionalities on [!DNL Brand Portal].\
Les organisations peuvent activer (ou désactiver) l'accès aux invités au [!DNL Brand Portal] compte de l'organisation à l'aide **de l'option Autoriser l'accès** des invités à partir **des paramètres d'accès** dans le panneau Outils d'administration.

<!--
Comment Type: annotation
Last Modified By: mgulati
Last Modified Date: 2018-08-17T10:42:59.879-0400
Removed the first para: "AEM Assets Brand Portal allows public users to enter the portal anonymously and have restricted access to the allowed public resources as guests. Organization users with guest role need not seek access and authentication from administrators."
-->

![](assets/enable-guest-access.png)

## Démarrage d’une session d’invité {#begin-guest-session}

Pour accéder à Brand Portal de manière anonyme, sélectionnez **[!UICONTROL Cliquez ici]** en regard de **Accès d’invité ?** sur [!DNL Brand Portal] l'écran de bienvenue. Les utilisateurs n’ont pas besoin de demander l’accès et d’attendre que l’administrateur les authentifie pour leur accorder l’accès à [!DNL Brand Portal].

![](assets/bp-login-screen.png)

## Durée d’une session d’invité {#guest-session-duration}

Une session d’utilisateur invité reste active pendant deux heures. This means that the state of the [!UICONTROL lightbox] is preserved until 1 hour from the session start time, and after 2 hours the current guest session restarts so the lightbox state is lost.\
For example, a guest user logs in to the [!DNL Brand Portal] at 1500 hours and adds assets to lightbox for download at 16:50 hours. If the user doesn't download the [!UICONTROL lightbox collection] (or its assets) before 17:00 hours, the [!UICONTROL lightbox] will become empty as the user will have to restart the session at the end of 1 hour (that is 1700 hours).

## Sessions d’invités simultanées permises {#concurrent-guest-sessions-allowed}

Le nombre de sessions d'invités simultanées est limité à 10 % du quota total d'utilisateurs par organisation. Ainsi, pour une organisation disposant du quota d'utilisateurs de 200, 20 utilisateurs invités maximum peuvent travailler simultanément. L'accès à la 21 e utilisateur est refusé et ne pourra accéder qu'en tant qu'invité lorsque la session de l'un des 20 utilisateurs invités actifs se termine.

## Interaction des utilisateurs invités avec Brand Portal {#guest-user-interaction-with-brand-portal}

### Navigation dans l’IU pour les invités

On entering the [!DNL Brand Portal] as the guest, users are able to see all the [assets and folders shared](../using/brand-portal-sharing-folders.md#sharefolders) publicly or with guest users exclusively. Réservée au contenu, cette vue affiche les ressources dans les dispositions Carte, Liste ou Colonnes.

![](assets/disabled-folder-hierarchy1.png)

However, Guest Users see the folder tree (starting from the root folder) and the shared folders arranged within their respective parent folders on logging in to the [!DNL Brand Portal], if administrators have enabled [Enable Folder Hierarchy](../using/brand-portal-general-configuration.md#main-pars-header-1621071021) configuration.

Ces dossiers parents sont des dossiers virtuels et ne peuvent faire l’objet d’aucune action. Vous pouvez identifier ces dossiers virtuels grâce à leur icône de verrou.

Aucune tâche d’action n’est visible lorsque vous les survolez ou les sélectionnez en mode Carte, à la différence des dossiers partagés. Le bouton Aperçu apparaît lorsque vous sélectionnez un dossier virtuel dans les modes Colonnes et Liste.

>[!NOTE]
>
>Notez que la miniature par défaut des dossiers virtuels est l’image de miniature du premier dossier partagé.

![](assets/enabled-hierarchy1.png) ![](assets/hierarchy1-nonadmin.png) ![](assets/hierarchy-nonadmin.png) ![](assets/hierarchy2-nonadmin.png)

L’option Paramètres permet aux utilisateurs invités d’ajuster les formats de carte en mode Carte ou les colonnes à afficher en mode Liste.

![](assets/nav-guest-user.png)

L'arborescence de contenu vous permet de parcourir la hiérarchie des ressources.

![](assets/guest-login-ui.png)

[!DNL Brand Portal] propose l'option **Aperçu** aux utilisateurs invités pour afficher les propriétés de ressource des fichiers/dossiers sélectionnés. L’option Aperçu est visible :

1. dans la barre d’outils supérieure lors de la sélection d’une ressource/d’un dossier ;
2. dans le menu déroulant, lors de la sélection du sélecteur de rail.

S’ils choisissent l’option Aperçu lorsqu’une ressource/un dossier est sélectionné, les utilisateurs peuvent voir le titre, le chemin et l’heure de création de la ressource. En revanche, sur la page des détails de la ressource, l’option Aperçu permet aux utilisateurs d’afficher les métadonnées de la ressource.

![](assets/overview-option-1.png)

![](assets/overview-rail-selector-1.png)

**[!UICONTROL L'option de navigation]** dans la barre de navigation gauche permet de naviguer entre les fichiers vers [!UICONTROL les collections] et de revenir à la session d'invités afin que les utilisateurs puissent parcourir les fichiers dans des fichiers ou [!UICONTROL des collections].

**L'option Filtre** permet aux utilisateurs invités de filtrer les fichiers et dossiers de fichiers à l'aide de prédicats de recherche définis par l'administrateur.

### Fonctions offertes aux utilisateurs invités

Guest users can access public assets on [!DNL Brand Portal], and also have few restrictions as discussed further.

Les utilisateurs invités peuvent :

* access all the public folders and [!UICONTROL collections] meant for all the [!DNL Brand Portal] users.
* browse members, detail page, and have full asset view of the members of all the public folders and [!UICONTROL collections].
* search assets across public folders and [!UICONTROL collections].
* add assets to lightbox [!UICONTROL collection]. These changes to the [!UICONTROL collection] persist during the session.
* download assets directly or through lightbox [!UICONTROL collection].

Les utilisateurs invités ne peuvent pas :

* create [!UICONTROL collections] and saved searches, or share them further.
* access folder and [!UICONTROL collections] settings.
* partager des ressources sous la forme de liens.

### Téléchargement de ressources au cours d’une session d’invité

Les utilisateurs invités peuvent télécharger directement les ressources partagées publiquement ou exclusivement avec les utilisateurs invités sur [!DNL Brand Portal]. Guest users can also add assets to [!UICONTROL Lightbox] (public [!UICONTROL collection]), and download the [!UICONTROL lightbox collection] before their session expires.

To download assets and [!UICONTROL collections], use the download icon from:

* quick action thumbnails, which appear on hovering over the asset or [!UICONTROL collection]
* the toolbar at the top, which appears on selecting the asset or [!UICONTROL collection]

![](assets/download-on-guest.png)

Sélectionnez **Activer l’accélération des téléchargements** dans la boîte de dialogue Téléchargement afin d’[améliorer les performances de téléchargement](../using/accelerated-download.md).

## Quitter une session d’invité {#exit-guest-session}

To exit a guest session, use **End Session** from the options available in the header. Cependant, si le navigateur utilisé pour la session invité est inactif, la session expire automatiquement après deux heures d'inactivité.

![](assets/end-guest-session.png)

## Surveillance des activités des utilisateurs invités {#monitoring-guest-user-activities}

Les administrateurs peuvent suivre l’interaction des utilisateurs invités avec [!DNL Brand Portal]. Reports generated in [!DNL Brand Portal] can provide key insights into guest user activities. Par exemple, le rapport **Téléchargement** peut être utilisé pour le suivi du nombre de ressources téléchargées par un utilisateur invité. **Le rapport Connexion** utilisateur peut informer le dernier utilisateur connecté au portail et la fréquence des connexions d'une durée spécifiée.
