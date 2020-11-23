---
title: Téléchargement de ressources
seo-title: Téléchargement de ressources
description: Tous les utilisateurs peuvent simultanément télécharger plusieurs ressources et dossiers auxquels ils ont accès. Ainsi, les ressources de marque approuvées peuvent être distribuées en toute sécurité pour une utilisation en mode hors connexion.
seo-description: Tous les utilisateurs peuvent simultanément télécharger plusieurs ressources et dossiers auxquels ils ont accès. Ainsi, les ressources de marque approuvées peuvent être distribuées en toute sécurité pour une utilisation en mode hors connexion.
uuid: 4b57118e-a76e-4d8a-992a-cb3c3097bc03
content-type: reference
contentOwner: Vishabh Gupta
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: download-install
discoiquuid: f90c2214-beea-4695-9102-8b952bc9fd17
translation-type: tm+mt
source-git-commit: 1a8658a3ced4fd211a1c1606a80bb51920ca8be1
workflow-type: tm+mt
source-wordcount: '1879'
ht-degree: 39%

---


# Téléchargement de fichiers depuis le portail des marques {#download-assets-from-bp}

<!-- Before update in Download experience - 26th Aug 2020 comment by Vishabh.
 All users can simultaneously download multiple assets and folders accessible to them from Brand Portal. This way, approved brand assets can be securely distributed for offline use. Read on to know how to download approved assets from Brand Portal, and what to expect from the [download performance](../using/brand-portal-download-assets.md#main-pars-header).
-->

Adobe Experience Manager Assets Brand Portal améliore l’expérience de téléchargement en permettant aux utilisateurs de télécharger simultanément plusieurs dossiers et ressources accessibles directement. Ainsi, les ressources de marque approuvées peuvent être distribuées en toute sécurité pour une utilisation en mode hors connexion. Lisez ce qui suit pour savoir comment télécharger des ressources approuvées à partir de Brand Portal et en savoir plus sur les [performances de téléchargement](../using/brand-portal-download-assets.md#expected-download-performance).


>[!NOTE]
>
>Dans la version 2020.10.0 de Brand Portal (et ultérieure), le paramètre Téléchargement **** rapide est activé par défaut, qui utilise IBM Aspera Connect pour accélérer le téléchargement des ressources. [Installez IBM Aspera Connect 3.9.9 dans l’extension de votre navigateur avant de télécharger les ressources à partir de Brand Portal. ](https://www.ibm.com/support/knowledgecenter/SSXMX3_3.9.9/kc/connect_welcome.html) For more details, see [guide to accelerate downloads from Brand Portal](../using/accelerated-download.md).
>
>Si vous ne souhaitez pas utiliser IBM Aspera Connect et poursuivre le processus de téléchargement normal, contactez l’administrateur du portail des marques pour désactiver le paramètre Téléchargement **** rapide.

## Configuration du téléchargement des ressources {#configure-download}

Les administrateurs du portail des marques peuvent configurer les paramètres de téléchargement des fichiers et les autorisations pour les utilisateurs du portail des marques, ce qui leur permet d’accéder aux rendus de fichiers et de les télécharger à partir de l’interface du portail des marques et de les télécharger.

L’accès et le téléchargement des rendus à partir de Brand Portal sont définis par les configurations suivantes :

* Activer les paramètres de téléchargement
* Configuration des autorisations de téléchargement

### Activer les paramètres de téléchargement {#enable-download-settings}

Les administrateurs peuvent activer les paramètres **[!UICONTROL de]** téléchargement des ressources pour définir l’ensemble de rendus accessibles aux utilisateurs du portail de marque pour le téléchargement.

Les paramètres disponibles sont les suivants :

* **[!UICONTROL Téléchargement rapide]**

   Il permet un téléchargement accéléré des ressources à l’aide d’IBM Aspera Connect. By default, the **[!UICONTROL Fast Download]** setting is enabled in the **[!UICONTROL Download Settings]**.

* **[!UICONTROL Rendus personnalisés]**

   Permet de télécharger des rendus personnalisés et (ou) dynamiques des ressources.

   Tous les rendus de ressources autres que l’actif d’origine et les rendus générés par le système sont appelés rendus personnalisés. Ils comprennent des rendus statiques et dynamiques disponibles pour les ressources. Un utilisateur peut créer un rendu statique personnalisé dans AEM Assets, alors que seul l’administrateur AEM peut créer des rendus dynamiques personnalisés. For details, see [how to apply image presets or dynamic renditions](../using/brand-portal-image-presets.md).

* **[!UICONTROL Rendus du système]**

   Permet de télécharger les rendus des ressources générés par le système.

   Il s’agit des miniatures qui sont automatiquement générées dans AEM Assets en fonction du workflow de mise à jour de ressource DAM.

Connectez-vous à votre client Brand Portal en tant qu’administrateur et accédez à **[!UICONTROL Outils]** > **[!UICONTROL Télécharger]**.

Les administrateurs peuvent activer toute combinaison de paramètres permettant aux utilisateurs du portail de marque d’accéder aux rendus et de les télécharger.

![](assets/download-configuration.png)


>[!NOTE]
>
>Seuls les administrateurs peuvent télécharger les ressources expirées. Pour plus d’informations sur les ressources arrivées à expiration, voir [Gestion des droits numériques des ressources](../using/manage-digital-rights-of-assets.md).

### Configuration des autorisations de téléchargement {#configure-download-permissions}

Outre les paramètres **[!UICONTROL de]** téléchargement, les administrateurs du portail de marque peuvent configurer davantage les autorisations de vue de différents groupes d’utilisateurs et (ou) télécharger les ressources d’origine et leurs rendus.

Log in to your Brand Portal tenant as an administrator and navigate to **[!UICONTROL Tools]** > **[!UICONTROL Users]**. Dans la page Rôles **** utilisateur, accédez à l’onglet **[!UICONTROL Groupes]** pour configurer la vue et (ou) les autorisations de téléchargement des groupes d’utilisateurs.

![autorisation-téléchargement-affichage](assets/download-permissions.png)

>[!NOTE]
>
>Si un utilisateur est ajouté à plusieurs groupes, et si l’un de ces groupes présente des restrictions, les restrictions s’appliquent à cet utilisateur.

En fonction de la configuration, le workflow de téléchargement reste le même pour les ressources uniques ou multiples, les dossiers contenant des ressources, les ressources qui sont ou non sous licence, ainsi que le téléchargement de ressources à l’aide du lien de partage.

La matrice suivante définit si un utilisateur a accès aux rendus en fonction des configurations [de](#configure-download)téléchargement :

| **Paramètres de téléchargement : Rendus personnalisés** | **Paramètres de téléchargement : Rendus système** | **Autorisations de groupe d’utilisateurs : Télécharger l’original** | **Autorisations de groupe d’utilisateurs : Télécharger des rendus** | **Résultat** |
|---|---|---|---|---|
| ACTIVE | ACTIVE | ACTIVE | ACTIVE | Vue et téléchargement de tous les rendus |
| ACTIVE | ACTIVE | OFF | OFF | Ressource d’origine de la vue |
| OFF | OFF | ACTIVE | ACTIVE | Vue et téléchargement de la ressource d’origine |
| ACTIVE | OFF | ACTIVE | ACTIVE | Vue et téléchargement des ressources d’origine et des rendus personnalisés |
| OFF | ACTIVE | ACTIVE | ACTIVE | Vue et téléchargement de rendus de ressources et de systèmes d’origine |
| ACTIVE | OFF | OFF | OFF | Ressource d’origine de la vue |
| OFF | ACTIVE | OFF | OFF | Ressource d’origine de la vue |
| OFF | OFF | OFF | ACTIVE | Ressource d’origine de la vue |
| OFF | OFF | ACTIVE | OFF | Vue et téléchargement de la ressource d’origine |
| OFF | OFF | OFF | OFF | Ressource d’origine de la vue |



## Téléchargement de ressources {#download-assets}

Les utilisateurs du portail de marque peuvent télécharger plusieurs fichiers, dossiers contenant des fichiers et collections depuis l’interface du portail de marque.

>[!NOTE]
>
>Contactez l’administrateur du portail des marques si vous n’êtes pas autorisé à accéder aux rendus ou à les télécharger.

Si l’utilisateur a accès à des rendus, la boîte de dialogue de **[!UICONTROL téléchargement]** améliorée s’affiche avec les fonctionnalités suivantes :
* afficher tous les rendus disponibles de toutes les ressources dans la liste de téléchargement ;
* exclure les rendus des ressources qui ne sont pas nécessaires pour le téléchargement ;
* Appliquez le même jeu de rendus à tous les types de ressource similaires en un seul clic.
* Appliquez un ensemble différent de rendus pour différents types de fichier.
* Créez un dossier distinct pour chaque rendu de fichier.
* télécharger les ressources sélectionnées et leurs rendus.

![boîte-de-dialogue-télécharger](assets/download-dialog-box.png)

>[!NOTE]
>
>La boîte de dialogue **[!UICONTROL Télécharger]** s’affiche uniquement si les ressources sont sélectionnées pour le téléchargement et si les rendus **** personnalisés ou les rendus **** système sont activés dans les paramètres de **[!UICONTROL téléchargement.]**


### Étapes de téléchargement des ressources {#bulk-download}

Vous trouverez ci-dessous la procédure à suivre pour télécharger des fichiers ou des dossiers contenant des fichiers à partir de l’interface du portail de marque :

1. Connectez-vous à votre locataire du portail de marques. Par défaut, la vue **[!UICONTROL Fichiers]** s’ouvre et contient tous les fichiers et dossiers publiés.

   Utilisez l’une des méthodes suivantes :

   * Sélectionnez les fichiers ou les dossiers à télécharger. Dans la barre d’outils supérieure, cliquez sur l’icône **[!UICONTROL Télécharger]**.

      ![select-multiple-assets](assets/select-assets-new.png)

   * To download specific asset renditions of an asset, hover the pointer over the asset and click the **[!UICONTROL Download]** icon available in the quick action thumbnails.

      ![select-asset](assets/select-asset.png)


      >[!NOTE]
      >
      >Si vous téléchargez les ressources pour la première fois et qu’IBM Aspera Connect n’est pas installé dans votre navigateur, vous êtes invité à installer l’accélérateur de téléchargement Aspera.


      >[!NOTE]
      >
      >Si les ressources que vous téléchargez comprennent également des ressources sous licence, vous êtes redirigé vers la page **[!UICONTROL Gestion des droits d’auteur]**. Dans cette page, sélectionnez les ressources, cliquez d’abord sur **[!UICONTROL Accepter]**, puis sur **[!UICONTROL Télécharger]**. Si vous choisissez de ne pas accepter, les ressources sous licence ne sont pas téléchargées.
      > 
      >Dans le cas des ressources protégées par une licence, un [contrat de licence leur est associé](https://helpx.adobe.com/fr/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) en définissant la [propriété de métadonnées](https://helpx.adobe.com/fr/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) appropriée dans Experience Manager Assets.


      ![license-asset](assets/licensed-asset-new.png)

1. La boîte de dialogue **[!UICONTROL Télécharger]** répertoriant tous les fichiers sélectionnés s’ouvre.

   Cliquez sur un fichier pour vue les rendus disponibles et cochez les cases correspondant aux rendus à télécharger.

   Vous pouvez sélectionner ou exclure manuellement les rendus de fichiers individuels ou cliquer sur l’icône **Appliquer** pour sélectionner le même ensemble de rendus à télécharger pour des types de fichiers similaires (tous les fichiers image de cet exemple). Dans la boîte de dialogue **[!UICONTROL Appliquer tout]** , cliquez sur **[!UICONTROL Terminé]** pour appliquer la règle à tous les actifs similaires.

   ![appliquer tout](assets/apply.png)

   Vous pouvez également supprimer un fichier de la liste de téléchargement (si nécessaire) en cliquant sur l’icône **Supprimer** .

   ![supprimer](assets/remove.png)

   Pour conserver la hiérarchie des dossiers de Brand Portal lors du téléchargement des ressources, cochez la case **[!UICONTROL Créer un dossier distinct pour chaque ressource]**. Par défaut, la hiérarchie des dossiers du portail des marques est ignorée et tous les fichiers sont téléchargés dans un dossier zip.

   Le bouton de téléchargement indique le nombre d’éléments sélectionnés. Une fois les règles appliquées, cliquez sur **[!UICONTROL Télécharger les éléments]**.

   ![boîte-de-dialogue-télécharger](assets/download-dialog-new.png)

1. By default the **[!UICONTROL Fast Download]** setting is enabled in the **[!UICONTROL Download Settings]**. Par conséquent, une zone de confirmation s’affiche pour permettre un téléchargement accéléré à l’aide d’IBM Aspera Connect.

   Pour continuer à utiliser le téléchargement **** rapide, cliquez sur **[!UICONTROL Autoriser]**. Tous les rendus sélectionnés sont téléchargés dans un dossier zip à l’aide d’IBM Aspera Connect.

   Si vous ne souhaitez pas utiliser IBM Aspera Connect, cliquez sur **[!UICONTROL Refuser]**. Si le téléchargement **** rapide est refusé ou échoue, le système remplit un message d’erreur. Cliquez sur le bouton Téléchargement **** normal pour continuer à télécharger les ressources. Les rendus sélectionnés sont téléchargés dans un dossier zip sans utiliser IBM Aspera Connect.

>[!NOTE]
>
>Si le paramètre Téléchargement **** rapide est désactivé par l’administrateur, les rendus sélectionnés sont directement téléchargés dans un dossier zip sans utiliser IBM Aspera Connect.


>[!NOTE]
>
>Si un dossier, une collection ou plus de 20 fichiers sont sélectionnés pour téléchargement, la boîte de dialogue **[!UICONTROL Télécharger]** est ignorée et tous les rendus de fichiers accessibles à l’utilisateur, à l’exception des rendus dynamiques, sont téléchargés dans un dossier zip. Les rendus de fichier sont téléchargés dans un dossier distinct pour chaque fichier du dossier zip.


>[!NOTE]
>
>Le portail de marque prend en charge la configuration de Contenu multimédia dynamique en mode hybride et Scene7.
>
>(*Si l’instance (d’auteur) AEM est en cours d’exécution en mode **hybride Dynamic Media***.)
>
>Pour prévisualiser ou télécharger les rendus dynamiques d’une ressource, vérifiez que Dynamic Media est activé et que le rendu Pyramid TIFF de la ressource existe au niveau de l’instance d’auteur AEM Assets à partir de laquelle les ressources ont été publiées. Lorsqu’un fichier est publié d’AEM au portail de marque, son rendu pyramidal est également publié.



Si vous n’êtes pas [autorisé par l’administrateur à accéder aux rendus d’origine](../using/brand-portal-adding-users.md#main-pars-procedure-202029708), les rendus d’origine des ressources sélectionnées ne sont pas téléchargés.

![message sans accès](assets/no-access-message.png)

<!-- This issue has been resolved, check with engineering.
>[!NOTE]
>
>Once you have downloaded the asset renditions, the **[!UICONTROL Download]** button is disabled to avoid creating duplicate copies of the renditions. To download more (missing or another copy of renditions), refresh the browser to re-enable the download button.
-->

### Téléchargement de fichiers à partir de la page des détails des fichiers {#download-assets-from-asset-details-page}

Outre le processus de téléchargement, il existe une autre méthode de téléchargement des rendus pour des ressources individuelles directement à partir de la page des détails de la ressource.

Les utilisateurs peuvent prévisualisation différents rendus, sélectionner des rendus spécifiques et les télécharger directement depuis le panneau **[!UICONTROL Rendus]** de la page des détails de la ressource sans avoir à ouvrir la boîte de dialogue de **[!UICONTROL téléchargement]** .


Vous trouverez ci-dessous la procédure à suivre pour télécharger des rendus de ressources à partir de la page des détails de la ressource :

1. Connectez-vous à votre client du portail de marques et cliquez sur le fichier pour ouvrir la page des détails du fichier.
1. Click the overlay icon on the left, and then click **[!UICONTROL Renditions]**.

   ![rendu-navigation](assets/rendition-navigation.png)

1. Le panneau **[!UICONTROL Rendus]** liste tous les rendus de ressources accessibles en fonction des configurations [de](#configure-download)téléchargement de ressources.

   Sélectionnez les rendus spécifiques à télécharger, puis cliquez sur **[!UICONTROL Télécharger les éléments]**.

   ![panneau-rendus](assets/renditions-panel.png)

1. By default the **[!UICONTROL Fast Download]** setting is enabled in the **[!UICONTROL Download Settings]**. Par conséquent, une zone de confirmation s’affiche pour permettre un téléchargement accéléré à l’aide d’IBM Aspera Connect.

   Pour continuer à utiliser le téléchargement **** rapide, cliquez sur **[!UICONTROL Autoriser]**. Tous les rendus sélectionnés sont téléchargés dans un dossier zip à l’aide d’IBM Aspera Connect.

   Si vous refusez d’utiliser le téléchargement **** rapide, le système renseigne un message d’erreur. Cliquez sur le bouton Téléchargement **** normal pour continuer le téléchargement. Les rendus sélectionnés sont téléchargés dans un dossier zip sans utiliser IBM Aspera Connect.

>[!NOTE]
>
>Si le paramètre Téléchargement **** rapide est désactivé par l’administrateur, les rendus sélectionnés sont directement téléchargés dans un dossier zip sans utiliser IBM Aspera Connect.


>[!NOTE]
>
>Les ressources téléchargées individuellement sont visibles dans le rapport sur les ressources téléchargées. Toutefois, si un dossier contenant des ressources est téléchargé, le dossier et les ressources ne sont pas affichés dans le rapport sur les ressources téléchargées.

<!--
>[!NOTE]
>
>Assets that are individually downloaded are visible in the assets download report. However, if a folder containing assets is downloaded, the folder and assets are not displayed in the assets download report.
-->

<!-- Backup of content before updating the new feature docs.
## Configure asset download {#configure-download}

The download configuration allows the Brand Portal administrators to define the set of renditions available to the Brand Portal users for downloading the assets. The administrator can configure the asset **[!UICONTROL Download]** settings from the Brand Portal interface. 

The available configurations are:

* **[!UICONTROL Fast Download]** 

  Enables high-speed download of the assets. To know more, see [guide to accelerate downloads from Brand Portal](../using/accelerated-download.md).

* **[!UICONTROL Custom Renditions]** 
  
  Download custom and (or) dynamic renditions of the assets. 
  All the asset renditions other than the original asset and system-generated renditions are called as custom renditions. It includes static as well as dynamic renditions available for the asset. Any user can create a custom static rendition in AEM Assets, whereas, only the AEM administrator can create custom dynamic renditions. To know more, see [how to apply image presets or dynamic renditions](../using/brand-portal-image-presets.md)

* **[!UICONTROL System Renditions]** 

  Download system-generated renditions of the assets. These are the thumbnails which are automatically generated in AEM Assets based on the "DAM update asset" workflow. 

Log in to your Brand Portal tenant as an administrator and navigate to **[!UICONTROL Tools]** > **[!UICONTROL Download]**. By default, the **[!UICONTROL Fast Download]** configuration is enabled in the **[!UICONTROL Download Settings]**. 

The administrators can enable any combination to configure the asset download process.

![](assets/download-configuration.png)


Based on the configuration, the download workflow remains constant for stand-alone assets, multiple assets, folders containing assets, licensed or unlicensed assets, and downloading assets using share link. 


* If both **[!UICONTROL Custom Renditions]** and **[!UICONTROL System Renditions]** configurations are turned-off, the original renditions of the assets are downloaded without any additional dialog being presented to the users.    


* If any of the **[!UICONTROL Custom Renditions]** or **[!UICONTROL System Renditions]** configuration is enabled, an additional **[!UICONTROL Download]** dialog box appears wherein you can choose whether to download the original asset along with its renditions, or download only specific renditions. 

>[!NOTE]
>
>Only the administrators can download the expired assets. For more information about expired assets, see [manage digital rights of assets](../using/manage-digital-rights-of-assets.md).

## Steps to download assets {#steps-to-download-assets}

Following are the steps to download assets or folders containing assets from Brand Portal:

1. From the Brand Portal interface, do one of the following:

   * Select the folders or assets you want to download. From the toolbar at the top, click the **[!UICONTROL Download]** icon.

     ![](assets/downloadassets-1.png)

   * To download a specific asset or folder, hover the pointer over the asset or folder and click the **[!UICONTROL Download]** icon available in the quick action thumbnails.

     ![](assets/downloadsingleasset-1.png)


     >[!NOTE]
     >
     >If you are downloading the assets for the first time and do not have IBM Aspera Connect installed in your browser, it will prompt you to install the Aspera download accelerator. 


     >[!NOTE]
     >
     >If the assets you are downloading also include licensed assets, you are redirected to the **[!UICONTROL Copyright Management]** page. In this page, select the assets, click **[!UICONTROL Agree]**, and then click **[!UICONTROL Download]**. If you choose to disagree, licensed assets are not downloaded. 
     > 
     >License-protected assets have [license agreement attached](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) to them, which is done by setting asset's [metadata property](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) in Experience Manager Assets.


     ![](assets/licensed-asset-download-1.png)

     
     >[!NOTE]
     >
     >Ensure to select all the required asset renditions while downloading them from the asset details page, and click **[!UICONTROL Download]**. The selected renditions are downloaded to your local machine.
     > 
     >Once you download, the **[!UICONTROL Download]** button is disabled to avoid creating duplicate copies of the downloaded renditions. To download more (missing or another copy of renditions), refresh the browser to re-enable the download button.

     If any of the **[!UICONTROL Custom Renditions]** or **[!UICONTROL System Renditions]** configuration is enabled in the **[!UICONTROL Download Settings]**, the **[!UICONTROL Download]** dialog appears with the **[!UICONTROL Asset(s)]** check box selected by default. If the **[!UICONTROL Fast Download]** configuration is enabled, the **[!UICONTROL Enable download acceleration]** check box is selected by default.

     ![](assets/download-dialog.png)

     >[!NOTE]
     >
     >If the downloading assets are image files, and you select only the **[!UICONTROL Asset(s)]** check box in the **[!UICONTROL Download]** dialog but are not [authorized by the administrator to have access to the original renditions of image files](../using/brand-portal-adding-users.md#main-pars-procedure-202029708) then no image files are downloaded and a notification appears, stating that you have been restricted by the administrator to access original renditions.

     ![](assets/restrictaccess-note.png)

1. To download the renditions in addition to the original assets, select the **[!UICONTROL Rendition(s)]** check box. However, if you want to download the system-generated renditions along with the custom renditions, clear the **[!UICONTROL Exclude System Renditions]** check box.

   ![](assets/download-system-rendition.png)

   * To download only the renditions, clear the **[!UICONTROL Asset(s)]** check box.

     >[!NOTE]
     >
     >By default, only the assets are downloaded. However, original renditions of image files are not downloaded if you are not [authorized by the administrator to have access to the original renditions of image files](../using/brand-portal-adding-users.md#main-pars-procedure-202029708).

    * To share the selected assets with other users through a link, select the **[!UICONTROL Email]** check box. An email notification is sent to the users with the download link. To know how to download assets from shared links, see [downloading assets from shared links](../using/brand-portal-link-share.md#main-pars-header-1703469193).  

      ![](assets/download-link.png)

      >[!NOTE]
      >
      >The download link on email notification expires after 45 days.
      >
      >The administrators can customize email messages, that is, logo, description, and footer, using the [Branding](../using/brand-portal-branding.md) feature.


    * You can select a predefined image preset or create a custom dynamic rendition from the **[!UICONTROL Download]** dialog box. 

      To apply a [custom image preset to the asset and its renditions](../using/brand-portal-image-presets.md#applyimagepresetswhendownloadingimages), select the **[!UICONTROL Dynamic Rendition(s)]** check box. Specify the image preset properties (such as size, format, color space, resolution, and image modifier) to apply the custom image preset while downloading the asset and its renditions. To download only the dynamic renditions, clear the **[!UICONTROL Asset(s)]** check box.

      ![](assets/dynamic-rendition.png)

      >[!NOTE]
      >
      >Brand Portal supports configuring Dynamic Media in both - Hybird and Scene 7 mode. 
      >
      >(*If AEM author instance is running on **Dynamic Media Hybrid mode***)
      >
      >To preview or download dynamic renditions of an asset, ensure that the dynamic media is enabled and the asset's Pyramid tiff rendition exists at the AEM Assets author instance from where the assets have been published. When an asset is published to Brand Portal, its Pyramid tiff rendition is also published.
      
  
    * To preserve the Brand Portal folder hierarchy while downloading assets, select the **[!UICONTROL Create separate folder for each asset]** check box. By default, the Brand Portal folder hierarchy is ignored and all the assets are downloaded in one folder in your local system.

1. Click **[!UICONTROL Download]**.

   The assets (and renditions if selected) are downloaded as a zip file to your local folder. However, no zip file is created if a single asset is downloaded without any of the renditions. 

   If you are not [authorized by the administrator to have access to the original renditions](../using/brand-portal-adding-users.md#main-pars-procedure-202029708), the original renditions of the selected assets are not downloaded. 

   >[!NOTE]
   >
   >Assets that are individually downloaded are visible in the assets download report. However, if a folder containing assets is downloaded, the folder and assets are not displayed in the assets download report.
-->

## Performances de téléchargement attendues {#expected-download-performance}

L’expérience de téléchargement de fichier peut varier pour les utilisateurs situés à différents emplacements, en fonction de facteurs tels que la connexion Internet locale et la latence du serveur. Les performances de téléchargement prévues pour un fichier de 2 Go observées à différents emplacements de clients sont les suivantes, avec le serveur Brand Portal situé en Oregon aux États-Unis :

| Emplacement du client | Latence entre le client et le serveur | Vitesse de téléchargement prévue | Durée de téléchargement d’un fichier de 2 Go |
|-------------------------|-----------------------------------|-------------------------|------------------------------------|
| Ouest des États-Unis (Californie du Nord) | 18 millisecondes | 7,68 Mo/s. | 4 minutes |
| Ouest des États-Unis (Oregon) | 42 millisecondes | 3,84 Mo/s. | 9 minutes |
| Est des États-Unis (Virginie du Nord) | 85 millisecondes | 1,61 Mo/s. | 21 minutes |
| Asie-Pacifique (Tokyo) | 124 millisecondes | 1,13 Mo/s. | 30 minutes |
| Noida | 275 millisecondes | 0,5 Mo/s. | 68 minutes |
| Sydney | 175 millisecondes | 0,49 Mo/s. | 69 minutes |
| Londres | 179 millisecondes | 0,32 Mo/s. | 106 minutes |
| Singapour | 196 millisecondes | 0,5 Mo/s. | 68 minutes |


>[!NOTE]
>
>Les données citées sont observées dans les situations de test et peuvent varier pour des utilisateurs à des emplacements différents avec une latence et une bande passante différentes.

