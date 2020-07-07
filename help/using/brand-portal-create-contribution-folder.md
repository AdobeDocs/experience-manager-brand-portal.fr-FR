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
source-git-commit: b41f86824afd5be043c7b91035b01b71fdb69a26
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 79%

---


# Création d’un dossier de contribution {#create-contribution-folder}

Les administrateurs AEM et les non-administrateurs autorisés à créer un dossier peuvent créer un dossier **Contribution** dans AEM Assets.

Pour créer un dossier **Contribution**, créez un dossier de type **Contribution des ressources**, en vous assurant qu’il accepte l’envoi de ressources de la part des utilisateurs de Brand Portal.  Cela déclenche automatiquement un workflow qui crée deux sous-dossiers supplémentaires, appelés **SHARED** et **NEW**, dans le dossier **Contribution** nouvellement créé. 

**Pour créer un dossier de contribution, procédez comme suit :**
1. Connectez-vous à votre instance d’auteur AEM
URL par défaut : http://localhost:4502/aem/start.html
1. Accédez à **[!UICONTROL Ressources > Fichiers]**. Tous les dossiers existants dans le référentiel AEM Assets sont répertoriés.
1. Cliquez sur **[!UICONTROL Créer]** pour créer un dossier. La fenêtre contextuelle Créer un dossier s’ouvre.
1. Saisissez le **[!UICONTROL Titre]** et le **[!UICONTROL Nom]** du dossier et cochez la case **[!UICONTROL Contribution des ressources]**.
Il est recommandé d’utiliser dans le nom du dossier des lettres minuscules sans espace.
1. Cliquez sur **[!UICONTROL Créer]**.
   ![](assets/create-contribution-folder.png)
1. Le dossier de contribution nouvellement créé est répertorié dans le référentiel AEM Assets.
1. Cliquez pour ouvrir le dossier de contribution. Vous pouvez voir deux sous-dossiers, **[!UICONTROL SHARED]** et **[!UICONTROL NEW]**, automatiquement créés dans le dossier de contribution.\
   ![](assets/contribution-folder.png)

Vous pouvez désormais configurer les propriétés du dossier Contribution. Voir [Configuration des propriétés du dossier de contribution](brand-portal-configure-contribution-folder-properties.md).

>[!NOTE]
>
>Un utilisateur non administrateur peut uniquement créer et partager un dossier de contributions de ressources. Une fois le dossier de contribution créé, un utilisateur non administrateur ne peut pas le modifier ni le supprimer.
>
>L’imbrication du dossier de contribution des ressources n’est pas prise en charge. Vous pouvez créer plusieurs dossiers de contribution dans un dossier, mais vous ne devez pas créer de dossier de contribution dans un autre dossier de contribution.
