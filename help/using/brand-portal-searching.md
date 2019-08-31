---
title: Recherche de ressources sur Brand Portal
seo-title: Recherche de ressources et recherche enregistrée sur AEM Brand Portal
description: La fonctionnalité de recherche de Brand Portal vous permet de rechercher rapidement des ressources appropriées au moyen de l’omni-recherche, et les filtres de recherche vous aident à affiner encore davantage votre recherche. Enregistrez vos recherches sous la forme de collections dynamiques pour une utilisation ultérieure.
seo-description: La fonctionnalité de recherche de Brand Portal vous permet de rechercher rapidement des ressources appropriées au moyen de l’omni-recherche, et les filtres de recherche vous aident à affiner encore davantage votre recherche. Enregistrez vos recherches sous la forme de collections dynamiques pour une utilisation ultérieure.
uuid: c 2955198-bdc 0-4853-a 13 a -661 e 6 a 9 ec 61 f
contentOwner: bdhar
content-type: référence
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
topic-tags: Searchandpromote
discoiquuid: dc 751 cd 7-f 663-46 d 2-84 c 4-5 bb 12 a 4 fe 1 ba
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Recherche de ressources sur Brand Portal {#search-assets-on-brand-portal}

La fonctionnalité de recherche de Brand Portal vous permet de rechercher rapidement les ressources appropriées au moyen de  l’omni-recherche, et la recherche facettée qui utilise des filtres vous aident à affiner encore davantage votre recherche. Vous pouvez également enregistrer vos recherches sous la forme de collections dynamiques pour une utilisation ultérieure.

## Recherche de ressources à l’aide de l’omni-recherche {#search-assets-using-omnisearch}

Pour rechercher des fichiers sur le portail de marque :

1. From the toolbar, click the **[!UICONTROL Search]** icon, or press the "**[!UICONTROL /]**" key to launch Omnisearch.

   ![](assets/omnisearchicon-1.png)

2. Dans la zone de recherche, saisissez un mot-clé pour les ressources à rechercher.

   ![](assets/omnisearch.png)

   >[!NOTE]
   >
   >Pour que des suggestions de recherche s’affichent, au moins 3 caractères sont nécessaires dans l’omni-recherche.

3. Pour accéder rapidement aux ressources qui vous intéressent, effectuez un choix parmi les suggestions associées qui apparaissent dans la liste déroulante.

   ![](assets/assets-search-result.png)

   *Recherche de ressources à l’aide de l’omni-recherche*

## Recherche à l’aide des facettes du panneau Filtres {#search-using-facets-in-filters-panel}

Les facettes de recherche du panneau Filtres ajoutent de la granularité à votre expérience de recherche et rendent la fonctionnalité de recherche efficace. Les facettes de recherche utilisent plusieurs dimensions (prédicats) qui permettent d'effectuer des recherches complexes. Vous pouvez facilement descendre dans la hiérarchie jusqu’au niveau de détail souhaité pour une recherche plus précise.

Par exemple, si vous recherchez une image, vous pouvez indiquer si vous souhaitez une image bitmap ou vectorielle. Vous pouvez réduire davantage l’étendue de la recherche en spécifiant le type MIME de l’image dans la facette de recherche Type de fichier. De même, lors de la recherche de documents, vous pouvez spécifier le format, par exemple PDF ou MS Word.

![Panneau Filtres dans le panneau Marque portalfilters](assets/file-type-search.png "du portail de marque")

The [!UICONTROL Filters] panel includes a few standard facets, such as- [!UICONTROL Path Browser], [!UICONTROL File Type], [!UICONTROL File Size], [!UICONTROL Status], and [!UICONTROL Orientation]. However, you can [add custom search facets](../using/brand-portal-search-facets.md) or remove specific search facets from the [!UICONTROL Filters] panel by adding or removing predicates in the underlying Search Form. See the list of the available and usable [search predicates on Brand Portal](../using/brand-portal-search-facets.md#list-of-search-predicates).

To apply filters to your search, using the available [search facets](../using/brand-portal-search-facets.md):

1. Click the overlay icon and select **[!UICONTROL Filter]**.

   ![](assets/selectorrail.png)

2. Dans le panneau **[!UICONTROL Filtres]à gauche, sélectionnez les options adéquates pour appliquer les filtres correspondants.**
 Par exemple, utilisez les filtres standard suivants :

   * **[!UICONTROL Explorateur de chemin d'accès]** pour rechercher des fichiers dans un répertoire spécifique. The default search path of the predicate for Path Browser is **[!UICONTROL /content/dam/mac/&lt;tenant-id&gt;/]**, which can be configured by editing the default search form.
   >[!NOTE]
   >
   >To non-admin users, [!UICONTROL Path Browser] in [!UICONTROL Filter] panel shows only the content structure of the folders (and their ancestor folders) shared with them.\
   >Pour les administrateurs, le navigateur de chemins permet de naviguer vers n'importe quel dossier de Brand Portal.

   * **[!UICONTROL Type de fichier]** pour spécifier le type (image, document, multimédia, archive) du fichier de fichiers que vous recherchez. En outre, vous pouvez réduire l’étendue de votre recherche. Par exemple, spécifiez le type MIME (Tiff, Bitmap, Images GIMP) de l’image ou le format (PDF ou MS Word) des documents.
   * **[!UICONTROL Taille du fichier]** pour rechercher des fichiers en fonction de leur taille. Vous pouvez spécifier les limites inférieure et supérieure pour la plage de tailles afin d’affiner votre recherche et de spécifier l’unité de mesure à rechercher.
   * **[!UICONTROL Etat]** de recherche des ressources en fonction des états des ressources (Approbation approuvée, Modifications demandées, Rejetées, En attente) et Expiration.
   * **[!UICONTROL Note moyenne]** pour rechercher des fichiers en fonction de la note des ressources.
   * **[!UICONTROL Orientation]** pour rechercher des fichiers en fonction de l'orientation (horizontale, verticale, carrée) des ressources.
   * **[!UICONTROL Style]** pour rechercher des ressources en fonction de leur style (couleur, monochrome).
   * **[!UICONTROL Format vidéo]** pour rechercher des ressources vidéo en fonction de leur format (DVI, Flash, MPEG4, MPEG, OGG Theora, QuickTime, Windows Media, WebM).
   Vous pouvez utiliser des [facettes de recherche personnalisées](../using/brand-portal-search-facets.md) dans le panneau Filtres en modifiant le formulaire de recherche sous-jacent.

   * **[!UICONTROL S’il est utilisé dans le formulaire de recherche, le prédicat de propriété]** permet de rechercher des ressources qui correspondent à une propriété de métadonnées sur laquelle est mappée le prédicat.\
      Par exemple, si l'attribut Propriété est mappé sur [!UICONTROL `jcr:content /metadata/dc:title`], vous pouvez rechercher des fichiers en fonction de leur titre.\
      Le prédicat [!UICONTROL de propriété] prend en charge les recherches de texte pour :

      **Expressions partielles**
Pour permettre la recherche de ressources à l’aide des expressions partielles dans le prédicat de propriété, cochez la case **[!UICONTROL Recherche partielle]dans le formulaire de recherche.**\
      Cela vous permet de rechercher les ressources souhaitées même si vous ne spécifiez pas les mots/expressions exacts utilisés dans les métadonnées de la ressource.\
      Vous pouvez :
* Indiquez un mot survenant dans votre expression recherchée dans la facette du panneau Filtres. For example, if you search for the term **climb** (and Property Predicate is mapped to [!UICONTROL `dc:title`] property), then all the assets with the word **climb** in their title phrase are returned.
* Spécifier une partie du mot apparaissant dans l’expression recherchée, ainsi qu’un caractère générique (*) pour remplir les trous.
Par exemple, la recherche de :
      **escalade *** renvoie tous les actifs dont les mots commencent par les caractères « escalade » dans leur expression de titre.
      *** renvoie** tous les actifs dont les mots se terminent par des caractères « escalade » dans leur expression de titre.
      *** ascen*** renvoie tous les actifs dont les mots contiennent les caractères « escalade » dans leur expression de titre.\
      **Texte
sensible à la casse** Pour autoriser la recherche sensible à la casse dans l'attribut de propriété, activez la case à cocher **[!UICONTROL Ignorer la casse]** dans le formulaire de recherche. Par défaut, la recherche de texte sur le prédicat de propriété est sensible à la casse.
   >[!NOTE]
   >
   >Lorsque vous cochez la case **[!UICONTROL Recherche partielle]**, l’option [!UICONTROL Ignorer la casse] est sélectionnée par défaut.

   ![](assets/wildcard-prop-1.png)

   Les résultats de la recherche sont affichés en fonction des filtres appliqués, avec le nombre de résultats.

   ![](assets/omnisearch-with-filters.png)

   Résultat de la recherche de ressources avec le nombre de résultats

3. Vous pouvez facilement accéder à un élément à partir d’un résultat de recherche et revenir au même résultat à l’aide du bouton Précédent de votre navigateur sans avoir à relancer la requête de recherche.

## Enregistrement d’une recherche en tant que collection dynamique {#save-your-searches-as-smart-collection}

Vous pouvez enregistrer les paramètres d’une recherche comme collection dynamique pour répéter rapidement la même recherche sans avoir à redéfinir les mêmes paramètres.

Pour enregistrer les paramètres de recherche comme collection dynamique :

1. Tap/ click **[!UICONTROL Save Smart Collection]** and provide a name for the smart collection.

   Pour rendre la collection dynamique accessible à tous les utilisateurs, cochez **[!UICONTROL Public]**. Un message confirme que la collection dynamique a été créée et ajoutée à la liste de vos recherches enregistrées.

   >[!NOTE]
   >
   >Vous pouvez empêcher les utilisateurs non-administrateurs de rendre des collections dynamiques publiques pour éviter que le Brand Portal de l’organisation présente un nombre très important de collections dynamiques publiques créées par les utilisateurs non-administrateurs. Organizations can disable the **[!UICONTROL Allow public smart collections creation]** configuration from **[!UICONTROL General]** settings available in admin tools panel.

   ![](assets/save_smartcollectionui.png)

2. To save the smart collection in a different name, and select or clear the **[!UICONTROL Public]** checkbox, click **[!UICONTROL Edit Smart Collection]**.

   ![](assets/edit_smartcollection.png)

3. Dans la boîte de dialogue **[!UICONTROL Modif. collecte dynam.]**, sélectionnez **Enregistrer sous]et saisissez le nom de la collection dynamique.[!UICONTROL ** Cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/saveas_smartsearch.png)
