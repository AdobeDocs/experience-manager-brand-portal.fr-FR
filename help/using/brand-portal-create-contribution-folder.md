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
translation-type: ht
source-git-commit: 413a6bd17d689d0af0cce20bbd7dedb6ae3cf9b5

---


# Création d’un dossier de contribution {#create-contribution-folder}

Les utilisateurs d’AEM (administrateurs/non-administrateurs) peuvent créer des dossiers dans AEM Assets avec une propriété **Contribution des ressources** supplémentaire, en s’assurant que les nouveaux dossiers s’ouvrent lorsque des utilisateurs Brand Portal envoient des ressources. Cela déclenche automatiquement un workflow qui crée deux sous-dossiers supplémentaires, appelés **SHARED** et **NEW**, dans le dossier **Contribution** nouvellement créé. 

**Pour créer un dossier de contribution, procédez comme suit :**
1. Connectez-vous à votre instance d’auteur AEM
URL par défaut : http:// localhost:4502/aem/start.html
1. Accédez à **[!UICONTROL Ressources &gt; Fichiers]**. Tous les dossiers existants dans le référentiel AEM Assets sont répertoriés.
1. Cliquez sur **[!UICONTROL Créer]** pour créer un dossier. La fenêtre contextuelle Créer un dossier s’ouvre.
1. Saisissez le **[!UICONTROL Titre]** et le **[!UICONTROL Nom]** du dossier et cochez la case **[!UICONTROL Contribution des ressources]**.
Il est recommandé d’utiliser dans le nom du dossier des lettres minuscules sans espace.
1. Cliquez sur **[!UICONTROL Créer]**.
   ![](assets/create-contribution-folder.png)
1. Le dossier de contribution nouvellement créé est répertorié dans le référentiel AEM Assets.
1. Cliquez pour ouvrir le dossier de contribution. Vous pouvez voir deux sous-dossiers, **[!UICONTROL SHARED]** et **[!UICONTROL NEW]**, automatiquement créés dans le dossier de contribution.\
   ![](assets/contribution-folder.png)

Vous pouvez maintenant configurer les propriétés du dossier de contribution nouvellement créé. Voir [Configuration des propriétés du dossier de contribution](brand-portal-configure-contribution-folder-properties.md).