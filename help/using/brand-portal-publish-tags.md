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
source-git-commit: 32c3cdb8e3fafd74cfb36e6bcfe0811e7152b2d0

---


# Publication de balises sur Brand Portal {#publish-tags-to-brand-portal}

Learn how to publish tags from [!DNL AEM] Assets to [!DNL Brand Portal].

Les balises sont utiles pour organiser les ressources et faciliter la recherche des ressources auxquelles elles sont associées. Les balises peuvent être considérées comme des mots-clés ou des étiquettes (métadonnées) qui sont attachés aux ressources, et permettent de les trouver rapidement suite à une recherche. To know how to assign tags to assets in [!DNL AEM] Assets, refer [use tags to organize assets](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets).

Tags (associated with assets and collections in [!DNL AEM]) are auto-published to [!DNL Brand Portal] when the assets (and collections) with associated tags are published to [!DNL Brand Portal]. Les balises publiées sont utiles pour rechercher et trouver les ressources associées.

>[!NOTE]
>
>It is, however, recommended to exclusively publish tags to [!DNL Brand Portal] before publishing the assets (and collections) with which the tags are associated. Cela assure une publication plus rapide des ressources (et des collections) sur [!DNL Brand Portal].

## Manage tags {#manage-tags}

You can use the pre-existing tags to attach to an asset or create new tags from [!DNL AEM] Tags console (**Tools | Tagging |[!DNL AEM]Tags**). In both the scenarios you must first publish the tags to [!DNL Brand Portal] and then associate them with appropriate assets.

To create tags on [!DNL AEM], publish the tags on [!DNL Brand Portal], and associate the tags with appropriate assets (or collections), follow these steps:

1. **Créez des balises**
dans l'instance [!DNL AEM] Auteur avec des privilèges d'administrateur et accédez à la console **[!DNL AEM]Balises** à partir de la navigation globale :

   1. Select **Tools**

   2. Select **General**

   3. Select **Tagging**

2. Select **Create** and then select **Create Tag** option.
3. Spécifiez les paramètres suivants :

   * **Titre**
      *(obligatoire)* Titre d'affichage de la balise.
   * **Nom**
      *(Obligatoire)* Nom de la balise. Si aucun nom n’est spécifié, un nom de nœud valide est créé à partir du titre. See [TagID](https://helpx.adobe.com/experience-manager/6-5/sites/developing/using/framework.html#TagID).
   * **Description**
      *(Facultatif)* Description de la balise.
   * **Chemin d’accès aux balises** Chemin JCR de la balise.

4. Sélectionnez **Envoyer** pour créer la balise.

   Once you have created a tag on [!DNL AEM] instance, the tag will be available to be attached to an asset (using Properties section or Manage Tags section of that asset).

5. **Publiez la balise.[!DNL Brand Portal]**

   Go to **[!DNL AEM]Tags** console (Tools | Tagging | [!DNL AEM] Tags), select the desired tag and Publish to **[!DNL Brand Portal]**.

6. **Joignez la balise à une ressource (ou collection)**.

   Sélectionnez une ressource (ou collection) et joignez la balise désirée en utilisant la section Propriétés ou Gérer les balises de cette ressource. To know more about how to assign tags to assets in [!DNL AEM] Assets, refer [use tags to organize assets](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets).

7. **Publiez des fichiers (ou collections) vers[!DNL Brand Portal]**.\
   When you publish an asset (or collection) to [!DNL Brand Portal], the attached tag is also available on [!DNL Brand Portal].

   To see the attached tag on the respective asset (or collection) in [!DNL Brand Portal], log in to [!DNL Brand Portal] and select the asset, under Properties section you will see the attached Tag.

## Rechercher une promotion {#search-promote}

[!DNL AEM] Assets  vous permet de faire apparaître des ressources spécifiques dans les premiers résultats des recherches basées sur une balise de mot-clé.[!DNL Brand Portal]

Pour promouvoir une ressource pour un mot-clé de recherche, suivez ces étapes :

1. Ouvrez la page **Propriétés** d’une ressource sur l’instance d’auteur [!DNL AEM]
2. Accédez à l’onglet **Avancé**.
3. In **Search Promote** within **Elevate for search keywords** section, select **Add** to add the search keywords or tags.

   ![](assets/search-promote.png)

4. Enregistrez les modifications.
5. Publish the asset to [!DNL Brand Portal].
6. Connectez-vous [!DNL Brand Portal]. Consultez l’onglet **Avancé** dans la section **Propriétés** de la ressource.
Note that the **Search Promote** keyword is also visible in the Properties of that asset.
