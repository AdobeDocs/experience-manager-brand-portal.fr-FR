---
title: Publication de balises sur Brand Portal
description: Découvrez comment publier des balises à partir d’Experience Manager Assets sur Brand Portal.
topic-tags: publish
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
exl-id: 842656a6-1a2b-4b64-954d-1e663923a1a1
source-git-commit: 32a67abf466dd3bf635b851b02377ed23591915e
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 38%

---

# Publication de balises sur Brand Portal {#publish-tags-to-brand-portal}

Découvrez comment publier des balises à partir d’Experience Manager Assets sur Brand Portal.

Les balises s’avèrent utiles pour organiser les ressources et améliorer la recherche des ressources auxquelles elles sont associées. Les balises peuvent être considérées comme des mots-clés ou des étiquettes (métadonnées) qui sont jointes aux ressources et permettent de retrouver rapidement les ressources suite à une recherche. Pour savoir comment affecter des balises à des ressources dans Experience Manager Assets, reportez-vous à [Utilisation des balises pour organiser les ressources](https://experienceleague.adobe.com/fr/docs/experience-manager-65/content/assets/managing/organize-assets).

Les balises (liées aux ressources et aux collections dans AEM) sont automatiquement publiées sur Brand Portal quand les ressources (et les collections) associées à des balises sont publiées sur Brand Portal. Les balises publiées sont utiles pour retrouver les ressources associées.

>[!NOTE]
>
>Adobe recommande de publier exclusivement des balises sur Brand Portal avant de publier les ressources (et les collections) auxquelles elles sont associées. Cette approche permet de publier plus rapidement les ressources (et les collections) dans Brand Portal.

## Gérer les balises {#manage-tags}

Vous pouvez utiliser les balises préexistantes à joindre à une ressource ou créer de nouvelles balises à partir de la console Balises AEM (**[!UICONTROL Outils | Balisage | AEM Balises]**). Dans les deux scénarios, vous devez d’abord publier les balises sur Brand Portal, puis les associer aux ressources appropriées.

Pour créer des balises sur AEM, les publier sur Brand Portal et les associer aux ressources (ou aux collections) appropriées, procédez comme suit :

1. **Créer des balises**
Connectez-vous à une instance d’auteur AEM avec les droits d’administrateur et accédez à la console **[!UICONTROL AEM Balises]** à partir de la navigation globale :

   1. Sélectionnez **[!UICONTROL Outils]**.

   1. Sélectionnez **[!UICONTROL Général]**.

   1. Sélectionnez **[!UICONTROL Balisage]**.

1. Sélectionnez **[!UICONTROL Créer]** , puis l’option **[!UICONTROL Créer une balise]** .
1. Précisez les paramètres suivants :

   * **[!UICONTROL Titre]**

     *(obligatoire)* Titre affiché pour la balise.
   * **[!UICONTROL Nom]**

     *(obligatoire)* Nom de la balise. Si aucun nom n’est spécifié, un nom de nœud valide est créé à partir du titre. Voir [ID de balise](https://experienceleague.adobe.com/fr/docs/experience-manager-65/content/implementing/developing/platform/tagging/framework).
   * **Description**

     *(facultative)* Description de la balise.
   * **Chemin d’accès aux balises** 
Chemin JCR de la balise.

1. Sélectionner **[!UICONTROL Envoyer]** pour créer la balise.

   Une fois que vous avez créé une balise sur une instance AEM, elle peut être jointe à une ressource (à l’aide de la section Propriétés ou Gestion des balises de cette ressource).

1. **Publiez la balise sur Brand Portal**.

   Accédez à la console **[!UICONTROL AEM Balises]** ([!UICONTROL Outils | Balisage | AEM Balises]), sélectionnez la balise souhaitée et Publish vers Brand Portal.

1. **Joignez la balise à une ressource (ou collection)**.

   Sélectionnez une ressource (ou collection) et joignez la balise de votre choix à l’aide de la section Propriétés ou Gérer les balises de cette ressource. Pour plus d’informations sur l’affectation de balises à des ressources dans AEM Assets, accédez à [Utilisation de balises pour organiser les ressources](https://experienceleague.adobe.com/fr/docs/experience-manager-65/content/assets/managing/organize-assets).

1. **Publiez les ressources (ou les collections) sur Brand Portal**.\
   Quand vous publiez une ressource (ou collection) sur Brand Portal, la balise jointe est également disponible sur Brand Portal.

   Pour afficher la balise jointe sur la ressource (ou collection) respective dans Brand Portal, connectez-vous à Brand Portal, puis sélectionnez la ressource. Sous la section Propriétés , vous pouvez voir la balise jointe.

## Rechercher une promotion {#search-promote}

AEM Assets Brand Portal vous permet de faire apparaître des ressources spécifiques en tant que premiers résultats des recherches basées sur une balise de mot-clé.

Pour promouvoir une ressource pour un mot-clé de recherche, suivez ces étapes :

1. Ouvrez la page **[!UICONTROL Propriétés]** d’une ressource sur l’instance d’auteur AEM.
1. Accédez à l’onglet **[!UICONTROL Avancé]** .
1. Dans la section **[!UICONTROL Rechercher une promotion]** de **[!UICONTROL Élever pour les mots-clés de recherche]**, sélectionnez **[!UICONTROL Ajouter]** pour ajouter les mots-clés ou les balises de recherche.

   ![](assets/search-promote.png)

1. Enregistrez les modifications.
1. Publish la ressource sur Brand Portal.
1. Connectez-vous à Brand Portal. Affichez l’onglet **[!UICONTROL Avancé]** dans la section **[!UICONTROL Propriétés]** de la ressource.
Notez que le mot-clé **[!UICONTROL Rechercher une promotion]** est également visible dans les propriétés de cette ressource.
