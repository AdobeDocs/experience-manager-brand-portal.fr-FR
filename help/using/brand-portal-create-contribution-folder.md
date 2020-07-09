---
title: Création d’un dossier de contribution
seo-title: Création d’un dossier de contribution
description: 'Découvrez comment créer un dossier de contribution dans AEM Assets. '
seo-description: Découvrez comment créer un dossier de contribution dans AEM Assets.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: 643514893d72dd34022a3b804daeca083eb67ad4
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 42%

---


# Création d’un dossier de contribution {#create-contribution-folder}


Les administrateurs AEM et les utilisateurs non administrateurs autorisés à créer un dossier peuvent créer un dossier de contribution en AEM Assets.
Pour créer un dossier de contribution, créez un nouveau dossier de type Contribution des ressources, en veillant à ce que le nouveau dossier créé soit ouvert à l’envoi des ressources par les utilisateurs du portail des marques.  Cela déclenche automatiquement un processus qui crée deux sous-dossiers supplémentaires, appelés SHARED et NEW, dans le dossier de contribution.

>[!NOTE]
>
>Vous pouvez créer plusieurs dossiers de contribution dans un dossier, mais pas dans un autre dossier de contribution.


Pour créer un dossier de contributions :
1. Connectez-vous à votre instance d’auteur AEM.

   L’URL par défaut est http:// localhost:4502/aem/start.html.

1. Navigate to **[!UICONTROL Assets]** > **[!UICONTROL Files]**. It lists all the existing folders in the AEM Assets repository.

1. Cliquez sur **[!UICONTROL Créer]** pour créer un dossier. **[!UICONTROL La boîte de dialogue Créer un dossier]** s’ouvre.

1. Enter **[!UICONTROL Title]** and **[!UICONTROL Name]** of the folder and enable the **[!UICONTROL Asset Contribution]** checkbox.
Il est recommandé d’utiliser des lettres minuscules sans espace pour nommer le dossier.

1. Cliquez sur **[!UICONTROL Créer]**. Le dossier de contribution nouvellement créé est répertorié dans le référentiel AEM Assets.

   >[!NOTE]
   >
   >Un utilisateur non administrateur peut créer et partager un dossier de contribution de ressources, mais il ne peut ni le modifier ni le supprimer.

   ![](assets/create-contribution-folder.png)

1. Cliquez pour ouvrir le dossier de contribution. Vous pouvez voir deux sous-dossiers, **[!UICONTROL SHARED]** et **[!UICONTROL NEW]**, automatiquement créés dans le dossier de contribution.

   ![](assets/contribution-folder.png)

You can now [configure the contribution folder properties](brand-portal-configure-contribution-folder-properties.md).


