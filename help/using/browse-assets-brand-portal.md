---
title: Exploration des ressources sur Brand Portal
seo-title: Exploration des ressources sur Brand Portal
description: Explorez les ressources, parcourez les hiérarchies de ressources et recherchez des ressources grâce à diverses options de modes et d’éléments d’IU sur Brand Portal.
seo-description: Explorez les ressources, parcourez les hiérarchies de ressources et recherchez des ressources grâce à diverses options de modes et d’éléments d’IU sur Brand Portal.
uuid: 178ce217-0050-4922-a204-f4539d46f539
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: introduction
discoiquuid: a70ce694-81d1-4829-9e61-b6412e013e5c
translation-type: ht
source-git-commit: 86078dd07b5d487f8cf5cd08bc46e4745529c873
workflow-type: ht
source-wordcount: '1039'
ht-degree: 100%

---


# Exploration des ressources sur Brand Portal {#browsing-assets-on-brand-portal}

AEM Assets Brand Portal fournit plusieurs fonctionnalités et éléments d’IU pour faciliter l’exploration des ressources, la navigation à travers les hiérarchies de ressources et la recherche de ressources en utilisant différentes options de modes.

Le logo AEM dans la barre d’outils AEM supérieure permet aux utilisateurs administrateurs d’accéder au panneau des outils d’administration.

![](assets/aemlogo.png)

![](assets/admin-tools-panel-2.png)

![](assets/bp_subheader.png)<br />

Le sélecteur de rail dans la partie supérieure gauche de Brand Portal se déroule pour afficher les options permettant de naviguer au sein des hiérarchies de ressources, de simplifier la recherche et d’afficher les ressources.

![](assets/siderail-1.png)

Vous pouvez afficher, parcourir et sélectionner les ressources à l’aide de l’un des modes disponibles (Carte, Colonnes et Liste) dans le sélecteur de mode dans la partie supérieure droite de Brand Portal.

![](assets/viewselector.png)

## Affichage et sélection de ressources {#viewing-and-selecting-resources}

L’affichage, la navigation et la sélection sont identiques sur le plan conceptuel dans tous les modes, mais leur manipulation présente de légères variations en fonction du mode utilisé.

Vous pouvez afficher, parcourir et sélectionner (pour une action ultérieure) vos ressources dans tous les modes disponibles :

* Mode Colonnes
* Mode Carte
* Mode Liste

### Mode Carte

![](assets/card-view.png)

Le mode Carte affiche les cartes d’informations de chaque élément au niveau actuel. Ces cartes présentent les les informations suivantes :

* Représentation visuelle de la ressource/du dossier.
* Type
* Titre
* Nom
* Date et heure de publication de la ressource sur Brand Portal à partir d’AEM
* Taille
* Dimensions

Vous pouvez parcourir la hiérarchie vers le bas en appuyant ou en cliquant sur des cartes (en veillant à éviter les actions rapides) ou vers le haut en utilisant le [chemin de navigation de l’en-tête](https://helpx.adobe.com/fr/experience-manager/6-5/sites/authoring/using/basic-handling.html#TheHeader).

![](assets/cardquickactions.png)

#### Mode Carte pour les utilisateurs non-administrateurs

En mode Carte, les cartes de dossiers affichent les informations sur la hiérarchie des dossiers d’affichage aux utilisateurs non-administrateurs (éditeur, observateur et utilisateur invité). Cette fonctionnalité permet aux utilisateurs de connaître l’emplacement des dossiers auxquels ils accèdent par rapport à la hiérarchie parente.
Les informations sur la hiérarchie de dossiers sont particulièrement utiles pour différencier des dossiers portant des noms similaires à d’autres dossiers partagés à partir d’une hiérarchie de dossiers distincte. Si les utilisateurs non-administrateurs ne connaissent pas la structure de dossiers des ressources partagées avec eux, les ressources/dossiers aux noms similaires peuvent paraître déroutants.

* Les chemins affichés sur les cartes respectives sont tronqués pour s’adapter à la taille de celles-ci. Toutefois, les utilisateurs peuvent afficher le chemin complet sous la forme d’une info-bulle en passant le pointeur de la souris sur le chemin tronqué.

![](assets/folder-hierarchy1.png)

**Option Aperçu pour afficher les propriétés des ressources**

L’option Aperçu est proposée aux utilisateurs non-administrateurs (éditeurs, observateurs et utilisateurs invités) pour leur permettre d’afficher les propriétés des ressources/dossiers sélectionnés. L’option Aperçu est visible :

* dans la barre d’outils supérieure lors de la sélection d’une ressource/d’un dossier ;
* dans le menu déroulant, lors de la sélection du sélecteur de rail.

S’ils choisissent l’option **[!UICONTROL Aperçu]** lorsqu’une ressource/un dossier est sélectionné, les utilisateurs peuvent voir le titre, le chemin et l’heure de création de la ressource. En revanche, sur la page des détails de la ressource, l’option Aperçu permet aux utilisateurs d’afficher les métadonnées de la ressource.

![](assets/overview-option.png)

![](assets/overview-rail-selector.png)

#### Paramètres d’affichage en mode Carte

La boîte de dialogue **[!UICONTROL Paramètres d’affichage]** s’ouvre lors de la sélection de l’option **[!UICONTROL Paramètres d’affichage]** dans le sélecteur de mode. Elle vous permet de redimensionner les miniatures des ressources en mode Carte. De cette façon, vous pouvez personnaliser votre affichage et contrôler le nombre de miniatures affichées.

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

La colonne Chemin vous permet d’identifier facilement l’emplacement des ressources dans la hiérarchie de dossiers. Vous pouvez naviguer vers le bas de la hiérarchie en appuyant/cliquant sur le nom de la ressource, puis revenir vers le haut à l’aide des [chemins de navigation de l’en-tête](https://helpx.adobe.com/fr/experience-manager/6-5/sites/authoring/using/basic-handling.html#TheHeader).

<!--
Comment Type: draft lastmodifiedby="mgulati" lastmodifieddate="2018-08-17T03:12:05.096-0400" type="annotation">Removed:- "Selecting assets in list view To select all items in the list, use the checkbox at the upper left of the list. When all items in the list are selected, this check box appears checked. To deselect all, click or tap the checkbox. When only some items are selected, it appears with a minus sign. To select all, click or tap the checkbox. To deselect all, click or tap the checkbox again. You can change the order of items using the dotted vertical bar at the far right of each item in the list. Tap/click the vertical selection bar and drag the item to a new position in the list."
 -->

### Paramètres d’affichage en mode Liste

Le mode Liste affiche le **[!UICONTROL Nom]** des ressources comme première colonne par défaut. Des informations complémentaires, telles que le **[!UICONTROL Titre]**, les **[!UICONTROL Paramètres régionaux]**, le **[!UICONTROL Type]**, les **[!UICONTROL Dimensions]**, la **[!UICONTROL Taille]**, l’**[!UICONTROL Évaluation]** et l’état de publication de la ressource, sont également affichées. Vous pouvez toutefois choisir les colonnes à afficher à l’aide de **[!UICONTROL Paramètres d’affichage]**.

![](assets/list-view-setting.png)

### Mode Colonnes

![](assets/column-view.png)

Utilisez le mode Colonnes pour parcourir une arborescence de contenu à travers une série de colonnes en cascade. Ce mode vous aide à visualiser et à parcourir la hiérarchie de ressources.

La sélection d’une ressource dans la première colonne (à l’extrémité gauche) présente les ressources enfants dans la deuxième colonne à droite. La sélection d’une ressource dans la deuxième colonne présente les ressources enfants dans la troisième colonne à droite, et ainsi de suite.

Vous pouvez parcourir l’arborescence vers le haut et vers le bas en appuyant ou en cliquant sur le nom de la ressource ou sur le chevron à droite du nom.

* Le nom de la ressource et le chevron sont mis en surbrillance lorsque vous cliquez ou appuyez dessus.
* Le fait d’appuyer ou de cliquer sur la miniature sélectionne la ressource.
* Lorsqu’elle est sélectionnée, une coche est apposée sur la miniature et le nom de la ressource est mis en surbrillance.
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

Pour ouvrir l’arborescence, appuyez/cliquez sur le sélecteur de rail en haut à gauche et sélectionnez **[!UICONTROL Arborescence de contenu]** dans le menu.

![](assets/contenttree.png)

Dans la hiérarchie de contenu, accédez à la ressource de votre choix.

![](assets/content-tree.png)

## Détails de la ressource   {#asset-details}

La page Détails de la ressource permet d’afficher une ressource, de la télécharger, de partager son lien, de la déplacer vers une collection ou d’afficher sa page de propriétés. Elle vous permet également de parcourir la page de détails d’autres ressources au sein du même dossier, l’une après l’autre.

![](assets/asset-detail.png)

Pour consulter les métadonnées de la ressource, ou afficher ses différents rendus, utilisez le sélecteur de rail sur la page Détails de la ressource.

![](assets/asset-overview.png)

Vous pouvez afficher tous les rendus disponibles de la ressource sur la page Détails de la ressource, puis sélectionner un rendu pour le prévisualiser.

![](assets/renditions.png)

Pour ouvrir la page des propriétés de la ressource, utilisez l’option **[!UICONTROL Propriétés (p)]** de la barre supérieure.

![](assets/asset-properties.png)

Vous pouvez également afficher la liste de toutes ses ressources associées (ressources sources ou dérivées sur AEM) sur la page des propriétés de la ressource, car les relations de la ressource sont également publiées d’AEM vers Brand Portal.
