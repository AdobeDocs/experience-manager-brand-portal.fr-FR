---
title: Exploration des ressources sur Brand Portal
seo-title: Exploration des ressources sur Brand Portal
description: Explorez les ressources, parcourez les hiérarchies de ressources et recherchez des ressources grâce à diverses options de modes et d’éléments d’IU sur Brand Portal.
seo-description: Explorez les ressources, parcourez les hiérarchies de ressources et recherchez des ressources grâce à diverses options de modes et d’éléments d’IU sur Brand Portal.
uuid: 178 ce 217-0050-4922-a 204-f 4539 d 46 f 539
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
content-type: référence
topic-tags: introduction
discoiquuid: a 70 ce 694-81 d 1-4829-9 e 61-b 6412 e 013 e 5 c
translation-type: tm+mt
source-git-commit: 770c353b1143d879280df310012ce9d4d30b40c9

---


# Exploration des ressources sur Brand Portal {#browsing-assets-on-brand-portal}

[!DNL AEM] Ressources [! DNL Brand Portal offre différentes fonctionnalités et différents éléments d'interface utilisateur qui facilitent la navigation dans les ressources, la navigation dans les hiérarchies de ressources et la recherche de fichiers lors de l'utilisation d'options d'affichage différentes.

[!DNL AEM][!DNL AEM]Le logo  dans la barre d’outils  supérieure permet aux utilisateurs administrateurs d’accéder au panneau des outils d’administration.

![](assets/aemlogo.png)

![](assets/admin-tools-panel-2.png)

![](assets/bp_subheader.png)

Rail selector at the upper left in [!DNL Brand Portal] drops-down to expose options to navigate into asset hierarchies, streamline your search, and display resources.

![](assets/siderail-1.png)

Vous pouvez afficher, parcourir et sélectionner les ressources à l’aide de l’un des modes disponibles (Carte, Colonnes et Liste) dans le sélecteur de mode dans la partie supérieure droite de [!DNL Brand Portal].

![](assets/viewselector.png)

## Affichage et sélection de ressources {#viewing-and-selecting-resources}

L’affichage, la navigation et la sélection sont identiques sur le plan conceptuel dans tous les modes, mais leur manipulation comporte de légères variations en fonction du mode utilisé.

Vous pouvez afficher, parcourir et sélectionner (pour action ultérieure) vos ressources dans les modes disponibles :

* Mode Colonnes
* Mode Carte
* Mode Liste

### Mode Carte

![](assets/card-view.png)

Le mode Carte affiche les cartes d’informations de chaque élément au niveau actuel. Ces cartes présentent les les détails suivants :

* Représentation visuelle de la ressource/du dossier.
* Type
* Titre
* Nom
* Date et heure de publication de la fichier a été publié [!DNL Brand Portal] à partir de [!DNL AEM]
* Taille
* Dimensions

You can navigate down the hierarchy by tapping/clicking cards (taking care to avoid the quick actions) or up again by using the [breadcrumbs in the header](https://helpx.adobe.com/experience-manager/6-5/sites/authoring/using/basic-handling.html#TheHeader).

![](assets/cardquickactions.png)

#### Mode Carte pour les utilisateurs non administrateurs

Les cartes des dossiers, dans l'Affichage Carte, affichent les informations de hiérarchie des dossiers à des utilisateurs non administrateurs (éditeur, observateur et utilisateur invité). Cette fonctionnalité permet aux utilisateurs de connaître l'emplacement des dossiers, y accède par rapport à la hiérarchie parent.
Les informations sur la hiérarchie des dossiers sont particulièrement utiles pour différencier les dossiers dont les noms sont similaires à ceux d'autres dossiers partagés à partir d'une hiérarchie de dossiers différente. Si les utilisateurs non administrateurs ne connaissent pas la structure de dossiers des ressources partagées avec eux, les ressources/dossiers aux noms similaires peuvent sembler confus.

* Les chemins affichés sur les cartes correspondantes sont tronqués pour s'adapter aux tailles de carte. Cependant, les utilisateurs peuvent voir le chemin d'accès complet en tant qu'horodatage sur le chemin tronqué.

![](assets/folder-hierarchy1.png)

**Option Aperçu pour afficher les propriétés des ressources**

L'option Aperçu est disponible pour les utilisateurs non administrateurs (Editeurs, Visionneuses et Utilisateurs invités) pour afficher les propriétés de ressource des fichiers/dossiers sélectionnés. L’option Aperçu est visible :

1. dans la barre d’outils supérieure lors de la sélection d’une ressource/d’un dossier ;
2. dans le menu déroulant, lors de la sélection du sélecteur de rail.

S’ils choisissent l’option Aperçu lorsqu’une ressource/un dossier est sélectionné, les utilisateurs peuvent voir le titre, le chemin et l’heure de création de la ressource. En revanche, sur la page des détails de la ressource, l’option Aperçu permet aux utilisateurs d’afficher les métadonnées de la ressource.

![](assets/overview-option.png)

![](assets/overview-rail-selector.png)

#### Paramètres d’affichage en mode Carte

La boîte de dialogue Paramètres d’affichage s’ouvre lors de la sélection de Paramètres d’affichage dans le sélecteur de vue. Il vous permet de redimensionner les vignettes de fichiers en mode Carte. De cette façon, vous pouvez personnaliser votre affichage et contrôler le nombre de miniatures qui s’affiche.

![](assets/cardviewsettings.png)

### Mode Liste

![](assets/list-view.png)

Le mode Liste répertorie les informations pour chaque ressource au niveau actuel. Le mode Liste fournit les informations suivantes :

* Image miniature des ressources
* Nom
* Titre
* Paramètres régionaux
* Type
* Dimension
* Taille
* Évaluation
* Chemin du dossier présentant la hiérarchie des ressources<sup>*</sup>
* Date de publication de cette ressource sur Brand Portal

* La colonne Chemin vous permet d’identifier facilement l’emplacement des ressources dans la hiérarchie de dossiers. You can navigate down the hierarchy by tapping/clicking the resource name, and back up by using the [breadcrumbs in the header](https://helpx.adobe.com/experience-manager/6-5/sites/authoring/using/basic-handling.html#TheHeader).

<!--
Comment Type: draft lastmodifiedby="mgulati" lastmodifieddate="2018-08-17T03:12:05.096-0400" type="annotation">Removed:- "Selecting assets in list view To select all items in the list, use the checkbox at the upper left of the list. When all items in the list are selected, this check box appears checked. To deselect all, click or tap the checkbox. When only some items are selected, it appears with a minus sign. To select all, click or tap the checkbox. To deselect all, click or tap the checkbox again. You can change the order of items using the dotted vertical bar at the far right of each item in the list. Tap/click the vertical selection bar and drag the item to a new position in the list."
 -->

### Paramètres d’affichage en mode Liste

List view shows asset **Name** as the first column by default. Des informations complémentaires, telles que le titre, les paramètres régionaux, le type, les dimensions, la taille, l’évaluation et l’état de publication sont également affichées. Toutefois, vous pouvez choisir les colonnes à afficher à l’aide de Paramètres d’affichage.

![](assets/list-view-setting.png)

### Mode Colonnes

![](assets/column-view.png)

Utilisez le mode Colonnes pour parcourir une arborescence de contenu à travers une série de colonnes en cascade. Ce mode vous aide à visualiser et parcourir la hiérarchie de ressources.

La sélection d’une ressource dans la première colonne (à l’extrémité gauche) présente les ressources enfants dans la deuxième colonne à droite. La sélection d’une ressource dans la deuxième colonne présente les ressources enfants dans la troisième colonne à droite, et ainsi de suite.

Vous pouvez parcourir l’arborescence vers le haut et vers le bas en appuyant ou en cliquant sur le nom de la ressource ou sur le chevron à droite du nom.

* Le nom de la ressource et le chevron sont mis en surbrillance lorsque vous cliquez ou appuyez dessus.
* Le fait d’appuyer ou de cliquer sur la miniature sélectionne la ressource.
* Lorsque cette option est sélectionnée, une coche est apposée sur la miniature, et le nom de la ressource est mis en surbrillance.
* Les détails de la ressource sélectionnée sont affichés dans la dernière colonne.

Lorsqu’une ressource est sélectionnée en mode Colonne, sa représentation visuelle est affichée dans la colonne finale avec les informations suivantes :

* Titre
* Nom
* Dimensions
* Date and time when asset was published to [!DNL Brand Portal] from [!DNL AEM]
* Taille
* Type
* Option Plus de détails pour accéder à la page de détails de la ressource

<!--
Comment Type: draft

<h3>Selecting Resources</h3>
-->

<!--
Comment Type: draft

<p>Selecting a specific resource depends on a combination of the view and the device:</p>
-->

<!--
Comment Type: draft

<table border="1" cellpadding="1" cellspacing="0" width="100%">
<tbody>
<tr>
<td> </td>
<td>Select</td>
<td>Deselect</td>
</tr>
<tr>
<td>Column View<br /> </td>
<td>
<ul>
<li>Desktop:<br /> Mouseover, then use the check mark quick action</li>
<li>Mobile device:<br /> Tap the thumbnail</li>
</ul> </td>
<td>
<ul>
<li>Desktop:<br /> Click the thumbnail</li>
<li>Mobile device:<br /> Tap the thumbnail</li>
</ul> </td>
</tr>
<tr>
<td>Card View<br /> </td>
<td>
<ul>
<li>Desktop:<br /> Mouseover, then use the check mark quick action</li>
<li>Mobile device:<br /> Tap-and-hold the card</li>
</ul> </td>
<td>
<ul>
<li>Desktop:<br /> Click the card</li>
<li>Mobile device:<br /> Tap the card</li>
</ul> </td>
</tr>
<tr>
<td>List View</td>
<td>
<ul>
<li>Desktop:<br /> Mouseover, then use the check mark quick action</li>
<li>Mobile device:<br /> Tap the thumbnail</li>
</ul> </td>
<td>
<ul>
<li>Desktop:<br /> Click the thumbnail</li>
<li>Mobile device:<br /> Tap the thumbnail</li>
</ul> </td>
</tr>
</tbody>
</table>
-->

<!--
Comment Type: draft

<h4>Deselecting All</h4>
-->

<!--
Comment Type: draft

<p>In all cases, as you select items the count of the items selected is displayed at the upper right of the toolbar.</p>
<p>You can deselect all items and exit selection mode by clicking or tapping the X next to the count.</p>
-->

<!--
Comment Type: draft

<p>In all views, all items can be deselected by tapping escape on the keyboard if you are using a desktop device.</p>
-->

## Arborescence de contenu {#content-tree}

Outre ces vues, utilisez l'arborescence pour explorer la hiérarchie des ressources pendant que vous affichez et sélectionnez les éléments ou dossiers souhaités.

To open the tree view, tap/click the rail selector at upper left and select the **Content tree** from the menu.

![](assets/contenttree.png)

Dans la hiérarchie de contenu, accédez à la ressource de votre choix.

![](assets/content-tree.png)

## Détails de la ressource {#asset-details}

La page Détails de la ressource permet d’afficher une ressource, de la télécharger, de partager le lien correspondant, de la déplacer vers une collection ou d’afficher sa page de propriétés. Elle vous permet également de parcourir la page de détails d’autres ressources au sein du même dossier, l’une après l’autre.

![](assets/asset-detail.png)

Pour consulter les métadonnées de la ressource, ou afficher ses différents rendus, utilisez le sélecteur de rail sur la page Détails de la ressource.

![](assets/asset-overview.png)

Vous pouvez afficher tous les rendus disponibles de la ressource sur la page Détails de la ressource, puis sélectionnez un rendu pour la prévisualiser.

![](assets/renditions.png)

To open the asset properties page, use *Properties (p)* option on the top bar.

![](assets/asset-properties.png)

You can also view a list of all its related assets (source or derived assets on AEM) on an asset's properties page, as asset relationship is also published from [!DNL AEM] to [!DNL Brand Portal].
