---
title: Créer un dossier de contribution
seo-title: Créer un dossier de contribution
description: 'Découvrez comment créer un dossier de contributions dans AEM Assets. '
seo-description: Découvrez comment créer un dossier de contributions dans AEM Assets.
uuid: null
content-type: référencereference
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: 413a6bd17d689d0af0cce20bbd7dedb6ae3cf9b5

---


# Create contribution folder {#create-contribution-folder}

Les utilisateurs d’AEM (administrateurs/non-administrateurs) peuvent créer de nouveaux dossiers dans AEM Assets avec une propriété supplémentaire **Asset Contribution** , afin de s’assurer que le nouveau dossier créé est ouvert à l’envoi de fichiers par les utilisateurs du portail de marque.  Cela déclenche automatiquement un flux de travail qui crée deux sous-dossiers supplémentaires, appelés **PARTAGÉS** et **NOUVEAU**, dans le dossier de **contribution** nouvellement créé.

**Pour créer un dossier de contributions :**
1. Connectez-vous à votre instance d’auteur AEMURL par défaut : http:// localhost:4502/aem/start.html
1. Accédez à **[!UICONTROL Ressources &gt; Fichiers]** Il répertorie tous les dossiers existants dans le référentiel AEM Assets.
1. Click **[!UICONTROL Create]** to create a new folder. La fenêtre contextuelle Créer un dossier s’ouvre.
1. Saisissez le **[!UICONTROL Titre]** et le **[!UICONTROL Nom]** du dossier et cochez la case Contribution **[!UICONTROL du]**fichier.
Il est recommandé d’utiliser des petits alphabets sans espace pour nommer le dossier.
1. Cliquez sur **[!UICONTROL Créer]**.
   ![](assets/create-contribution-folder.png)
1. Vous pouvez afficher le dossier de contributions nouvellement créé dans le référentiel AEM Assets.
1. Cliquez sur pour ouvrir le dossier de contributions, vous pouvez voir deux sous-dossiers **[!UICONTROL PARTAGÉS]** et **[!UICONTROL NOUVEAU]** automatiquement créés dans le dossier de contributions.\
   ![](assets/contribution-folder.png)

Vous pouvez désormais configurer les propriétés du dossier de contributions nouvellement créé. Voir [Configuration des propriétés](brand-portal-configure-contribution-folder-properties.md)du dossier Contribution.