---
title: Notes de mise à jour
seo-title: Release Notes
description: Découvrez les fonctionnalités, les améliorations, les problèmes critiques résolus et les problèmes connus de la version Adobe Experience Manager Assets Brand Portal 2022.02.0.
seo-description: Get an insight into the enhancements, critical issues fixed, and known issues in the Adobe Experience Manager Assets Brand Portal 2022.02.0 release.
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
exl-id: e4e89080-9863-4857-8f3a-fcd516ef3271
source-git-commit: 12187c4a98e1541be27b06eefedb1b654c5fb083
workflow-type: tm+mt
source-wordcount: '537'
ht-degree: 60%

---

# Notes de mise à jour {#release-notes}

Découvrez les nouvelles fonctionnalités, les améliorations, les problèmes critiques résolus et les problèmes connus de la version Adobe Experience Manager Assets Brand Portal 2022.02.0.

## Informations sur la version {#release-information}

| Produit | Adobe Experience Manager Assets Brand Portal |
|---|---|
| Version | 2022.02.0 |
| Date  | Février 2022 |

## Présentation {#overview}

Adobe Experience Manager (AEM) Assets Brand Portal permet d’acquérir, de contrôler et de distribuer facilement et en toute sécurité des ressources créatives approuvées destinées à des tiers externes et aux collaborateurs de l’entreprise sur différents appareils. Brand Portal améliore l’efficacité du partage des ressources, accélère la mise sur le marché des ressources et réduit les risques de non-conformité et d’accès non autorisé. Brand Portal permet aux utilisateurs de parcourir, rechercher, prévisualiser, télécharger et exporter des ressources dans des formats approuvés, à tout moment et n’importe où.

## Nouveautés de la version 2022.02.0 {#whats-new-in-2022.02.0}

<!--
### New Features {#new-features}

This release includes the following new features:

* AEM Assets as a Cloud Service is now entitled to have a pre-configured Brand Portal instance. The Cloud Manager user can activate Brand Portal on the AEM Assets as a Cloud Service instance.

* Asset Sourcing feature is now available on AEM Assets as a Cloud Service. It allows the Brand Portal users to upload assets to the permitted contribution folders and publish the contribution folder from Brand Portal to AEM Assets as a Cloud Service instance. 

* An additional **[!UICONTROL Asset Download]** setting has been introduced under the **[!UICONTROL Download Settings]**. It creates a separate folder for each asset while downloading the folders, collections, or bulk download of assets. 
-->
<!-- 
* The **[!UICONTROL Download]** dialog is revamped in a list view with additional options to exclude the renditions which are not required, apply the same set of rules for similar asset types, and download the selected asset renditions.
-->

<!--
* The new **[!UICONTROL Download]** dialog now appears with all the renditions of the selected assets or folders containing assets in a list view, wherein the Brand Portal users can apply same set of renditions for similar asset types and download the selected asset renditions. 
-->

<!-- 
* Navigation to the **[!UICONTROL Files]**, **[!UICONTROL Collections]**, and **[!UICONTROL Shared Links]** is now possible from all the Brand Portal pages in one-click.  

* The **[!UICONTROL Renditions]** panel in the asset details page now allows the Brand Portal users to select the original asset and (or) specific asset renditions, and directly download them from the **[!UICONTROL Renditions]** panel without having to open the **[!UICONTROL Download]** dialog.
-->

<!--
Brand Portal users can exclude specific renditions which are not required and directly download the original asset and its renditions from the **[!UICONTROL Renditions]** panel on the asset details page. 
-->

<!-- 
* In addition to the existing **[!UICONTROL Download]** configurations, the Brand Portal administrators can also [configure permissions for different group of users]() to view and (or) download the original asset and its renditions from the asset details page. These configurations will define who can access and (or) download the asset renditions.
-->

<!--
### Enhancements {#enhancements}

Brand Portal 2021.08.0 is an internal release that introduces Business profiles for enterprise and teams customers to give organizations better control over their assets. 

This release includes the following enhancements:

* The users now have organization-specific entitlement on the new and migrated organizations. If a user is entitled to multiple organizations, the user has to select the organization at the time of login.

* The new users that are added in Admin Console must **Join Team** to get entitled to the organization. 

>[!NOTE]
>
>Business profiles are currently applicable for the new organizations that are created after August 16, 2021. 
>
>Until your organization is migrated, you can continue to use Adobe ID, Enterprise ID, or Federated ID types to access the organization.   
-->

<!-- 
* For folder download, a separate folder is created for each asset using share link irrespective of the **[!UICONTROL Download Settings]**. 
* The Brand Portal **[!UICONTROL Usage Report]** has been modified to reflect only the active Brand Portal users.
-->

<!--
* The threshold of session timeout for the guest users has been reduced from 2 hours to 15 minutes.
* The additional **[!UICONTROL View pages]** option has been removed for multi-page PDFs as the user can now view the PDF pages from the Adobe Document Cloud Viewer.
-->


### Problèmes critiques résolus {#critical-issues-fixed}

Cette version comprend des correctifs pour les problèmes critiques suivants :

* Les utilisateurs ne peuvent pas rechercher, parcourir ou ouvrir des dossiers. L’interface utilisateur reflète le message d’erreur : `Failed to load data`.
* Le **[!UICONTROL Rendus]** ne répertorie pas tous les rendus statiques des ressources publiées sur Brand Portal.
* Le **[!UICONTROL Rendus]** Le panneau répertorie les rendus de recadrage intelligent de la ressource. Cependant, l’utilisateur ne peut pas prévisualiser ni télécharger les rendus de recadrage intelligent.
* La boîte de dialogue de téléchargement répertorie les rendus de recadrage intelligent de la ressource sélectionnée. Cependant, l’utilisateur ne peut pas télécharger les rendus de recadrage intelligent.
* Un utilisateur non administrateur obtient uniquement le rendu de ressource d’origine lors du téléchargement d’une ressource. Les rendus système et personnalisés ne sont pas téléchargés.
* Lors de l’application d’un filtre de recherche pour télécharger une ressource, la variable `Download` est désactivé dans la boîte de dialogue de téléchargement et ne permet pas à l’utilisateur de télécharger la ressource.
* If `Smart Tags` et (ou) `Color Tags` sont activés, la boîte de dialogue de téléchargement répertorie les `json` fichiers en tant que rendus et téléchargements de ces `json` dans le dossier zip archivé.
* Les utilisateurs anonymes ne peuvent pas télécharger de ressources à l’aide d’un lien partagé, car le lien redirige vers la page de connexion de Brand Portal.
* Le système ne reflète pas la valeur correcte pour le nombre d’utilisateurs simultanés principaux.


<!--
* Asset Sourcing email notifications are not delivered for some organizations. 

* Video files with extension `.mov` are not running on Brand Portal. 

* In the **[!UICONTROL Smart Collections]** dropdown list, only ten saved collections are visible. 
-->
<!--
* *_deleted tenants are listed as valid tenant which fails during the execution of TenantCustomizers/TenantUpdates where tenant id is returned as /etc/tenants/`<nodename>`.
-->

<!--
In case only the original assets are downloaded, the asset reflects its own extension and does not open until the extension is manually changed to zip. 
* The user interface of the collection folder does not respond on clicking the navigation arrow. 
* **[!UICONTROL Create]** button is visible in the **[!UICONTROL Column]** view even when the folders are empty.
* **[!UICONTROL Omni search]** fails with a 414 error message (Request-URI Too Long) if the dispatcher is bypassed while accessing the Brand Portal instance.
* An empty zip folder is downloaded if the asset contains a comma (`,`) in the file name.
* The viewer users get the option to add users to the collection they have created. 
* Inconsistent behavior is experienced when an asset (thumbnail or web rendition) is downloaded using share link.

See [what's new in Brand Portal 2021.02.0](whats-new.md).
-->


### Problèmes connus {#known-issues}

Cette version présente les problèmes connus suivants :

* Les utilisateurs ne peuvent pas se connecter à Brand Portal lors de la migration de leur organisation existante.

   Toutefois, les principaux utilisateurs connectés à Brand Portal peuvent continuer à travailler jusqu’à l’expiration de leur session en cours.

* Lorsque vous naviguez de Brand Portal vers Admin Console, les administrateurs peuvent voir un écran supplémentaire pour sélectionner l’organisation.

* If `Color Tags` sont activés et l’utilisateur télécharge un dossier ou une collection, une `xml` est téléchargé pour chaque ressource du dossier (ou collection) dans le dossier zip archivé.


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

* Advances in the asset download process which improves the Brand Portal user experience while [downloading assets from Brand Portal](download-assets.md). Brand Portal administrators can configure **[!UICONTROL Fast Download]**, **[!UICONTROL Custom Renditions]**, and **[!UICONTROL System Renditions]** from the **[!UICONTROL Download]** settings. 

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
* Portugais  brésilien
* Japonais
* Chinois simplifié
* Coréen

## Plates-formes certifiées {#certified-platforms}

Pour vérifier quelles sont les plates-formes certifiées pour exécuter cette version de Brand Portal, reportez-vous à la colonne **Prise en charge de l’interface utilisateur optimisée pour les écrans tactiles** du tableau **Navigateurs pris en charge pour l’interface utilisateur de création** dans la section [Exigences techniques](https://experienceleague.adobe.com/docs/experience-manager-65/deploying/introduction/technical-requirements.html?lang=fr).

## Liens {#links}

* [Page du produit Adobe Experience Manager sur adobe.com](https://business.adobe.com/fr/products/experience-manager/adobe-experience-manager.html)
* [Documentation Assets Brand Portal](https://experienceleague.adobe.com/docs/experience-manager-brand-portal/using/home.html?lang=fr)

## Assistance technique et accès au produit (sites à accès limité) {#product-access-and-support-restricted-sites}

Ces sites sont réservés aux clients. Si vous êtes client et avez besoin d’un accès, contactez votre responsable de compte Adobe.

<!--
* [https://daycare.day.com](https://daycare.day.com) 
-->

<!--
* [Customer Support]()
-->
