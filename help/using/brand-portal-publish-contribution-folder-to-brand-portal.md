---
title: 'Configuration et publication du dossier de contribution d’AEM Assets à Brand Portal '
seo-title: Configuration et publication du dossier de contribution d’AEM Assets à Brand Portal
description: Découvrez comment configurer et publier un dossier de contributions d'AEM Assets vers Brand Portal.
seo-description: Découvrez comment configurer et publier un dossier de contributions d'AEM Assets vers Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: 4221199d874ce63a936e5e6e02a16ee95cab4499
workflow-type: tm+mt
source-wordcount: '1113'
ht-degree: 80%

---


# Configurer le dossier de contribution en AEM Assets {#configure-contribution-folder}

Dans le cas de l’approvisionnement collaboratif des ressources, les utilisateurs d’AEM (administrateurs et non-administrateurs autorisés) peuvent créer des dossiers de type **Contribution des ressources**, en s’assurant qu’ils acceptent l’envoi de ressources de la part des utilisateurs de Brand Portal. Cela déclenche automatiquement un workflow qui crée deux sous-dossiers supplémentaires, appelés **SHARED** et **NEW**, dans le dossier **Contribution** nouvellement créé. 

L’utilisateur d’AEM définit ensuite les exigences en chargeant un résumé relatif aux types de ressources à ajouter au dossier de contribution, ainsi qu’un ensemble de ressources de base, dans le dossier **SHARED**, afin de s’assurer que les utilisateurs de Brand Portal disposent des informations de référence dont ils ont besoin. L’administrateur peut alors octroyer aux utilisateurs actifs de Brand Portal l’accès au dossier de contribution avant de publier le nouveau dossier Contribution sur Brand Portal.

La vidéo suivante explique comment configurer un dossier Contribution dans AEM Assets :

>[!VIDEO](https://video.tv.adobe.com/v/30547)

L’utilisateur d’AEM effectue les activités suivantes lors de la configuration d’un dossier de contribution :

* [Création d’un dossier de contribution](#create-contribution-folder)
* [Télécharger les besoins en ressources et affecter des contributeurs](#configure-contribution-folder-properties)
* [Chargement de ressources de base](#uplad-new-assets-to-contribution-folder)
* [Publier le dossier de contribution d’AEM Assets vers le portail des marques](#publish-contribution-folder-to-brand-portal)

## Création d’un dossier de contribution {#create-contribution-folder}


Les administrateurs AEM et les utilisateurs non-administrateurs autorisés à créer un dossier peuvent créer un dossier Contribution dans AEM Assets.
Pour créer un dossier Contribution, créez un nouveau dossier de type Contribution des ressources, en vous assurant qu’il accepte l’envoi de ressources de la part des utilisateurs de Brand Portal.  Cela déclenche automatiquement un workflow qui crée deux sous-dossiers supplémentaires, SHARED et NEW, dans le dossier Contribution.

>[!NOTE]
>
>Vous pouvez créer plusieurs dossiers de contribution dans un dossier. Ne créez pas de dossier de contribution dans un autre dossier de contribution.

**Pour créer un dossier de contribution, procédez comme suit :**
1. Connectez-vous à votre instance AEM Assets.

1. Accédez à **[!UICONTROL Ressources]** > **[!UICONTROL Fichiers]**. Tous les dossiers existants dans le référentiel AEM Assets sont répertoriés.

1. Cliquez sur **[!UICONTROL Créer]** pour créer un dossier. La boîte de dialogue **[!UICONTROL Créer un dossier]** apparaît.

1. Spécifiez le **[!UICONTROL Titre]** et le **[!UICONTROL Nom]** du dossier et cochez la case **[!UICONTROL Contribution des ressources]**.
Il est recommandé d’utiliser dans le nom du dossier des lettres minuscules sans espace.

1. Cliquez sur **[!UICONTROL Créer]**. Le dossier de contribution est répertorié dans le référentiel AEM Assets.

   >[!NOTE]
   >
   >Un utilisateur non-administrateur peut créer et partager un dossier de contribution de ressources, mais il ne peut ni le modifier ni le supprimer.


   ![](assets/create-contribution-folder.png)

1. Cliquez pour ouvrir le dossier de contribution. Vous pouvez voir deux sous-dossiers, **[!UICONTROL SHARED]** et **[!UICONTROL NEW]**, automatiquement créés dans le dossier de contribution.

   ![](assets/contribution-folder.png)

Vous pouvez également configurer les propriétés du dossier de contributions lors de la création du dossier de contributions.

## Configuration des propriétés du dossier de contribution {#configure-contribution-folder-properties}

L’administrateur d’AEM effectue les activités ci-après lors de la configuration des propriétés d’un dossier de contribution.

* **Ajouter une description** : fournissez une description détaillée du dossier de contribution.
* **Charger les instructions** : téléchargez le document sur les exigences en matière de ressources contenant des informations relatives aux ressources.
* **Ajouter les contributeurs** : Ajoutez les utilisateurs du portail de marque à leur accorder l’accès au dossier de contribution.

Les exigences en matière de ressources font référence aux détails fournis par les administrateurs pour aider les contributeurs (utilisateurs de Brand Portal) à comprendre le besoin et les exigences du dossier de contribution. L’administrateur charge un document sur les exigences en matière de ressources contenant un résumé sur le type de ressources à ajouter au dossier de contribution et des informations relatives aux ressources comme le but, le type d’images, la taille maximale, etc.

**Pour configurer les propriétés du dossier de contribution, procédez comme suit :**

1. Connectez-vous à votre instance AEM Assets.

1. Accédez à **[!UICONTROL Ressources > Fichiers]** et localisez le dossier de contribution.
1. Sélectionnez le dossier de contribution et cliquez sur **[!UICONTROL Propriétés]** pour ouvrir la fenêtre Propriétés du dossier.

   ![](assets/properties.png)

   ![](assets/contribution-folder-property1.png)

1. Accédez à l’onglet **[!UICONTROL Contribution des ressources]**.
1. Saisissez une **[!UICONTROL Description]** détaillée du dossier de contribution.
1. Cliquez sur **[!UICONTROL Upload Brief]**  (Charger un résumé) pour parcourir votre ordinateur local et charger un **document relatif aux exigences en matière de ressources**.

   ![](assets/upload.png)

1. Dans le champ **[!UICONTROL Ajouter l’utilisateur]**, ajoutez les utilisateurs du portail de marque avec lesquels vous souhaitez partager le dossier de contribution. Ces utilisateurs peuvent accéder au dossier de contributions et le télécharger à l’aide de l’interface du portail de marque.
1. Cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/contribution-folder-property3.png)

>[!NOTE]
>
>Les résultats de la recherche sont basés sur la liste des utilisateurs Brand Portal configurée dans AEM Assets. Vérifiez que vous disposez de la liste mise à jour des utilisateurs de Brand Portal.

## Chargement de ressources dans le dossier de contribution {#uplad-new-assets-to-contribution-folder}

Les utilisateurs de Brand Portal peuvent télécharger les exigences en matière de ressources pour comprendre le besoin en termes de contribution.
Ils peuvent alors créer des ressources à des fins de contribution et les charger dans le dossier NEW au sein du dossier de contribution.

>[!NOTE]
>
>Les utilisateurs de Brand Portal peuvent charger des ressources uniquement vers le dossier NEW.
>
>La limite de chargement maximale pour tout client Brand Portal est de **10** Go ; elle est appliquée de manière cumulative à tous les dossiers de contribution.


Après avoir publié les ressources nouvellement créées dans AEM Assets, les utilisateurs de Brand Portal peuvent les supprimer du dossier NEW. En revanche, l’administrateur de Brand Portal peut supprimer les ressources des dossiers NEW et SHARED.

Une fois l’objectif de création du dossier de contribution atteint, l’administrateur de Brand Portal peut le supprimer afin de libérer l’espace de chargement pour d’autres utilisateurs.

>[!NOTE]
>
>Il est recommandé de libérer l’espace de chargement après avoir publié le dossier de contribution dans AEM Assets afin qu’il soit accessible aux autres utilisateurs de Brand Portal pour les contributions.
>
>S’il est nécessaire d’étendre la limite de chargement de votre client Brand Portal au-delà de **10** Go, contactez l’assistance Adobe en spécifiant la limite requise.


**Pour charger de nouvelles ressources :**

1. Connectez-vous à votre instance Brand Portal.
Le tableau de bord de Brand Portal répertorie tous les dossiers existants auxquels l’utilisateur de Brand Portal est autorisé à accéder, ainsi que le dossier de contribution nouvellement partagé.

1. Sélectionnez le dossier de contribution et cliquez dessus pour l’ouvrir. Le dossier de contribution contient deux sous-dossiers : **[!UICONTROL SHARED]** (PARTAGÉ) et **[!UICONTROL NEW]** (NOUVEAU).

1. Cliquez sur le dossier **[!UICONTROL NEW]**.

   ![](assets/upload-new-assets1.png)

1. Cliquez sur **[!UICONTROL Créer]** > **[!UICONTROL Fichiers]** afin de charger des fichiers distincts ou un dossier (.zip) contenant plusieurs ressources.

   ![](assets/upload-new-assets2.png)

1. Parcourez les ressources (fichiers/dossiers) et chargez-les dans le dossier **[!UICONTROL NEW]**.

   ![](assets/upload-new-assets3.png)

Après avoir chargé tous les fichiers ou dossiers dans le dossier NEW, publiez le dossier de contribution dans AEM Assets.


## Publication du dossier de contribution sur Brand Portal {#publish-contribution-folder-to-brand-portal}

Une fois le dossier de contribution configuré, l’utilisateur d’AEM (administrateur/non-administrateur) peut le publier d’AEM Assets sur Brand Portal. Les utilisateurs du portail de marque autorisés à accéder au dossier de contribution recevront une notification par courrier électronique ou par pulsation à la fin de l’action de publication.


**Pour publier le dossier de contribution, procédez comme suit :**

1. Connectez-vous à votre instance AEM Assets.

1. Accédez à **[!UICONTROL Ressources > Fichiers]** et localisez le dossier de contribution dans lequel vous souhaitez publier du contenu sur Brand Portal.
1. Sélectionnez le dossier de contribution et cliquez sur **[!UICONTROL Publication rapide]** > **[!UICONTROL Publier sur le portail de marque]**.

   ![](assets/publish-contribution-folder-to-bp.png)

   Vous recevrez un message de réussite une fois que le dossier de contribution sera publié sur Brand Portal.

Une notification Push/par courrier électronique est envoyée aux utilisateurs de Brand Portal affectés au dossier de contribution. Les utilisateurs de Brand Portal peuvent accéder au dossier de contribution et commencer la contribution. Voir [Télécharger des ressources vers le dossier de contributions et publier vers AEM Assets](brand-portal-publish-contribution-folder-to-aem-assets.md).
