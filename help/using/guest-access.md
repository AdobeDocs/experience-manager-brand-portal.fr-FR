---
title: Accès des invités à Brand Portal
seo-title: Guest Access to Brand Portal
description: Autorisez l’accès des invités et facilitez l’intégration de nombreux utilisateurs sans authentification.
seo-description: Allow guest access and save the effort to onboard numerous users without authentication.
uuid: edb4378d-1710-44a2-97a6-594d99f62fff
contentOwner: VG
topic-tags: introduction
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: b9e9fe7b-0373-42d1-851b-7c76b47657c2
exl-id: ecce0a45-abae-41c4-9ea7-5dfdcf19e5ea
source-git-commit: 0670b8d372fd2dc5bdb1d0a928601e3e09a6dcf9
workflow-type: ht
source-wordcount: '1026'
ht-degree: 100%

---

# Accès des invités à Brand Portal {#guest-access-to-brand-portal}

Experience Manager Assets Brand Portal permet aux invités d’accéder au portail. Un utilisateur invité n’a pas besoin d’identifiants pour accéder au portail et a accès aux ressources (et aux collections) publiques du portail. Les utilisateurs ou les utilisatrices se trouvant dans une session d’invité peuvent ajouter des ressources à leur Lightbox (collection privée) et les télécharger jusqu’au terme de leur session, à moins que la personne invitée ne choisisse de [[!UICONTROL Terminer la session]](#exit-guest-session). Une session de personne invitée reste active pendant 15 minutes.

La fonctionnalité d’accès des invités permet aux entreprises de [partager rapidement les ressources approuvées](../using/brand-portal-sharing-folders.md#how-to-share-folders) avec l’audience prévue à grande échelle sans avoir besoin d’une intégration. À compter de la version 6.4.2, Brand Portal est capable de servir plusieurs utilisateurs invités simultanés sans dépasser 10 % du nombre total d’utilisateurs par entreprise. Autoriser l’accès des invités permet de gagner du temps dans le cadre de la gestion et de l’intégration de nombreux utilisateurs avec des fonctionnalités limitées sur Brand Portal.\
Les entreprises peuvent activer (ou désactiver) l’accès des invités à leur compte à l’aide de l’option **[!UICONTROL Autoriser l’accès des invités]** dans les paramètres **[!UICONTROL Accès]** du panneau des outils d’administration.

<!--
Comment Type: annotation
Last Modified By: mgulati
Last Modified Date: 2018-08-17T10:42:59.879-0400
Removed the first para: "AEM Assets Brand Portal allows public users to enter the portal anonymously and have restricted access to the allowed public resources as guests. Organization users with guest role need not seek access and authentication from administrators."
-->

![](assets/enable-guest-access.png)

## Démarrage d’une session d’invité {#begin-guest-session}

Pour accéder à Brand Portal de manière anonyme, sélectionnez **[!UICONTROL Cliquez ici]** en regard de **[!UICONTROL Accès d’invité ?]** sur l’écran de bienvenue de Brand Portal. Saisissez la réponse à la vérification de sécurité captcha pour obtenir l’accès à Brand Portal.

![](assets/bp-login-screen.png)

## Durée d’une session d’invité {#guest-session-duration}

Une session d’utilisateur invité reste active pendant 15 minutes.
L’état de **[!UICONTROL Lightbox]** est ainsi conservé jusqu’à 15 min à compter du début de la session. Après cela, la session d’invité en cours redémarre et l’état de Lightbox est donc perdu.

Par exemple, un utilisateur invité se connecte à Brand Portal à 15 h 00 et ajoute des ressources dans **[!UICONTROL Lightbox]** pour un téléchargement à 15 h 05. Si l’utilisateur ne télécharge pas la collection **[!UICONTROL Lightbox]** (ou ses ressources) avant 15 h 15 (dans les 15 minutes qui suivent la connexion), il doit redémarrer la session. **[!UICONTROL Lightbox]** est alors vide, ce qui signifie que les ressources chargées ne seront plus disponibles si la session a été perdue.

## Sessions d’invités simultanées permises {#concurrent-guest-sessions-allowed}

Le nombre de sessions d’invités simultanées est limité à 10 % du nombre total d’utilisateurs pour chaque entreprise. Pour une société disposant de 200 utilisateurs, un maximum de 20 utilisateurs invités peuvent ainsi travailler en même temps. Le 21e utilisateur se voit refuser l’accès et ne peut donc bénéficier d’un accès invité que si la session de l’un des 20 utilisateurs invités actifs se termine.

>[!NOTE]
>
>Brand Portal n’envoie pas de notification si le nombre d’utilisateurs sous licence dépasse la valeur convenue (quota). En outre, elle ne limite aucune activité des utilisateurs sous licence.

## Interaction des utilisateurs invités avec Brand Portal {#guest-user-interaction-with-brand-portal}

### Navigation dans l’IU des invités

Lorsqu’ils se connectent à Brand Portal en tant qu’invités, les utilisateurs peuvent voir l’ensemble des [ressources et dossiers partagés](../using/brand-portal-sharing-folders.md#sharefolders) publiquement ou avec les utilisateurs invités exclusivement. Réservé au contenu, ce mode affiche les ressources dans les dispositions Carte, Liste ou Colonnes.

![](assets/disabled-folder-hierarchy1.png)

Cependant, les utilisateurs invités voient l’arborescence de dossiers (à partir du dossier racine) et les dossiers partagés organisés dans leurs dossiers parents respectifs lors de leur connexion à Brand Portal, si les administrateurs ont activé la configuration [Activer la hiérarchie de dossiers](../using/brand-portal-general-configuration.md#main-pars-header-1621071021).

Ces dossiers parents sont les dossiers virtuels et aucune action ne peut être effectuée sur ces derniers. Vous pouvez identifier ces dossiers virtuels grâce à leur icône de cadenas.

Aucune tâche d’action n’est visible lorsque vous les survolez ou les sélectionnez en **[!UICONTROL mode Carte]**, à la différence des dossiers partagés. Le bouton **[!UICONTROL Aperçu]** apparaît lorsque vous sélectionnez un dossier virtuel dans les vues **[!UICONTROL Colonnes]** et **[!UICONTROL Liste]**.

>[!NOTE]
>
>La miniature par défaut des dossiers virtuels est l’image de miniature du premier dossier partagé.

![](assets/enabled-hierarchy1.png) ![](assets/hierarchy1-nonadmin.png) ![](assets/hierarchy-nonadmin.png) ![](assets/hierarchy2-nonadmin.png)

L’option **[!UICONTROL Paramètres]** permet aux utilisateurs invités d’ajuster les formats de carte dans la vue **[!UICONTROL Carte]** ou les colonnes à afficher dans la vue **[!UICONTROL Liste]**.

![](assets/nav-guest-user.png)

**[!UICONTROL Arborescence de contenu]** vous permet de vous déplacer dans la hiérarchie des ressources.

![](assets/guest-login-ui.png)

Brand Portal fournit aux utilisateurs invités l’option **[!UICONTROL Aperçu]** qui leur permet d’afficher les **[!UICONTROL Propriétés de l’élément]** pour les ressources/dossiers sélectionnés. L’option **[!UICONTROL Aperçu]** est visible :

* dans la barre d’outils supérieure lors de la sélection d’une ressource/d’un dossier ;
* dans le menu déroulant, lors de la sélection du sélecteur de rail.

S’ils choisissent l’option **[!UICONTROL Aperçu]** lorsqu’une ressource/un dossier est sélectionné, les utilisateurs peuvent voir le titre, le chemin et l’heure de création de la ressource. En revanche, sur la page des détails de la ressource, l’option **[!UICONTROL Aperçu]** permet aux utilisateurs d’afficher les métadonnées de la ressource.

![](assets/overview-option-1.png)

![](assets/overview-rail-selector-1.png)

L’option **[!UICONTROL Navigation]** dans le rail de gauche permet de naviguer des fichiers aux collections, et inversement, lors d’une session d’invité afin de permettre aux utilisateurs de parcourir les ressources dans les fichiers ou les collections.

L’option **[!UICONTROL Filtre]** permet aux utilisateurs invités de filtrer les fichiers et les dossiers de ressources à l’aide de prédicats de recherche définis par l’administrateur.

### Fonctions offertes aux utilisateurs invités

Les utilisateurs invités peuvent accéder aux ressources publiques sur Brand Portal. Quelques restrictions leur sont également appliquées, comme décrit plus loin.

**Les utilisateurs invités peuvent** :

* accéder à tous les dossiers et collections publics destinés à tous les utilisateurs de Brand Portal ;
* parcourir les membres et la page de détails, et disposer d’une vue complète des ressources des membres de tous les dossiers et collections publics ;
* rechercher des ressources au sein des dossiers et collections publics ;
* ajouter des ressources à la collection Lightbox (les modifications apportées à la collection persistent pendant la session) :
* télécharger des ressources directement ou via la collection Lightbox.

**Les utilisateurs invités ne peuvent pas** :

* créer des collections et des recherches enregistrées, ni les partager ;
* accéder aux paramètres des dossiers et collections ;
* partager des ressources sous la forme de liens.

### Téléchargement de ressources au cours d’une session d’invité

Les utilisateurs invités peuvent télécharger directement les ressources partagées publiquement ou exclusivement avec les utilisateurs invités sur Brand Portal. Ils peuvent également ajouter des ressources à **[!UICONTROL Lightbox]** (collection publique) et télécharger la collection **[!UICONTROL Lightbox]** avant l’expiration de leur session.

Pour télécharger des ressources et des collections, utilisez l’icône Télécharger à partir :

* des miniatures d’action rapide, qui apparaissent lorsque vous placez le curseur sur une ressource ou une collection ;
* de la barre d’outils supérieure, qui s’affiche lorsque vous sélectionnez une ressource ou une collection.

![](assets/download-on-guest.png)

Sélectionnez **[!UICONTROL Activer l’accélération des téléchargements]** dans la boîte de dialogue [!UICONTROL Télécharger] afin d’[améliorer les performances de téléchargement](../using/accelerated-download.md).

## Quitter une session d’invité {#exit-guest-session}

Pour quitter une session d’invité, utilisez **[!UICONTROL Terminer la session]** parmi les options disponibles dans l’en-tête. Toutefois, si l’onglet du navigateur utilisé pour la session d’invité est inactif, la session expire automatiquement après deux heures d’inactivité.

![](assets/end-guest-session.png)

## Surveillance des activités des utilisateurs invités {#monitoring-guest-user-activities}

Les administrateurs peuvent suivre l’interaction des utilisateurs invités avec Brand Portal. Les rapports générés dans Brand Portal peuvent fournir des informations clés sur les activités des personnes invitées. Par exemple, le rapport **[!UICONTROL Télécharger]** peut être utilisé pour le suivi du nombre de ressources téléchargées par un utilisateur invité. Le rapport **[!UICONTROL Connexions des utilisateurs]** peut indiquer lorsqu’un utilisateur invité s’est connecté pour la dernière fois au portail et la fréquence de ses connexions au cours d’une période donnée.
