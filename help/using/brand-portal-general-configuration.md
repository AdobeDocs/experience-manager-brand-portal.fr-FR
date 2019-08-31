---
title: Administration des configurations générales du client
seo-title: Administration des configurations générales du client
description: Configuration de l'accélération de téléchargement, public intelligent [! Création UICONTROL], public [! Création UICONTROL] et permet aux administrateurs de supprimer des fichiers sur les clients.
seo-description: Configuration de l'accélération de téléchargement, public intelligent [! Création UICONTROL], public [! Création UICONTROL] et permet aux administrateurs de supprimer des fichiers sur les clients.
uuid: 3 c 46 cd 7 c-c 38 b -4 bc 7-b 566-93 f 977 bc 8227
contentOwner: mgulati
topic-tags: administration
content-type: référence
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
discoiquuid: f 4 c 237 bc-f 6 a 4-4 bc 4-af 56-3 d 9 c 3027 daf 4
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Administration des configurations générales du client {#administer-general-tenant-configurations}

AEM Assets Brand Portal permet aux organisations de configurer les fonctionnalités suivantes pour des clients spécifiques :

* Suppression des ressources par les administrateurs
* Création de collections publiques par les utilisateurs non administrateurs
* Création de collections dynamiques publiques par les utilisateurs non administrateurs
* Accélération des téléchargements
* Hiérarchie parente des dossiers partagés visible pour les utilisateurs non-administrateurs

These configurations have been provided as **[!UICONTROL General Settings]** configurations on the administrative tools panel.

![](assets/general-configs.png)

**** Configuration permettant aux administrateurs de supprimer des fichiers de Brand Portal. (activée par défaut)

**Configuration B** pour permettre aux utilisateurs non administrateurs de créer des collections publiques. (activée par défaut)

**C** Configuration autorisant les utilisateurs non administrateurs à créer des collections dynamiques publiques. (activée par défaut)

**Configuration D** pour permettre l'accélération de téléchargement des fichiers téléchargés depuis le portail et depuis les liens partagés. (désactivée par défaut)

**E** Configuration pour afficher la hiérarchie de dossiers (à partir de la racine) des dossiers partagés pour les utilisateurs non administrateurs (éditeurs, observateurs et utilisateurs invités). (désactivée par défaut)

## Activation/désactivation des configurations générales {#enable-disable-general-configurations}

Pour activer/désactiver chacune de ces configurations :

1. Connectez-vous avec les privilèges d’administrateur.
2. Sélectionnez le logo AEM pour accéder aux outils d’administration dans la barre d’outils supérieure.
3. From the administrative tools panel, select **[!UICONTROL General]** to open the **[!UICONTROL General Settings]** page.
4. Utilisez le commutateur respectif pour activer/désactiver chacune des configurations générales.
5. **[!UICONTROL Enregistrez les modifications.]**
6. Déconnectez-vous pour que les modifications soient appliquées.

## Autorisation de la suppression des ressources de Brand Portal par les utilisateurs administrateurs {#allow-admin-users-to-delete-assets-from-brand-portal}

**[!UICONTROL Autoriser les utilisateurs à configurer]** la configuration permet aux entreprises d'autoriser (ou limiter) les utilisateurs disposant de droits d'administrateur à supprimer des fichiers et des dossiers de Brand Portal.

## Autorisation de la création de collections publiques par les utilisateurs non administrateurs {#allow-public-collections-creation-by-non-admins}

[[! UICONTP Autorisation de création des collections](../using/brand-portal-share-collection.md#main-pars-text-1915052376) publiques contrôle si les administrateurs peuvent créer des collections publiques sur le portail de marque. La configuration est activée par défaut. En la désactivant, les organisations peuvent éviter d’avoir de nombreuses collections publiques sur leur portail afin d’économiser l’espace du système.

## Autorisation de la création de collections dynamiques publiques par les utilisateurs non-administrateurs {#allow-public-smart-collections-creation-by-non-admins}

[[! UICONTP Autoriser la création de collections dynamiques](../using/brand-portal-searching.md#main-pars-header-500620467) publiques contrôle si les administrateurs peuvent enregistrer leurs recherches en tant que collections dynamiques et les rendre publiques pour ce client. La configuration est activée par défaut. En la désactivant, les organisations peuvent éviter la création d’un nombre très important de collections dynamiques publiques par les utilisateurs non-administrateurs sur le Brand Portal de l’organisation.

## Autorisation de l’accélération des téléchargements {#allow-download-acceleration}

[[! UICONTP La configuration de l'accélération de téléchargement]](../using/accelerated-download.md) permet aux entreprises d'autoriser les téléchargements accélérés des ressources à partir du portail de marque et des liens partagés en s'intégrant à IBM Aspera Connect qui est une application à la demande. L’application utilise une technologie propriétaire pour supprimer les en-têtes TCP.

## Activation de la hiérarchie de dossiers {#enable-folder-hierarchy}

[[! La configuration de la hiérarchie des dossiers UICONTP]](../using/brand-portal-sharing-folders.md#non-admin-user-access-to-shared-folders) permet aux administrateurs de contrôler la manière dont les utilisateurs non administrateurs (Editeurs, Lecteurs et Utilisateurs invités) visualisent les dossiers partagés après la connexion.
