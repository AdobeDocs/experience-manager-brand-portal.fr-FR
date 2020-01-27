---
title: Utilisation des facettes de recherche personnalisée
seo-title: Utilisation des facettes de recherche personnalisée
description: Les administrateurs peuvent ajouter des prédicats de recherche au panneau Filtres pour personnaliser les recherches et rendre la fonction de recherche polyvalente.
seo-description: Les administrateurs peuvent ajouter des prédicats de recherche au panneau Filtres pour personnaliser les recherches et rendre la fonction de recherche polyvalente.
uuid: 986fba5a-fac5-4128-ac75-d04da5b52d45
content-type: reference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 19faa028-246b-42c7-869f-97c95c7a1349
translation-type: ht
source-git-commit: 86078dd07b5d487f8cf5cd08bc46e4745529c873

---


# Utilisation des facettes de recherche personnalisée {#use-custom-search-facets}

Les administrateurs peuvent ajouter des prédicats de recherche au panneau [!UICONTROL Filtres] pour personnaliser les recherches et rendre la fonction de recherche polyvalente.

Brand Portal prend en charge la [recherche à facettes](../using/brand-portal-searching.md#search-using-facets-in-filters-panel) pour les recherches granulaires des ressources de marque approuvées grâce au panneau [**Filtres **](../using/brand-portal-searching.md#search-using-facets-in-filters-panel). Les facettes de recherche sont disponibles sur le panneau Filtres par l’intermédiaire du**[!UICONTROL  Formulaire de recherche]** des outils d’administration. Un formulaire de recherche par défaut, appelé Rail de recherche d’administrateurs de ressources, figure sur la page Formulaires de recherche dans les outils d’administration. Cependant, les administrateurs peuvent personnaliser le panneau Filtres par défaut en modifiant le formulaire de recherche par défaut (Rail de recherche d’administrateurs de ressources) en ajoutant, modifiant ou supprimant des prédicats de recherche, rendant de ce fait la fonctionnalité de recherche versatile.

Vous pouvez utiliser différents prédicats de recherche pour personnaliser le panneau **[!UICONTROL Filtres]**. Ajoutez par exemple le prédicat Propriété pour rechercher des ressources qui correspondent à une seule propriété spécifiée dans ce prédicat. Ajoutez le prédicat Options pour rechercher les ressources correspondant à une ou plusieurs valeurs que vous indiquez pour une propriété spécifique. Ajoutez le prédicat Période pour rechercher les ressources créées au cours d’une période donnée.

>[!NOTE]
>
>AEM permet aux entreprises de [publier les formulaires de recherche personnalisés sur Brand Portal à partir d’AEM Author](../using/publish-schema-search-facets-presets.md#publish-search-facets-to-brand-portal), au lieu de recréer le même formulaire sur Brand Portal.

## Ajout d’un prédicat de recherche {#add-a-search-predicate}

Pour ajouter un prédicat de recherche au panneau **[!UICONTROL Filtres]** :

1. Pour accéder aux outils d’administration, cliquez sur le logo AEM dans la barre d’outils supérieure.

   ![](assets/aemlogo.png)

1. Dans le panneau des outils d’administration, cliquez sur **[!UICONTROL Formulaires de recherche]**.

   ![](assets/navigation-panel-1.png)

1. Dans la page **[!UICONTROL Formulaires de recherche]**, sélectionnez**[!UICONTROL  Rail de recherche d’administrateurs de ressources]**.

   ![](assets/search-forms-page.png)

1. Dans la barre d’outils qui apparaît dans la partie supérieure, cliquez sur **[!UICONTROL Modifier]**pour ouvrir la page Modifier le formulaire de recherche.

   ![](assets/edit-search-form-1.png)

1. Sur la page [!UICONTROL Modifier le formulaire de recherche], faites glisser un prédicat de l’onglet [!UICONTROL Sélectionner le prédicat] vers le volet principal. Faites glisser, par exemple, **[!UICONTROL Prédicat de la propriété]**.

   Le champ **[!UICONTROL Propriété]**apparaît dans le volet principal et l’onglet**[!UICONTROL  Paramètres]** à droite affiche les prédicats de propriété.

   ![](assets/partial-prop-predicate.png)

   >[!NOTE]
   >
   >Le libellé d’en-tête de l’onglet **[!UICONTROL Paramètres]**identifie le type de prédicat sélectionné.

1. Dans l’onglet **[!UICONTROL Paramètres]**, saisissez un libellé, un texte d’espace réservé et une description pour le prédicat de propriété.

   * Sélectionnez **[!UICONTROL Recherche partielle]**si vous souhaitez autoriser la recherche par expression partielle (et la recherche par caractères génériques) de ressources en fonction des valeurs de propriétés spécifiées. Par défaut, le prédicat prend en charge la recherche en texte intégral.
   * Sélectionnez **[!UICONTROL Ignorer la casse ]**si vous souhaitez que la recherche de ressources en fonction des valeurs de propriétés ne soit pas sensible à la casse. Par défaut, la recherche des valeurs de propriétés dans le filtre de recherche est sensible à la casse.
   >[!NOTE]
   >
   >Lorsque vous cochez la case **[!UICONTROL Recherche partielle]**, l’option**[!UICONTROL  Ignorer la casse]** est sélectionnée par défaut.

1. Dans le champ **[!UICONTROL Nom de la propriété]**, ouvrez le sélecteur de propriétés, puis choisissez la propriété sur laquelle se base la recherche. Sinon, saisissez un nom de propriété. Par exemple, saisissez`  jcr :content/metadata/dc:title`ou`./jcr:content/metadata/dc:title`.

   ![](assets/title-prop.png)

1. Pour enregistrer les paramètres, cliquez sur **[!UICONTROL Terminé]**.
1. Dans l’interface utilisateur d’[!UICONTROL Assets], cliquez sur l’icône de recouvrement, puis sélectionnez **[!UICONTROL Filtrer]** pour accéder au panneau**[!UICONTROL  Filtres]**. Le prédicat **[!UICONTROL Propriété]**est ajouté au panneau.

   ![](assets/property-filter-panel.png)

1. Dans la zone de texte **[!UICONTROL Propriété]**, saisissez le titre de la ressource à rechercher. Par exemple : « Adobe ». Lorsque vous effectuez une recherche, les ressources dont le titre correspond à « Adobe » sont affichées dans les résultats de la recherche.

## Liste des prédicats de recherche {#list-of-search-predicates}

Tout comme vous ajoutez un prédicat **[!UICONTROL Propriété]**, vous pouvez ajouter les prédicats suivants au panneau**[!UICONTROL  Filtres]** :

| **Nom du prédicat** | **Description** | **Propriétés** |
|-------|-------|----------|
| **[!UICONTROL Explorateur de chemins d’accès]** | Prédicat de recherche permettant de rechercher des ressources à un emplacement spécifique. **Remarque :** *pour un utilisateur connecté, l’Eexplorateur de chemins d’accès sur le filtre montre seulement la structure de contenu des dossiers (et de leurs ancêtres) partagés avec l’utilisateur.* <br> Les utilisateurs administrateurs peuvent rechercher des ressources dans n’importe quel dossier en y accédant à l’aide de l’Eexplorateur de chemins d’accès. <br> Cependant, les utilisateurs non-administrateurs peuvent rechercher des ressources dans un dossier (qui leur est accessible) en accédant à ce dossier dans l’Eexplorateur de chemins d’accès. | <ul><li>Libellé du champ</li><li>Chemin</li><li>Description</li></ul> |
| **[!UICONTROL Propriété]** | Recherche des ressources en fonction d’une propriété de métadonnées spécifique. **Remarque :** *lorsque vous cochez la case Recherche partielle, l’option Ignorer la casse est sélectionnée par défaut*. | <ul><li>Libellé du champ</li><li>Espace réservé</li><li>Nom de la propriété</li><li>Recherche partielle</li><li>Ignorer la casse</li><li> Description</li></ul> |
| **[!UICONTROL Propriété Plusieurs valeurs]** | Similaire au prédicat de propriété, mais autorise des valeurs d’entrée multiples, séparées par un délimiteur (VIRGULE[,], par défaut). Les ressources qui correspondent aux valeurs d’entrée sont renvoyées dans les résultats. | <ul><li>Libellé du champ</li><li>Espace réservé</li><li>Nom de la propriété</li><li>Prise en charge des délimiteurs</li><li>Ignorer la casse</li><li>Description</li></ul> |
| **[!UICONTROL Balises]** | Prédicat de recherche permettant de rechercher des ressources en fonction des balises. Vous pouvez configurer la propriété Chemin d’accès pour renseigner diverses balises de la liste Balises. *Remarque : il se peut que les administrateurs doivent modifier la valeur de chemin, par exemple [!UICONTROL `/etc/tags/mac/<tenant_id>/<custom_tag_namespace>`], s’ils publient le formulaire de recherche à partir d’AEM, où le chemin d’accès n’inclut pas les informations du client comme [!UICONTROL `/etc/tags/<custom_tag_namespace>`]. | <ul><li>Libellé du champ</li><li>Nom de la propriété</li><li>Chemin</li><li>Description</li></ul> |
| **[!UICONTROL Chemin]** | Prédicat de recherche permettant de rechercher des ressources à un emplacement spécifique. | <ul><li>Libellé du champ</li><li>Chemin</li><li>Description</li></ul> |  |
| **[!UICONTROL Date relative]** | Prédicat de recherche permettant de rechercher des ressources en fonction de leur date de création. | <ul><li>Libellé du champ</li><li>Nom de la propriété</li><li>Date relative</li></ul> |
| **[!UICONTROL Étendue]** | Prédicat de recherche permettant de rechercher des ressources qui se trouvent dans une plage spécifiée de valeurs de propriété. Dans le panneau Filtres, vous pouvez spécifier les valeurs de propriété minimale et maximale de la période concernée. | <ul><li>Libellé du champ</li><li>Nom de la propriété</li><li>Description</li></ul> |
| **[!UICONTROL Période]** | Prédicat de recherche permettant de rechercher des ressources créées pendant une période spécifiée pour une propriété de date. Dans le panneau Filtres, vous pouvez spécifier les dates de début et de fin. | <ul><li>Libellé du champ</li><li>Espace réservé</li><li>Nom de la propriété</li><li>Texte de la plage (De)</li><li>Texte de la plage (À)</li><li>Description</li></ul> |
| **[!UICONTROL Date]** | Prédicat de recherche permettant de rechercher à l’aide d’un curseur des ressources selon une propriété de date. | <ul><li>Libellé du champ</li><li>Nom de la propriété</li><li>Description</li></ul> |
| **[!UICONTROL Taille de fichier]** | Prédicat de recherche permettant de rechercher des ressources en fonction de leur taille. | <ul><li>Libellé du champ</li><li>Nom de la propriété</li><li>Chemin</li><li>Description</li></ul> |
| **[!UICONTROL Dernière modification de la ressource]** | Prédicat de recherche permettant de rechercher des ressources en fonction de la date de dernière modification. | <ul><li>Libellé du champ</li><li>Nom de la propriété</li><li>Description</li></ul> |
| **[!UICONTROL État d’approbation]** | Prédicat de recherche permettant de rechercher des ressources en fonction de la propriété de métadonnées d’approbation. Le nom de la propriété par défaut est **dam:status**. | <ul><li>Libellé du champ</li><li>Nom de la propriété</li><li>Description</li></ul> |
| **[!UICONTROL État d’extraction]** | Prédicat de recherche permettant de rechercher des ressources en fonction de leur état d’extraction lors de leur publication depuis AEM Assets. | <ul><li>Libellé du champ</li><li>Nom de la propriété</li><li>Description</li></ul> |
| **[!UICONTROL Extraits par]** | Prédicat de recherche permettant de rechercher des ressources en fonction de l’utilisateur qui les a extraites. | <ul><li>Libellé du champ</li><li>Nom de la propriété</li><li>Description</li></ul> |
| **[!UICONTROL État d’expiration]** | Prédicat de recherche permettant de rechercher des ressources en fonction de l’état d’expiration. | <ul><li>Libellé du champ</li><li>Nom de la propriété</li><li>Description</li></ul> |
| **[!UICONTROL Membre de la collection]** | Prédicat de recherche permettant de rechercher des ressources en fonction de leur appartenance à une collection. | Description |
| **[!UICONTROL Masqué]** | Ce prédicat n’est pas explicitement visible par les utilisateurs finaux et il est utilisé pour les contraintes masquées, généralement pour limiter le type des résultats de la recherche à **dam:Asset**. | <ul><li>Libellé du champ</li><li>Nom de la propriété</li><li>Description</li></ul> |

>[!NOTE]
>
>N’utilisez pas les prédicats **[!UICONTROL Options]**,**[!UICONTROL &#x200B;État de publication]** et **[!UICONTROL Évaluation]**, car ils ne sont pas fonctionnels dans Brand Portal.

## Suppression d’un prédicat de recherche {#delete-a-search-predicate}

Pour supprimer un prédicat, procédez de la manière suivante :

1. Cliquez sur le logo Adobe pour accéder aux outils d’administration.

   ![](assets/aemlogo.png)

1. Dans le panneau des outils d’administration, cliquez sur **[!UICONTROL Formulaires de recherche]**.

   ![](assets/navigation-panel-2.png)

1. Dans la page **[!UICONTROL Formulaires de recherche]**, sélectionnez**[!UICONTROL  Rail de recherche d’administrateurs de ressources]**.

   ![](assets/search-forms-page.png)

1. Dans la barre d’outils qui apparaît dans la partie supérieure, cliquez sur **[!UICONTROL Modifier]**pour ouvrir la page Modifier le formulaire de recherche.

   ![](assets/edit-search-form-2.png)

1. Dans la page [!UICONTROL Modifier le formulaire de recherche], dans le panneau principal, sélectionnez le prédicat à supprimer. Sélectionnez, par exemple, **[!UICONTROL Prédicat de la propriété]**.

   L’onglet **[!UICONTROL Paramètres]**à droite affiche les champs de prédicat de propriété.

1. Pour supprimer un prédicat de propriété, cliquez sur l’icône représentant une corbeille. Dans la boîte de dialogue **[!UICONTROL Supprimer le champ]**, cliquez sur**[!UICONTROL  Supprimer]** pour confirmer l’action de suppression.

   Le champ **[!UICONTROL Prédicat de propriété]**est supprimé du panneau principal et l’onglet**[!UICONTROL  Paramètres]** devient vide.

   ![](assets/search-form-delete-predicate.png)

1. Pour enregistrer les modifications, cliquez sur **[!UICONTROL Terminé]**dans la barre d’outils.
1. Dans l’interface utilisateur d’**[!UICONTROL Assets]**, cliquez sur l’icône de recouvrement, puis sélectionnez**[!UICONTROL  Filtrer]** pour accéder au panneau **[!UICONTROL Filtres]**. Le prédicat**[!UICONTROL  Propriété]** est supprimé du panneau.

   ![](assets/property-predicate-removed.png)
