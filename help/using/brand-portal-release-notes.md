---
title: Notes de mise à jour
seo-title: Notes de mise à jour
description: Découvrez les fonctionnalités, les améliorations, les problèmes critiques résolus et les problèmes connus de la version Adobe Experience Manager Assets Brand Portal 2021.02.0.
seo-description: Découvrez les améliorations, les problèmes critiques résolus et les problèmes connus de la version Adobe Experience Manager Assets Brand Portal 2021.02.0.
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
translation-type: tm+mt
source-git-commit: 59eeaedd7f66a0a5affa53f82f3ebbb2bcea535d
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 54%

---


# Notes de mise à jour {#release-notes}

Découvrez les fonctionnalités, les améliorations, les problèmes critiques résolus et les problèmes connus de la version Adobe Experience Manager Assets Brand Portal 2021.02.0.

## Informations sur la version {#release-information}

| Produit | Adobe Experience Manager Assets Brand Portal |
|---|---|
| Version | 2021.02.0 |
| Date |  février 2021 |

## Présentation {#overview}

Adobe Experience Manager (AEM) Assets Brand Portal permet d’acquérir, de contrôler et de distribuer facilement et en toute sécurité des ressources créatives approuvées destinées à des tiers externes et aux collaborateurs de l’entreprise sur différents appareils. Brand Portal améliore l’efficacité du partage des ressources, accélère la mise sur le marché des ressources et réduit les risques de non-conformité et d’accès non autorisé. Brand Portal permet aux utilisateurs de parcourir, rechercher, prévisualiser, télécharger et exporter des ressources dans des formats approuvés, à tout moment et n’importe où.

## Nouveautés de la version 2021.02.0 {#whats-new-in-2021.02.0}

### Nouvelles fonctionnalités {#new-features}

Cette version comprend les nouvelles fonctionnalités suivantes :

* AEM Assets en tant que Cloud Service est automatiquement configuré avec le portail des marques en activant le portail des marques à partir de Cloud Manager.

* La fonction d’origine des ressources est désormais disponible en Cloud Service sur AEM Assets. Il permet aux utilisateurs du portail de marque de télécharger des fichiers vers les dossiers de contribution autorisés et de publier le dossier de contribution de Brand Portal vers AEM Assets en tant qu’instance Cloud Service.

* Un autre paramètre **[!UICONTROL Téléchargement de fichier]** a été introduit sous **[!UICONTROL Paramètres de téléchargement]**. Il crée un dossier distinct pour chaque fichier lors du téléchargement des dossiers, des collections ou du téléchargement en masse des fichiers.

<!-- 
* The **[!UICONTROL Download]** dialog is revamped in a list view with additional options to exclude the renditions which are not required, apply the same set of rules for similar asset types, and download the selected asset renditions. See [steps to download assets from Brand Portal](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#download-assets).
-->

<!--
* The new **[!UICONTROL Download]** dialog now appears with all the renditions of the selected assets or folders containing assets in a list view, wherein the Brand Portal users can apply same set of renditions for similar asset types and download the selected asset renditions. 
-->

<!-- 
* Navigation to the **[!UICONTROL Files]**, **[!UICONTROL Collections]**, and **[!UICONTROL Shared Links]** is now possible from all the Brand Portal pages in one-click.  

* The **[!UICONTROL Renditions]** panel in the asset details page now allows the Brand Portal users to select the original asset and (or) specific asset renditions, and directly download them from the **[!UICONTROL Renditions]** panel without having to open the **[!UICONTROL Download]** dialog. See [download assets from asset details page](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#download-assets-from-asset-details-page).
-->

<!--
Brand Portal users can exclude specific renditions which are not required and directly download the original asset and its renditions from the **[!UICONTROL Renditions]** panel on the asset details page. 
-->

<!-- 
* In addition to the existing **[!UICONTROL Download]** configurations, the Brand Portal administrators can also [configure permissions for different group of users](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#configure-download-permissions) to view and (or) download the original asset and its renditions from the asset details page. These configurations will define who can access and (or) download the asset renditions.
-->

### Améliorations {#enhancements}

Les améliorations suivantes ont été apportées à cette version :

* Pour le téléchargement de dossier, un dossier distinct est créé pour chaque ressource à l’aide du lien de partage, quel que soit le **[!UICONTROL Paramètres de téléchargement]**.
* Le **[!UICONTROL rapport d’utilisation du portail de marque]** a été modifié pour refléter uniquement les utilisateurs principaux du portail de marque.

<!--
* The threshold of session timeout for the guest users has been reduced from 2 hours to 15 minutes.
* The additional **[!UICONTROL View pages]** option has been removed for multi-page PDFs as the user can now view the PDF pages from the Adobe Document Cloud Viewer.
-->


### Problèmes critiques résolus {#critical-issues-fixed}

Cette version comprend des correctifs pour les problèmes critiques suivants :

* Au cas où seuls les fichiers d’origine seraient téléchargés, le fichier refléterait sa propre extension et ne s’ouvrirait pas tant que l’extension n’a pas été manuellement remplacée par zip.
* L’interface utilisateur du dossier de collecte ne répond pas lorsque vous cliquez sur la flèche de navigation.
* **[!UICONTROL Le]** bouton Créer est visible dans l’ **** affichage Colonne même si les dossiers sont vides.
* **[!UICONTROL La]** recherche Omni échoue avec un message d’erreur 414 (Request-URI Too Long) si le répartiteur est ignoré lors de l’accès à l’instance du portail de marques.
* Un dossier zip vide est téléchargé si le fichier contient une virgule (`,`) dans son nom.
* Les utilisateurs du lecteur de contenu peuvent ajouter des utilisateurs à la collection qu’ils ont créée.
* Un comportement incohérent se produit lorsqu’un fichier (miniature ou rendu Web) est téléchargé à l’aide d’un lien de partage.

Voir [les nouveautés de Brand Portal 2021.02.0](whats-new.md).


### Problèmes connus {#known-issues}

Cette version présente les problèmes connus suivants :

* Les utilisateurs ne reçoivent pas de notifications par courrier électronique pour les workflows de publication Ressource.

<!--
### Known Issues {#known-issues}

This release includes the following known issue:

* Search on the **[!UICONTROL Asset Reports]** shows processing on the product interface with no search result.
* The video DM encodes are not visible to the non-admin users on the asset details page.
* The alignment of the size of individual asset renditions and total download size is distorted in the Download dialog.
-->


<!--
* Download Settings configuration to configure asset download from Brand Portal. Fast download, custom renditions, and system renditions are the available configurations. 
-->

<!--
* Document Viewer has been introduced to enhance the PDF viewing experience. New options are available for viewing the PDF files in Brand Portal.

* Advances in the asset download process which improves the Brand Portal user experience while [downloading assets from Brand Portal](brand-portal-download-assets.md). Brand Portal administrators can configure **[!UICONTROL Fast Download]**, **[!UICONTROL Custom Renditions]**, and **[!UICONTROL System Renditions]** from the **[!UICONTROL Download]** settings. 

For details, see [what's new in Brand Portal 6.4.7](whats-new.md). 

### Critical Issues Fixed {#critical-issues-fixed-647}

This release includes fixes to the following critical issues:

* The viewer users are not permitted to share link for collections but the option to share is visible to them on the product interface.

* The **[!UICONTROL Download]** button on the options bar does not list all the licensed assets of the selected folder.

* The search takes longer to show the results for certain keywords.

* The **[!UICONTROL Agree]** and **[!UICONTROL Disagree]** check boxes does not appear on bulk selection of licensed and unlicensed assets during download.

* Filter-based search shows processing on the product interface with no search result. 

* The assets do not download from share link if the shared folder contains numerous and large assets.


### Known Issues {#known-issues-647}

This release includes the following known issues:

* If multiple assets are selected, license text does not appear on clicking Terms and Conditions on the license agreement page during download using share link.   

-->

## Langues {#languages}

L’interface utilisateur de Brand Portal est disponible dans les langues suivantes :

* Anglais
* Allemand
* Français
* Espagnol
* Italien
* Portugais brésilien
* Japonais
* Chinois simplifié
* Coréen

## Plates-formes certifiées {#certified-platforms}

Pour vérifier quelles sont les plates-formes certifiées pour exécuter cette version de Brand Portal, reportez-vous à la colonne **Prise en charge de l’interface utilisateur optimisée pour les écrans tactiles** du tableau **Navigateurs pris en charge pour l’interface utilisateur de création** dans la section [Exigences techniques](https://helpx.adobe.com/fr/experience-manager/6-4/sites/deploying/using/technical-requirements.html).

## Liens {#links}

* [Page du produit Adobe Experience Manager sur adobe.com](http://www.adobe.com/fr/marketing-cloud/experience-manager.html)
* [Documentation Assets Brand Portal](https://helpx.adobe.com/fr/experience-manager/brand-portal/user-guide.html)

## Assistance technique et accès au produit (sites à accès limité) {#product-access-and-support-restricted-sites}

Ces sites sont réservés aux clients. Si vous êtes client et avez besoin d’un accès, contactez votre responsable de compte Adobe.

<!--
* [https://daycare.day.com](https://daycare.day.com) 
-->

* [Accès aux produits](https://login.marketing.adobe.com)

* [Assistance clientèle d’Adobe](https://helpx.adobe.com/fr/contact.html)
