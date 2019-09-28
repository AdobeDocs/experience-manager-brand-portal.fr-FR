---
title: Publication de paramètres prédéfinis, de schémas et de facettes sur Brand Portal
seo-title: Publication de paramètres prédéfinis, de schémas et de facettes sur Brand Portal
description: Découvrez comment publier des paramètres prédéfinis, des schémas et des facettes sur Brand Portal.
seo-description: Découvrez comment publier des paramètres prédéfinis, des schémas et des facettes sur Brand Portal.
uuid: c836d9bb-074a-4113-9c91-b2bf7658b88d
topic-tags: 'serveur '
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: référencereference
discoiquuid: bc305abc-9373-4d33-9179-0a5f3904b352
translation-type: tm+mt
source-git-commit: 86d4d5c358ea795e35db2dce8c9529ed14e9ee2d

---


# Publication de paramètres prédéfinis, de schémas et de facettes sur Brand Portal {#publish-presets-schema-and-facets-to-brand-portal}

L’article est consacré à la publication des paramètres d’image prédéfinis, des schémas de métadonnées et des facettes de recherche personnalisées sur Brand Portal à partir de l’instance d’auteur AEM. Publishing capability enables organizations to reuse the image presets, metadata schemas, and search facets created/modified at AEM Author instance thereby reducing duplicate efforts.

>[!NOTE]
>
>La fonction de publication des paramètres d’image prédéfinis, des schémas de métadonnées et des facettes de recherche sur Brand Portal à partir de l’instance d’auteur AEM est disponible à partir d’AEM 6.2 SP1-CFP7 et d’AEM 6.3 SP1-CFP1 (6.3.1.1).

## Publication des paramètres d’image prédéfinis sur Brand Portal {#publish-image-presets-to-brand-portal}

Les paramètres d’image prédéfinis sont un ensemble de commandes de redimensionnement et de formatage qui sont appliqués à l’image au moment de sa livraison. Les paramètres d’image prédéfinis peuvent être créés et modifiés sur Brand Portal. Alternatively, if AEM Author instance is running in dynamic media mode then users can create presets at the AEM Author and publish them to AEM Assets Brand Portal, and avoid re-creating the same presets at Brand Portal.\
Une fois que le paramètre prédéfini est créé, il est répertorié en tant que rendu dynamique sur le rail de rendus des détails de ressources et la boîte de dialogue de téléchargement.

>[!NOTE]
>
>If AEM Author instance is not running in [!UICONTROL Dynamic Media Mode] (customer has not purchased Dynamic Media), then the [!UICONTROL Pyramid TIFF]  rendition of the assets are not created at the time of upload. Image presets or dynamic renditions work on [!UICONTROL Pyramid TIFF] of an asset, so if [!UICONTROL Pyramid TIFF] is not available on AEM Author instance then it is not available on Brand Portal as well. En conséquence, aucun rendu dynamique n’est présent dans le rail de rendus de la page des détails de la ressource et dans la boîte de dialogue de téléchargement.

Pour publier des paramètres d’image prédéfinis sur Brand Portal :

1. In AEM Author instance, tap/ click the AEM logo to access the global navigation console and tap/ click the Tools icon and navigate to **[!UICONTROL Assets]** &gt; **[!UICONTROL Image Presets]**.
1. Sélectionnez un ou plusieurs paramètres d’image prédéfinis dans la liste, puis cliquez/appuyez sur **[!UICONTROL Publier sur Brand Portal]**.

![](assets/publishpreset.png)

>[!NOTE]
>
>Quand les utilisateurs cliquent sur **[!UICONTROL Publier sur Brand Portal]**, les paramètres d’image prédéfinis sont placés en file d’attente pour publication. Nous conseillons aux utilisateurs de surveiller le journal des agents de réplication pour contrôler la réussite de la publication.

To unpublish an image preset from Brand Portal:

1. In AEM Author instance, tap/ click the AEM logo to access the global navigation console and tap/click the **[!UICONTROL Tools]** icon and navigate to **[!UICONTROL Assets &gt; Image Presets]**.
1. Sélectionnez un paramètre d’image prédéfini puis **[!UICONTROL Supprimer de Brand Portal]parmi les options disponibles dans la partie supérieure.**

## Publication d’un schéma de métadonnées sur Brand Portal  {#publish-metadata-schema-to-brand-portal}

Le schéma de métadonnées décrit la mise en page et les propriétés affichées sur la page de propriétés d’une ressource ou de collections.

![](assets/metadata-schema-editor.png) ![](assets/asset-properties-1.png)

Si les utilisateurs ont modifié le schéma par défaut sur l’instance Auteur AEM et sont disposés à utiliser le même schéma que le schéma par défaut sur le portail de marque, ils peuvent simplement publier les formulaires de schéma de métadonnées sur le portail de marque. Dans un tel scénario, le schéma par défaut du portail de marque est remplacé par les schémas par défaut publiés à partir de l’instance Auteur AEM.

Si les utilisateurs ont créé un schéma personnalisé sur l’instance Auteur AEM, ils peuvent le publier sur le portail de marque au lieu de le recréer. Les utilisateurs peuvent alors appliquer ce schéma personnalisé à n’importe quel dossier/collection dans Brand Portal.

>[!NOTE]
>
>Les schémas par défaut ne peuvent pas être publiés sur le portail de marque s’ils sont verrouillés sur l’instance AEM (c’est-à-dire s’ils ne sont pas modifiés).

![](assets/default-schema-form.png)

>[!NOTE]
>
>Si un schéma est appliqué à un dossier sur l’instance d’auteur AEM, il doit également exister sur le portail de marque afin de conserver la cohérence dans la page des propriétés de la ressource sur AEM Author et le portail de marque.

Pour publier un schéma de métadonnées sur Brand Portal à partir d’une instance d’auteur AEM :

1. In AEM Author instance, tap/ click the AEM logo to access the global navigation console and tap/click the Tools icon and navigate to **[!UICONTROL Assets &gt; Metadata Schemas]**.
1. Sélectionnez un schéma de métadonnées puis **[!UICONTROL Publier sur Brand Portal]** parmi les options disponibles dans la partie supérieure.

>[!NOTE]
>
>Quand les utilisateurs cliquent sur **[!UICONTROL Publier sur Brand Portal]**, les schémas de métadonnées sont placés en file d’attente pour publication. Nous conseillons aux utilisateurs de surveiller le journal des agents de réplication pour contrôler la réussite de la publication.

Pour annuler la publication d’un schéma de métadonnées sur Brand Portal :

1. In AEM Author instance, tap/ click the AEM logo to access the global navigation console and tap/click the Tools icon and navigate to **[!UICONTROL Assets &gt; Metadata Schemas]**.
1. Sélectionnez un schéma de métadonnées puis **[!UICONTROL Supprimer de Brand Portal]** parmi les options disponibles dans la partie supérieure.

## Publication de facettes de recherche sur Brand Portal {#publish-search-facets-to-brand-portal}

Les formulaires de recherche fournissent aux utilisateurs la fonctionnalité de [recherche facettée](../using/brand-portal-search-facets.md) sur Brand Portal. Les facettes de recherche donnent une plus grande granularité aux recherches sur le portail de marque. Tous les [prédicats ajoutés](https://helpx.adobe.com/experience-manager/6-5/assets/using/search-facets.html#AddingaPredicate) dans le formulaire de recherche sont disponibles pour les utilisateurs en tant que facettes de recherche dans les filtres de recherche.

![](assets/property-predicate-removed.png)
![](assets/search-form.png)

If you are willing to use custom search form **[!UICONTROL Assets Admin Search Rail]** from AEM Author instance, then instead of re-creating the same form on Brand Portal you can publish the customized search form from AEM Author instance to Brand Portal.

>[!NOTE]
>
>Locked search form **[!UICONTROL Assets Admin Search Rail]** on AEM Assets cannot be published to Brand Portal unless it is edited. Once edited and published to Brand Portal, this search form overrides the search form on Brand Portal.

Pour publier la facette de recherche modifiée sur Brand Portal à partir de l’interface d’auteur AEM :

1. Tap/click the AEM logo, and then go to **[!UICONTROL Tools]** &gt; **[!UICONTROL General]** &gt; **[!UICONTROL Search Forms]**.
1. Sélectionnez le formulaire de recherche modifié et ensuite **[!UICONTROL Publier sur Brand Portal]**.

   >[!NOTE]
   >
   >Quand les utilisateurs cliquent sur **[!UICONTROL Publier sur Brand Portal]**, les facettes de recherche sont placées en file d’attente pour publication. Nous conseillons aux utilisateurs de surveiller le journal des agents de réplication pour contrôler la réussite de la publication.

Pour annuler la publication de formulaires de recherche sur Brand Portal :

1. In AEM Author instance, tap/ click the AEM logo to access the global navigation console and tap/click the Tools icon and navigate to **[!UICONTROL General &gt; Search Forms]**.
1. Sélectionnez le formulaire de recherche et ensuite **[!UICONTROL Supprimer de Brand Portal]** parmi les options disponibles dans la partie supérieure.

>[!NOTE]
>
>L'action **[!UICONTROL Annuler la publication sur Brand Portal]** laisse le formulaire de recherche par défaut sur Brand  Portal et ne rétablit pas le dernier formulaire de recherche utilisé avant la publication.

### Restrictions {#limitations}

1. Peu de prédicats de recherche ne sont pas applicables aux filtres de recherche sur le portail de marque. Quand ces prédicats de recherche sont publiés en tant qu’élément du formulaire de recherche sur Brand Portal à partir de l’instance d’auteur AEM, ils sont filtrés. Les utilisateurs voient donc moins de prédicats dans le formulaire publié sur le portail de marque. Voir [Prédicats de recherche applicables aux filtres sur Brand Portal](../using/brand-portal-search-facets.md#list-of-search-predicates).

1. For [!UICONTROL Options Predicate], if a user is using any custom path to read options at AEM Author instance, it won't work at the Brand Portal. Ces chemins et options supplémentaires ne sont pas publiés sur Brand Portal avec le formulaire de recherche. In this case, users can select the **[!UICONTROL Manual]** option in **[!UICONTROL Add Options]** within **[!UICONTROL Options Predicate]** to add these options manually at Brand Portal.

![](assets/options-predicate-manual.png)
