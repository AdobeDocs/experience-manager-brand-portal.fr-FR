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
source-git-commit: 2931e19289ad8a722e3bb952e39f25b374f743c4
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 59%

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

* La boîte de dialogue **[!UICONTROL Télécharger]** est repensée dans une vue de liste avec des options supplémentaires pour exclure les rendus qui ne sont pas requis, appliquer le même ensemble de règles pour des types de ressource similaires et télécharger les rendus de ressource sélectionnés.

<!--
* The new **[!UICONTROL Download]** dialog now appears with all the renditions of the selected assets or folders containing assets in a list view, wherein the Brand Portal users can apply same set of renditions for similar asset types and download the selected asset renditions. 
-->

* La navigation vers les **[!UICONTROL fichiers]**, les **[!UICONTROL collections]** et les liens **** partagés est désormais possible à partir de toutes les pages du portail de marque en un seul clic.

* Le panneau **[!UICONTROL Rendus]** de la page des détails de la ressource permet désormais aux utilisateurs du portail de la marque de sélectionner la ressource d’origine et (ou) des rendus de ressources spécifiques, puis de les télécharger directement à partir du panneau **[!UICONTROL Rendus]** sans avoir à ouvrir la boîte de dialogue **[!UICONTROL Télécharger]** .

<!--
Brand Portal users can exclude specific renditions which are not required and directly download the original asset and its renditions from the **[!UICONTROL Renditions]** panel on the asset details page. 
-->

* Outre les configurations de **[!UICONTROL téléchargement]** existantes, les administrateurs du portail de marque peuvent également configurer des autorisations pour différents groupes d’utilisateurs sur la vue et (ou) télécharger la ressource d’origine et ses rendus à partir de la page des détails de la ressource. Ces configurations définissent qui peut accéder et (ou) télécharger les rendus de ressources.


### Problèmes critiques résolus {#critical-issues-fixed}

Cette version comprend des correctifs pour le problème critique suivant :

* Les utilisateurs ne peuvent pas vue les pages PDF si le PDF contient des sous-ressources.


### Problèmes connus {#known-issues}

Cette version comprend le problème connu suivant :

* Si l’utilisateur télécharge la ressource à l’aide du lien de partage, la ressource d’origine est téléchargée même lorsque l’option **[!UICONTROL Autoriser le téléchargement du fichier]** d’origine est désactivée.



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
* Brésilien   Portugais
* Japonais
* Chinois simplifié
* Coréen

## Plates-formes certifiées   {#certified-platforms}

Pour vérifier quelles sont les plates-formes certifiées pour exécuter cette version de Brand Portal, reportez-vous à la colonne **Prise en charge de l’interface utilisateur optimisée pour les écrans tactiles** du tableau **Navigateurs pris en charge pour l’interface utilisateur de création** dans la section [Exigences techniques](https://helpx.adobe.com/fr/experience-manager/6-4/sites/deploying/using/technical-requirements.html).

## Liens {#links}

* [Page du produit Adobe Experience Manager sur adobe.com](http://www.adobe.com/fr/marketing-cloud/experience-manager.html)
* [Documentation Assets Brand Portal](https://helpx.adobe.com/fr/experience-manager/brand-portal/user-guide.html)

## Assistance technique et accès au produit (sites à accès limité) {#product-access-and-support-restricted-sites}

Ces sites sont réservés aux clients. Si vous êtes client et avez besoin d’un accès, contactez votre responsable de compte Adobe.

* [https://daycare.day.com](https://daycare.day.com)

* [Accès aux produits](https://login.marketing.adobe.com)

* [Assistance clientèle d’Adobe](https://helpx.adobe.com/fr/contact.html)
