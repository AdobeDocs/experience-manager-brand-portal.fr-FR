---
title: Configuration des propriétés du dossier Contribution
seo-title: Configuration des propriétés du dossier Contribution
description: 'Découvrez comment configurer les propriétés d’un dossier de contributions dans les ressources AEM. '
seo-description: 'Découvrez comment configurer les propriétés d’un dossier de contributions dans les ressources AEM. '
uuid: null
content-type: référencereference
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: a32de22b7d5ac2b53b31aab8675dfdac1f5a724c

---


# Configuration des propriétés du dossier de contributions {#configure-contribution-folder-properties}

L’administrateur AEM effectue les activités suivantes lors de la configuration des propriétés d’un dossier de contributions.

* **Ajouter une description**: Fournissez une description de haut niveau du dossier des contributions.
* **Brève** téléchargement :  Télécharger le document Asset Requirement contenant des informations relatives aux ressources.
* **Ajouter des contributeurs**: Ajoutez des utilisateurs ou des groupes du portail de marque pour leur accorder l’accès au dossier de contributions.

Les besoins en ressources se rapportent aux détails fournis par les administrateurs pour aider les contributeurs (utilisateurs du portail de marque) à comprendre le besoin et les exigences du dossier de contributions. L’administrateur télécharge un document sur les besoins en ressources qui contient une brève description du type de ressources à ajouter au dossier de contributions et des informations relatives aux ressources, par exemple, l’objectif, le type d’images, la taille maximale, etc.

L’administrateur peut alors accorder aux utilisateurs/groupes du portail de marque l’accès au dossier de contributions avant de publier le dossier de contributions nouvellement créé dans le portail de marque.

**Pour configurer les propriétés du dossier de contributions :**
1. Connectez-vous à votre instance d’auteur AEMURL par défaut : http:// localhost:4502/aem/start.html
1. Accédez à **[!UICONTROL Ressources &gt; Fichiers]** et localisez le dossier des contributions.
1. Sélectionnez le dossier des contributions et cliquez sur **[!UICONTROL Propriétés]** ![](assets/properties.png). La fenêtre Propriétés du dossier s’ouvre.
   ![](assets/contribution-folder-property1.png)
1. Accédez à l’onglet Contribution **** du fichier.
1. Saisissez une **[!UICONTROL description]** détaillée du dossier des contributions.
1. Cliquez sur **[!UICONTROL Télécharger un résumé]** pourparcourir votre ordinateur local et télécharger un document ![](assets/upload.png) **** de ressources requises.
1. Dans **[!UICONTROL Ajouter un utilisateur ou un groupe]**, recherchez et **[!UICONTROL ajoutez]** des utilisateurs ou des groupes du portail de marque avec lesquels partager le dossier de contributions.
Ces utilisateurs/groupes du portail de marque auront l’autorisation d’accéder au dossier de contributions et de télécharger du contenu depuis leur interface du portail de marque sans avoir besoin d’accéder à l’instance d’auteur AEM.
1. Cliquez sur **[!UICONTROL Enregistrer]**.
   ![](assets/contribution-folder-property2.png)

>[!NOTE]
>
>Les résultats de la recherche sont basés sur la liste des utilisateurs du portail de marque configurée dans AEM Assets. Vérifiez que vous disposez de la liste des utilisateurs du portail de marques mise à jour. Voir [Téléchargement de la liste des](brand-portal-upload-user-list.md)utilisateurs du portail de marque.