---
title: Configuration de l’origine des ressources
seo-title: Configuration de l’origine des ressources
description: Découvrez comment configurer la fonctionnalité de source de ressources dans AEM Assets.
seo-description: Découvrez comment configurer la fonctionnalité de source de ressources dans AEM Assets.
uuid: null
content-type: reference
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: add4009bd99e5af8ed0c9ffea63647c166b7c75d

---


# Configuration de l’origine des ressources {#configure-asset-sourcing}

Les administrateurs d’AEM peuvent configurer **l’approvisionnement** des ressources à partir de l’instance d’auteur AEM. L’administrateur active la configuration de l’indicateur de fonctionnalité Sources de ressources à partir de la configuration **de la console Web** AEM et télécharge la liste des utilisateurs actifs du portail de marque dans **AEM Assets**.

>[!NOTE]
>
>Avant de commencer la configuration, assurez-vous que votre instance AEM Assets est intégrée à Brand Portal. See, [Configure AEM Assets integration with Brand Portal](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html).


La vidéo suivante explique comment configurer l’approvisionnement en ressources sur votre instance d’auteur AEM :

>[!VIDEO](https://video.tv.adobe.com/v/29771?captions=fre_fr)

## Activation de l’approvisionnement des ressources {#enable-asset-sourcing}

Les administrateurs d’AEM peuvent activer l’approvisionnement des ressources depuis Configuration de la console web AEM (ou Configuration Manager).

**Pour activer l’approvisionnement des ressources, procédez comme suit :**
1. Connectez-vous à votre instance d’auteur AEM et ouvrez Configuration Manager.
URL par défaut : http:// localhost:4502/system/console/configMgr
1. À l’aide du mot-clé **Approvisionnement des ressources**, recherchez la **[!UICONTROL configuration de l’indicateur de la fonctionnalité d’approvisionnement des ressources]**.
1. Cliquez sur **[!UICONTROL Configuration de l’indicateur de la fonctionnalité d’approvisionnement des ressources]** pour ouvrir la fenêtre de configuration.
1. Activez la case à cocher **[!UICONTROL feature.flag.active.status]**.
1. Cliquez sur **[!UICONTROL Enregistrer]**.

![](assets/enable-asset-sourcing.png)

## Chargement de la liste des utilisateurs de Brand Portal {#upload-bp-user-list}

Les administrateurs d’AEM peuvent charger le fichier de configuration des utilisateurs de Brand Portal (.csv) contenant la liste des utilisateurs Brand Portal actifs dans AEM Assets. Un dossier de contribution peut uniquement être partagé avec les utilisateurs actifs de Brand Portal définis dans la liste des utilisateurs. L’administrateur peut également ajouter de nouveaux utilisateurs dans le fichier de configuration et charger la liste modifiée des utilisateurs.

Il peut ajouter de nouveaux utilisateurs dans AEM Admin Console. Pour plus d’informations, voir [Gestion des utilisateurs](brand-portal-adding-users.md). Une fois des utilisateurs ajoutés dans Admin Console, ceux-ci peuvent être ajoutés au fichier de configuration des utilisateurs de Brand Portal, puis se voir attribuer l’autorisation d’accéder au dossier de contribution.

**Pour charger la liste des utilisateurs de Brand Portal, procédez comme suit :**
1. Connectez-vous à votre instance d’auteur AEM
URL par défaut : http:// localhost:4502/aem/start.html
1. Dans le panneau **Outils** ![](assets/tools.png), accédez à **[!UICONTROL Ressources &gt; Utilisateurs Brand Portal]**.
   ![](assets/upload-user-list1.png)
1. La fenêtre de chargement des contributeurs de Brand Portal s’affiche.
Recherchez sur votre ordinateur local le **fichier de configuration (.csv)** contenant la liste des utilisateurs actifs de Brand Portal, puis chargez-le.
1. Cliquez sur **[!UICONTROL Enregistrer]**.
   ![](assets/upload-user-list2.png)


Les administrateurs peuvent donner un accès à des utilisateurs/groupes spécifiques à partir de cette liste d’utilisateurs lors de la configuration du dossier de contribution.

Pour plus d’informations, voir [Configuration du dossier de contribution](brand-portal-contribution-folder.md).
