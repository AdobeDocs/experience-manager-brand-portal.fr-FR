---
title: Approvisionnement des ressources dans Brand Portal
seo-title: Approvisionnement des ressources dans Brand Portal
description: Découvrez la fonctionnalité d’approvisionnement des ressources disponible dans Adobe Experience Manager Assets Brand Portal.
seo-description: Découvrez la fonctionnalité d’approvisionnement des ressources disponible dans Adobe Experience Manager Assets Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
sub-product: ressources
topics: collaboration, content-velocity, sharing
doc-type: feature-video
activity: use
audience: author, marketer
version: 6.5
kt: 3838
exl-id: 2c132a7a-ed10-4856-8378-67939167ea60
source-git-commit: bfbc90e3cdc9e3fc72a6e54f6730922753585471
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 91%

---

# Présentation de l’approvisionnement des ressources {#overview-asset-sourcing-in-bp}

L’**approvisionnement des ressources** permet aux utilisateurs d’AEM (administrateurs/non-administrateurs) de créer des dossiers avec une propriété **Contribution des ressources** supplémentaire, en s’assurant que les nouveaux dossiers s’ouvrent lorsque des utilisateurs de Brand Portal envoient des ressources. Cela déclenche automatiquement un workflow qui crée deux sous-dossiers supplémentaires, appelés **SHARED** et **NEW**, dans le dossier **Contribution** nouvellement créé. L’administrateur d’AEM définit ensuite les exigences en chargeant un résumé relatif aux types de ressources à ajouter au dossier de contribution, ainsi qu’un ensemble de ressources de base, dans le dossier **SHARED**, afin de s’assurer que les utilisateurs de Brand Portal disposent des informations de référence dont ils ont besoin. L’administrateur peut alors octroyer aux utilisateurs actifs de Brand Portal l’accès au dossier de contribution avant de publier le nouveau dossier **Contribution** sur Brand Portal. Dès que l’utilisateur a fini d’ajouter du contenu dans le dossier **NEW**, il peut republier le dossier de contribution dans l’environnement d’auteur AEM. Notez que l’importation du nouveau contenu publié dans AEM Assets et la prise en compte de cette opération peuvent prendre quelques minutes.

En outre, toutes les fonctionnalités existantes restent inchangées. Les utilisateurs de Brand Portal peuvent afficher, rechercher et télécharger des ressources à partir du dossier de contribution, ainsi que des autres dossiers autorisés. Quant aux administrateurs, ils peuvent partager le dossier de contribution de manière plus avancée, modifier les propriétés et ajouter des ressources aux collections.

![Approvisionnement des ressources dans Brand Portal](assets/asset-sourcing.png)

>[!VIDEO](https://video.tv.adobe.com/v/29365/?quality=12)

## Prérequis {#prerequisites}

* AEM Assets as a Cloud Service, AEM Assets 6.5.2 ou version ultérieure.
* Vérifiez que votre instance d’AEM Assets est configurée avec Brand Portal. Voir [Configuration d’AEM Assets avec Brand Portal](../using/configure-aem-assets-with-brand-portal.md).

<!--
* Ensure that your Brand Portal tenant is configured with one AEM Assets author instance.
-->

>[!NOTE]
>
>La fonctionnalité d’approvisionnement des ressources est activée par défaut sur AEM Assets as a Cloud Service, AEM Assets 6.5.9 et versions ultérieures.
>
>Les configurations existantes continueront à fonctionner sur les versions antérieures.

>[!NOTE]
>
>Il existe un problème connu dans AEM Assets 6.5.4. Les utilisateurs de Brand Portal ne peuvent pas publier les ressources du dossier de contribution dans AEM Assets lors de la mise à niveau vers Adobe Developer Console.
>
>Le problème a été corrigé dans AEM 6.5.5. Vous pouvez mettre à niveau votre instance AEM Assets vers le Service Pack le plus récent, AEM 6.5.5, et [mettre à niveau vos configurations](https://docs.adobe.com/content/help/fr-FR/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) sur Adobe Developer Console.
>
>Pour une solution immédiate sur AEM 6.5.4, il est recommandé de [télécharger le correctif](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) et de l’installer sur votre instance d’auteur.

<!--
## Configure Asset Sourcing {#configure-asset-sourcing}

**Asset Sourcing** is configured from within the AEM Assets author instance. The administrators can enable the Asset Sourcing feature flag configuration from the **AEM Web Console Configuration** and upload the active Brand Portal users list in **AEM Assets**.

>[!NOTE]
>
>Asset Sourcing is by default enabled on AEM Assets as a Cloud Service. The AEM administrator can directly upload the active Brand Portal users to allow them access to the Asset Sourcing feature.

>[!NOTE]
>
>Before you begin with the configuration, ensure that your AEM Assets instance is configured with Brand Portal. See, [Configure AEM Assets with Brand Portal](../using/configure-aem-assets-with-brand-portal.md). 

The following video demonstrates, how to configure Asset Sourcing on your AEM Assets author instance:

>[!VIDEO](https://video.tv.adobe.com/v/29771)
-->

<!--
### Enable Asset Sourcing {#enable-asset-sourcing}

AEM administrators can enable the Asset Sourcing feature flag from within the AEM Web Console Configuration (a.k.a Configuration Manager).

>[!NOTE]
>
>This step is not applicable for AEM Assets as a Cloud Service.


**To enable Asset Sourcing:**
1. Log in to your AEM Assets author instance and open Configuration Manager. 
Default URL: http:// localhost:4502/system/console/configMgr.
1. Search using the keyword **Asset Sourcing** to locate **[!UICONTROL Asset Sourcing Feature Flag Config]**.
1. Click **[!UICONTROL Asset Sourcing Feature Flag Config]** to open the configuration window.
1. Select the **[!UICONTROL feature.flag.active.status]** check box.
1. Click **[!UICONTROL Save]**.

![](assets/enable-asset-sourcing.png)
-->


### Chargement de la liste des utilisateurs de Brand Portal {#upload-bp-user-list}

Les administrateurs AEM peuvent charger le fichier de configuration des utilisateurs Brand Portal (.csv) contenant la principale liste des utilisateurs Brand Portal dans AEM Assets pour leur permettre d’accéder à la fonctionnalité d’approvisionnement des ressources.

Un dossier de contribution peut uniquement être partagé avec les utilisateurs actifs de Brand Portal définis dans la liste des utilisateurs. L’administrateur peut également ajouter de nouveaux utilisateurs dans le fichier de configuration et charger la liste modifiée des utilisateurs.

>[!NOTE]
>
>Vérifiez que votre instance d’AEM Assets est configurée avec Brand Portal. Voir [Configuration d’AEM Assets avec Brand Portal](../using/configure-aem-assets-with-brand-portal.md).

>[!NOTE]
>
>Ce format de fichier CSV est identique à celui pris en charge dans Admin Console pour importer des utilisateurs en bloc. Vous devez indiquer vos nom, prénom et adresse email.

Les administrateurs peuvent ajouter de nouveaux utilisateurs dans AEM Admin Console. Pour plus d’informations, voir [Gestion des utilisateurs](brand-portal-adding-users.md). Une fois des utilisateurs ajoutés dans Admin Console, ceux-ci peuvent être ajoutés au fichier de configuration des utilisateurs de Brand Portal, puis se voir attribuer l’autorisation d’accéder au dossier de contribution.

**Pour charger la liste des utilisateurs de Brand Portal, procédez comme suit :**
1. Connectez-vous à votre instance AEM Assets.
1. Dans le panneau **Outils**, accédez à **[!UICONTROL Ressources]** > **[!UICONTROL Utilisateurs Brand Portal]**.

1. La fenêtre de chargement des contributeurs de Brand Portal s’affiche.
Recherchez sur votre ordinateur local le **fichier de configuration (.csv)** contenant la liste des utilisateurs actifs de Brand Portal, puis chargez-le.
1. Cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/upload-user-list2.png)


Les administrateurs peuvent donner un accès à des utilisateurs spécifiques à partir de cette liste d’utilisateurs lors de la configuration d’un dossier de contribution. Seuls les utilisateurs affectés à un dossier de contribution auront accès au dossier de contribution et publieront des fichiers de Brand Portal vers AEM Assets.

## Voir également {#reference-articles}

* [Configuration et publication du dossier de contribution sur Brand Portal](brand-portal-publish-contribution-folder-to-brand-portal.md)

* [Publication du dossier de contribution sur AEM Assets](brand-portal-publish-contribution-folder-to-aem-assets.md)
