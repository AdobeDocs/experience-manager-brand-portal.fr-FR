---
title: Publication de balises sur Brand Portal
seo-title: Publication de balises sur Brand Portal
description: Découvrez comment publier des balises à partir d’AEM Assets sur Brand Portal.
seo-description: Découvrez comment publier des balises à partir d’AEM Assets sur Brand Portal.
uuid: 4167367 e -1 af 8-476 b -97 a 5-730 c 43 bd 0816
topic-tags: 'serveur '
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
content-type: référence
discoiquuid: 3 c 8 e 9251-195 d -4 c 56-a 9 a 9-27 bc 8 b 2 a 82 a 4
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Publication de balises sur Brand Portal {#publish-tags-to-brand-portal}

Découvrez comment publier des balises à partir d’AEM Assets sur Brand Portal.

Les balises sont utiles pour organiser les ressources et faciliter la recherche des ressources auxquelles elles sont associées. Les balises peuvent être considérées comme des mots-clés ou des étiquettes (métadonnées) qui sont attachés aux ressources, et permettent de les trouver rapidement suite à une recherche. Pour savoir comment affecter des balises aux ressources dans AEM Assets, voir [Utilisation de balises pour organiser des ressources](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets).

Les balises (liées aux ressources et aux collections dans AEM) sont publiées automatiquement sur Brand Portal quand les ressources (et les collections) avec les balises associées sont publiées. sur Brand Portal. Les balises publiées sont utiles pour rechercher et trouver les ressources associées.

>[!NOTE]
>
>Toutefois, il est recommandé de publier les balises exclusivement sur Brand Portal avant de publier les ressources (et les collections) auxquelles elles sont associées. Cela assure une publication plus rapide des ressources (et des collections) sur Brand Portal.

## Manage tags {#manage-tags}

Vous pouvez joindre les balises préexistantes à une ressource ou créer des balises à partir de la console Balises AEM (**[!UICONTROL Outils | Balisage | Balises AEM]**). Dans les deux scénarios, vous devez d’abord publier les balises sur Brand Portal et les associer ensuite aux ressources appropriées.

Pour créer des balises sur AEM, les publier sur Brand Portal et les associer aux ressources (ou aux collections) appropriées, suivez ces étapes :

1. **Création des balises**
Sign in to AEM Author instance with administrative privileges, and access **[!UICONTROL AEM Tags]** console from global navigation:

   1. Select **[!UICONTROL Tools]**

   2. Select **[!UICONTROL General]**

   3. Select **[!UICONTROL Tagging]**

2. Select **[!UICONTROL Create]** and then select **[!UICONTROL Create Tag]** option.
3. Spécifiez les paramètres suivants :

   * **[!UICONTROL Titre]**
      *(obligatoire)* Titre d'affichage de la balise.
   * **[!UICONTROL Nom]**
      *(Obligatoire)* Nom de la balise. Si aucun nom n’est spécifié, un nom de nœud valide est créé à partir du titre. See [TagID](https://helpx.adobe.com/experience-manager/6-5/sites/developing/using/framework.html#TagID).
   * **Description**
      *(Facultatif)* Description de la balise.
   * **Chemin d’accès aux balises** Chemin JCR de la balise.

4. Sélectionnez **[!UICONTROL Envoyer]pour créer la balise.**

   Une fois que vous avez créé une balise sur l'instance AEM, la balise sera disponible pour être jointe à un fichier (à l'aide de la section Propriétés ou de la section Gérer les balises de ce fichier).

5. **Publiez la balise sur Brand Portal**.

   Go to **[!UICONTROL AEM Tags]** console ([!UICONTROL Tools | Tagging | AEM Tags]), select the desired tag and Publish to Brand Portal.

6. **Joignez la balise à une ressource (ou collection)**.

   Sélectionnez une ressource (ou collection) et joignez la balise désirée en utilisant la section Propriétés ou Gérer les balises de cette ressource. To know more about how to assign tags to assets in AEM Assets, refer [use tags to organize assets](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets).

7. **Publiez les ressources (ou les collections) sur Brand Portal**.\
   Quand vous publiez une ressource (ou collection) sur Brand Portal, la balise jointe est également disponible sur Brand Portal.

   Pour voir la balise jointe sur la ressource (ou collection) respective dans Brand Portal, connectez-vous à Brand Portal et sélectionnez la ressource. Vous verrez la balise jointe sous la section Propriétés.

## Rechercher une promotion {#search-promote}

AEM Assets Brand Portal vous permet de faire apparaître des ressources spécifiques dans les premiers résultats des recherches basées sur une balise de mot-clé.

Pour promouvoir une ressource pour un mot-clé de recherche, suivez ces étapes :

1. Ouvrez la page **[!UICONTROL Propriétés]d’une ressource sur l’instance d’auteur AEM.**
2. Accédez à l’onglet **[!UICONTROL Avancé].**
3. In **[!UICONTROL Search Promote]** within **[!UICONTROL Elevate for search keywords]** section, select **[!UICONTROL Add]** to add the search keywords or tags.

   ![](assets/search-promote.png)

4. Enregistrez les modifications.
5. Publiez la ressource sur Brand Portal.
6. Connectez-vous à Brand Portal. Consultez l’onglet **[!UICONTROL Avancé]** dans la section **Propriétés]de la ressource.[!UICONTROL **
Note that the **[!UICONTROL Search Promote]** keyword is also visible in the Properties of that asset.
