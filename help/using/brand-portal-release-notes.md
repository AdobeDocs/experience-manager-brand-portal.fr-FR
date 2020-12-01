---
title: Notes de mise à jour
seo-title: Notes de mise à jour
description: Découvrez les fonctionnalités, les améliorations, les problèmes critiques résolus et les problèmes connus de la version Adobe Experience Manager Assets Brand Portal 2020.10.0.
seo-description: Découvrez les améliorations, les problèmes critiques résolus et les problèmes connus de la version Adobe Experience Manager Assets Brand Portal 2020.10.0.
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
translation-type: tm+mt
source-git-commit: 5cf924ce71433e33506449bbad608d5e57a41b8d
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 86%

---


# Notes de mise à jour {#release-notes}

Découvrez les fonctionnalités, les améliorations, les problèmes critiques résolus et les problèmes connus de la version Adobe Experience Manager Assets Brand Portal 2020.10.0.

## Informations sur la version {#release-information}

| Produit | Adobe Experience Manager Assets Brand Portal |
|---|---|
| Version | 2020.10.0 |
| Date | Octobre 2020 |

## Présentation {#overview}

Adobe Experience Manager (AEM) Assets Brand Portal permet d’acquérir, de contrôler et de distribuer facilement et en toute sécurité des ressources créatives approuvées destinées à des tiers externes et aux collaborateurs de l’entreprise sur différents appareils. Brand Portal améliore l’efficacité du partage des ressources, accélère la mise sur le marché des ressources et réduit les risques de non-conformité et d’accès non autorisé. Brand Portal permet aux utilisateurs de parcourir, rechercher, prévisualiser, télécharger et exporter des ressources dans des formats approuvés, à tout moment et n’importe où.

## Nouveautés de la version 2020.10.0 {#whats-new-in-2020.10.0}

### Nouvelles fonctionnalités {#new-features}

Cette version comprend les nouvelles fonctionnalités suivantes :

* La boîte de dialogue **[!UICONTROL Télécharger]** est repensée dans une vue de liste avec des options supplémentaires pour exclure les rendus non requis, appliquer le même ensemble de règles pour des types de ressource similaires et télécharger les rendus de ressource sélectionnés. Voir [étapes de téléchargement des ressources à partir du portail de marque](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#download-assets).

<!--
* The new **[!UICONTROL Download]** dialog now appears with all the renditions of the selected assets or folders containing assets in a list view, wherein the Brand Portal users can apply same set of renditions for similar asset types and download the selected asset renditions. 
-->

* La navigation vers **[!UICONTROL Fichiers]**, **[!UICONTROL Collections]** et **[!UICONTROL Liens partagés]** est désormais possible à partir de toutes les pages de Brand Portal, en un seul clic.

* Le panneau **[!UICONTROL Rendus]** de la page des détails de la ressource permet désormais aux utilisateurs de Brand Portal de sélectionner la ressource d’origine ou des rendus de ressources spécifiques, puis de les télécharger directement à partir du panneau **[!UICONTROL Rendus]** sans avoir à ouvrir la boîte de dialogue **[!UICONTROL Télécharger.]** Voir [téléchargement de ressources à partir de la page des détails des ressources](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#download-assets-from-asset-details-page).

<!--
Brand Portal users can exclude specific renditions which are not required and directly download the original asset and its renditions from the **[!UICONTROL Renditions]** panel on the asset details page. 
-->

* Outre les configurations de **[!UICONTROL téléchargement]** existantes, les administrateurs de Brand Portal peuvent configurer des autorisations pour différents groupes d’utilisateurs afin de voir ou télécharger la ressource d’origine et ses rendus à partir de la page des détails de la ressource. [](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#configure-download-permissions) Ces configurations définissent qui peut accéder aux rendus de ressources ou les télécharger.

### Améliorations {#enhancements}

Les améliorations suivantes ont été apportées à cette version :

* Le délai d’expiration de la session pour les utilisateurs invités est passé de 2 heures à 15 minutes.
* L’option supplémentaire **[!UICONTROL Afficher les pages]** a été supprimée pour les fichiers PDF de plusieurs pages, car l’utilisateur peut désormais afficher les pages PDF à partir du lecteur Adobe Document Cloud.


<!--
### Critical Issues Fixed {#critical-issues-fixed}

This release includes fixes to the following critical issue:

* The users are not able to view the PDF pages if the PDF contains sub assets.
-->

### Problèmes connus {#known-issues}

Cette version présente les problèmes connus suivants :

* La recherche dans les **[!UICONTROL Rapports sur les ressources]** affiche le traitement dans l’interface du produit sans résultat de recherche.
* Les codages vidéo DM ne sont pas visibles pour les utilisateurs non-administrateurs sur la page des détails de la ressource.
* La taille totale du téléchargement n’est pas alignée sur la taille des rendus de ressources individuels dans la boîte de dialogue Télécharger.



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
* Brésilien Portugais
* Japonais
* Chinois simplifié
* Coréen

## Plates-formes certifiées  {#certified-platforms}

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
