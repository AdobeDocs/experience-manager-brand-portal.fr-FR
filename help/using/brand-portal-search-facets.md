---
title: Utilisation des facettes de recherche personnalisée
seo-title: Utilisation des facettes de recherche personnalisée
description: Les administrateurs peuvent ajouter des prédicats de recherche au panneau Filtres pour personnaliser les recherches et rendre la fonction de recherche polyvalente.
seo-description: Les administrateurs peuvent ajouter des prédicats de recherche au panneau Filtres pour personnaliser les recherches et rendre la fonction de recherche polyvalente.
uuid: 986fba5a-fac5-4128-ac75-d04da5b52d45
content-type: référencereference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 19faa028-246b-42c7-869f-97c95c7a1349
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Utilisation des facettes de recherche personnalisée {#use-custom-search-facets}

Administrators can add search predicates to the [!UICONTROL Filters] panel to customize search and make the search functionality versatile.

Brand Portal supports [faceted search](../using/brand-portal-searching.md#search-using-facets-in-filters-panel) for granular searches of approved brand assets, which is possible due to [**Filters** panel](../using/brand-portal-searching.md#search-using-facets-in-filters-panel). Les facettes de recherche sont disponibles sur le panneau Filtres par l’intermédiaire du **[!UICONTROL Formulaire de recherche]des outils d’administration.** Un formulaire de recherche par défaut, appelé Rail de recherche d’administrateurs de ressources, figure sur la page Formulaires de recherche dans les outils d’administration. Cependant, les administrateurs peuvent personnaliser le panneau Filtres par défaut en modifiant le formulaire de recherche par défaut (Rail de recherche d’administrateurs de ressources) en ajoutant, modifiant ou supprimant des prédicats de recherche, rendant de ce fait la fonctionnalité de recherche versatile.

Vous pouvez utiliser différents prédicats de recherche pour personnaliser le panneau **[!UICONTROL Filtres].** Ajoutez par exemple le prédicat Propriété pour rechercher des ressources qui correspondent à une seule propriété spécifiée dans ce prédicat. Ajoutez le prédicat Options pour rechercher les ressources correspondant à une ou plusieurs valeurs que vous indiquez pour une propriété spécifique. Ajoutez le prédicat Période pour rechercher les ressources créées au cours d’une période donnée.

>[!NOTE]
>
>AEM allows organizations to [publish the customized search forms from AEM Author](../using/publish-schema-search-facets-presets.md#publish-search-facets-to-brand-portal) to Brand Portal, instead of re-creating the same form on Brand Portal.

## Ajout d’un prédicat de recherche {#add-a-search-predicate}

Pour ajouter un prédicat de recherche au panneau **[!UICONTROL Filtres] :**

1. To access administrative tools, click the AEM logo from the toolbar at the top.

   ![](assets/aemlogo.png)

2. Dans le panneau des outils d’administration, cliquez sur **[!UICONTROL Formulaires de recherche]**.

   ![](assets/navigation-panel-1.png)

3. Dans la page **[!UICONTROL Formulaires de recherche]**, sélectionnez **[!UICONTROL Rail de recherche d’administrateurs de ressources]**.

   ![](assets/search-forms-page.png)

4. Dans la barre d’outils qui apparaît dans la partie supérieure, cliquez sur **[!UICONTROL Modifier]pour ouvrir la page Modifier le formulaire de recherche.**

   ![](assets/edit-search-form-1.png)

5. Sur la page [!UICONTROL Modifier le formulaire de recherche], faites glisser un prédicat de l’onglet [!UICONTROL Sélectionner le prédicat] vers le volet principal. Faites glisser, par exemple, **[!UICONTROL Prédicat de la propriété]**.

   Le champ **[!UICONTROL Propriété]** apparaît dans le volet principal et l’onglet **Paramètres]à droite affiche les prédicats de propriété.[!UICONTROL **

   ![](assets/partial-prop-predicate.png)

   >[!NOTE]
   >
   >Le libellé d’en-tête de l’onglet **[!UICONTROL Paramètres]identifie le type de prédicat sélectionné.**

6. Dans l’onglet **[!UICONTROL Paramètres], saisissez un libellé, un texte d’espace réservé et une description pour le prédicat de propriété.**

   * Select **[!UICONTROL Partial Search]**, if you want to allow partial phrase search (and wildcard search) of assets-based on the specified property value. Par défaut, le prédicat prend en charge la recherche en texte intégral.
   * Select **[!UICONTROL Ignore Case]**, if you want the asset search based on property value to be non-case sensitive. Par défaut, la recherche des valeurs de propriétés dans le filtre de recherche est sensible à la casse.
   >[!NOTE]
   >
   >Lorsque vous cochez la case **[!UICONTROL Recherche partielle]**, l’option [!UICONTROL Ignorer la casse] est sélectionnée par défaut.

7. Dans le champ [!UICONTROL Nom de la propriété], ouvrez le sélecteur de propriétés, puis choisissez la propriété sur laquelle se base la recherche. Sinon, saisissez un nom de propriété. For example, enter [!UICONTROL `  jcr :content/metadata/dc:title`] or [!UICONTROL `./jcr:content/metadata/dc:title`].

   ![](assets/title-prop.png)

8. Pour enregistrer les paramètres, cliquez sur **[!UICONTROL Terminé].**
9. Dans l’interface utilisateur d’[!UICONTROL Assets], cliquez sur l’icône de recouvrement, puis sélectionnez **[!UICONTROL Filtrer]** pour accéder au panneau **Filtres[!UICONTROL .]** Le prédicat **[!UICONTROL Propriété]est ajouté au panneau.**

   ![](assets/property-filter-panel.png)

10. Dans la zone de texte **[!UICONTROL Propriété], saisissez le titre de la ressource à rechercher.** Par exemple, "Adobe". Lorsque vous effectuez une recherche, les ressources dont le titre correspond à « Adobe » sont affichées dans les résultats de la recherche.

## Liste des prédicats de recherche {#list-of-search-predicates}

Tout comme vous ajoutez un prédicat **[!UICONTROL Propriété]**, vous pouvez ajouter les prédicats suivants au panneau **Filtres[!UICONTROL  :]**

| **Nom du prédicat** | **Description** | **Propriétés** |
|-------|-------|----------|
| [!UICONTROL Explorateur de chemins d’accès] | Prédicat de recherche permettant de rechercher des ressources à un emplacement spécifique. **Remarque :** *Ppour un utilisateur connecté, l’Eexplorateur de chemins d’accès sur le filtre montre seulement la structure de contenu des dossiers (et de leurs ancêtres) partagés avec l’utilisateur.* <br> Les utilisateurs administrateurs peuvent rechercher des ressources dans n’importe quel dossier en y accédant à l'aide de l’Eexplorateur de chemins d’accès. <br> Cependant, les utilisateurs non-administrateurs peuvent rechercher des ressources dans un dossier (qui leur est accessible) en accédant à ce dossier dans l’Eexplorateur de chemins d’accès. | <ul><li>Libellé du champ</li><li>Chemin</li><li>Description</li></ul> |
| [!UICONTROL Propriétés] | Recherche des ressources en fonction d’une propriété de métadonnées spécifique. **Remarque :** *Llorsque vous cochez la case Recherche partielle, l’option Ignorer la casse est sélectionnée par défaut*. | <ul><li>Libellé du champ</li><li>Espace réservé</li><li>Nom de la propriété</li><li>Recherche partielle</li><li>Ignorer la casse</li><li> Description</li></ul> |
| [!UICONTROL Propriété Plusieurs valeurs] | Similaire au prédicat de propriété, mais autorise des valeurs d’entrée multiples, séparées par un délimiteur (VIRGULE[,], par défaut). Les ressources qui correspondent aux valeurs d’entrée sont renvoyées dans les résultats. | <ul><li>Libellé du champ</li><li>Espace réservé</li><li>Nom de la propriété</li><li>Prise en charge des délimiteurs</li><li>Ignorer la casse</li><li>Description</li></ul> |
| [!UICONTROL Balises] | Prédicat de recherche permettant de rechercher des ressources en fonction des balises. Vous pouvez configurer la propriété Chemin d’accès pour remplir diverses balises de la liste Balises. *Note: Administrators might need to change the path value, for example, [!UICONTROL `/etc/tags/mac/<tenant_id>/<custom_tag_namespace>`], if they publish the search form from AEM, where the path does not include tenant information, for example, [!UICONTROL `/etc/tags/<custom_tag_namespace>`]. | <ul><li>Libellé du champ</li><li>Nom de la propriété</li><li>Chemin</li><li>Description</li></ul> |
| [!UICONTROL Chemin] | Prédicat de recherche permettant de rechercher des ressources à un emplacement spécifique. | <ul><li>Libellé du champ</li><li>Chemin</li><li>Description</li></ul> |  |
| [!UICONTROL Date relative] | Prédicat de recherche permettant de rechercher des ressources en fonction de leur date de création. | <ul><li>Libellé du champ</li><li>Nom de la propriété</li><li>Date relative</li></ul> |
| [!UICONTROL Étendue] | Prédicat de recherche permettant de rechercher des ressources qui se trouvent dans une plage spécifiée de valeurs de propriété. Dans le panneau Filtres, vous pouvez spécifier les valeurs de propriété minimale et maximale de la période concernée. | <ul><li>Libellé du champ</li><li>Nom de la propriété</li><li>Description</li></ul> |
| [!UICONTROL Période] | Prédicat de recherche permettant de rechercher des ressources créées pendant une période spécifiée pour une propriété de date. Dans le panneau Filtres, vous pouvez spécifier les dates de début et de fin. | <ul><li>Libellé du champ</li><li>Espace réservé</li><li>Nom de la propriété</li><li>Texte de la plage (De)</li><li>Texte de la plage (À)</li><li>Description</li></ul> |
| [!UICONTROL Date] | Prédicat de recherche permettant de rechercher à l’'aide d’'un curseur des ressources selon une propriété de date. | <ul><li>Libellé du champ</li><li>Nom de la propriété</li><li>Description</li></ul> |
| [!UICONTROL Taille de fichier] | Prédicat de recherche permettant de rechercher des ressources en fonction de leur taille. | <ul><li>Libellé du champ</li><li>Nom de la propriété</li><li>Chemin</li><li>Description</li></ul> |
| [!UICONTROL Dernière modification de la ressource] | Prédicat de recherche permettant de rechercher des ressources en fonction de la date de dernière modification. | <ul><li>Libellé du champ</li><li>Nom de la propriété</li><li>Description</li></ul> |
| [!UICONTROL État d’approbation] | Prédicat de recherche permettant de rechercher des ressources en fonction de la propriété de métadonnées d’approbation. Le nom de la propriété par défaut est **dam:status**. | <ul><li>Libellé du champ</li><li>Nom de la propriété</li><li>Description</li></ul> |
| [!UICONTROL État d’extraction] | Prédicat de recherche permettant de rechercher des ressources en fonction de leur état d’extraction lors de leur publication depuis AEM Assets. | <ul><li>Libellé du champ</li><li>Nom de la propriété</li><li>Description</li></ul> |
| [!UICONTROL Extrait par] | Prédicat de recherche permettant de rechercher des ressources en fonction de l’utilisateur qui les a extraites. | <ul><li>Libellé du champ</li><li>Nom de la propriété</li><li>Description</li></ul> |
| [!UICONTROL État d’expiration] | Prédicat de recherche permettant de rechercher des ressources en fonction de l’état d’expiration. | <ul><li>Libellé du champ</li><li>Nom de la propriété</li><li>Description</li></ul> |
| [!UICONTROL Membre de la collection] | Prédicat de recherche permettant de rechercher des ressources en fonction de leur appartenance à une collection. | Description |
| [!UICONTROL Masqué] | This predicate is not explicitly visible to the end users and is used for any hidden constraints typically for restricting search results type to **dam:Asset**. | <ul><li>Libellé du champ</li><li>Nom de la propriété</li><li>Description</li></ul> |

>[!NOTE]
>
>Do not use **[!UICONTROL Options Predicate]**, **[!UICONTROL Publish Status Predicate]**, and **[!UICONTROL Rating Predicate]** as these predicates are not functional in Brand Portal.

## Suppression d’un prédicat de recherche {#delete-a-search-predicate}

Pour supprimer un prédicat, procédez de la manière suivante :

1. Cliquez sur le logo Adobe pour accéder aux outils d’administration.

   ![](assets/aemlogo.png)

2. Dans le panneau des outils d’administration, cliquez sur **[!UICONTROL Formulaires de recherche]**.

   ![](assets/navigation-panel-2.png)

3. Dans la page **[!UICONTROL Formulaires de recherche]**, sélectionnez **[!UICONTROL Rail de recherche d’administrateurs de ressources]**.

   ![](assets/search-forms-page.png)

4. Dans la barre d’outils qui apparaît dans la partie supérieure, cliquez sur **[!UICONTROL Modifier]pour ouvrir la page Modifier le formulaire de recherche.**

   ![](assets/edit-search-form-2.png)

5. Dans la page [!UICONTROL Modifier le formulaire de recherche], dans le panneau principal, sélectionnez le prédicat à supprimer. Sélectionnez, par exemple, **[!UICONTROL Prédicat de la propriété]**.

   L’onglet **[!UICONTROL Paramètres]à droite affiche les champs de prédicat de propriété.**

6. Pour supprimer un prédicat de propriété, cliquez sur l’icône représentant une corbeille. Dans la boîte de dialogue **[!UICONTROL Supprimer le champ]**, cliquez sur **Supprimer]pour confirmer l’action de suppression.[!UICONTROL **

   Le champ **[!UICONTROL Prédicat de propriété]** est supprimé du panneau principal et l’onglet **Paramètres]devient vide.[!UICONTROL **

   ![](assets/search-form-delete-predicate.png)

7. Pour enregistrer les modifications, cliquez sur **[!UICONTROL Terminé]dans la barre d’outils.**
8. Dans l’interface utilisateur d’**[!UICONTROL Assets]**, cliquez sur l’icône de recouvrement, puis sélectionnez **[!UICONTROL Filtrer] pour accéder au panneau** Filtres **.** Le prédicat **[!UICONTROL Propriété]est supprimé du panneau.**

   ![](assets/property-predicate-removed.png)
