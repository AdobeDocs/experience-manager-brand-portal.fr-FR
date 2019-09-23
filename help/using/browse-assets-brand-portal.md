---
title: Exploration des ressources sur Brand Portal
seo-title: Exploration des ressources sur Brand Portal
description: Explorez les ressources, parcourez les hiérarchies de ressources et recherchez des ressources grâce à diverses options de modes et d’éléments d’IU sur Brand Portal.
seo-description: Explorez les ressources, parcourez les hiérarchies de ressources et recherchez des ressources grâce à diverses options de modes et d’éléments d’IU sur Brand Portal.
uuid: 178ce217-0050-4922-a204-f4539d46f539
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: référencereference
topic-tags: introduction
discoiquuid: a70ce694-81d1-4829-9e61-b6412e013e5c
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Exploration des ressources sur Brand Portal {#browsing-assets-on-brand-portal}

AEM Assets Brand Portal fournit plusieurs fonctionnalités et éléments d’IU pour faciliter l’exploration des ressources, la navigation à travers les hiérarchies de ressources et la recherche de ressources en utilisant différentes options de modes.

Le logo AEM dans la barre d’outils AEM supérieure permet aux utilisateurs administrateurs d’accéder au panneau des outils d’administration.

![](assets/aemlogo.png)

![](assets/admin-tools-panel-2.png)

![](assets/bp_subheader.png)

Le sélecteur de rail dans la partie supérieure gauche de Brand Portal se déroule pour afficher les options permettant de naviguer au sein des hiérarchies de ressources, de simplifier la recherche et d’afficher les ressources.

![](assets/siderail-1.png)

Vous pouvez afficher, parcourir et sélectionner les ressources à l’aide de l’un des modes disponibles (Carte, Colonnes et Liste) dans le sélecteur de mode dans la partie supérieure droite de Brand Portal.

![](assets/viewselector.png)

## Affichage et sélection de ressources {#viewing-and-selecting-resources}

Viewing, navigating, and selecting each are conceptually the same across all views, but have small variations in handling, depending on the view you are using.

Vous pouvez afficher, parcourir et sélectionner (pour une action ultérieure) vos ressources dans tous les modes disponibles :

* Mode Colonnes
* Mode Carte
* Mode Liste

### Mode Carte

![](assets/card-view.png)

Le mode Carte affiche les cartes d’informations de chaque élément au niveau actuel. Ces cartes présentent   les informations suivantes :

* Représentation visuelle de la ressource/du dossier.
* Type
* Titre
* Nom
* Date et heure de   La ressource a été publiée sur le portail de marque à partir d’AEM
* Taille
* Dimensions

You can navigate down the hierarchy by tapping/clicking cards (taking care to avoid the quick actions) or up again by using the [breadcrumbs in the header](https://helpx.adobe.com/experience-manager/6-5/sites/authoring/using/basic-handling.html#TheHeader).

![](assets/cardquickactions.png)

#### Mode Carte pour les utilisateurs non-administrateurs

En mode Carte, les cartes de dossiers affichent les informations sur la hiérarchie des dossiers d’affichage aux utilisateurs non-administrateurs (éditeur, observateur et utilisateur invité). Cette fonctionnalité permet aux utilisateurs de connaître l’emplacement des dossiers auxquels ils accèdent par rapport à la hiérarchie parente.
Les informations sur la hiérarchie de dossiers sont particulièrement utiles pour différencier des dossiers ayantportant des noms similaires à d’autres dossiers partagés à partir d’une hiérarchie de dossiers distincte. Si les utilisateurs non-administrateurs ne connaissent pas la structure de dossiers des ressources partagées avec eux, les ressources/dossiers aux noms similaires peuvent paraître déroutants.

* Les chemins affichés sur les cartes respectives sont tronqués pour s’adapter à la taille des cartesde celles-ci. However, users can see the full path as a tool-tip on hovering over the truncated path.

![](assets/folder-hierarchy1.png)

**Option Aperçu pour afficher les propriétés des ressources**

L’option Aperçu est proposée aux utilisateurs non-administrateurs (éditeurs, observateurs et utilisateurs invités) pour leur permettre d’afficher les propriétés des ressources/dossiers sélectionnés. L’option Aperçu est visible :

* dans la barre d’outils en haut de la page lors de la sélection d’un fichier/dossier.
* in the drop-down on selecting the rail Selector.

On selecting the [!UICONTROL Overview] option while an asset/folder is selected, users can see the title, path, and time of asset creation. En revanche, sur la page des détails de la ressource, l’option Aperçu permet aux utilisateurs d’afficher les métadonnées de la ressource.

![](assets/overview-option.png)

![](assets/overview-rail-selector.png)

#### Paramètres d’affichage en mode Carte

[!UICONTROL La boîte de dialogue Paramètres d’affichage s’ouvre lors de la sélection de l’option Paramètres d’affichage dans le sélecteur de mode. ]**** Elle vous permet de redimensionner les miniatures des ressources en mode Carte. De cette façon, vous pouvez personnaliser votre affichage et contrôler le nombre de miniatures affichées.

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

Le mode Liste affiche le [!UICONTROL Nom] des ressources comme première colonne par défaut. Additional information, such as asset [!UICONTROL Title], [!UICONTROL Locale], [!UICONTROL Type], [!UICONTROL Dimensions], [!UICONTROL Size], [!UICONTROL Rating], publish status are also shown. However, you can select the columns to be shown using [!UICONTROL View Settings].

![](assets/list-view-setting.png)

### Mode Colonnes

![](assets/column-view.png)

Utilisez le mode Colonnes pour parcourir une arborescence de contenu à travers une série de colonnes en cascade. Ce mode vous aide à visualiser et à parcourir la hiérarchie de ressources.

La sélection d’une ressource dans la première colonne (à l’extrémité gauche) présente les ressources enfants dans la deuxième colonne à droite. La sélection d’une ressource dans la deuxième colonne présente les ressources enfants dans la troisième colonne à droite, et ainsi de suite.

Vous pouvez parcourir l’arborescence vers le haut et vers le bas en appuyant ou en cliquant sur le nom de la ressource ou sur le chevron à droite du nom.

* Le nom de la ressource et le chevron sont mis en surbrillance lorsque vous cliquez ou appuyez dessus.
* Le fait d’appuyer ou de cliquer sur la miniature sélectionne la ressource.
* Lorsqu'elle est sélectionnée, une coche est apposée sur la miniature et le nom de la ressource est mis en surbrillance.
* Les détails de la ressource sélectionnée sont affichés dans la dernière colonne.

Lorsqu’une ressource est sélectionnée en mode Colonne, sa représentation visuelle est affichée dans la colonne finale avec les informations suivantes :

* Titre
* Nom
* Dimensions
* Date et heure de publication de la ressource sur Brand Portal à partir d’AEM
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

## Arborescence de contenu   {#content-tree}

En plus de ces vues, utilisez l’arborescence pour descendre dans la hiérarchie de ressources lorsque vous affichez et sélectionnez les ressources ou dossiers de votre choix.

Pour ouvrir l’arborescence, appuyez/cliquez sur le sélecteur de rail en haut à gauche et sélectionnez **[!UICONTROL Arborescence de contenu]dans le menu.**

![](assets/contenttree.png)

Dans la hiérarchie de contenu, accédez à la ressource de votre choix.

![](assets/content-tree.png)

## Détails de la ressource   {#asset-details}

La page Détails de la ressource permet d’afficher une ressource, de la télécharger, de partager son lien, de la déplacer vers une collection ou d’afficher sa page de propriétés. Elle vous permet également de parcourir la page de détails d’autres ressources au sein du même dossier, l’une après l’autre.

![](assets/asset-detail.png)

To view the asset's metadata, or view its various renditions, use the rail selector on asset detail page.

![](assets/asset-overview.png)

Vous pouvez afficher tous les rendus disponibles de la ressource sur la page Détails de la ressource, puis sélectionner un rendu pour le prévisualiser.

![](assets/renditions.png)

To open the asset properties page, use **[!UICONTROL Properties (p)]** option from the top bar.

![](assets/asset-properties.png)

Vous pouvez également afficher la liste de toutes ses ressources associées (ressources sources ou dérivées sur AEM) sur la page des propriétés de la ressource, car les relations de la ressource sont également publiées d’AEM vers Brand Portal.
