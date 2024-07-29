---
title: Publication de paramètres prédéfinis, de schémas et de facettes sur Brand Portal
seo-title: Publish presets, schema, and facets to Brand Portal
description: Découvrez comment publier des paramètres prédéfinis, des schémas et des facettes sur Brand Portal.
seo-description: Learn how to publish presets, schema, and facets to Brand Portal.
uuid: c836d9bb-074a-4113-9c91-b2bf7658b88d
topic-tags: publish
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
discoiquuid: bc305abc-9373-4d33-9179-0a5f3904b352
exl-id: 9b585606-6538-459b-87a9-2e68df0087b3
source-git-commit: 133ea1fc342e4460e7d0661205c7411a509143eb
workflow-type: tm+mt
source-wordcount: '1133'
ht-degree: 87%

---

# Publication de paramètres prédéfinis, de schémas et de facettes sur Brand Portal {#publish-presets-schema-and-facets-to-brand-portal}

L’article est consacré à la publication des paramètres d’image prédéfinis, des schémas de métadonnées et des facettes de recherche personnalisées sur Brand Portal à partir de l’instance AEM Author. La fonction de publication permet aux entreprises de réutiliser les paramètres d’image prédéfinis, les schémas de métadonnées et les facettes de recherche créées/modifiées sur l’instance AEM Author, ce qui réduit le travail en double.

>[!NOTE]
>
>La fonction de publication des paramètres d’image prédéfinis, des schémas de métadonnées et des facettes de recherche sur Brand Portal à partir de l’instance AEM Author est disponible à partir d’AEM 6.2 SP1-CFP7 et d’AEM 6.3 SP1-CFP1 (6.3.1.1).

## Publication des paramètres d’image prédéfinis sur Brand Portal {#publish-image-presets-to-brand-portal}

Les paramètres d’image prédéfinis sont un ensemble de commandes de redimensionnement et de formatage qui sont appliqués à l’image au moment de sa livraison. Les paramètres d’image prédéfinis peuvent être créés et modifiés dans Brand Portal. Autrement, si l’instance AEM Author s’exécute en mode Dynamic Media, les utilisateurs peuvent aussi créer des paramètres prédéfinis sur cette instance et les publier sur AEM Assets Brand Portal afin d’éviter de recréer les mêmes paramètres prédéfinis sur Brand Portal.\
Une fois que le paramètre prédéfini est créé, il est répertorié en tant que rendu dynamique sur le rail de rendus des détails de ressources et la boîte de dialogue de téléchargement.

>[!NOTE]
>
>Si l’instance AEM Author n’est pas exécutée en mode **[!UICONTROL Dynamic Media]** (le client n’a pas acheté Dynamic Media), le rendu **[!UICONTROL Pyramid TIFF]** des ressources ne sera pas créé au moment du chargement. Les paramètres d’image prédéfinis ou les rendus dynamiques fonctionnent avec le format **[!UICONTROL Pyramid TIFF]** d’une ressource. Ainsi, si le rendu **[!UICONTROL Pyramid TIFF]** n’est pas disponible sur l’instance AEM Author, il ne l’est pas non plus sur Brand Portal. En conséquence, aucun rendu dynamique n’est présent dans le rail de rendus de la page des détails de la ressource et dans la boîte de dialogue de téléchargement.

Pour publier des paramètres d’image prédéfinis sur Brand Portal :

1. Dans l’instance d’auteur AEM, appuyez/cliquez sur le logo pour accéder à la console de navigation globale, puis appuyez/cliquez sur l’icône Outils et accédez à **[!UICONTROL Ressources > Paramètres d’image prédéfinis]**.
1. Sélectionnez un ou plusieurs paramètres d’image prédéfinis dans la liste, puis cliquez/appuyez sur **[!UICONTROL Publier sur Brand Portal]**.

![](assets/publishpreset.png)

>[!NOTE]
>
>Quand les utilisateurs cliquent sur **[!UICONTROL Publier sur Brand Portal]**, les paramètres d’image prédéfinis sont placés en file d’attente pour publication. Nous conseillons aux utilisateurs de surveiller le journal des agents de réplication pour contrôler la réussite de la publication.

Pour dépublier un paramètre d’image prédéfini sur Brand Portal :

1. Dans l’instance d’auteur AEM, appuyez/cliquez sur le logo AEM pour accéder à la console de navigation globale, cliquez sur l’icône **[!UICONTROL Outils]** et accédez à **[!UICONTROL Assets > Paramètres d’image prédéfinis]**.
1. Sélectionnez un paramètre d’image prédéfini puis **[!UICONTROL Supprimer de Brand Portal]** parmi les options disponibles dans la partie supérieure.

## Publication d’un schéma de métadonnées sur Brand Portal   {#publish-metadata-schema-to-brand-portal}

Le schéma de métadonnées décrit la mise en page et les propriétés affichées sur la page de propriétés d’une ressource ou de collections.

![](assets/metadata-schema-editor.png) ![](assets/asset-properties-1.png)

Si les utilisateurs ont modifié le schéma par défaut sur l’instance AEM Author et souhaitent utiliser le même schéma comme schéma par défaut sur Brand Portal, ils peuvent simplement publier les formulaires de schéma de métadonnées sur Brand Portal. Dans un tel scénario, le schéma par défaut sur Brand Portal est remplacé par les schémas par défaut publiés à partir de l’instance AEM Author.

Si les utilisateurs ont créé un schéma personnalisé sur l’instance AEM Author, ils peuvent le publier sur Brand Portal au lieu de l’y recréer. Les utilisateurs peuvent alors appliquer ce schéma personnalisé à n’importe quel dossier/collection dans Brand Portal.

>[!NOTE]
>
>Les schémas par défaut ne peuvent pas être publiés sur Brand Portal s’ils sont verrouillés sur l’instance AEM (c’est-à-dire qu’ils n’ont pas été modifiés).

![](assets/default-schema-form.png)

>[!NOTE]
>
>Si un schéma de dossier a été appliqué sur l’instance AEM Author, le même schéma doit également exister sur Brand Portal pour maintenir la cohérence dans la page des propriétés de ressource sur AEM Author et Brand Portal.

Pour publier un schéma de métadonnées sur Brand Portal à partir d’une instance d’auteur AEM :

1. Dans l’instance d’auteur AEM, appuyez/cliquez sur le logo AEM pour accéder à la console de navigation globale, cliquez sur l’icône Outils et accédez à **[!UICONTROL Assets > Schémas de métadonnées]**.
1. Sélectionnez un schéma de métadonnées puis **[!UICONTROL Publier sur Brand Portal]** parmi les options disponibles dans la partie supérieure.

>[!NOTE]
>
>Quand les utilisateurs cliquent sur **[!UICONTROL Publier sur Brand Portal]**, les schémas de métadonnées sont placés en file d’attente pour publication. Nous conseillons aux utilisateurs de surveiller le journal des agents de réplication pour contrôler la réussite de la publication.

Pour annuler la publication d’un schéma de métadonnées sur Brand Portal :

1. Dans l’instance d’auteur AEM, appuyez/cliquez sur le logo AEM pour accéder à la console de navigation globale, cliquez sur l’icône Outils et accédez à **[!UICONTROL Assets > Schémas de métadonnées]**.
1. Sélectionnez un schéma de métadonnées puis **[!UICONTROL Supprimer de Brand Portal]** parmi les options disponibles dans la partie supérieure.

## Publication de facettes de recherche sur Brand Portal {#publish-search-facets-to-brand-portal}

Les formulaires de recherche fournissent aux utilisateurs la fonctionnalité de [recherche facettée](../using/brand-portal-search-facets.md) sur Brand Portal. Les facettes de recherche permettent d’effectuer des recherches plus précises sur Brand Portal. Tous les [prédicats ajoutés](https://experienceleague.adobe.com/docs/experience-manager-65/assets/administer/search-facets.html?lang=fr) dans le formulaire de recherche sont disponibles pour les utilisateurs en tant que facettes de recherche dans les filtres de recherche.

![](assets/property-predicate-removed.png)
![](assets/search-form.png)

Si vous souhaitez utiliser le formulaire de recherche personnalisé **[!UICONTROL Rail de recherche d’administration de ressources]** à partir de l’instance d’auteur AEM, au lieu de recréer le même formulaire sur Brand Portal, vous pouvez publier le formulaire de recherche personnalisé sur Brand Portal à partir de l’instance d’auteur AEM.

>[!NOTE]
>
>Le formulaire de recherche verrouillé **[!UICONTROL Rail de recherche d’administration de ressources]** sur AEM Assets ne peut pas être publié sur Brand Portal sans être modifié. Une fois modifié et publié sur Brand Portal, ce formulaire de recherche remplace celui qui se trouve sur Brand Portal.

Pour publier la facette de recherche modifiée sur Brand Portal à partir de l’interface AEM Author :

1. Cliquez sur le logo AEM, puis accédez à **[!UICONTROL Outils > Général > Search Forms]**.
1. Sélectionnez le formulaire de recherche modifié et ensuite **[!UICONTROL Publier sur Brand Portal]**.

   >[!NOTE]
   >
   >Quand les utilisateurs cliquent sur **[!UICONTROL Publier sur Brand Portal]**, les facettes de recherche sont placées en file d’attente pour publication. Nous conseillons aux utilisateurs de surveiller le journal des agents de réplication pour contrôler la réussite de la publication.

Pour annuler la publication de formulaires de recherche sur Brand Portal :

1. Dans l’instance d’auteur AEM, appuyez/cliquez sur le logo AEM pour accéder à la console de navigation globale, cliquez sur l’icône Outils et accédez à **[!UICONTROL Général > Rechercher dans Forms]**.
1. Sélectionnez le formulaire de recherche et ensuite **[!UICONTROL Supprimer de Brand Portal]** parmi les options disponibles dans la partie supérieure.

>[!NOTE]
>
>L’action **[!UICONTROL Dépublier sur Brand Portal]** laisse le formulaire de recherche par défaut sur Brand Portal et ne rétablit pas le dernier formulaire de recherche utilisé avant la publication.

### Restrictions {#limitations}

1. Peu de prédicats de recherche ne s’appliquent pas aux filtres de recherche sur Brand Portal. Quand ces prédicats de recherche sont publiés en tant qu’élément du formulaire de recherche sur Brand Portal à partir de l’instance AEM Author, ils sont filtrés. En conséquence, les utilisateurs voient moins de prédicats dans le formulaire publié sur Brand Portal. Voir [Prédicats de recherche applicables aux filtres sur Brand Portal](../using/brand-portal-search-facets.md#list-of-search-predicates).

1. Pour [!UICONTROL Options du prédicat], si un utilisateur utilise n’importe quel chemin personnalisé pour lire les options sur l’instance AEM Author, cela ne fonctionnera pas sur Brand Portal. Ces chemins et options supplémentaires ne sont pas publiés sur Brand Portal avec le formulaire de recherche. Dans ce cas, les utilisateurs peuvent sélectionner l’option **[!UICONTROL Manuel]** sous **[!UICONTROL Ajouter des options]** dans **[!UICONTROL Options du prédicat]** pour ajouter ces options manuellement sur Brand Portal.

![](assets/options-predicate-manual.png)
