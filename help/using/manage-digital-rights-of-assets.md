---
title: Gestion des droits numériques des ressources
seo-title: Gestion des droits numériques des ressources
description: L’octroi de licences pour les ressources ainsi que la définition de l’expiration des ressources et des liens partagés assurent une utilisation contrôlée de ces ressources et les préservent.
seo-description: L’octroi de licences pour les ressources ainsi que la définition de l’expiration des ressources et des liens partagés assurent une utilisation contrôlée de ces ressources et les préservent.
uuid: ce 30 e 398-0109-41 bf-a 4 d 2-2 fcca 476 f 499
contentOwner: bdhar
topic-tags: téléchargement-install
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
content-type: référence
discoiquuid: f 77003 ba -31 fe -4 a 9 e -96 c 8-dbc 4 c 2 eba 79 e
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Gestion des droits numériques des ressources {#manage-digital-rights-of-assets}

La sécurisation de la distribution et de l’utilisation des ressources créatives et des documents de marque est essentielle pour protéger votre marque. Elle peut être appliquée à l'échelle de l'organisation et à l'extérieur en associant une date d'expiration (et une heure) aux ressources approuvées publiées depuis AEM vers Brand Portal ou en les autorisant à utiliser des licences à usage conditionnel. En outre, Brand Portal vous permet de spécifier une date d’expiration pour les liens vers les ressources partagées à partir de Brand Portal.

Poursuivez la lecture de cet article pour savoir comment les ressources sont sécurisées sur Brand Portal et comprendre les autorisations d’utilisation associées.

## Expiration de ressources {#asset-expiration}

L’expiration de ressources est une façon efficace de contrôler l’utilisation des ressources approuvées sur Brand Portal à travers une organisation. Tous les actifs publiés à partir d'AEM Assets sur le portail de marque peuvent avoir une date d'expiration, ce qui limite l'utilisation de ces ressources par différents rôles d'utilisateur.

### Autorisations d’utilisation liées aux ressources expirées {#usage-permissions-expired-assets}

Dans Brand Portal, les administrateurs peuvent afficher, télécharger et ajouter des ressources expirées aux collections. En revanche, les éditeurs et les observateurs peuvent seulement afficher et ajouter des ressources expirées aux collections.

Les administrateurs peuvent publier les ressources expirées sur Brand Portal à partir d’AEM Assets. Cependant, les ressources expirées ne peuvent pas être partagées par l’intermédiaire d’un lien à partir de Brand Portal. If you select any expired asset from a folder containing both expired and non-expired assets, the **[!UICONTROL Share Link]** action is not available. Toutefois, si vous sélectionnez un dossier contenant des ressources expirées et non expirées, les actions [!UICONTROL Partager] et **[!UICONTROL Partager le lien]** sont disponibles.

>[!NOTE]
>
>Un dossier peut toujours être partagé sous forme de lien, même s'il contient des ressources expirées. Dans ce cas, le lien ne répertorie pas les ressources expirées et seuls les fichiers non expirés sont partagés.

Le tableau suivant montre les autorisations d’utilisation des ressources expirées :

|  | **[!UICONTROL Partager le lien]** | **[!UICONTROL Téléchargement]** | **[!UICONTROL Propriétés]** | **[!UICONTROL Ajouter à la collection]** | **[!UICONTROL Supprimer]** |
|---|---|---|---|---|---|
| **[!UICONTROL Administrateur]** | Non disponible | Disponible | Disponible | Disponible | Disponible |
| **[!UICONTROL Éditeur]** | Non disponible | Non disponible | Disponible | Disponible | Non disponible |
| **[!UICONTROL Observateur]** | Non disponible | Non disponible | Disponible | Disponible | Non disponible |
| **[!UICONTROL Utilisateur invité]** | Non disponible | Non disponible | Disponible | Disponible | Non disponible |

>[!NOTE]
>
>Si les lecteurs et les éditeurs téléchargent un dossier contenant des fichiers expirés et non expirés, seuls les fichiers non expirés sont téléchargés. Si un dossier contient seulement des ressources expirées, un dossier vide est téléchargé.

### État d’expiration des ressources {#expiration-status-of-assets}

You can view the expiration status of assets in their [!UICONTROL Card View]. Un drapeau rouge sur la carte indique que la ressource a expiré.

![](assets/expired_assets_cardview.png)

>[!NOTE]
>
>Les modes Liste et Colonnes n’indiquent pas l’état d’expiration des ressources.

## Expiration des liens de ressources {#asset-link-expiration}

While sharing assets through links, Administrators and Editors can set a date and time of expiration using the **[!UICONTROL Expiration]** field in the **[!UICONTROL Link Sharing]** dialog box. L'expiration par défaut du lien est de sept jours à compter de la date de partage du lien.

![](assets/asset-link-sharing.png)

Cela assure que des ressources partagées via des liens expirent aux date et heure définies par les administrateurs et les éditeurs Brand Portal, et qu’elles ne peuvent plus être affichées ni téléchargées au-delà de la date d’expiration. Comme les ressources partagées via des liens peuvent également être visualisées par des utilisateurs externes qui ne font pas partie de l'organisation, en spécifiant l'expiration, vous pouvez vous assurer que les ressources approuvées sont protégées et non exposées à des entités inconnues au-delà d'une heure spécifiée.

For more information about link sharing, refer to [Share assets as a link](../using/brand-portal-link-share.md).

## Ressources sous licence {#licensed-assets}

Les ressources sous licence sont sujettes à l’acceptation d’un accord de licence avant leur téléchargement à partir de Brand Portal. Cet accord pour les ressources sous licence s’affiche quand vous téléchargez directement des ressources à partir de Brand Portal ou par l’intermédiaire d’un lien partagé. Qu’elles soient ou non expirées, les ressources protégées par une licence peuvent être affichées par tous les utilisateurs. Cependant, le téléchargement et l’utilisation des ressources sous licence expirées sont limités. Pour connaître le comportement des ressources sous licence expirées et des activités permises en fonction des rôles d’utilisateur, voir [Autorisations d’utilisation des ressources expirées](../using/manage-digital-rights-of-assets.md#usage-permissions-expired-assets).

License-protected assets have [license agreement attached](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) to them, which is done by setting asset's [metadata property](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) in AEM Assets.

If you choose to download license-protected asset(s), you are redirected to [!UICONTROL Copyright Management] page.

![](assets/asset-copyright-mgmt.png)

Vous devez y sélectionner la ressource à télécharger et accepter l’accord de licence associé. If you do not accept the license agreement, the [!UICONTROL Download] button is not enabled.

![](assets/licensed-asset-download-2.png)

Si la sélection contient plusieurs ressources protégées, sélectionnez-en une à la fois, acceptez le contrat de licence et procédez au téléchargement de la ressource.

## Génération d’un rapport sur les ressources expirées {#generate-report-about-expired-assets}

Les administrateurs peuvent générer et télécharger un rapport répertoriant toutes les ressources expirées dans une période spécifique. Ce rapport contient des informations détaillées, telles que la taille, le type, le chemin spécifiant l'emplacement de la ressource dans la hiérarchie des ressources, quand la ressource a expiré, et quand la ressource a été publiée— à propos des ressources expirées. Les colonnes de ce rapport peuvent être personnalisées pour afficher plus de données selon les besoins des utilisateurs.

![](assets/assets-expired.png)

For more information about the reports feature, refer [Work with reports](../using/brand-portal-reports.md#work-with-reports).
