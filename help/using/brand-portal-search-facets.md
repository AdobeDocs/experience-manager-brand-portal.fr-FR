---
title: Utilisation de facettes de recherche personnalisée
seo-title: Utilisation de facettes de recherche personnalisée
description: Les administrateurs peuvent ajouter des prédicats de recherche au panneau Filtres pour personnaliser les recherches et rendre la fonction de recherche polyvalente.
seo-description: Les administrateurs peuvent ajouter des prédicats de recherche au panneau Filtres pour personnaliser les recherches et rendre la fonction de recherche polyvalente.
uuid: 986 fba 5 a-fac 5-4128-ac 75-d 04 da 5 b 52 d 45
content-type: référence
topic-tags: administration
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
discoiquuid: 19 faa 028-246 b -42 c 7-869 f -97 c 95 c 7 a 1349
translation-type: tm+mt
source-git-commit: ea7fdd2df0696ed309227fa77e3f79d0141bcb58

---


# Utilisation des facettes de recherche personnalisée {#use-custom-search-facets}

Les administrateurs peuvent ajouter des prédicats de recherche au panneau Filtres pour personnaliser les recherches et rendre la fonction de recherche polyvalente.

[!DNL Brand Portal] prend en charge [la recherche factice](../using/brand-portal-searching.md#search-using-facets-in-filters-panel) pour des recherches granulaires des ressources de marque approuvées, ce qui est possible en raison du panneau [**Filtres**](../using/brand-portal-searching.md#search-using-facets-in-filters-panel). Search facets are made available on Filters panel through **Search Form** in the admin tools. Un formulaire de recherche par défaut, appelé Rail de recherche d’administrateurs de ressources, figure sur la page Formulaires de recherche dans les outils d’administration. Cependant, les administrateurs peuvent personnaliser le panneau Filtres par défaut en modifiant le formulaire de recherche par défaut (Rail de recherche d’administrateurs de ressources) en ajoutant, modifiant ou supprimant des prédicats de recherche, rendant de ce fait la fonctionnalité de recherche versatile.

You can use various search predicates to customize the **Filters** panel. Par exemple, ajoutez le prédicat de propriété pour rechercher des fichiers qui correspondent à une propriété unique que vous spécifiez dans ce prédicat. Ajoutez les options permettant de rechercher des fichiers qui correspondent à une ou plusieurs valeurs spécifiées pour une propriété particulière. Ajoutez le prédicat de plage de dates pour rechercher les fichiers créés dans une plage de dates spécifiée.

>[!NOTE]
>
>[!DNL AEM] permet aux entreprises [de publier les formulaires de recherche personnalisés à partir de [! DNL AEM] Auteur](../using/publish-schema-search-facets-presets.md#publish-search-facets-to-brand-portal) à [!DNL Brand Portal], au lieu de recréer le même formulaire.[!DNL Brand Portal]

## Ajout d’un prédicat de recherche {#add-a-search-predicate}

Pour ajouter un prédicat de recherche au panneau **Filtres** :

1. To access administrative tools, click the [!DNL AEM] logo from the toolbar at the top.

   ![](assets/aemlogo.png)

2. Dans le panneau des outils d’administration, cliquez sur **Formulaires de recherche**.

   ![](assets/navigation-panel-1.png)

3. Dans la page **Formulaires de recherche**, sélectionnez **Rail de recherche d’administrateurs de ressources**.

   ![](assets/search-forms-page.png)

4. Dans la barre d’outils qui apparaît dans la partie supérieure, cliquez sur **Modifier** pour ouvrir la page Modifier le formulaire de recherche.

   ![](assets/edit-search-form-1.png)

5. In the **Edit Search Form** page, drag a predicate from the **Select Predicate** tab to the main pane. For example, drag **Property Predicate**.

   Le champ **Propriété** apparaît dans le panneau principal et l’onglet **Paramètres** à droite affiche les prédicats de propriété.

   ![](assets/partial-prop-predicate.png)

   >[!NOTE]
   >
   >Le libellé d’en-tête de l’onglet **Paramètres** identifie le type de prédicat sélectionné.

6. In the **Settings** tab, enter a label, placeholder text, and description for the property predicate.

   * Select **Partial Search**, if you want to allow partial phrase search (and wildcard search) of assets-based on the specified property value. Par défaut, le prédicat prend en charge la recherche en texte intégral.
   * Select **Ignore Case**, if you want the asset search based on property value to be non-case sensitive. Par défaut, la recherche des valeurs de propriétés dans le filtre de recherche est sensible à la casse.
   >[!NOTE]
   >
   >Lorsque vous cochez la case **Recherche partielle**, l’option **Ignorer la casse** est sélectionnée par défaut.

7. In the **Property Name** field, open property picker and select the property based on which the search is performed. Sinon, saisissez un nom pour la propriété. For example, enter `  jcr :content/metadata/dc:title` or `./jcr:content/metadata/dc:title`.

   ![](assets/title-prop.png)

8. Pour enregistrer les paramètres, cliquez sur **Terminé**.
9. From the **Assets** user interface, click the overlay icon and choose **Filter** to navigate to the **Filters** panel. The **Property** predicate is added to the panel.

   ![](assets/property-filter-panel.png)

10. Dans la zone de texte **Propriété**, saisissez le titre de la ressource à rechercher. Par exemple, saisissez « Adobe ». Lorsque vous effectuez une recherche, les ressources dont le titre correspond à « Adobe » sont répertoriées dans les résultats de la recherche.

## Liste des prédicats de recherche {#list-of-search-predicates}

Similar to the way you add a **Property** predicate, you can add the following predicates to the **Filters** panel:

| **Nom du prédicat** | **Description** | **Propriétés** |
|-------|-------|----------|
| Explorateur de chemins d’accès | Prédicat de recherche permettant de rechercher des ressources à un emplacement spécifique. **Remarque :***Pour un utilisateur connecté, le navigateur de chemins sur le filtre affiche uniquement la structure de contenu des dossiers (et leurs ancêtres) partagés avec l'utilisateur.* <br> Les utilisateurs administrateurs peuvent rechercher des ressources dans n’importe quel dossier en y accédant en utilisant l’explorateur de chemins d’accès. <br> En revanche, les utilisateurs non administrateurs peuvent rechercher des fichiers dans un dossier (accessible pour eux) en accédant à ce dossier dans le navigateur de chemins. | <ul><li>Libellé du champ</li><li>Chemin</li><li>Description</li></ul> |
| Propriétés | Recherche des ressources en fonction d’une propriété de métadonnées spécifique. **Remarque :***Lorsque vous sélectionnez Recherche partielle, Ignorer la casse est sélectionné par défaut*. | <ul><li>Libellé du champ</li><li>Espace réservé</li><li>Nom de la propriété</li><li>Recherche partielle</li><li>Ignorer la casse</li><li> Description</li></ul> |
| Propriété Plusieurs valeurs | Similar to property predicate but allows multiple input values, separated by a delimiter (default is COMMA[,]) assets matching any of the input values are returned in results. | <ul><li>Libellé du champ</li><li>Espace réservé</li><li>Nom de la propriété</li><li>Prise en charge des délimiteurs</li><li>Ignorer la casse</li><li>Description</li></ul> |
| Balises | Prédicat de recherche permettant de rechercher des ressources en fonction des balises. Vous pouvez configurer la propriété Chemin d’accès pour remplir diverses balises de la liste Balises. *Remarque : Les administrateurs doivent peut-être modifier la valeur de chemin, par exemple,* `/etc/tags/mac/<tenant_id>/<custom_tag_namespace>`*s'ils publient le formulaire de recherche à partir[!DNL AEM]duquel le chemin d'accès n'inclut pas les informations du client,* `/etc/tags/<custom_tag_namespace>`par exemple. | <ul><li>Libellé du champ</li><li>Nom de la propriété</li><li>Chemin</li><li>Description</li></ul> |
| Chemin | Prédicat de recherche permettant de rechercher des ressources à un emplacement spécifique. | <ul><li>Libellé du champ</li><li>Chemin</li><li>Description</li></ul> |  |
| Date relative | Prédicat de recherche permettant de rechercher des ressources en fonction de leur date de création. | <ul><li>Libellé du champ</li><li>Nom de la propriété</li><li>Date relative</li></ul> |
| Étendue | Prédicat de recherche permettant de rechercher des ressources qui se trouvent dans une plage spécifiée de valeurs de propriété. Dans le panneau Filtres, vous pouvez spécifier des valeurs de propriétés minimale et maximale pour la plage. | <ul><li>Libellé du champ</li><li>Nom de la propriété</li><li>Description</li></ul> |
| Période | Prédicat de recherche permettant de rechercher des ressources créées dans une plage spécifiée pour une propriété de date. Dans le panneau Filtres, vous pouvez spécifier les dates de début et de fin. | <ul><li>Libellé du champ</li><li>Espace réservé</li><li>Nom de la propriété</li><li>Texte de la plage (De)</li><li>Texte de la plage (À)</li><li>Description</li></ul> |
| Date | Prédicat de recherche permettant de rechercher des ressources selon une propriété de date. | <ul><li>Libellé du champ</li><li>Nom de la propriété</li><li>Description</li></ul> |
| Taille de fichier | Prédicat de recherche permettant de rechercher des ressources en fonction de leur taille.. | <ul><li>Libellé du champ</li><li>Nom de la propriété</li><li>Chemin</li><li>Description</li></ul> |
| Dernière modification de la ressource | Prédicat de recherche permettant de rechercher des ressources en fonction de la date de dernière modification. | <ul><li>Libellé du champ</li><li>Nom de la propriété</li><li>Description</li></ul> |
| État d’approbation | Prédicat de recherche permettant de rechercher des ressources en fonction de la propriété de métadonnées d’approbation. Le nom de la propriété par défaut est **dam:status**. | <ul><li>Libellé du champ</li><li>Nom de la propriété</li><li>Description</li></ul> |
| État de passage en caisse | Search predicate to search assets based on the check-out status of an asset when it was published from [!DNL AEM] Assets. | <ul><li>Libellé du champ</li><li>Nom de la propriété</li><li>Description</li></ul> |
| Extrait par | Prédicat de recherche permettant de rechercher des ressources en fonction de l’utilisateur qui les a extraites. | <ul><li>Libellé du champ</li><li>Nom de la propriété</li><li>Description</li></ul> |
| État d’expiration | Prédicez la recherche pour rechercher des fichiers en fonction de l'état d'expiration. | <ul><li>Libellé du champ</li><li>Nom de la propriété</li><li>Description</li></ul> |
| Membre de la collection | Prédicat de recherche permettant de rechercher des ressources en fonction de leur appartenance à une collection. | Description |
| Masqué | Ce prédicat n’est pas explicitement visible par les utilisateurs finaux et est utilisé pour les contraintes masquées afin de limiter le type des résultats de la recherche à **dam.:Asset**. | <ul><li>Libellé du champ</li><li>Nom de la propriété</li><li>Description</li></ul> |

>[!NOTE]
>
>N’utilisez pas les prédicats **Options**, **État de publication** et **Évaluation**, car ils ne sont pas fonctionnels dans [!DNL Brand Portal].

## Suppression d’un prédicat de recherche {#delete-a-search-predicate}

Pour supprimer un prédicat, procédez de la manière suivante :

1. Cliquez sur le logo Adobe pour accéder aux outils d’administration.

   ![](assets/aemlogo.png)

2. Dans le panneau des outils d’administration, cliquez sur **Formulaires de recherche**.

   ![](assets/navigation-panel-2.png)

3. Dans la page **Formulaires de recherche**, sélectionnez **Rail de recherche d’administrateurs de ressources**.

   ![](assets/search-forms-page.png)

4. Dans la barre d’outils qui apparaît dans la partie supérieure, cliquez sur **Modifier** pour ouvrir la page Modifier le formulaire de recherche.

   ![](assets/edit-search-form-2.png)

5. In the **Edit Search Form** page, from the main pane, select the predicate you want to delete. For example, select **Property Predicate**.

   L’onglet **Paramètres** à droite affiche les champs de prédicat de propriété.

6. Pour supprimer un prédicat de propriété, cliquez sur l’icône représentant une corbeille. Dans la boîte de dialogue **Supprimer le champ**, cliquez sur **Supprimer** pour confirmer l’action de suppression.

   Le champ **Prédicat de propriété** est supprimé du panneau principal et l’onglet **Paramètres** devient vide.

   ![](assets/search-form-delete-predicate.png)

7. To save the changes, click **Done** in the toolbar.
8. From the **Assets** user interface, click the overlay icon and choose **Filter** to navigate to the **Filters** panel. The **Property** predicate is removed from the panel.

   ![](assets/property-predicate-removed.png)
