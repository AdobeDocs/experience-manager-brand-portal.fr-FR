---
title: Publication de balises sur Brand Portal
seo-title: Publication de balises sur Brand Portal
description: Découvrez comment publier des balises à partir d’AEM Assets sur Brand Portal.
seo-description: Découvrez comment publier des balises à partir d’AEM Assets sur Brand Portal.
uuid: 4167367e-1af8-476b-97a5-730c43bd0816
topic-tags: publish
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
discoiquuid: 3c8e9251-195d-4c56-a9a9-27bc8b2a82a4
translation-type: tm+mt
source-git-commit: 86d4d5c358ea795e35db2dce8c9529ed14e9ee2d
workflow-type: tm+mt
source-wordcount: '623'
ht-degree: 93%

---


# Publication de balises sur Brand Portal {#publish-tags-to-brand-portal}

Découvrez comment publier des balises à partir d’AEM Assets sur Brand Portal.

Les balises sont utiles pour organiser les ressources et faciliter la recherche des ressources auxquelles elles sont associées. Les balises peuvent être considérées comme des mots-clés ou des étiquettes (métadonnées) qui sont attachés aux ressources, et permettent de les trouver rapidement suite à une recherche. Pour savoir comment affecter des balises aux ressources dans AEM Assets, voir [Utilisation de balises pour organiser des ressources](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets).

Les balises (liées aux ressources et aux collections dans AEM) sont automatiquement publiées sur Brand Portal quand les ressources (et les collections) associées à des balises sont publiées sur Brand Portal. Les balises publiées sont utiles pour retrouver les ressources associées.

>[!NOTE]
>
>Toutefois, il est recommandé de publier les balises exclusivement sur Brand Portal avant de publier les ressources (et les collections) auxquelles elles sont associées. Cela assure une publication plus rapide des ressources (et des collections) sur Brand Portal.

## Gestion des balises {#manage-tags}

Vous pouvez associer les balises préexistantes à une ressource ou créer des balises à partir de la console Balises AEM (**[!UICONTROL Outils | Balisage | Balises AEM]**). Dans les deux scénarios, vous devez d’abord publier les balises sur Brand Portal et les associer ensuite aux ressources appropriées.

Pour créer des balises sur AEM, les publier sur Brand Portal et les associer aux ressources (ou aux collections) appropriées, suivez ces étapes :

1. **Création des balises**
Connectez-vous à l’instance AEM Author avec les privilèges d’administrateur et accédez ensuite à la console **[!UICONTROL Balises AEM]** à partir de la navigation globale :

   1. Sélectionnez **[!UICONTROL Outils]**.

   1. Sélectionnez **[!UICONTROL Général]**.

   1. Sélectionnez **[!UICONTROL Balisage]**.

1. Sélectionner **[!UICONTROL Créer]** et ensuite l’option **[!UICONTROL Créer une balise]**.
1. Précisez les paramètres suivants :

   * **[!UICONTROL Titre]**

      *(obligatoire)* Titre affiché pour la balise.
   * **[!UICONTROL Nom]**
      *(obligatoire)* Nom de la balise. Si aucun nom n’est spécifié, un nom de nœud valide est créé à partir du titre. See [TagID](https://helpx.adobe.com/experience-manager/6-5/sites/developing/using/framework.html#TagID).
   * **Description**

      *(facultative)* Description de la balise.
   * **Chemin d’accès aux balises** 
Chemin JCR de la balise.

1. Sélectionner **[!UICONTROL Envoyer]** pour créer la balise.

   Une fois que vous avez créé une balise sur l’instance AEM, celle-ci peut être associée à une ressource (en utilisant la section Propriétés ou Gestion des balises de cette ressource).

1. **Publiez la balise sur Brand Portal**.

   Accédez à la console **[!UICONTROL Balises AEM]** ([!UICONTROL Outils | Balisage | Balises AEM]), puis sélectionnez la balise de votre choix et Publier sur Brand Portal.

1. **JoindreAssocier la balise à une ressource (ou collection)**.

   Sélectionnez une ressource (ou collection) et joignezassociez la balise désirée en utilisant la section Propriétés ou Gérer les balises de cette ressource. To know more about how to assign tags to assets in AEM Assets, refer [use tags to organize assets](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets).

1. **Publiez les ressources (ou les collections) sur Brand Portal**.\
   Quand vous publiez une ressource (ou collection) sur Brand Portal, la balise jointe est également disponible sur Brand Portal.

   Pour voir la balise jointe sur la ressource (ou collection) respective dans Brand Portal, connectez-vous à Brand Portal et sélectionnez la ressource. Vous verrez la balise jointe sous la section Propriétés.

## Rechercher une promotion {#search-promote}

AEM Assets Brand Portal vous permet de faire apparaître des ressources spécifiques dans les premiers résultats des recherches basées sur une balise de mot-clé.

Pour promouvoir une ressource pour un mot-clé de recherche, suivez ces étapes :

1. Ouvrez la page **[!UICONTROL Propriétés]** d’une ressource sur l’instance AEM Author.
1. Accédez à l’onglet **[!UICONTROL Avancé]**.
1. Dans **[!UICONTROL Rechercher une promotion]** au sein de la section **[!UICONTROL Élever pour les mots-clés de recherche]**, sélectionnez **[!UICONTROL Ajouter]** afin d’ajouter les mots-clés ou les balises de recherche.

   ![](assets/search-promote.png)

1. Enregistrez les modifications.
1. Publiez la ressource sur Brand Portal.
1. Connectez-vous à Brand Portal. Consultez l’onglet **[!UICONTROL Avancé]** dans la section **[!UICONTROL Propriétés]** de la ressource.
Notez que le mot-clé **[!UICONTROL Rechercher une promotion]** est également visible dans les propriétés de cette ressource.
