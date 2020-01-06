---
title: Création d’un dossier de contribution
seo-title: Création d’un dossier de contribution
description: 'Découvrez comment créer un dossier de contribution dans AEM Assets. '
seo-description: Découvrez comment créer un dossier de contribution dans AEM Assets.
uuid: null
content-type: reference
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: 22b327619eb73c0099f903bb7314d2cb2d796bc4

---


# Création d’un dossier de contribution {#create-contribution-folder}

Les administrateurs AEM et les utilisateurs non administrateurs autorisés à créer un dossier peuvent créer un dossier **de contribution** dans les ressources AEM.
Pour créer un dossier **de contribution** , créez un nouveau dossier de type Contribution **** du fichier, en vous assurant que le nouveau dossier créé est ouvert à l’envoi des fichiers par les utilisateurs du portail de marque.  Cela déclenche automatiquement un workflow qui crée deux sous-dossiers supplémentaires, appelés **SHARED** et **NEW**, dans le dossier **Contribution** nouvellement créé. 

**Pour créer un dossier de contribution, procédez comme suit :**
1. Connectez-vous à votre instance d’auteur AEM
URL par défaut : http:// localhost:4502/aem/start.html
1. Accédez à **[!UICONTROL Ressources > Fichiers]**. Tous les dossiers existants dans le référentiel AEM Assets sont répertoriés.
1. Cliquez sur **[!UICONTROL Créer]**pour créer un dossier. La fenêtre contextuelle Créer un dossier s’ouvre.
1. Saisissez le **[!UICONTROL Titre]**et le**[!UICONTROL  Nom]** du dossier et cochez la case **[!UICONTROL Contribution des ressources]**.
Il est recommandé d’utiliser dans le nom du dossier des lettres minuscules sans espace.
1. Cliquez sur **[!UICONTROL Créer]**.   ![](assets/create-contribution-folder.png)
1. Le dossier de contribution nouvellement créé est répertorié dans le référentiel AEM Assets.
1. Cliquez pour ouvrir le dossier de contribution. Vous pouvez voir deux sous-dossiers, **[!UICONTROL SHARED]**et**[!UICONTROL  NEW]**, automatiquement créés dans le dossier de contribution.\
   ![](assets/contribution-folder.png)

Vous pouvez désormais configurer les propriétés du dossier de contributions. Voir [Configuration des propriétés du dossier de contribution](brand-portal-configure-contribution-folder-properties.md).

>[!NOTE]
>
>Veillez à attribuer un nom approprié au dossier Contribution, car vous ne pouvez pas modifier le nom du dossier après sa création.