---
title: Publication de paramètres prédéfinis, de schémas et de facettes sur Brand Portal
description: Découvrez comment publier des paramètres prédéfinis, des schémas et des facettes sur Brand Portal.
topic-tags: publish
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
exl-id: 9b585606-6538-459b-87a9-2e68df0087b3
source-git-commit: 4d9d7afa2cd45ea68c2e15338c92aa29ecf09f91
workflow-type: tm+mt
source-wordcount: '1116'
ht-degree: 43%

---

# Publication de paramètres prédéfinis, de schémas et de facettes sur Brand Portal {#publish-presets-schema-and-facets-to-brand-portal}

L’article est consacré à la publication des paramètres d’image prédéfinis, des schémas de métadonnées et des facettes de recherche personnalisées sur Brand Portal à partir de l’instance AEM Author. La fonction de publication permet aux entreprises de réutiliser les paramètres d’image prédéfinis, les schémas de métadonnées et les facettes de recherche créées ou modifiées sur une instance d’auteur AEM. Cette approche permet de réduire les efforts en double.

>[!NOTE]
>
>La possibilité de publier des paramètres d’image prédéfinis, des schémas de métadonnées et des facettes de recherche de l’instance d’auteur AEM vers Brand Portal est disponible à partir d’AEM 6.2 SP1-CFP7 et d’Adobe 6.3 SP 1-CFP 1 (6.3.1.1) et versions ultérieures.

## Publication des paramètres d’image prédéfinis sur Brand Portal {#publish-image-presets-to-brand-portal}

Les paramètres d’image prédéfinis sont un ensemble de commandes de redimensionnement et de formatage qui sont appliqués à l’image au moment de sa livraison. Les paramètres d’image prédéfinis peuvent être créés et modifiés dans Brand Portal. Si une instance d’auteur AEM est en cours d’exécution en mode Dynamic Media, les utilisateurs peuvent également créer des paramètres prédéfinis dans AEM Author et les publier dans AEM Assets Brand Portal. Cette approche permet d’éviter de recréer les mêmes paramètres prédéfinis dans Brand Portal.
Une fois le paramètre prédéfini créé, il est répertorié en tant que rendu dynamique dans le rail de rendus des détails de la ressource et dans la boîte de dialogue de téléchargement.

>[!NOTE]
>
>Si l’instance d’auteur AEM n’est pas exécutée en **[!UICONTROL mode Dynamic Media]** (le client n’a pas acheté Dynamic Media), le rendu **[!UICONTROL TIFF Pyramid]** des ressources n’est pas créé au moment du chargement. Les paramètres d’image prédéfinis ou les rendus dynamiques fonctionnent sur le **[!UICONTROL TIFF Pyramid]** d’une ressource. Par conséquent, si **[!UICONTROL TIFF Pyramid]** n’est pas disponible sur l’instance d’auteur AEM, il n’est pas disponible sur Brand Portal. Par conséquent, aucun rendu dynamique n’est présent dans le rail de rendus de la page des détails de la ressource et de la boîte de dialogue de téléchargement.

Pour publier des paramètres d’image prédéfinis sur Brand Portal :

1. Dans l’instance d’auteur AEM, cliquez sur le logo AEM pour accéder à la console de navigation globale, cliquez sur l’icône Outils et accédez à **[!UICONTROL Assets > Paramètres d’image prédéfinis]**.
1. Sélectionnez un ou plusieurs paramètres d’image prédéfinis dans la liste, puis cliquez sur **[!UICONTROL Publish to Brand Portal]**.

![](assets/publishpreset.png)

>[!NOTE]
>
>Lorsque les utilisateurs cliquent sur **[!UICONTROL Publish to Brand Portal]**, les paramètres d’image prédéfinis sont placés en file d’attente pour publication. Nous conseillons aux utilisateurs de surveiller le journal des agents de réplication pour contrôler la réussite de la publication.

Pour dépublier un paramètre d’image prédéfini sur Brand Portal :

1. Dans l’instance d’auteur AEM, cliquez sur le logo AEM pour accéder à la console de navigation globale, cliquez sur l’icône **[!UICONTROL Outils]** et accédez à **[!UICONTROL Assets > Paramètres d’image prédéfinis]**.
1. Sélectionnez un paramètre d’image prédéfini puis **[!UICONTROL Supprimer de Brand Portal]** parmi les options disponibles dans la partie supérieure.

## Publication d’un schéma de métadonnées sur Brand Portal  {#publish-metadata-schema-to-brand-portal}

Le schéma de métadonnées décrit la mise en page et les propriétés affichées sur la page de propriétés d’une ressource ou de collections.

![](assets/metadata-schema-editor.png) ![](assets/asset-properties-1.png)

Si les utilisateurs ont modifié le schéma par défaut sur une instance d’auteur AEM et souhaitent utiliser le même schéma comme schéma par défaut sur Brand Portal, publiez les formulaires de schéma de métadonnées sur Brand Portal. Dans un tel scénario, les schémas par défaut publiés à partir de l’instance d’auteur AEM remplacent le schéma par défaut dans Brand Portal.

Si les utilisateurs ont créé un schéma personnalisé sur l’instance AEM Author, ils peuvent le publier sur Brand Portal au lieu de l’y recréer. Les utilisateurs peuvent alors appliquer ce schéma personnalisé à n’importe quel dossier/collection dans Brand Portal.

>[!NOTE]
>
>Les schémas par défaut ne peuvent pas être publiés dans Brand Portal s’ils étaient verrouillés sur l’instance AEM. En d’autres termes, ils ne sont pas édités.

![](assets/default-schema-form.png)

>[!NOTE]
>
>Si un schéma de dossier est appliqué sur l’instance d’auteur AEM, le même schéma doit également exister sur Brand Portal. Cela permet de maintenir la cohérence de la page des propriétés de la ressource sur AEM Auteur et Brand Portal.

Pour publier un schéma de métadonnées sur Brand Portal à partir d’une instance d’auteur AEM :

1. Dans l’instance d’auteur AEM, cliquez sur le logo AEM pour accéder à la console de navigation globale, cliquez sur l’icône Outils et accédez à **[!UICONTROL Assets > Schémas de métadonnées]**.
1. Sélectionnez un schéma de métadonnées puis **[!UICONTROL Publier sur Brand Portal]** parmi les options disponibles dans la partie supérieure.

>[!NOTE]
>
>Quand les utilisateurs cliquent sur **[!UICONTROL Publier sur Brand Portal]**, les schémas de métadonnées sont placés en file d’attente pour publication. Nous conseillons aux utilisateurs de surveiller le journal des agents de réplication pour contrôler la réussite de la publication.

Pour annuler la publication d’un schéma de métadonnées sur Brand Portal :

1. Dans l’instance d’auteur AEM, cliquez sur le logo AEM pour accéder à la console de navigation globale, cliquez sur l’icône Outils et accédez à **[!UICONTROL Assets > Schémas de métadonnées]**.
1. Sélectionnez un schéma de métadonnées puis **[!UICONTROL Supprimer de Brand Portal]** parmi les options disponibles dans la partie supérieure.

## Publication de facettes de recherche sur Brand Portal {#publish-search-facets-to-brand-portal}

Les formulaires de recherche fournissent aux utilisateurs la fonctionnalité de [recherche facettée](../using/brand-portal-search-facets.md) sur Brand Portal. Les facettes de recherche permettent d’effectuer des recherches plus précises sur Brand Portal. Tous les [prédicats ajoutés](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/administer/search-facets) dans le formulaire de recherche sont disponibles pour les utilisateurs en tant que facettes de recherche dans les filtres de recherche.

![](assets/property-predicate-removed.png)
![](assets/search-form.png)

Pour utiliser un formulaire de recherche personnalisé sur le **[!UICONTROL rail de recherche d’administration Assets]** à partir de l’instance d’auteur AEM, publiez-le directement sur Brand Portal au lieu de le recréer.

>[!NOTE]
>
>Pour publier un formulaire de recherche verrouillé sur le **[!UICONTROL rail de recherche d’administration Assets]** d’AEM Assets vers Brand Portal, vous devez d’abord le modifier. Une fois modifié et publié, ce formulaire de recherche remplace le formulaire de recherche existant sur Brand Portal.

Pour publier la facette de recherche modifiée sur Brand Portal à partir de l’interface AEM Author :

1. Cliquez sur le logo AEM, puis accédez à **[!UICONTROL Outils > Général > Search Forms]**.
1. Sélectionnez le formulaire de recherche modifié et ensuite **[!UICONTROL Publier sur Brand Portal]**.

   >[!NOTE]
   >
   >Quand les utilisateurs cliquent sur **[!UICONTROL Publier sur Brand Portal]**, les facettes de recherche sont placées en file d’attente pour publication. Nous conseillons aux utilisateurs de surveiller le journal des agents de réplication pour contrôler la réussite de la publication.

Pour annuler la publication de formulaires de recherche sur Brand Portal :

1. Dans l’instance d’auteur AEM, cliquez sur le logo AEM pour accéder à la console de navigation globale, cliquez sur l’icône Outils et accédez à **[!UICONTROL Général > Rechercher dans Forms]**.
1. Sélectionnez le formulaire de recherche et ensuite **[!UICONTROL Supprimer de Brand Portal]** parmi les options disponibles dans la partie supérieure.

>[!NOTE]
>
>L’action **[!UICONTROL Annuler la publication à partir de Brand Portal]** laisse le formulaire de recherche par défaut sur Brand Portal et ne rétablit pas le dernier formulaire de recherche utilisé avant la publication.

### Restrictions {#limitations}

1. Peu de prédicats de recherche ne s’appliquent pas aux filtres de recherche sur Brand Portal. Quand ces prédicats de recherche sont publiés en tant qu’élément du formulaire de recherche sur Brand Portal à partir de l’instance AEM Author, ils sont filtrés. En conséquence, les utilisateurs voient moins de prédicats dans le formulaire publié sur Brand Portal. Voir [Prédicats de recherche applicables aux filtres sur Brand Portal](../using/brand-portal-search-facets.md#list-of-search-predicates).

1. Pour [!UICONTROL Options Predicate], si un utilisateur utilise n’importe quel chemin personnalisé pour lire les options sur une instance d’auteur AEM, cela ne fonctionne pas sur Brand Portal. Ces chemins et options supplémentaires ne sont pas publiés sur Brand Portal avec le formulaire de recherche. Dans ce cas, les utilisateurs peuvent sélectionner l’option **[!UICONTROL Manuel]** sous **[!UICONTROL Ajouter des options]** dans **[!UICONTROL Options du prédicat]** pour ajouter ces options manuellement sur Brand Portal.

![](assets/options-predicate-manual.png)
