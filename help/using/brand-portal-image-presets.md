---
title: Application de paramètres d’image prédéfinis ou de rendus dynamiques
seo-title: Application de paramètres d’image prédéfinis ou de rendus dynamiques
description: 'Tout comme une macro, un paramètre d’image prédéfini est un ensemble prédéfini de commandes de dimensionnement et de formatage enregistrées sous un nom. Les paramètres d’image prédéfinis permettent à AEM Assets Brand Portal de fournir dynamiquement des images ayant des tailles, des propriétés et des formats différents. '
seo-description: 'Tout comme une macro, un paramètre d’image prédéfini est un ensemble prédéfini de commandes de dimensionnement et de formatage enregistrées sous un nom. Les paramètres d’image prédéfinis permettent à AEM Assets Brand Portal de fournir dynamiquement des images ayant des tailles, des propriétés et des formats différents. '
uuid: a 3 c 8705 c -5 fbd -472 c -8 b 61-f 65 b 3 e 552 c 1 b
content-type: référence
topic-tags: administration
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
discoiquuid: a 512 dfa 0-fef 3-4 c 3 f-a 389-a 0 a 3 a 7415 bac
translation-type: tm+mt
source-git-commit: c0169450c5cf1d8c99f8604df3bd2667445ff1ed

---


# Application de paramètres d’image prédéfinis ou de rendus dynamiques {#apply-image-presets-or-dynamic-renditions}

Tout comme une macro, un paramètre d’image prédéfini est un ensemble prédéfini de commandes de dimensionnement et de formatage enregistrées sous un nom. Les paramètres d’image prédéfinis permettent à AEM Assets Brand Portal de fournir dynamiquement des images ayant des tailles, des propriétés et des formats différents.

Un paramètre d’image prédéfini est utilisé pour générer des rendus dynamiques d’images qui peuvent être prévisualisées et téléchargées. Lorsque vous prévisualisez des images et leurs rendus, vous pouvez choisir un paramètre prédéfini en vue de reformater les images selon les spécifications définies par l’administrateur.

Pour afficher les rendus dynamiques d'un fichier dans le portail de marque, assurez-vous que son rendu Pyramid tiff existe dans l'instance d'auteur AEM depuis l'emplacement où vous publiez sur Brand Portal. Lorsque vous publiez une ressource, son rendu PTIFF est également publié sur Brand Portal. Il n’existe aucun moyen pour générer le rendu PTIFF à partir de Brand Portal.

>[!NOTE]
>
>Lorsque vous téléchargez des images et leurs rendus, il n’existe aucune option pour les paramètres prédéfinis existants. Vous pouvez en revanche spécifier les propriétés d’un paramètre prédéfini d’image personnalisé. Pour plus d’informations, voir [Application de paramètres d’image prédéfinis lors du téléchargement d’images](../using/brand-portal-image-presets.md#main-pars-text-1403412644).

Pour plus d’informations sur les paramètres requis lors de la création de paramètres d’image prédéfinis, voir [Gestion des paramètres d’image prédéfinis](https://docs.adobe.com/docs/en/AEM/6-0/administer/integration/dynamic-media/image-presets.html).

## Création d’un paramètre d’image prédéfini {#create-an-image-preset}

Les administrateurs peuvent créer des paramètres d’image prédéfinis qui apparaissent comme des rendus dynamiques sur la page des détails des ressources. Vous pouvez créer entièrement un paramètre d’image prédéfini ou en enregistrer un existant sous un nouveau nom. Lors de la création d’un paramètre d’image prédéfini, choisissez une taille pour la diffusion des images et les commandes de formatage. Lorsqu’une image est diffusée en vue d’être affichée, son aspect est optimisé selon les commandes sélectionnées.
Remarque : seuls les administrateurs peuvent créer des paramètres d’image prédéfinis dans Brand Portal.

Remarque : seuls les administrateurs peuvent créer des paramètres d’image prédéfinis dans Brand Portal.

>[!NOTE]
>
>Les rendus dynamiques sont créés pour les ressources pour lesquelles PTIFF est disponible. Ainsi, si une ressource ne dispose pas de rendu Pyramid TIFF créé sur AEM et publié sur Brand Portal, seuls les rendus système peuvent être exportés, mais les rendus dynamiques sont présentés en tant qu’option.
Le mode hybride de Media Dynamic doit être activé sur AEM (auteur) pour créer un rendu ptiff d’une ressource. Lorsqu'un tel fichier est publié sur le portail de marque, les paramètres d'image prédéfinis sont appliqués et les rendus dynamiques sont affichés.

1. Dans la barre d'outils AEM en haut, cliquez sur le logo Adobe pour accéder aux outils d'administration.

2. From the administrative tools panel, click **[!UICONTROL Image Presets]**.

   ![](assets/admin-tools-panel-4.png)

3. Dans la page des paramètres d’image prédéfinis, cliquez sur **[!UICONTROL Créer]**.

   ![](assets/image_preset_homepage.png)

4. In the **[!UICONTROL Edit Image Preset]** page, enter values into the **[!UICONTROL Basic]** and **[!UICONTROL Advanced]** tabs as appropriate, including a name. The options are outlined in [Image Preset options](https://docs.adobe.com/docs/en/AEM/6-0/administer/integration/dynamic-media/image-presets.html#Image%20preset%20options). Les paramètres prédéfinis s’affichent dans le volet de gauche et peuvent être utilisés à la volée avec d’autres ressources.

   ![](assets/image_preset_create.png)

   >[!NOTE]
   >
   >You can also use the **[!UICONTROL Edit Image Preset]** page to edit the properties of an existing image preset. To edit an image preset, select it from the image presets page, and click **[!UICONTROL Edit]**.

5. Cliquez sur **[!UICONTROL Enregistrer]**. Le paramètre d’image prédéfini est créé et affiché dans la page des paramètres d’image prédéfinis.
6. Pour supprimer un paramètre d’image prédéfini, sélectionnez-le dans la page des paramètres d’image prédéfinis et cliquez sur **[!UICONTROL Supprimer]**. Dans la page de confirmation, cliquez sur **[!UICONTROL Supprimer]pour confirmer la suppression.** Le paramètre d’image prédéfini est supprimé de la page des paramètres d’image prédéfinis.

## Application de paramètres d’image prédéfinis lors de la prévisualisation d’images  {#apply-image-presets-when-previewing-images}

Lorsque vous prévisualisez des images et leurs rendus, effectuez un choix parmi les paramètres prédéfinis existants pour reformater les images selon les spécifications définies par l’administrateur.

1. Dans l'interface de Portal Portal, cliquez sur une image pour l'ouvrir.
2. Click the overlay icon on the left, and choose **[!UICONTROL Renditions]**.

   ![](assets/image-preset-previewrenditions.png)

3. From the **[!UICONTROL Renditions]** list, select the appropriate dynamic rendition, for example, **[!UICONTROL Thumbnail]**. L’image d’aperçu est rendue selon votre choix de rendu.

   ![](assets/image-preset-previewrenditionthumbnail.png)

## Application de paramètres d’image prédéfinis lors du téléchargement d’images {#apply-image-presets-when-downloading-images}

Lors du téléchargement d'images et de leurs rendus depuis Brand Portal, vous ne pouvez pas choisir parmi les paramètres d'image prédéfinis existants. Vous pouvez toutefois personnaliser les propriétés des paramètres d’image prédéfinis en fonction du reformatage souhaité des images.

1. Dans l'interface de Brand Portal, effectuez l'une des opérations suivantes :

   * Placez le pointeur sur l’image que vous souhaitez télécharger. From the quick action thumbnails available, click the **[!UICONTROL Download]** icon.
   ![](assets/downloadsingleasset.png)

   * Sélectionnez l’image que vous souhaitez télécharger. From the toolbar at the top, click the **[!UICONTROL Download]** icon.
   ![](assets/downloadassets.png)

2. Dans la boîte de dialogue **[!UICONTROL Télécharger], sélectionnez les options requises selon que vous souhaitez télécharger la ressource avec ou sans ses rendus.**

   ![](assets/donload-assets-dialog.png)

3. Pour télécharger des rendus dynamiques de la ressource, sélectionnez l’option **[!UICONTROL Rendu(s) dynamique(s)].**
4. Personnalisez les propriétés du paramètre d’image prédéfini sur lesquelles vous souhaitez reformater dynamiquement l’image et ses rendus lors du téléchargement. Indiquez la taille, le format, l’espace colorimétrique, la résolution et le modificateur d’image.

   ![](assets/dynamicrenditions.png)

5. Cliquez sur **[!UICONTROL Télécharger]**. Les rendus dynamiques personnalisés sont téléchargés dans un fichier ZIP avec l’image et les rendus que vous avez choisis de télécharger. Cependant, aucun fichier ZIP n’est créé si une seule ressource est téléchargée, ce qui garantit un téléchargement rapide.
