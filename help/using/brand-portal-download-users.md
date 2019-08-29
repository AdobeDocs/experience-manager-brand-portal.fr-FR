---
title: Téléchargement de ressources
seo-title: Téléchargement de ressources
description: Tous les utilisateurs peuvent simultanément télécharger plusieurs ressources et dossiers auxquels ils ont accès. Ainsi, les ressources de marque approuvées peuvent être distribuées en toute sécurité pour une utilisation en mode hors connexion.
seo-description: Tous les utilisateurs peuvent simultanément télécharger plusieurs ressources et dossiers auxquels ils ont accès. Ainsi, les ressources de marque approuvées peuvent être distribuées en toute sécurité pour une utilisation en mode hors connexion.
uuid: 4 b 57118 e-a 76 e -4 d 8 a -992 a-cb 3 c 3097 bc 03
content-type: référence
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
topic-tags: téléchargement-install
discoiquuid: f 90 c 2214-beea -4695-9102-8 b 952 bc 9 fd 17
translation-type: tm+mt
source-git-commit: 32c3cdb8e3fafd74cfb36e6bcfe0811e7152b2d0

---


# Téléchargement de ressources {#download-assets}

Tous les utilisateurs peuvent simultanément télécharger plusieurs ressources et dossiers auxquels ils ont accès à partir de [!DNL Brand Portal]. Ainsi, les ressources de marque approuvées peuvent être distribuées en toute sécurité pour une utilisation en mode hors connexion. Read on to know how to download approved assets from [!DNL Brand Portal], and what to expect from the [download performance](../using/brand-portal-download-users.md#main-pars-header).

>[!NOTE]
>
>Seuls les administrateurs peuvent télécharger les ressources arrivées à expiration. Pour plus d’informations sur les ressources arrivées à expiration, voir [Gestion des droits numériques des ressources](../using/manage-digital-rights-of-assets.md).

## Étapes de téléchargement des ressources {#steps-to-download-assets}

To download assets or folders containing assets for [!DNL Brand Portal], follow these steps:

1. From the [!DNL Brand Portal] interface, do one of the following:

   * Sélectionnez les dossiers ou les ressources que vous souhaitez télécharger. From the toolbar at the top, click the **Download** icon.
   ![](assets/downloadassets-1.png)

   * Pour télécharger un seul dossier ou une ressource, placez le pointeur dessus. From the quick action thumbnails available, click the **Download** icon.
   ![](assets/downloadsingleasset-1.png)

   >[!NOTE]
   >
   >Si les ressources que vous téléchargez comprennent également des ressources sous licence, vous êtes redirigé vers la page **Gestion des droits d’auteur**. Dans cette page, sélectionnez les ressources, cliquez sur **Accepter**, puis cliquez sur **Télécharger**. Si vous choisissez de ne pas accepter, les ressources sans licence ne sont pas téléchargées.\
   >License-protected assets have [license agreement attached](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) to them, which is done by setting asset's [metadata property](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) in [!DNL AEM] Assets.

   ![](assets/licensed-asset-download-1.png)

   The **Download** dialog box appears with the **Asset(s)** option selected by default.

   ![](assets/donload-assets-dialog-1.png)

   >[!NOTE]
   >
   >If the assets you are downloading are image files, and you select only the **Asset(s)** option in Download dialog but are not [authorized by the administrator to have access to the original renditions of image files](../using/brand-portal-adding-users.md#main-pars-procedure-202029708) then no image files are downloaded and a Notice prompts, stating that you have been restricted by administrator to access original renditions.

   ![](assets/restrictaccess-note.png)

2. To download the renditions of assets in addition to the assets, select **Rendition(s)**. However, to allow auto-generated renditions to download along with custom renditions, deselect **Exclude Auto Generated Renditions**, which is selected by default.

   ![](assets/exclude-auto-renditions.png)

   To download only the renditions, deselect **Asset(s)**.

   >[!NOTE]
   >
   >Par défaut, seules les ressources sont téléchargées. However, original renditions of image files are not downloaded if you are not [authorized by the administrator to have access to the original renditions of image files](../using/brand-portal-adding-users.md#main-pars-procedure-202029708).

   * To speed up the download of asset files from [!DNL Brand Portal], select **Enable download acceleration** option and [follow the wizard](../using/accelerated-download.md#main-pars-header-405749062). To know more about faster download of assets refer [Guide to accelerate downloads from [!DNL Brand Portal]](../using/accelerated-download.md).

   * Pour appliquer un [paramètre prédéfini d’image à la ressource et ses rendus](../using/brand-portal-image-presets.md#applyimagepresetswhendownloadingimages), sélectionnez **Rendu (s) dynamique (s)**. Indiquez les propriétés du paramètre prédéfini d’image personnalisé (taille, format, espace colorimétrique, résolution et modificateur d’image) pour l’appliquer lors du téléchargement de la ressource et de ses rendus. Pour télécharger uniquement les rendus dynamiques, désélectionnez **Ressource(s)**.
   ![](assets/dynamic-renditions.png)

   >[!NOTE]
   >
   >To preview (or download) dynamic renditions of any asset, ensure that the dynamic media is enabled and the asset's [!UICONTROL Pyramid tiff] rendition exists at the [!DNL AEM] author instance, from where the assets have been published. When an asset is published to [!DNL Brand Portal], its [!UICONTROL Pyramid tiff] rendition is also published. Il n'existe aucun moyen de générer le rendu [!UICONTROL Pyramid tiff] .[!DNL Brand Portal]

   * To preserve the [!DNL Brand Portal] folder hierarchy while downloading assets, select **Create separate folder for each asset**. By default, [!DNL Brand Portal] folder hierarchy is ignored and all assets are downloaded in one folder in your local system.

   * To send an email notification to users with a link for downloading the assets, select **Email**.
   ![](assets/download-link.png)

   >[!NOTE]
   >
   >Le lien de téléchargement figurant dans la notification électronique expire après 45 jours.
   >
   >Administrators can customize email messages, that is, logo, description, and footer, using the [Branding](../using/brand-portal-branding.md) feature.

3. Cliquez sur **Télécharger**.

   Les ressources (et les rendus s’ils sont sélectionnés) sont téléchargés en tant que fichier ZIP dans votre dossier local. Cependant, aucun fichier ZIP n’est créé lorsqu’une seule ressource est téléchargée sans aucun des rendus, assurant ainsi un téléchargement rapide.

   Les rendus originaux des ressources sélectionnées ne sont pas téléchargés si vous n’êtes pas [autorisé par l’administrateur à y accéder](../using/brand-portal-adding-users.md#main-pars-procedure-202029708).

   >[!NOTE]
   >
   >Les ressources sélectionnées individuellement et téléchargées sont visibles dans le rapport sur les ressources téléchargées. Toutefois, si un dossier contenant des ressources est téléchargé, ni le dossier, ni les actifs ne sont affichés dans le rapport téléchargé.

   Pour savoir comment télécharger des ressources à partir de liens partagés, voir [Téléchargement de ressources à partir de liens partagés](../using/brand-portal-link-share.md#main-pars-header-1703469193).

## Performances de téléchargement attendues {#expected-download-performance}

L'expérience de téléchargement de fichier peut varier selon les utilisateurs, selon des facteurs tels que la connectivité Internet locale et la latence du serveur. The expected download performance for 2 GB file observed at different client locations is as follows, with [!DNL Brand Portal] server at Oregon in United States:

| Emplacement du client | Latence entre le client et le serveur | Vitesse de téléchargement prévue | Temps nécessaire pour télécharger un fichier 2 Go |
|-------------------------|-----------------------------------|-------------------------|------------------------------------|
| Ouest des États-Unis (Californie du Nord) | 18 millisecondes | 7,68 Mo/s | 4 minutes |
| Ouest des États-Unis (Oregon) | 42 millisecondes | 3,84 Mo/s | 9 minutes |
| Est des États-Unis (Virginie du Nord) | 85 millisecondes | 1,61 Mo/s. | 21 minutes |
| Asie-Pacifique (Tokyo) | 124 millisecondes | 1,13 Mo/s | 30 minutes |
| Noida | 275 millisecondes | 0,5 Mo/s | 68 minutes |
| Sydney | 175 millisecondes | 0,49 Mo/s | 69 minutes |
| Londres | 179 millisecondes | 0,32 Mo/s | 106 minutes |
| Singapour | 196 millisecondes | 0,5 Mo/s | 68 minutes |

**Remarque**: Les données citées sont observées dans les conditions de test, lesquelles peuvent varier pour les utilisateurs à différents emplacements qui voient une latence et une bande passante variées.
