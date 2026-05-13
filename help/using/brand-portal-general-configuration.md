---
title: Administration des configurations générales du client
description: Configurez l’accélération des téléchargements, la création de collections publiques, dynamiques ou non, et permettez aux utilisateurs administrateurs de supprimer des ressources sur les clients.
contentOwner: mgulati
topic-tags: administration
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
role: Admin
exl-id: 5607be8e-0a7f-4692-b71b-5f66eb9ac5ee
TQID: https://experienceleague.adobe.com/W08soCNQvrQy3ZttX4Oa2m-dvmTSxyeTpPmHNLedgPA
product_v2:
  - id: d09181b5-a36a-43de-ba01-36641440bc43
  - id: fd1f54a9-f50c-467d-8956-cebbaf4f3eb8
feature_v2:
  - id: cda65036-5305-4f01-89da-9b3506ae8c50
  - id: da0dfbce-df02-4f8b-b32d-a4e3b1d05085
subfeature_v2:
  - id: e00c7c12-7035-41fe-ad76-1ec82c8c3f01
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e48edcb1ed5d76686794f7a7ed6389c7f4ab1ed3
workflow-type: tm+mt
source-wordcount: 396
ht-degree: 53%

---

# Administration des configurations générales du client {#administer-general-tenant-configurations}

Experience Manager Assets Brand Portal permet aux organisations de configurer les fonctionnalités suivantes pour des clients spécifiques :

* Suppression des ressources par les administrateurs
* Création de collections publiques par des utilisateurs non administrateurs
* Création de collections dynamiques publiques par des utilisateurs non administrateurs
* La hiérarchie parente des dossiers partagés est visible par les utilisateurs non-administrateurs

Ces configurations ont été fournies en tant que configurations **[!UICONTROL Paramètres généraux]** dans le panneau des outils d’administration.

![](assets/general-config.png)

**A** - Configuration pour permettre aux administrateurs de supprimer des ressources de Brand Portal. (activée par défaut).

**B** - Configuration pour permettre aux utilisateurs non-administrateurs de créer des collections publiques. (activée par défaut).

**C** - Configuration pour permettre aux utilisateurs non-administrateurs de créer des collections dynamiques publiques. (activée par défaut).

**D** - Configuration pour afficher la hiérarchie de dossiers (à partir de la racine) des dossiers partagés aux utilisateurs non-administrateurs (éditeurs, observateurs, utilisateurs invités). (désactivée par défaut).

## Activation ou désactivation des configurations générales {#enable-disable-general-configurations}

Pour activer ou désactiver chacune de ces configurations :

1. Connectez-vous avec des droits d’administrateur.
1. Sélectionnez le logo Experience Manager pour accéder aux outils d’administration dans la barre d’outils supérieure.
1. À partir du panneau des outils d’administration, sélectionnez **[!UICONTROL Général]** pour ouvrir la page **[!UICONTROL Paramètres généraux]**.
1. Utilisez le bouton (bascule) correspondant pour activer ou désactiver l’une des configurations générales.
1. **[!UICONTROL Enregistrez]** les modifications.
1. Déconnectez-vous afin que les modifications puissent prendre effet.

## Autorisation de la suppression des ressources de Brand Portal par les utilisateurs administrateurs {#allow-admin-users-to-delete-assets-from-brand-portal}

La configuration **[!UICONTROL Autoriser les utilisateurs à supprimer]** permet aux organisations d’autoriser les utilisateurs avec les privilèges d’administrateur à supprimer des ressources et des dossiers de Brand Portal, ou de les en restreindre.

## Autorisation de la création de collections publiques par les utilisateurs non-administrateurs {#allow-public-collections-creation-by-non-admins}

La configuration [[!UICONTROL Autoriser la création de collections publiques]](../using/brand-portal-share-collection.md#main-pars-text-1915052376) contrôle si les utilisateurs non-administrateurs peuvent créer des collections publiques sur Brand Portal. La configuration est activée par défaut. En désactivant la configuration, les entreprises peuvent éviter d’avoir de nombreuses collections publiques sur leur portail afin d’économiser de l’espace système.

## Autorisation de la création de collections dynamiques publiques par les utilisateurs non administrateurs {#allow-public-smart-collections-creation-by-non-admins}

La configuration [[!UICONTROL Autoriser la création de collections dynamiques publiques]](../using/brand-portal-searching.md#main-pars-header-500620467) contrôle si les non-administrateurs peuvent enregistrer leurs recherches sous la forme de collections dynamiques et les rendre publiques pour ce client. La configuration est activée par défaut. En désactivant la configuration, les organisations peuvent éviter qu’un grand nombre de collections dynamiques publiques soient créées par des utilisateurs non administrateurs sur le Brand Portal de l’organisation.

<!-- 
## Allow download acceleration {#allow-download-acceleration}

[[!UICONTROL Allow download acceleration]](../using/accelerated-download.md) configuration lets the organizations to allow accelerated downloads of assets from Brand Portal and shared links, by integrating with IBM Aspera Connect that is an install-on-demand application. The application uses proprietary technology to remove TCP overheads.
-->

## Activer la hiérarchie de dossiers {#enable-folder-hierarchy}

La configuration [[!UICONTROL Activer la hiérarchie de dossiers]](../using/brand-portal-sharing-folders.md#non-admin-user-access-to-shared-folders) permet aux administrateurs de contrôler la façon dont, une fois connectés, les utilisateurs non-administrateurs (éditeurs, observateurs et utilisateurs invités) voient les dossiers partagés.
