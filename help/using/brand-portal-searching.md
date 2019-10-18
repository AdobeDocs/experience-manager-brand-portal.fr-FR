---
title: Recherche de ressources sur Brand Portal
seo-title: Recherche de ressources et recherche enregistrée sur AEM Brand Portal
description: La fonctionnalité de recherche de Brand Portal vous permet de rechercher rapidement des ressources appropriées au moyen de l’omni-recherche. et lLes filtres de recherche vous permettent d’affiner encore davantage votre recherche. Enregistrez vos recherches sous la forme de collections dynamiques pour une utilisation ultérieure.
seo-description: La fonctionnalité de recherche de Brand Portal vous permet de rechercher rapidement des ressources appropriées au moyen de l’omni-recherche. et lLes filtres de recherche vous permettent d’affiner encore davantage votre recherche. Enregistrez vos recherches sous la forme de collections dynamiques pour une utilisation ultérieure.
uuid: c2955198-bdc0-4853-a13a-661e6a9ec61f
contentOwner: bdhar
content-type: référencereference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: SearchandPromote
discoiquuid: dc751cd7-f663-46d2-84c4-5bb12a4fe1ba
translation-type: ht
source-git-commit: 86d4d5c358ea795e35db2dce8c9529ed14e9ee2d

---


# Recherche de ressources sur Brand Portal {#search-assets-on-brand-portal}

La fonctionnalité de recherche de Brand Portal vous permet de rechercher rapidement les ressources appropriées au moyen de  l’omni-recherche, et la recherche facettée qui utilise des filtres vous aident à affiner encore davantage votre recherche. Vous pouvez également enregistrer vos recherches sous la forme de collections dynamiques pour une utilisation ultérieure.

## Recherche de ressources à l’aide de l’omni-recherche {#search-assets-using-omnisearch}

Pour rechercher des ressources sur Brand Portal :

1. Dans la barre d’outils, cliquez sur l’icône **[!UICONTROL Rechercher]** ou appuyez sur la touche « **[!UICONTROL /]** » pour lancer l’omni-recherche.

   ![](assets/omnisearchicon-1.png)

1. Dans la zone de recherche, saisissez un mot-clé pour les ressources à rechercher.

   ![](assets/omnisearch.png)

   >[!NOTE]
   >
   >Pour que des suggestions de recherche s’affichent, au moins 3 caractères sont nécessaires dans l’omni-recherche.

1. Pour accéder rapidement aux ressources qui vous intéressent, choisissez l’une des suggestions associées qui apparaissent dans la liste déroulante.

   ![](assets/assets-search-result.png)

   *Recherche de ressources à l’aide de l’omni-recherche*

Pour en savoir plus sur le comportement de la recherche avec des ressources avec balisage intelligent, consultez la section traitant de la [présentation du comportement et des résultats de recherche](https://helpx.adobe.com/fr/experience-manager/6-5/assets/using/search-assets.html).

## Recherche à l’aide des facettes du panneau Filtres{#search-using-facets-in-filters-panel}

Les facettes de recherche du panneau Filtres ajoutent de la granularité à votre expérience de recherche et optimisent la fonctionnalité de recherche. Elles utilisent plusieurs dimensions (prédicats) qui vous permettent d’effectuer des recherches complexes. Vous pouvez facilement descendre dans la hiérarchie jusqu’au niveau de détail souhaité pour effectuer une recherche plus précise.

Par exemple, si vous recherchez une image, vous pouvez indiquer si vous souhaitez une image bitmap ou vectorielle. Vous pouvez réduire davantage l’étendue de la recherche en spécifiant le type MIME de l’image dans la facette de recherche Type de fichier. De même, lors de la recherche de documents, vous pouvez spécifier le format, par exemple PDF ou MS Word.<br />

![Panneau Filtres dans Brand Portal](assets/file-type-search.png "Panneau Filtres dans Brand Portal")

Le panneau [!UICONTROL Filtres] contient quelques facettes standard ([!UICONTROL Explorateur de chemins], [!UICONTROL Type de fichier], [!UICONTROL Taille de fichier], [!UICONTROL État] et [!UICONTROL Orientation]). Vous pouvez toutefois [ajouter des facettes de recherche personnalisées](../using/brand-portal-search-facets.md) ou supprimer des facettes de recherche spécifiques du panneau [!UICONTROL Filtres] en ajoutant ou en supprimant des prédicats dans le formulaire de recherche sous-jacent. Consultez la liste des [prédicats de recherche disponibles et utilisables sur Brand Portal](../using/brand-portal-search-facets.md#list-of-search-predicates).

Pour appliquer des filtres à votre recherche avec les [facettes de recherche](../using/brand-portal-search-facets.md) disponibles :

1. Cliquez sur l’icône de recouvrement, puis sélectionnez **[!UICONTROL Filtrer]**.

   ![](assets/selectorrail.png)

1. Dans le panneau **[!UICONTROL Filtres]** à gauche, sélectionnez les options adéquates pour appliquer les filtres correspondants.
Par exemple, utilisez les filtres standard suivants :

   * **[!UICONTROL Explorateur de chemins d’accès]** pour rechercher des ressources dans un répertoire donné. Le chemin de recherche par défaut du prédicat pour l’Explorateur de chemins d’accès est **[!UICONTROL /content/dam/mac/&lt;tenant-id&gt;/]**, mais il peut être configuré en modifiant le formulaire de recherche par défaut.
   >[!NOTE]
   >
   >Pour les utilisateurs non administrateurs, l’[!UICONTROL Explorateur de chemins d’accès] du panneau [!UICONTROL Filtres] affiche seulement la structure de contenu des dossiers (et de leurs ancêtres) partagés avec l’utilisateur.\
   >Pour les utilisateurs administrateurs, l’Explorateur de chemins d’accès permet d’accéder à n’importe quel dossier de Brand Portal.

   * **[!UICONTROL Type de fichier]** pour spécifier le type (image, document, fichier multimédia, archive) du fichier de ressource que vous recherchez. En outre, vous pouvez réduire l’étendue de votre recherche. Par exemple, spécifiez le type MIME (Tiff, Bitmap, Images GIMP) de l’image ou le format (PDF ou MS Word) des documents.
   * **[!UICONTROL Taille de fichier]** pour rechercher des ressources en fonction de leur taille. Vous pouvez spécifier les limites inférieure et supérieure de la plage de tailles afin d’affiner votre recherche et déterminer l’unité de mesure à rechercher.
   * **[!UICONTROL État]** pour rechercher des ressources en fonction de leur état comme Approbation (approuvée, modifications requises, rejetée, en attente) et Expiration.
   * **[!UICONTROL Note moyenne]** pour rechercher des ressources en fonction de leur évaluation.
   * **[!UICONTROL Orientation]** pour rechercher des ressources en fonction de leur orientation (horizontal, vertical, carré).
   * **[!UICONTROL Style]** pour rechercher des ressources en fonction de leur style (couleur, monochrome).
   * **[!UICONTROL Format vidéo]** pour rechercher des ressources vidéo en fonction de leur format (DVI, Flash, MPEG4, MPEG, OGG Theora, QuickTime, Windows Media, WebM).
   Vous pouvez utiliser des [facettes de recherche personnalisées](../using/brand-portal-search-facets.md) dans le panneau Filtres en modifiant le formulaire de recherche sous-jacent.

   * S’il est utilisé dans le formulaire de recherche, le **[!UICONTROL prédicat de propriété]** permet de rechercher des ressources qui correspondent à une propriété de métadonnées sur laquelle est mappée le prédicat.\
      Par exemple, si Prédicat de la propriété est mappé sur [!UICONTROL `jcr:content /metadata/dc:title`], vous pouvez rechercher des fichiers en fonction de leur titre.\
      [!UICONTROL Prédicat de propriété] prend en charge les recherches de texte pour les éléments suivants :

      **Expressions partielles**
Pour permettre la recherche de ressources à l’aide d’expressions partielles dans le prédicat de propriété, cochez la case **[!UICONTROL Recherche partielle]** dans le formulaire de recherche.\
      Vous pouvez ainsi rechercher les ressources souhaitées même si vous ne spécifiez pas les mots/expressions exacts utilisés dans les métadonnées de la ressource.\
      Vous pouvez :
* Spécifier un mot apparaissant dans l’expression recherchée dans la facette du panneau Filtres. Par exemple, si vous recherchez le terme **climb** (et que le prédicat de propriété est mappé sur la propriété [!UICONTROL `dc:title`]), toutes les ressources ayant le mot **climb** dans l’expression de leur titre sont renvoyées.
* Spécifier une partie du mot apparaissant dans l’expression recherchée, ainsi qu’un caractère générique (*) pour remplir les trous.
Par exemple, la recherche de :
      **climb*** renvoie toutes les ressources ayant des mots commençant par les caractères « climb » dans l’expression de leur titre.
      ***climb** renvoie toutes les ressources ayant des mots se terminant par « climb » dans l’expression de leur titre.
      ***climb*** renvoie toutes les ressources ayant des mots comprenant les caractères « climb » dans l’expression de leur titre.\
      **Texte insensible à la casse**
Pour autoriser une recherche insensible à la casse dans le prédicat de propriété, cochez la case **[!UICONTROL Ignorer la casse]** dans le formulaire de recherche. Par défaut, la recherche de texte sur le prédicat de propriété est sensible à la casse.
   >[!NOTE]
   >
   >Lorsque vous cochez la case **[!UICONTROL Recherche partielle]**, l’option [!UICONTROL Ignorer la casse] est sélectionnée par défaut.

   ![](assets/wildcard-prop-1.png)

   Les résultats de la recherche sont affichés en fonction des filtres appliqués, avec le nombre de résultats.

   ![](assets/omnisearch-with-filters.png)

   Résultat de la recherche de ressources avec le nombre de résultats

1. Vous pouvez facilement accéder à un élément du résultat de recherche et revenir à ce même résultat à l’aide du bouton Précédent de votre navigateur sans avoir à relancer la requête de recherche.

## Enregistrement d’une recherche en tant que collection dynamique{#save-your-searches-as-smart-collection}

Vous pouvez enregistrer les paramètres d’une recherche en tant que collection dynamique pour pouvoir la répéter rapidement sans avoir à redéfinir les mêmes paramètres.

Pour enregistrer les paramètres de recherche comme collection dynamique :

1. Appuyez/cliquez sur **[!UICONTROL Enregistrer la collection dynamique]** et donnez-lui un nom.

   Pour rendre la collection dynamique accessible à tous les utilisateurs, cochez **[!UICONTROL Public]**. Un message confirme que la collection dynamique a été créée et ajoutée à la liste de vos recherches enregistrées.

   >[!NOTE]
   >
   >Vous pouvez empêcher les utilisateurs non-administrateurs de rendre des collections dynamiques publiques pour éviter que le Brand Portal de l’organisation présente un nombre très important de collections dynamiques publiques créées par les utilisateurs non-administrateurs. Les organisations peuvent désactiver la configuration **Autoriser la création de collections dynamiques publiques** dans **[!UICONTROL Paramètres généraux]au niveau du panneau des outils d’administration.**

   ![](assets/save_smartcollectionui.png)

1. Pour enregistrer la collection dynamique sous un autre nom et cocher ou décocher la case **[!UICONTROL Public]**, cliquez sur **[!UICONTROL Modif. collecte dynam.]**

   ![](assets/edit_smartcollection.png)

1. Dans la boîte de dialogue **[!UICONTROL Modif. collecte dynam.]**, sélectionnez **[!UICONTROL Enregistrer sous]** et saisissez le nom de la collection dynamique. Cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/saveas_smartsearch.png)
