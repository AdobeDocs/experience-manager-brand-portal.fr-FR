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
source-git-commit: ea7fdd2df0696ed309227fa77e3f79d0141bcb58

---


# Administration des configurations générales du client {#administer-general-tenant-configurations}

[!DNL AEM] Les ressources [!DNL Brand Portal] permettent aux entreprises de configurer les fonctionnalités suivantes pour des destinataires spécifiques :

* Suppression des ressources par les administrateurs
* Public [!UICONTROL collection] creation by non-admin users
* Public smart [!UICONTROL collection] creation by non-admin users
* Accélération des téléchargements
* Hiérarchie parente des dossiers partagés visible pour les utilisateurs non-administrateurs

These configurations have been provided as **General Settings** configurations on the administrative tools panel.

![](assets/general-configs.png)

**** Configuration permettant aux administrateurs de supprimer des fichiers [!DNL Brand Portal]. (activée par défaut)

**Configuration B** pour permettre aux utilisateurs non administrateurs de créer [!UICONTROL des collections publiques]. (La valeur par défaut est activée)

**Configuration C** pour permettre aux utilisateurs non administrateurs de créer des collections dynamiques [!UICONTROL publiques]. (La valeur par défaut est activée)

**Configuration D** pour permettre l'accélération de téléchargement des fichiers téléchargés depuis le portail et depuis les liens partagés. (désactivée par défaut)

**E** Configuration pour afficher la hiérarchie de dossiers (à partir de la racine) des dossiers partagés pour les utilisateurs non administrateurs (éditeurs, observateurs et utilisateurs invités). (désactivée par défaut)

## Activation/désactivation des configurations générales {#enable-disable-general-configurations}

Pour activer/désactiver chacune de ces configurations :

1. Connectez-vous avec les privilèges d’administrateur.
2. Select the [!DNL AEM] logo to access administrative tools, from the toolbar at the top.
3. From the administrative tools panel, select **General** to open the **General Settings** page.
4. Utilisez le commutateur respectif pour activer/désactiver chacune des configurations générales.
5. **Enregistrez les modifications.**
6. Déconnectez-vous pour que les modifications soient appliquées.

## Allow admin users to delete assets from [!DNL Brand Portal] {#allow-admin-users-to-delete-assets-from-brand-portal}

**Autoriser les utilisateurs à supprimer** la configuration permet aux entreprises d'autoriser (ou limiter) les utilisateurs disposant de droits d'administrateur à supprimer des fichiers et des dossiers [!DNL Brand Portal].

## Autorisation de la création de collections publiques par les utilisateurs non administrateurs {#allow-public-collections-creation-by-non-admins}

[Autoriser la création de [!UICONTROL collections]publiques] (../using/brand-portal-share-[!UICONTROL collection]. md # main-pars-text -1915052376) Contrôle si les administrateurs peuvent créer [!UICONTROL des collections publiques]sur [!DNL Brand Portal]. La configuration est activée par défaut. By disabling the configuration organizations can prevent having numerous public [!UICONTROL collection]s on their portal so that system space can be saved.

## Autorisation de la création de collections dynamiques publiques par les utilisateurs non-administrateurs {#allow-public-smart-collections-creation-by-non-admins}

[La configuration de la création](../using/brand-portal-searching.md#main-pars-header-500620467) de collections dynamiques publiques contrôle si les non-administrateurs peuvent enregistrer leurs recherches en [!UICONTROL tant que collections] dynamiques et les rendre publiques pour ce client. La configuration est activée par défaut. By disabling the configuration organizations can prevent having a huge number of public smart [!UICONTROL collections] created by non-admin users on organization's [!DNL Brand Portal].

## Autorisation de l’accélération des téléchargements {#allow-download-acceleration}

La configuration [Autoriser l’accélération des téléchargements](../using/accelerated-download.md)[!DNL Brand Portal] permet aux organisations d’autoriser l’accélération des téléchargements des ressources à partir de et des liens partagés, grâce à l’intégration à IBM Aspera Connect, une application qui s’installe à la demande. L’application utilise une technologie propriétaire pour supprimer les en-têtes TCP.

## Activation de la hiérarchie de dossiers {#enable-folder-hierarchy}

La configuration [Activer la hiérarchie de dossiers](../using/brand-portal-sharing-folders.md#non-admin-user-access-to-shared-folders) permet aux administrateurs de contrôler la façon dont les utilisateurs non-administrateurs (éditeurs, observateurs et utilisateurs invités) voient les dossiers partagés après connexion.
