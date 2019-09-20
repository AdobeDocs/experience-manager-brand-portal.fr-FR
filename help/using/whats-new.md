---
title: Nouveautés d’AEM Assets Brand Portal
seo-title: Nouveautés d’AEM Assets Brand Portal
description: Découvrez les nouvelles fonctionnalités et améliorations de la version 6.4.4.
seo-description: Découvrez les nouvelles fonctionnalités et améliorations de la version 6.4.4.
uuid: 2c59d738-9b53-4f25-a205-13bf75c80b77
contentOwner: bdhar
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: référencereference
topic-tags: introduction
discoiquuid: fec32ca3-142b-4a11-9b92-5113fc27277a
translation-type: ht
source-git-commit: cbb64eb8a79480a1ccedbe5131a38ddf6eaec88d

---


# Nouveautés d’AEM Assets Brand Portal {#what-s-new-in-aem-assets-brand-portal}

Adobe Experience Manager (AEM) Assets Brand Portal permet d’acquérir, de contrôler et de distribuer facilement et en toute sécurité des ressources créatives approuvées destinées à des tiers externes et aux collaborateurs de l’entreprise sur différents appareils. Brand Portal améliore l’efficacité du partage des ressources, accélère la mise sur le marché des ressources et réduit les risques de non-conformité et d’accès non autorisé. Adobe a pour objectif d’améliorer l’expérience globale de Brand Portal. Vous trouverez ci-dessous un aperçu des nouvelles fonctionnalités et améliorations.

## Changements dans la version 6.4.4 {#what-is-changing-in}

La version 6.4.4 de Brand Portal est axée sur les améliorations apportées à la recherche de texte et les principales requêtesdemandes des clients. Consultez les dernières [Notes de mise à jour de Brand  Portal](brand-portal-release-notes.md).

### Améliorations de la recherche {#search-enhancements}

Brand Portal 6.4.4 et les versions ultérieures prennent en charge la recherche de texte partielle sur le prédicat de propriété du panneau de filtrage. Pour permettre la recherche de texte partielle, vous devez activer l’option **Recherche partielle** dans le prédicat Propriété du formulaire de recherche.

Lisez les sections suivantes pour en savoir plus sur la recherche de texte partielle et la recherche par caractères génériques.

#### Recherche par expression partielle   {#partial-phrase-search}

Vous pouvez maintenant rechercher des ressources en spécifiant uniquement une partie (c’est-à-dire un mot ou deux) de l’expression recherchée dans le volet de filtrage.

**Cas d’utilisation**


La recherche par expression partielle s’avère utile lorsque vous n’êtes pas sûr de la combinaison exacte des mots apparaissant dans l’expression recherchée.

Par exemple, si votre formulaire de recherche dans Brand Portal utilise le prédicat de propriété pour une recherche partielle sur le titre des ressources, la spécification du terme **champ** renvoie toutes les ressources contenant le mot champ dans l’expression de leur titre.

![](assets/partialphrasesearch.png)

#### Recherche par caractères génériques {#wildcard-search}

Brand Portal permet d’utiliser un astérisque (*) dans la requête de recherche avec une partie du mot de l’expression recherchée.

**Cas d’utilisation**
Si vous n’êtes pas sûr des mots exacts apparaissant dans l’expression recherchée, vous pouvez utiliser une recherche par caractères génériques pour remplir les trous de votre requête.

Par exemple, la spécification de **climb*** renvoie toutes les ressources ayant des mots commençant par les caractères **climb** dans l’expression de leur titre si le formulaire de recherche dans Brand Portal utilise le prédicat de propriété pour une recherche partielle sur le titre des ressources.

![](assets/wildcard-prop.png)

De même, la spécification de :

* ***climb** renvoie toutes les ressources ayant des mots se terminant par les caractères **climb** dans l’expression de leur titre.

* ***climb*** renvoie toutes les ressources ayant des mots comprenant les caractères **climb** dans l’expression de leur titre.

>[!NOTE]
>
>Lorsque vous cochez la case **Recherche partielle**, l’option **Ignorer la casse** est sélectionnée par défaut.

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal-searching.md#facetedsearchbyapplyingfilterstosearch)

## Changements dans la version 6.4.3 {#what-changed-in}

La version 6.4.3 de Brand Portal fournitpropose aux organisations un alias alternatif en plus de leur ID de client dans l’URL d’accès à Brand Portal, une nouvelle configuration de hiérarchie de dossiers, des améliorations de la prise en charge des vidéos, la publication programmée à partir de l’instance d’auteur AEM vers Brand Portal ainsi que des améliorations opérationnelles. Elle répond également aux requêtesdemandes des clients.

### Navigation dans la hiérarchie de dossiers pour les non-administrateurs

Les administrateurs peuvent maintenant configurer la façon dont les dossiers s’affichent pour les utilisateurs non-administrateurs (éditeurs, observateurs et utilisateurs invités) lors de leur connexion. La configuration [Activer la hiérarchie de dossiers](../using/brand-portal-general-configuration.md) a été ajoutée dans **Paramètres généraux** au sein du panneau des outils d’administration. Si la configuration est :

* **activée**, l’arborescence de dossiers à partir du dossier racine est visible pour les utilisateurs non-administrateurs, ce qui leur procure une expérience de navigation semblable à celle des administrateurs ;
* **désactivée**, seuls les dossiers partagés sont affichés sur la page d’entrée.

![](assets/enable-folder-hierarchy.png)
**Le cas d’utilisation**

La fonctionnalité [Activer la hiérarchie de dossiers](../using/brand-portal-general-configuration.md) (lorsqu’elle est activée) vous aide à différencier les dossiers portant les mêmes noms, mais partagés depuis différentes hiérarchies. Lorsqu’ils se connectent, les utilisateurs non-administrateurs voient maintenant les dossiers parents virtuels (et ancêtres) des dossiers partagés.
![](assets/disabled-folder-hierarchy1-2.png) ![](assets/enabled-hierarchy1-2.png)

Les dossiers partagés sont organisés au sein des répertoires respectifs dans des dossiers virtuels. Vous pouvez identifier ces dossiers virtuels grâce à leur icône de cadenas.

Notez que la miniature par défaut des dossiers virtuels est l’image de miniature du premier dossier partagé.

![](assets/hierarchy1-nonadmin-2.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal-general-configuration.md)

### Recherche dans un chemin ou une hiérarchie de dossiers spécifique

Le prédicat **Explorateur de chemins d’accès** a été introduit dans le formulaire de recherche pour permettre la recherche de ressources dans un répertoire spécifique. Le chemin de recherche par défaut du prédicat de recherche pour l’explorateur de chemins d’accès est */content/dam/mac/&lt;id-de-client&gt;/* et il peut être configuré en modifiant le formulaire de recherche par défaut.

* Les utilisateurs administrateurs peuvent utiliser l’explorateur de chemins d’accès pour accéder à n’importe quel répertoire de dossiers sur Brand Portal.
* Les utilisateurs non-administrateurs peuvent utiliser l’explorateur de chemins d’accès pour accéder uniquement aux dossiers partagés avec eux, et revenir vers les dossiers parents.
Par exemple, */content/dam/mac/ &lt; id_ -de-client &gt;/foldera/folderb/folderc* est partagé avec un utilisateur non-administrateur. L’'utilisateur peut rechercher des ressources dans le folderC à l’'aide du navigateurde l’explorateur de chemins d’accès. Cet utilisateur peut également accéder à folderB et folderA (puisqu’'il s’'agit de parents du folderC partagé avec l’'utilisateur).

![](assets/edit-search-form.png)

**Le cas d’utilisation**

Vous pouvez maintenant restreindre la recherche de ressources au sein d’un dossier spécifique auquel vous avez accédé, au lieu de partir du dossier racine.

Notez que la recherche sous ces dossiers renvoie des résultats provenant seulement des ressources qui ont été partagées avec l’utilisateur.

![](assets/filter-panel.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal-search-facets.md#listofsearchpredicates)

### Prise en charge des rendus vidéo Dynamic Media

Les utilisateurs dont l’instance d’auteur AEM est en mode hybride Dynamic Media peuvent prévisualiser et télécharger les rendus Dynamic Media, en plus des fichiers vidéo originaux.

Pour autoriser la prévisualisation et le téléchargement des rendus Dynamic Media sur des comptes de client spécifiques, les administrateurs doivent spécifier **Configuration Dynamic Media** (URL du service vidéo (URL de la passerelle DM) et ID d’enregistrement pour récupérer la vidéo dynamique) dans la configuration **Vidéo** à partir du panneau des outils d’administration.

**Le cas d’utilisation**
Vous pouvez prévisualiser les vidéos Dynamic Media sur  :

* la page des détails de la ressource ;
* l’'affichage de la carte de la ressource ;
* la page de prévisualisation du partage de lien.

Les codes des vidéos Dynamic Media peuvent être téléchargés à partir de :

* Brand Portal
* Lien partagé

![](assets/edit-dynamic-media-config.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal.md#tenantaliasforportalurl)

### Publication planifiée sur Brand Portal

Le processusworkflow de publication des ressources (et dossiers) de l’'instance d’auteur d’e [AEM (6.4.2.0)](https://helpx.adobe.com/experience-manager/6-4/release-notes/sp-release-notes.html#main-pars_header_9658011) vers Brand  Portal peut être planifié pour une date et une heure ultérieures.

De façon similaire, les ressources publiées peuvent être supprimées du portail à une date (ou heure) ultérieure, en planifiant le workflow Annuler la publication sur Brand Portal.

![](assets/schedule-publish.png)
![](assets/publishlater-workflow.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal.md#tenantaliasforportalurl)

### Alias de client configurable dans l’URL

Les organisations peuvent obtenir une URL de portail personnalisée comprenant un préfixe alternatif dans l’URL. Pour obtenir un alias pour le nom de client dans leur URL de portail existante, les organisations doivent entrer en contact avec l’assistance Adobe.

Notez que seul le préfixe de l’URL Brand Portal peut être personnalisé et non l’URL entière.\
Par exemple, une organisation avec le domaine existant **geomettrix.brand-portal.adobe.com** peut demander et obtenir la création de **geomettrixinc.brand-portal.adobe.com**.

Cependant, l’instance d’auteur AEM peut uniquement être [configurée](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html) avec l’URL d’ID client et non avec l’URL (alternative) d’alias du client.

**Le cas d’utilisation**
Les organisations peuvent répondre à leurs besoins de brandingvalorisation de marque en faisant personnaliser l’URL de leur portail, au lieu de se contenter de l’URL fournie par Adobe.

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal.md#tenantaliasforportalurl)

### Amélioration de l’expérience de téléchargement

La version offre une simplifie l’expérience de téléchargement simplifiée avec un nombre réduit de clics et d’avertissements lors du :

* choix du téléchargement exclusif des rendus (et non des ressources originales) ;
* téléchargement des ressources quand l’accès aux rendus originaux est restreint.

## Changements dans la version 6.4.2   {#what-changed-in-1}

La version 6.4.2 de Brand Portal apporte propose toute une gamme un ensemble de fonctionnalités visant non seulement à répondre aux besoins de distribution de ressources des organisations. Ces fonctionnalités mais aussi à les aider permettant aussi aux organisations àde toucher un grand nombre d’utilisateurs répartis à travers le monde grâce à l’accès des invités et à une expérience optimale facilitée par des téléchargements accélérés. Brand Portal fournit également un meilleur contrôle aux organisations par le biais de nouvelles configurations pour les administrateurs et de nouveaux rapports, et il répond aux requêtesdemandes des clients.

### Accès des invités

![](assets/bp-login-screen-1.png)

AEM Brand Portal permet à des invités d’accéder au portail. Un utilisateur invité ne requiert pas d’identifiants pour accéder au portail et il peut consulter et télécharger tous les dossiers et collections publics. Les utilisateurs invités peuvent ajouter des ressources à leur Lightbox (collection privée) et les télécharger. Ils peuvent aussi voir les prédicats de recherche de balises intelligentes ou non définis par les administrateurs. La session d’invité ne permet pas aux utilisateurs de créer des collections et des recherches enregistrées, ni de les partager à nouveau, d’accéder aux paramètres de collections et de dossiers et de partager les ressources en tant que liens.

Dans une entreprise, les sessions d’invités multiples simultanées sont permises, mais limitées à 10 % du nombre total d’utilisateurs de cette entreprise.

Une session d’invité reste active pendant deux heures. Par conséquent, l’état de Lightbox est également conservé jusqu’à deux heures à compter de l’heure de début de la session. Au bout de deux heures, la session d’invité doit redémarrer et l’état de Lightbox est donc perdu.

### Accélération des téléchargements

Les utilisateurs de Brand Portal peuvent tirer parti des téléchargements rapides reposant sur IBM Aspera Connect pour obtenir des vitesses jusqu’à 25 fois plus rapides et profiter d’une expérience de téléchargement transparente quel que soit leur situation géographique. Pour télécharger les ressources plus rapidement à partir de Brand Portal ou du lien partagé, les utilisateurs doivent sélectionner l’option **Activer l’accélération des téléchargements** dans la boîte de dialogue de téléchargement, à condition que l’accélération des téléchargements soit activée dans leur organisation.

![](assets/donload-assets-dialog-2.png)

Pour activer l’accélération des téléchargements reposant sur IBM Aspera, les administrateurs doivent sélectionner l’option **Activer l’accélération des téléchargements** (qui est désactivée par défaut) dans [Paramètres généraux](brand-portal-general-configuration.md#allow-download-acceleration) au niveau du panneau des outils d’administration. Pour connaître les conditions préalables et les étapes de dépannage afin de télécharger des fichiers de ressources plus rapidement à partir de Brand Portal et de liens partagés, consultez le [Guide d’accélération des téléchargements à partir de Brand Portal](../using/accelerated-download.md#main-pars-header).

### Rapport sur les connexions des utilisateurs

Un nouveau rapport a été ajouté pour suivre les connexions des utilisateurs. Le rapport **Connexions des utilisateurs** peut être essentiel pour permettre aux entreprises de réaliser un audit et de garder un œil sur les administrateurs délégués et d’autres utilisateurs de Brand Portal.

Le rapport consigne les noms d’affichage, les adresses e-mail, les personnagesrôles (administrateur, observateur, éditeur et invité), les groupes, la dernière connexion, l’état d’activité et le nombre de connexions de chaque utilisateur à partir du déploiement de Brand Portal 6.4.2 jusqu’au moment de la génération du rapport. Les administrateurs peuvent exporter le rapport au format .csv. Utilisé avec les autres rapports, le rapport Connexions des utilisateurs permet aux entreprises de contrôler plus étroitement les interactions des utilisateurs avec les ressources de marque approuvées, assurant ainsi le respect des directives des bureaux de conformité d’entreprise.

![](assets/user-logins-1.png)

### Accès aux rendus originaux

Les administrateurs peuvent restreindre l’accès des utilisateurs aux fichiers images originaux (.jpeg, .tiff, .png, .bmp, .gif, .pjpeg, x-portable-anymap, x-portable-bitmap, x-portable-graymap, x-portable-pixmap, x-rgb, x-xbitmap, x-xpixmap, x-icon, image/photoshop, image/x-photoshop, .psd, image/vnd.adobe.photoshop) et accorder l’accès aux rendus de basse résolution téléchargés à partir de Brand Portal ou d’un lien partagé. Cet accès peut être contrôlé au niveau de groupe d’utilisateurs depuis l’onglet Groupes de la page Rôles utilisateur du panneau des outils d’administration.

![](assets/access-original-rend-1.png)

* Par défaut, tous les utilisateurs peuvent télécharger les rendus originaux, car l’option Accès à l’original est activée pour tous.
* Les administrateurs doivent désélectionner les cases correspondantes afin d’empêcher un groupe d’utilisateurs d’accéder aux rendus originaux.
* Si un utilisateur est membre de plusieurs groupes, mais qu’un seul de ces groupes est sujet à des restrictions, celles-ci s’appliquent à cet utilisateur.
* Les restrictions ne s’appliquent pas aux administrateurs, même s’ils sont membres de groupes aux droits restreints.
* Les permissionsautorisations de l’utilisateur partageant des ressources sous forme de liens s’appliquent aux utilisateurs qui téléchargent des ressources à partir de liens partagés.

### Chemin de hiérarchie de dossiers en modes Carte et Liste

En mode Carte, les cartes de dossiers affichent désormais lesdes informations sur la hiérarchie de dossiers pour les utilisateurs non-administrateurs (éditeur, observateur et utilisateur invité). Cette fonctionnalité permet aux utilisateurs de connaître l’emplacement des dossiers auxquels ils accèdent par rapport à la hiérarchie parente.

Les informations sur la hiérarchie de dossiers sonts’avèrent particulièrement utiles pour différencier des dossiers ayant portant des noms similaires à d’autres dossiers partagés à partir d’une hiérarchie de dossiers distincte. Si les utilisateurs non-administrateurs ne connaissent pas la structure de dossiers des ressources partagées avec eux, les ressources/dossiers aux noms similaires peuvent paraître déroutants.

* Les chemins affichés sur les cartes respectives sont tronqués pour s’adapter à la taille des cartesde celles-ci. Toutefois, lLes utilisateurs peuvent voir toutefois afficher le chemin complet sous forme d’info-bulle en passant la souris pointant sur le chemin tronqué.

![](assets/folder-hierarchy1-1.png)

Le mode Liste affiche le chemin du dossier des ressources dans une colonne pour tous les utilisateurs de Brand Portal.

![](assets/list-view-1.png)

### Option Aperçu pour afficher les propriétés des ressources

Brand Portal fournit aux utilisateurs non -administrateurs (éditeurs, observateurs et utilisateurs invités) l’option Aperçu qui leur permet d’afficher les propriétés de ressources/dossiers sélectionnés. L’option Aperçu est visible :

1. dans la barre d’outils supérieure lors de la sélection d’une ressource/d’un dossier ;
2. dans le menu déroulant, lors de la sélection du sélecteur de rail.

S’ils choisissent l’option Aperçu lorsqu’une ressource/un dossier est sélectionné, les utilisateurs peuvent voir le titre, le chemin et l’heure de création de la ressource. En revanche, sur la page des détails de la ressource, l’option Aperçu permet aux utilisateurs d’afficher les métadonnées de la ressource.

![](assets/overview-option-2.png)

![](assets/overview-rail-selector-2.png)

## Nouvelles configurations

Six nouvelles configurations ont été ajoutées pour permettre aux administrateurs d’activer/de désactiver les fonctionnalités suivantes sur les clients spécifiques :

* Autoriser l’accès des invités
* Autoriser les utilisateurs à demander l’accès à Brand Portal
* Autoriser les administrateurs à supprimer des ressources de Brand Portal
* Autoriser la création de collections publiques
* Autoriser la création de collections dynamiques publiques
* Autoriser l’accélération des téléchargements

Les configurations ci-dessus sont disponibles sous Accès et Paramètres généraux dans le panneau des outils d’administration.

![](assets/access-configs-1.png)
![](assets/general-configs-1.png)
![](assets/admin-tools-panel-13.png)

### Adobe.io héberge une IU pour configurer les intégrations oAuth

À compter de la version 6.4.2, Brand Portal utilise l’interface Adobe.io [https://legacy-oauth.cloud.adobe.io/](https://legacy-oauth.cloud.adobe.io/) pour créer l’application JWT qui rend possible la configuration des intégrations oAuth de façon à permettre l’intégration d’AEM Assets avecà Brand Portal. Auparavant, l’IU de configuration des intégrations OAuth était hébergée sur [https://marketing.adobe.com/developer/](https://marketing.adobe.com/developer/). Pour en savoir plus sur l’intégration d’AEM Assets avecà Brand Portal pour publier des ressources et des collections poursur Brand Portal, consultez [Configuration de l’intégration d’AEM Assets avec Brand Portal](https://helpx.adobe.com/in/experience-manager/6-4/assets/using/brand-portal-configuring-integration.html).

## Améliorations de la recherche

Les administrateurs peuvent rendre les prédicats de propriétés non sensibles à la casse en utilisant le prédicat de propriété mis à jour qui dispose d’une case à cocher pour l’option Ignorer la casse. Cette option est disponible pour les prédicats de propriété et les prédicats de propriété à plusieurs valeurs.\
Toutefois, la recherche non sensible à la casse est comparativement plus lente que la recherche par défaut de prédicat de propriété. La multiplication de prédicats non sensibles à la casse dans le filtre de recherche peut ralentir la recherche. Il est donc conseillé d’utiliser la fonction de recherche non sensible à la casse judicieusement.

## Changements dans la version 6.4.1   {#what-changed-in-2}

Brand Portal 6.4.1 est une version de mise à niveau de la plate-forme qui contient plusieurs nouvelles fonctionnalités et des améliorations essentielles en termes de navigation et de recherche, ainsi que des améliorations de performances visant à offrir une expérience client optimale.

### Améliorations de la navigation

* Nouveau rail d’arborescence de contenu pour naviguer rapidement au sein d’une hiérarchie de ressources.

![](assets/contenttree-2.png)

* Nouveaux raccourcis clavier comme _(p)_ pour accéder à la page Propriétés, _(e)_ pour la fonction Modifier et _(Ctrl+c)_ pour Copier.
* Amélioration du défilement et de l’expérience de chargement différé en modes Carte et Liste afin de parcourir un grand nombre de ressources.
* Amélioration du Mmode Carte amélioré avec la prise en charge de cartes de différentes dimensions en fonction du paramètre d’affichage.

![](assets/cardviewsettings-1.png)

* Le mode Carte affiche désormaismaintenant un horodatage lorsque vous placez le curseurpointez sur le libellé de la date.

* Amélioration du mode Colonne avec l’option **Plus de détails** affichée sous la capture instantanée de la ressource, ce qui vous permet d’accéder à la page des détails d’une ressource.

![](assets/columnmoredetail.png)

* Le mode Liste affiche désormaismaintenant par défaut le nom de fichier des ressources dans la première colonne, en plus des informations suivantes : paramètres régionaux, type de ressource, dimensions, taille, évaluation et publication. La nouvelle option **Paramètres d’affichage** peut être utilisée pour configurer la quantité de détails à afficher en mode Liste.

* Amélioration apportée aux détails des ressources avec la possibilité d’effectuer des allers et retours entre les ressources à l’aide des nouveaux boutons de navigation et d’afficher le nombre de ressources.

![](assets/navbtn.png)

* Possibilité de prévisualiser les fichiers audio, téléchargés depuis AEM, dans la page des détails des ressources.
* Nouvelle fonctionnalité Ressources associées dans les propriétés des ressources. Les ressources associées à d’autres ressources sources/dérivées dans AEM et publiées sur Brand Portal préservent désormais leurs relations intactes dans Brand Portal, avec des liens vers les ressources associées dans la page des propriétés.
* Introduction d’une nouvelle configuration pour limiter la création de collections publiques par les utilisateurs n’étant pas administrateurs. Les entreprises peuvent collaborer avec l’équipe de support Adobe pour configurer cette fonctionnalité sur des comptes spécifiques.

### Améliorations de la recherche

* Introduction d’une fonctionnalité permettant de revenir à la même position dans les résultats de recherche, après avoir accédé à un élément de recherche, sans avoir à relancer la requête.
* Nouveau compteur de résultats de recherche pour afficher le nombre de résultats d’une recherche.
* Amélioration du filtre de recherche par type de fichier avec la possibilité de filtrer les résultats de recherche en fonction de types MIME plus précis, tels que .jpg, .png et .psd, par rapport aux options antérieures Images, Documents et Multimédia.
* Améliorations des filtres de recherche pour les collections avec des horodatages précis au lieu de la fonctionnalité précédente de curseur temporel.
* Introduction de nouveaux filtres Type d’accès dans la recherche des collections publiques et non publiques.

![](assets/accesstypefilter.png)

### Optimisations des téléchargements

* Un seul fichier volumineux est directement téléchargé, sans créer unde fichier zip, pour améliorer la vitesse et le débit.
* La limite de téléchargement de fichier compressé a été augmentée de 1 Go à 5 Go.

* Les utilisateurs peuvent désormaismaintenant choisir de ne télécharger que les fichiers personnalisés et originaux   et de bloquer les rendus prêts à l'emploi, lors du téléchargement de ressources à partir de Brand  Portal ou via la fonctionnalité de liens partagés.

![](assets/excludeautorendition.png)

### Améliorations des performances

* Vitesse de téléchargement des ressources jusqu’à 100 % plus rapide.
* Réponse de la recherche des ressources jusqu'à  40 % plus efficace.
* Performances de navigation jusqu’à 40 % plus réactives.

**Remarque** : Lles améliorations citées sont celles constatées lors des tests effectués en laboratoire.

### Amélioration des fonctionnalités de création de rapports

**Introduction Ajout du rapport Partage de liens**


Introduction Ajout d’un nouveau rapport afin de fournir des informations sur les liens partagés. Le rapport Partage de liens répertorie toutes les URL vers les ressources partagées avec des utilisateurs internes et externes à l’organisation pendant la période spécifiée. Il indique également si le lien a été partagé, par qui et sa date d’expiration.

![](assets/navigatereport.png)

**Modification du point d’entrée pour accéder au rapport Utilisation**


Le rapport Utilisation est maintenant consolidé avec d’autres rapports. Il est désormais consultable dans la console Rapports de ressources. Pour accéder à la console Rapports de ressources, naviguez jusqu’à **Créer/gérer des rapports** dans le panneau des outils d’administration.

![](assets/accessassetreport.png)

**Amélioration de l’'expérience des utilisateurs avec la création de rapports**
L'’interface de création de rapports sur Brand  Portal est devenue plus intuitive et offre un bien meilleur plus de contrôle aux entreprises. Hormis la création de divers rapports, les administrateurs peuvent désormais reconsulter les rapports générés et les télécharger ou les supprimer, car ils sont enregistrés dans Brand Portal.

Chaque rapport créé peut être personnalisé en ajoutant ou en supprimant des colonnes par défaut. De plus, des colonnes personnalisées peuvent être ajoutées aux rapports Téléchargement, Expiration et Publication pour contrôler leur degré de précision.

### Améliorations des outils d’administration

Amélioration du sélecteur de propriété dans les outils d’administration pour les métadonnées, la recherche et les rapports avec le type et la fonctionnalité de navigation afin de simplifier l’expérience de l’administrateur.

### Autres améliorations

* Les ressources publiées sur Brand Portal depuis AEM 6.3.2.1 et AEM 6.4 peuvent maintenant être disponibles publiquement pour des utilisateurs standard de Brand Portal., Pour cela, il suffit de en cochant cocher la case Publication de dossier public dans la boîte de dialogue de réplication d’AEM Assets Brand Portal.

![](assets/public-folder-publish.png)

* Lorsqu’'une personne demande a demandé la permission d'accéder l’accès à Brand Portal, les administrateurs en sont informés par des e-mails de demande d’accès, en plus des notifications de la zone de notification de Brand Portal.

## Changements dans la version 6.3.2 {#what-changed-in-3}

Brand Portal 6.3.2 comprend des fonctionnalités nouvelles et améliorées qui répondent aux principales demandes des clients, ainsi que des améliorations de performances générales.

### Demande d’accès à Brand Portal   {#request-access-to-brand-portal}

Les utilisateurs peuvent désormaismaintenant demander l’accès à Brand Portal à l’aide de la nouvelle option Besoin d’un accès disponible sur l’écran de connexion de Brand Portal.

![](assets/bplogin_request_access.png)

Selon qu'ils disposent ou non d’un Adobe ID, les utilisateurs peuvent suivre la procédure adéquate pour envoyer une demande. Les administrateurs de produit Brand Portal reçoivent ces demandes dans la zone de notification et accordent l’accès via Adobe Admin Console.

Pour plus d’informations, voir [Demande d’accès à Brand Portal](../using/brand-portal.md#requestaccesstobrandportal).

### Amélioration apportée au rapport sur les ressources téléchargées   {#enhancement-in-the-assets-downloaded-report}

Le rapport sur les ressources téléchargées comporte désormais le nombre de téléchargements de ressources par utilisateur pendant la période (date et heure) spécifiée. Les utilisateurs peuvent télécharger ce rapport au format .csv et compiler des données telles que le nombre total de téléchargements pour une ressource sous licence.

![](assets/reports_download_downloaded_by.png)

Pour plus d’informations, reportez-vous aux étapes 3 et 6 dans [Création et gestion de rapports supplémentaires](../using/brand-portal-reports.md#createandmanageadditionalreports).

### Notification de maintenance de Brand Portal   {#brand-portal-maintenance-notification}

Brand Portal affiche désormais une bannière de notification quelques jours avant une activité de maintenance. Exemple de notification :

![](assets/bp_maintenance_notification-1.png)

Pour plus d'’informations, voir [Notification de maintenance de Brand Portal](https://helpx.adobe.com/experience-manager/brand-portal/using/brand-portal.html#BrandPortalmaintenancenotification).

### Amélioration des ressources sous licence partagées à l’aide de la fonctionnalité de partage de liens {#enhancement-for-licensed-assets-shared-using-the-link-share-feature}

Lorsque vous téléchargez des ressources sous licence à l’aide de la fonctionnalité de partage de liens, vous êtes désormais invité à accepter le contrat de licence de ces ressources.

![](assets/copyright_management.png)

Pour plus d’informations, voir l’étape 12 dans [Partage de ressources en tant que lien](../using/brand-portal-link-share.md#shareassetsasalink).

### Amélioration du sélecteur d’utilisateur {#user-picker-enhancement}

Les performances du sélecteur d’utilisateur ont été améliorées pour prendre en compte les besoins des clients avec une base d’utilisateurs vastevolumineuse.

### Modifications du brandingde la valorisation de marque  Experience Cloud   {#experience-cloud-branding-changes}

Brand Portal se conforme désormais au nouveau branding à la nouvelle valorisation de marque Adobe Experience Cloud.

![](assets/bp_solution_switcher.png)

## Changements dans la version 6.3.1   {#what-changed-in-4}

Brand Portal 6.3.1 comprend de nouvelles fonctionnalités améliorées orientées vers l’alignement de Brand Portal sur AEM.

### Mise à niveau de l’interface utilisateur   {#upgraded-user-interface}

Pour aligner l’expérience utilisateur de Brand Portal sur AEM, Adobe passe à l’interface utilisateur Coral 3. Ce changement améliore l’utilisation générale, y compris la navigation et l’aspect.

#### Amélioration de l’expérience de navigation {#enhanced-navigational-experience}

* Accès rapide aux outils d’administration par le biais du nouveau logo Adobe :

![](assets/aemlogo-3.png)

* Navigation dans le produit via un recouvrement :

![](assets/overlay_navigation.png)

* Accès rapide aux dossiers parents :

![](assets/navigationparentfolders.png)

* Recherche et accès rapides au contenu et aux outils requis :

![](assets/omnisearchicon.png)

### Amélioration de la navigation   {#enhanced-browsing-experience}

* Nouveau mode Colonnes pour parcourir les dossiers imbriqués :

![](assets/millercolumnnavigation.png) ![](assets/multi-columnview.png)

* Dans la liste des ressources contenues dans un dossier, les dernières ressources téléchargées apparaissent en début de liste.

### Amélioration de la recherche   {#enhanced-search-experience}

* La nouvelle fonctionnalité de recherche Omni permet d’accélérer l'accès au contenu, aux fonctionnalités ou aux balises pertinents par le biais de suggestions automatiques qui s’affichent lorsque vous saisissez des mots-clés de recherche. La fonctionnalité de recherche Omni est disponible dans toutes les fonctions de recherche.

![](assets/omnisearch_whatsnew.png)

* Vous pouvez également ajouter des filtres à la recherche Omni pour affiner davantage et accélérer votre recherche et l’accélérer.

![](assets/omnisearch_withfilters.png)

* La nouvelle recherche basée sur l’évaluation des ressources permet de rechercher des ressources avec des évaluations, si elles ont été publiées depuis AEM Assets.
* La nouvelle fonctionnalité de recherche à valeurs multiples accepte plusieurs mots-clés avec l’opérateur ET pour trouver des ressources plus rapidement.
* La nouvelle fonctionnalité d’améliorationoptimisation des recherches permet d’améliorer la pertinence des recherches de sorte que des ressources spécifiques apparaissent en tête des résultats de la recherche.
* La nouvelle fonctionnalité de recherche basée sur le chemin d’accès permet de fournir le chemin d’accès à un dossier imbriqué afin de pouvoir rechercher les ressources contenues dans ce dossier.

#### Nouvelle recherche basée sur les balises intelligentes   {#new-smart-tags-based-search}

Si des images avec des balises intelligentes sont publiées depuis AEM Assets vers Brand Portal, vous pouvez rechercher ces images dans Brand Portal à l’aide des noms des balises intelligentes en tant que mots-clés. Cette fonctionnalité n’est disponible que pour les fichiers.

### Amélioration des téléchargements   {#enhanced-downloading-experience}

Après avoir téléchargé un dossier imbriqué, vous pouvez conserver la hiérarchie des dossiers d’origine. Les ressources situées dans un dossier imbriqué peuvent être téléchargées dans un seul dossier au lieu de plusieurs dossiers distincts.

### Amélioration des performances   {#improved-performance}

Des améliorations apportées aux fonctionnalités de navigation, de recherche et de téléchargement accroissent de manière significative les performances de Brand Portal.

### Nouvelle gestion des droits numériques pour les ressources {#new-digital-rights-management-for-assets}

Les administrateurs peuvent définir la date et l’heure d’expiration des ressources avant de les partager. Une fois qu’une ressource est arrivée à expiration, elle est visible par les observateurs et les éditeurs, mais ne peut pas être téléchargée. Lorsqu’une ressource arrive à expiration, les administrateurs reçoivent une notification.

### Amélioration du tri des ressources   {#enhanced-asset-sorting}

Le tri des ressources dans un dossier en mode Liste n’est plus limité au nombre de ressources affichées sur la première page. Toutes les ressources d’un dossier sont triées, qu’elles soient répertoriées ou non sur la première page.

### Amélioration du reportingde la création de rapports {#reporting-capabilities}

Les administrateurs peuvent créer et gérer trois types de rapports : ressources téléchargées, ressources arrivées à expiration et ressources publiées. Il est également possible de configurer les colonnes d’un rapport et d’exporter des rapports au format CSV.

![](assets/newreport.png)

### Métadonnées supplémentaires   {#additional-metadata}

Brand Portal 6.3.1 introduitcomporte des métadonnées supplémentaires qui font partie d’AEM Assets 6.3. Vous pouvez utiliser le formulaire Éditeur de schéma pour contrôler les métadonnées qui doivent être visibles sur la page Propriétés des ressources. Les métadonnées des ressources ne sont pas visibles par les utilisateurs de partage de lien externes. Ceux-ci ne peuvent que prévisualiser et télécharger des ressources à l’aide de l’URL du partage de lien.

![](assets/additionsinmetadata.png)

### Fonctionnalités supplémentaires pour les administrateurs {#additional-capabilities-for-administrators}

* Avant de finaliser les personnalisations du papier peint de l’écran de connexion, les administrateurs peuvent prévisualiser les modifications.

![](assets/wallpaperpreview.png)

* Lorsqu’un administrateur ajoute de nouveaux utilisateurs, ils n’ont pas besoin d’accepter d’invitations pour être ajoutés au compte Brand Portal ; ils le sont automatiquement.

### Nouvelles fonctionnalités de publication d’AEM Assets 6.3   {#new-publishing-capabilities-in-aem-assets}

* Les administrateurs d’AEM peuvent publier un schéma de métadonnées depuis AEM Assets sur Brand Portal à l’aide d’AEM 6.3 SP 1-CFP 1 (6.3.1.1) disponible depuis le quatrième trimestre de 2017.

![](assets/publish_metadataschemaaemassets.png)

* Les administrateurs AEM peuvent publier toutes les balises depuis AEM Assets sur Brand Portal à l’aide d’AEM 6.2 SP1-CFP7 et AEM 6.3 SP 1-CFP 1 (6.3.1.1).

![](assets/publish_tags_aemassets.png)

* Dans AEM Assets, vous pouvez publier des ressources et des collections qui comportent des balises, notamment des balises intelligentes. Vous pouvez ensuite rechercher ces ressources ou collections en utilisant ces balises en tant que mots-clés dans Brand Portal.

## FoireForum aux questions {#frequently-asked-questions}

**Ques. Est-ce que je n’aurai plus accès aux ressources et fonctionnalités existantes ou aux configurations que j’ai créées ?****Rép.** Toutes les fonctionnalités et configurations existantes ne sont pas modifiées. Les utilisateurs finaux ne sont pas affectés. De plus, le contenu reste intact.

**Ques. Quand vais-je passer à la nouvelle version de Brand Portal ?**
**Rép.** Brand Portal 6.4.4 est sortia été publié en production en février 2019. La sortie de la nouvelle version de Brand Portal est attendue au troisième trimestre 2019.

>[!NOTE]
>
>Le calendrier des nouvelles versions est provisoire et susceptible d’être modifié. Contactez votre gestionnaire de compte ou le service clientèle Adobe pour obtenir le calendrier de version mis à jour.

**Ques. Cela aura-t-il une incidence pour mes utilisateurs ?**
**Rép.** Ce changement concerne exclusivement Brand Portal. Il n’y a donc aucune incidence pour les utilisateurs finaux.

**Ques. Suis-je tenu d’'effectuer une action particulière ?**
**Rép.** Aucune action ne doit être effectuée par l’administrateur. Une fois que vous avez accès au nouveau portail Brand Portal, consultez la documentation pour découvrir toutes les fonctionnalités.

**Ques. Qui dois-je contacter en cas de questions ?**
**Rép.** Contactez votre gestionnaire de compte ou le service à la clientèle Adobe.
