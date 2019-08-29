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
source-git-commit: 32c3cdb8e3fafd74cfb36e6bcfe0811e7152b2d0

---


# Recherche de ressources sur Brand Portal {#search-assets-on-brand-portal}

[!DNL Brand Portal] La fonction de recherche vous permet de rechercher rapidement des ressources pertinentes à l'aide de la fonction omnisearch et de recherche facettée qui utilise des filtres pour vous aider à réduire davantage la recherche. You can also save your searches as smart [!UICONTROL collections] for the future.

## Recherche de ressources à l’aide de l’omni-recherche {#search-assets-using-omnisearch}

To search for assets on [!DNL Brand Portal]:

1. From the toolbar, click the **Search** icon, or press the "**/**" key to launch Omnisearch.

   ![](assets/omnisearchicon-1.png)

2. Dans la zone de recherche, saisissez un mot-clé pour les ressources à rechercher.

   ![](assets/omnisearch.png)

   >[!NOTE]
   >
   >Pour que des suggestions de recherche s’affichent, au moins 3 caractères sont nécessaires dans l’omni-recherche.

3. Pour accéder rapidement aux ressources qui vous intéressent, effectuez un choix parmi les suggestions associées qui apparaissent dans la liste déroulante.

   ![](assets/assets-search-result.png)

   Recherche de ressources à l’aide de l’omni-recherche

## Recherche à l’aide des facettes du panneau Filtres {#search-using-facets-in-filters-panel}

Les facettes de recherche du panneau Filtres ajoutent de la granularité à votre expérience de recherche et rendent la fonctionnalité de recherche efficace. Les facettes de recherche utilisent plusieurs dimensions (prédicats) qui permettent d'effectuer des recherches complexes. Vous pouvez facilement descendre dans la hiérarchie jusqu’au niveau de détail souhaité pour une recherche plus précise.

Par exemple, si vous recherchez une image, vous pouvez indiquer si vous souhaitez une image bitmap ou vectorielle. Vous pouvez réduire davantage l’étendue de la recherche en spécifiant le type MIME de l’image dans la facette de recherche Type de fichier. De même, lors de la recherche de documents, vous pouvez spécifier le format, par exemple PDF ou MS Word.

![Panneau Filtres dans [!DNL Brand Portal]](assets/file-type-search.png "le panneau Filtres de [! DNL Brand Portal]")

Le panneau Filtres contient des facettes standard (Explorateur de chemins d’accès, Type de fichier, Taille de fichier, État et Orientation, par exemple). However, you can [add custom search facets](../using/brand-portal-search-facets.md) or remove specific search facets from the **Filters** panel by adding or removing predicates in the underlying Search Form. See the list of the available and usable [search predicates on Brand Portal](../using/brand-portal-search-facets.md#list-of-search-predicates).

To apply filters to your search, using the available [search facets](../using/brand-portal-search-facets.md):

1. Click the overlay icon and select **Filter**.

   ![](assets/selectorrail.png)

2. Dans le panneau **Filtres** à gauche, sélectionnez les options adéquates pour appliquer les filtres correspondants.
 Par exemple, utilisez les filtres standard suivants :

   * **Explorateur de chemin d'accès** pour rechercher des fichiers dans un répertoire spécifique. The default search path of the predicate for Path Browser is */content/dam/mac/&lt;tenant-id&gt;/*, which can be configured by editing the default search form.
   >[!NOTE]
   >
   >Pour les utilisateurs non administrateurs, le navigateur de chemins dans le panneau Filtre affiche uniquement la structure de contenu des dossiers (et leurs dossiers ancêtres) partagés avec eux.\
   >To admin users, Path Browser allows navigating to any folder in [!DNL Brand Portal].

   * **Type de fichier** pour spécifier le type (image, document, multimédia, archive) du fichier de fichiers que vous recherchez. En outre, vous pouvez réduire l’étendue de votre recherche. Par exemple, spécifiez le type MIME (Tiff, Bitmap, Images GIMP) de l’image ou le format (PDF ou MS Word) des documents.
   * **Taille du fichier** pour rechercher des fichiers en fonction de leur taille. Vous pouvez spécifier les limites inférieure et supérieure pour la plage de tailles afin d’affiner votre recherche et de spécifier l’unité de mesure à rechercher.
   * **Etat** de recherche des ressources en fonction des états des ressources (Approbation approuvée, Modifications demandées, Rejetées, En attente) et Expiration.
   * **Note moyenne** pour rechercher des fichiers en fonction de la note des ressources.
   * **Orientation** pour rechercher des fichiers en fonction de l'orientation (horizontale, verticale, carrée) des ressources.
   * **Style** pour rechercher des ressources en fonction de leur style (couleur, monochrome).
   * **Format vidéo** pour rechercher des ressources vidéo en fonction de leur format (DVI, Flash, MPEG4, MPEG, OGG Theora, QuickTime, Windows Media, WebM).
   Vous pouvez utiliser des [facettes de recherche personnalisées](../using/brand-portal-search-facets.md) dans le panneau Filtres en modifiant le formulaire de recherche sous-jacent.

   * S’il est utilisé dans le formulaire de recherche, le **prédicat de propriété** permet de rechercher des ressources qui correspondent à une propriété de métadonnées sur laquelle est mappée le prédicat.\
      Par exemple, si l'attribut Propriété est mappé sur `jcr:content /metadata/dc:title`, vous pouvez rechercher des fichiers en fonction de leur titre.\
      Le prédicat de propriété prend en charge les recherches de texte pour :

      **Expressions partielles**
Pour permettre la recherche de ressources à l’aide des expressions partielles dans le prédicat de propriété, cochez la case **Recherche partielle** dans le formulaire de recherche.\
      Cela vous permet de rechercher les ressources souhaitées même si vous ne spécifiez pas les mots/expressions exacts utilisés dans les métadonnées de la ressource.\
      Vous pouvez :
* Indiquez un mot survenant dans votre expression recherchée dans la facette du panneau Filtres. For example, if you search for the term **climb** (and Property Predicate is mapped to `dc:title` property), then all the assets with the word **climb** in their title phrase are returned.
* Spécifier une partie du mot apparaissant dans l’expression recherchée, ainsi qu’un caractère générique (*) pour remplir les trous.
Par exemple, la recherche de :
      **escalade *** renvoie tous les actifs dont les mots commencent par les caractères « escalade » dans leur expression de titre.
      *** renvoie** tous les actifs dont les mots se terminent par des caractères « escalade » dans leur expression de titre.
      *** ascen*** renvoie tous les actifs dont les mots contiennent les caractères « escalade » dans leur expression de titre.\
      **Texte
sensible à la casse** Pour autoriser la recherche sensible à la casse dans l'attribut de propriété, activez la case à cocher **Ignorer la casse** dans le formulaire de recherche. Par défaut, la recherche de texte sur le prédicat de propriété est sensible à la casse.
   >[!NOTE]
   >
   >Lorsque vous cochez la case **Recherche partielle**, l’option **Ignorer la casse** est sélectionnée par défaut.

   ![](assets/wildcard-prop-1.png)

   Les résultats de la recherche sont affichés en fonction des filtres appliqués, avec le nombre de résultats.

   ![](assets/omnisearch-with-filters.png)

   Résultat de la recherche de ressources avec le nombre de résultats

3. Vous pouvez facilement accéder à un élément à partir d’un résultat de recherche et revenir au même résultat à l’aide du bouton Précédent de votre navigateur sans avoir à relancer la requête de recherche.

## Enregistrement d’une recherche en tant que collection dynamique {#save-your-searches-as-smart-collection}

Vous pouvez enregistrer les paramètres d’une recherche comme collection dynamique pour répéter rapidement la même recherche sans avoir à redéfinir les mêmes paramètres.

Pour enregistrer les paramètres de recherche comme collection dynamique :

1. Tap/ click **Save Smart Collection** and provide a name for the smart collection.

   Pour rendre la collection dynamique accessible à tous les utilisateurs, cochez **Public**. Un message confirme que la collection dynamique a été créée et ajoutée à la liste de vos recherches enregistrées.

   >[!NOTE]
   >
   >Non-admin users can be restricted from making smart [!UICONTROL collections] public, to avoid having a huge number of public smart [!UICONTROL collections] created by non-admin users on organization's [!DNL Brand Portal]. Organizations can disable the **Allow public smart[!UICONTROL collections]creation** configuration from **General** settings available in admin tools panel.

   ![](assets/save_smartcollectionui.png)

1. Pour enregistrer la collection dynamique sous un autre nom, cochez ou décochez la case **Public**, puis cliquez sur **Modif. collecte dynam.**.

   ![](assets/edit_smartcollection.png)

1. Dans la boîte de dialogue **Modif. collecte dynam.**, sélectionnez **Enregistrer sous** et saisissez le nom de la collection dynamique. Cliquez sur **Enregistrer**.

   ![](assets/saveas_smartsearch.png)
