---
title: Application de paramètres d’image prédéfinis ou de rendus dynamiques
seo-title: Application de paramètres d’image prédéfinis ou de rendus dynamiques
description: 'Tout comme une macro, un paramètre d’image prédéfini est un ensemble prédéfini de commandes de dimensionnement et de formatage enregistrées sous un nom. Les paramètres d’image prédéfinis permettent à AEM Assets Brand Portal de fournir dynamiquement des images ayant des tailles, des propriétés et des formats différents. '
seo-description: 'Tout comme une macro, un paramètre d’image prédéfini est un ensemble prédéfini de commandes de dimensionnement et de formatage enregistrées sous un nom. Les paramètres d’image prédéfinis permettent à AEM Assets Brand Portal de fournir dynamiquement des images ayant des tailles, des propriétés et des formats différents. '
uuid: a3c8705c-5fbd-472c-8b61-f65b3e552c1b
content-type: reference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: a512dfa0-fef3-4c3f-a389-a0a3a7415bac
role: Admin
exl-id: 212a1b3a-686f-4250-be06-b679b6039887
source-git-commit: 26b009fec800d9b437bde5838009c71b1b3b7ac6
workflow-type: ht
source-wordcount: '871'
ht-degree: 100%

---

# Application de paramètres d’image prédéfinis ou de rendus dynamiques {#apply-image-presets-or-dynamic-renditions}

Tout comme une macro, un paramètre d’image prédéfini est un ensemble prédéfini de commandes de dimensionnement et de formatage enregistrées sous un nom. Les paramètres d’image prédéfinis permettent à AEM Assets Brand Portal de fournir dynamiquement des images ayant des tailles, des propriétés et des formats différents.

Un paramètre d’image prédéfini est utilisé pour générer des rendus dynamiques d’images qui peuvent être prévisualisées et téléchargées. Lorsque vous prévisualisez des images et leurs rendus, vous pouvez choisir un paramètre prédéfini en vue de reformater les images selon les spécifications définies par l’administrateur.

(*Si l’instance (d’auteur) AEM est en cours d’exécution en **mode hybride Dynamic Media***) Pour afficher les rendus dynamiques d’une ressource dans Brand Portal, vérifiez que son rendu PTIFF (Pyramid TIFF) existe dans l’instance d’auteur AEM à partir de laquelle vous procédez à la publication sur Brand Portal. Lorsque vous publiez une ressource, son rendu PTIFF est également publié sur Brand Portal.

>[!NOTE]
>
>Lorsque vous téléchargez des images et leurs rendus, il n’existe aucune option pour les paramètres prédéfinis existants. Vous pouvez en revanche spécifier les propriétés d’un paramètre prédéfini d’image personnalisé. Pour plus d’informations, voir [Application de paramètres d’image prédéfinis lors du téléchargement d’images](../using/brand-portal-image-presets.md#main-pars-text-1403412644).


Pour plus d’informations sur les paramètres requis lors de la création de paramètres d’image prédéfinis, voir [Gestion des paramètres d’image prédéfinis](https://docs.adobe.com/docs/en/AEM/6-0/administer/integration/dynamic-media/image-presets.html).

## Création d’un paramètre d’image prédéfini {#create-an-image-preset}

Les administrateurs d’AEM peuvent créer des paramètres d’image prédéfinis qui apparaissent comme des rendus dynamiques sur la page des détails des ressources. Vous pouvez créer entièrement un paramètre d’image prédéfini ou en enregistrer un existant sous un nouveau nom. Lors de la création d’un paramètre d’image prédéfini, choisissez une taille pour la diffusion des images et les commandes de formatage. Lorsqu’une image est diffusée en vue d’être affichée, son aspect est optimisé selon les commandes sélectionnées.

>[!NOTE]
>
>Les rendus dynamiques d’une image sont créés à l’aide de son fichier Pyramid TIFF. Si le fichier Pyramid TIFF n’est disponible pour aucune ressource, les rendus dynamiques de cette ressource ne peuvent pas être récupérés dans Brand Portal.
>
>Si l’instance d’auteur AEM est en cours d’exécution en mode **hybride Dynamic Media**, les rendus Pyramid TIFF des ressources d’image sont créés et enregistrés dans le référentiel AEM.
>
>En revanche, si l’instance d’auteur AEM est en cours d’exécution en **mode Dynamic Media Scene7**, les rendus Pyramid TIFF des ressources d’image existent sur le serveur Scene7.
>
>Lorsque des ressources de ce type sont publiées sur Brand Portal, les paramètres d’image prédéfinis sont appliqués et les rendus dynamiques sont affichés.


1. Dans la barre d’outils AEM supérieure, cliquez sur le logo Adobe pour accéder aux outils d’administration.

1. Dans le panneau des outils d’administration, cliquez sur **[!UICONTROL Paramètres d’image prédéfinis]**.

   ![](assets/admin-tools-panel-4.png)

1. Dans la page des paramètres d’image prédéfinis, cliquez sur **[!UICONTROL Créer]**.

   ![](assets/image_preset_homepage.png)

1. Dans la page **[!UICONTROL Modifier le paramètre d’image prédéfini]**, saisissez les valeurs adéquates dans les onglets **[!UICONTROL De base]** et **[!UICONTROL Avancé]**, notamment un nom. Les options sont décrites dans [Options d’image prédéfinies](https://docs.adobe.com/docs/en/AEM/6-0/administer/integration/dynamic-media/image-presets.html#Image%20preset%20options). Les paramètres prédéfinis s’affichent dans le volet de gauche et peuvent être utilisés à la volée avec d’autres ressources.

   ![](assets/image_preset_create.png)

   >[!NOTE]
   >
   >Vous pouvez également utiliser la page **[!UICONTROL Modifier le paramètre d’image prédéfini]** pour modifier les propriétés d’un paramètre d’image prédéfini existant. Pour modifier un paramètre d’image prédéfini, sélectionnez-le dans la page des paramètres d’image prédéfinis, puis cliquez sur **[!UICONTROL Modifier]**.

1. Cliquez sur **[!UICONTROL Enregistrer]**. Le paramètre d’image prédéfini est créé et affiché dans la page des paramètres d’image prédéfinis.
1. Pour supprimer un paramètre d’image prédéfini, sélectionnez-le dans la page des paramètres d’image prédéfinis et cliquez sur **[!UICONTROL Supprimer]**. Dans la page de confirmation, cliquez sur **[!UICONTROL Supprimer]** pour confirmer la suppression. Le paramètre d’image prédéfini est supprimé de la page des paramètres d’image prédéfinis.

## Application de paramètres d’image prédéfinis lors de la prévisualisation d’images  {#apply-image-presets-when-previewing-images}

Lorsque vous prévisualisez des images et leurs rendus, choisissez parmi les paramètres prédéfinis existants pour reformater les images selon les spécifications définies par l’administrateur.

1. Dans l’interface de Brand Portal, cliquez sur l’image pour l’ouvrir.
1. Cliquez sur l’icône de recouvrement située à gauche, puis sélectionnez **[!UICONTROL Rendus]**.

   ![](assets/image-preset-previewrenditions.png)

1. Dans la liste **[!UICONTROL Rendus]**, sélectionnez le rendu dynamique adéquat, par exemple **[!UICONTROL Miniature]**. L’image d’aperçu est rendue selon le rendu que vous avez sélectionné.

   ![](assets/image-preset-previewrenditionthumbnail.png)

## Application de paramètres d’image prédéfinis lors du téléchargement d’images {#apply-image-presets-when-downloading-images}

Lorsque vous téléchargez des images et leurs rendus à partir de Brand Portal, vous ne pouvez pas effectuer de choix parmi les paramètres d’image prédéfinis existants. Vous pouvez toutefois personnaliser les propriétés des paramètres d’image prédéfinis en fonction du reformatage souhaité des images.

1. Dans l’interface de Brand Portal, effectuez l’une des opérations suivantes :

   * Placez le pointeur sur l’image que vous souhaitez télécharger. Dans les miniatures d’action rapide disponibles, cliquez sur l’icône **[!UICONTROL Télécharger]**.

   ![](assets/downloadsingleasset.png)

   * Sélectionnez l’image que vous souhaitez télécharger. Dans la barre d’outils supérieure, cliquez sur l’icône **[!UICONTROL Télécharger]**.

   ![](assets/downloadassets.png)

1. Dans la boîte de dialogue **[!UICONTROL Télécharger]**, sélectionnez les options requises selon que vous souhaitez télécharger la ressource avec ou sans ses rendus.

   ![](assets/donload-assets-dialog.png)

1. Pour télécharger des rendus dynamiques de la ressource, sélectionnez l’option **[!UICONTROL Rendu(s) dynamique(s)]**.
1. Personnalisez les propriétés du paramètre d’image prédéfini sur lesquelles vous souhaitez reformater dynamiquement l’image et ses rendus lors du téléchargement. Indiquez la taille, le format, l’espace colorimétrique, la résolution et le modificateur d’image.

   ![](assets/dynamicrenditions.png)

1. Cliquez sur **[!UICONTROL Télécharger]**. Les rendus dynamiques personnalisés sont téléchargés dans un fichier ZIP avec l’image et les rendus que vous avez choisis de télécharger. Cependant, aucun fichier ZIP n’est créé si une seule ressource est téléchargée, ce qui garantit un téléchargement rapide.
