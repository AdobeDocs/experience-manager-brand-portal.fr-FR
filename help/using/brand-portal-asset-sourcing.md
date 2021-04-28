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
translation-type: ht
source-git-commit: e8bb1149582329f5304bda7e5e67e8dcc27cfc7b
workflow-type: ht
source-wordcount: '841'
ht-degree: 100%

---

# Présentation de l’approvisionnement des ressources {#overview-asset-sourcing-in-bp}

L’**approvisionnement des ressources** permet aux utilisateurs d’AEM (administrateurs/non-administrateurs) de créer des dossiers avec une propriété **Contribution des ressources** supplémentaire, en s’assurant que les nouveaux dossiers s’ouvrent lorsque des utilisateurs de Brand Portal envoient des ressources. Cela déclenche automatiquement un workflow qui crée deux sous-dossiers supplémentaires, appelés **SHARED** et **NEW**, dans le dossier **Contribution** nouvellement créé. L’administrateur d’AEM définit ensuite les exigences en chargeant un résumé relatif aux types de ressources à ajouter au dossier de contribution, ainsi qu’un ensemble de ressources de base, dans le dossier **SHARED**, afin de s’assurer que les utilisateurs de Brand Portal disposent des informations de référence dont ils ont besoin. L’administrateur peut alors octroyer aux utilisateurs actifs de Brand Portal l’accès au dossier de contribution avant de publier le nouveau dossier **Contribution** sur Brand Portal. Dès que l’utilisateur a fini d’ajouter du contenu dans le dossier **NEW**, il peut republier le dossier de contribution dans l’environnement d’auteur AEM. Notez que l’importation du nouveau contenu publié dans AEM Assets et la prise en compte de cette opération peuvent prendre quelques minutes.

En outre, toutes les fonctionnalités existantes restent inchangées. Les utilisateurs de Brand Portal peuvent afficher, rechercher et télécharger des ressources à partir du dossier de contribution, ainsi que des autres dossiers autorisés. Quant aux administrateurs, ils peuvent partager le dossier de contribution de manière plus avancée, modifier les propriétés et ajouter des ressources aux collections.

## Conditions préalables {#prerequisites}

* AEM Assets as a Cloud Service, AEM Assets 6.5.2 ou version ultérieure.
* Vérifiez que votre instance d’AEM Assets est configurée avec Brand Portal. Voir [Configuration d’AEM Assets avec Brand Portal](../using/configure-aem-assets-with-brand-portal.md).
* Assurez-vous que votre client Brand Portal est configuré avec une instance d’auteur AEM Assets.

>[!VIDEO](https://video.tv.adobe.com/v/29365/?quality=12)

![Approvisionnement des ressources dans Brand Portal](assets/asset-sourcing.png)


>[!NOTE]
>
>Il existe un problème connu dans AEM Assets 6.5.4. Les utilisateurs de Brand Portal ne peuvent pas publier les ressources du dossier de contribution dans AEM Assets lors de la mise à niveau vers Adobe Developer Console.
>
>Le problème a été corrigé dans AEM 6.5.5. Vous pouvez mettre à niveau votre instance AEM Assets vers le Service Pack le plus récent, AEM 6.5.5, et [mettre à niveau vos configurations](https://docs.adobe.com/content/help/fr-FR/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) sur Adobe Developer Console.
>
>Pour une solution immédiate sur AEM 6.5.4, il est recommandé de [télécharger le correctif](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) et de l’installer sur votre instance d’auteur.

## Configuration de l’approvisionnement des ressources {#configure-asset-sourcing}

L’**approvisionnement des ressources** est configuré à partir de l’instance d’auteur AEM Assets. Les administrateurs peuvent activer la configuration de l’indicateur de la fonctionnalité d’approvisionnement des ressources depuis la **configuration de la console web AEM** et charger la liste des utilisateurs Brand Portal actifs dans **AEM Assets**.

>[!NOTE]
>
>L’approvisionnement des ressources est activé par défaut dans AEM Assets as a Cloud Service. L’administrateur AEM peut directement charger les utilisateurs actifs de Brand Portal pour leur permettre d’accéder à la fonction d’approvisionnement des ressources.

>[!NOTE]
>
>Veillez à configurer l’instance d’AEM Assets à Brand Portal avant de commencer la configuration. Voir [Configuration d’AEM Assets avec Brand Portal](../using/configure-aem-assets-with-brand-portal.md).

La vidéo suivante explique comment configurer l’approvisionnement des ressources sur l’instance d’auteur AEM Assets :

>[!VIDEO](https://video.tv.adobe.com/v/29771)

### Activation de l’approvisionnement des ressources {#enable-asset-sourcing}

Les administrateurs d’AEM peuvent activer l’indicateur d’approvisionnement des ressources depuis Configuration de la console web AEM (ou Configuration Manager).

>[!NOTE]
>
>Cette étape ne s’applique pas à AEM Assets as a Cloud Service.


**Pour activer l’approvisionnement des ressources, procédez comme suit :**
1. Connectez-vous à votre instance d’auteur AEM Assets et ouvrez Configuration Manager.
URL par défaut : http:// localhost:4502/system/console/configMgr.
1. À l’aide du mot-clé **Asset Sourcing** (Approvisionnement des ressources), recherchez la **[!UICONTROL Asset Sourcing Feature Flag Config]** (Configuration de l’indicateur de la fonctionnalité d’approvisionnement des ressources).
1. Cliquez sur **[!UICONTROL Asset Sourcing Feature Flag Config]** (Configuration de l’indicateur de la fonctionnalité d’approvisionnement des ressources) pour ouvrir la fenêtre de configuration.
1. Cochez la case **[!UICONTROL feature.flag.active.status]**.
1. Cliquez sur **[!UICONTROL Enregistrer]**.

![](assets/enable-asset-sourcing.png)

### Chargement de la liste des utilisateurs de Brand Portal {#upload-bp-user-list}

Les administrateurs d’AEM peuvent charger le fichier de configuration des utilisateurs de Brand Portal (.csv) contenant la liste des utilisateurs Brand Portal actifs dans AEM Assets. Un dossier de contribution peut uniquement être partagé avec les utilisateurs actifs de Brand Portal définis dans la liste des utilisateurs. L’administrateur peut également ajouter de nouveaux utilisateurs dans le fichier de configuration et charger la liste modifiée des utilisateurs.

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
