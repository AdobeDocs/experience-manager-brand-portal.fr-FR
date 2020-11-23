---
title: Configuration des propriétés du dossier de contribution
seo-title: Configuration des propriétés du dossier de contribution
description: 'Découvrez comment configurer les propriétés d’un dossier de contribution dans AEM Assets. '
seo-description: 'Découvrez comment configurer les propriétés d’un dossier de contribution dans AEM Assets. '
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
version: 6.5
discoiquuid: null
translation-type: tm+mt
source-git-commit: c8f859fd371f303a8424ed473927812f658d2b8e
workflow-type: tm+mt
source-wordcount: '316'
ht-degree: 83%

---


# Configuration des propriétés du dossier de contribution {#configure-contribution-folder-properties}

L’administrateur d’AEM effectue les activités ci-après lors de la configuration des propriétés d’un dossier de contribution.

* **Ajouter une description** : fournissez une description détaillée du dossier de contribution.
* **Charger les instructions** : téléchargez le document sur les exigences en matière de ressources contenant des informations relatives aux ressources.
* **Ajouter les contributeurs**: Ajoutez les utilisateurs du portail de marque à leur accorder l’accès au dossier de contribution.

Les exigences en matière de ressources font référence aux détails fournis par les administrateurs pour aider les contributeurs (utilisateurs de Brand Portal) à comprendre le besoin et les exigences du dossier de contribution. L’administrateur charge un document sur les exigences en matière de ressources contenant un résumé sur le type de ressources à ajouter au dossier de contribution et des informations relatives aux ressources comme le but, le type d’images, la taille maximale, etc.

L’administrateur peut ensuite accorder aux utilisateurs du portail de marque l’accès au dossier de contributions avant de publier le dossier de contributions nouvellement créé sur le portail de marques.

**Pour configurer les propriétés du dossier de contribution, procédez comme suit :**

1. Connectez-vous à votre instance d’auteur AEM
URL par défaut : http://localhost:4502/aem/start.html
1. Accédez à **[!UICONTROL Ressources > Fichiers]** et localisez le dossier de contribution.
1. Sélectionnez le dossier de contribution et cliquez sur **[!UICONTROL Propriétés]** ![](assets/properties.png). La fenêtre Propriétés du dossier s’affiche.
   ![](assets/contribution-folder-property1.png)
1. Accédez à l’onglet **[!UICONTROL Contribution des ressources]**.
1. Saisissez une **[!UICONTROL Description]** détaillée du dossier de contribution.
1. Cliquez sur **[!UICONTROL Upload Brief]** ![](assets/upload.png) (Charger un résumé) pour parcourir votre ordinateur local et charger un **document relatif aux exigences en matière de ressources**.
1. Dans le champ **[!UICONTROL Ajouter un utilisateur ou un groupe]**, ajoutez les utilisateurs de Brand Portal avec lesquels vous souhaitez partager le dossier de contribution. Ces utilisateurs peuvent accéder au dossier de contributions et le télécharger à l’aide de l’interface du portail de marque.
1. Cliquez sur **[!UICONTROL Save]**.

![](assets/contribution-folder-property2.png)

>[!NOTE]
>
>Actuellement, vous ne pouvez pas ajouter de groupes à un dossier de contribution.
>
>Les résultats de la recherche sont basés sur la liste des utilisateurs Brand Portal configurée dans AEM Assets. Vérifiez que vous disposez de la liste mise à jour des utilisateurs de Brand Portal. Voir [Chargement de la liste des utilisateurs de Brand Portal](brand-portal-configure-asset-sourcing.md).
