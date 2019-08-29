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
source-git-commit: 770c353b1143d879280df310012ce9d4d30b40c9

---


# Gestion des droits numériques des ressources {#manage-digital-rights-of-assets}

La sécurisation de la distribution et de l’utilisation des ressources créatives et des documents de marque est essentielle pour protéger votre marque. This can be enforced across the organization and outside by associating an expiration date (and time) with approved assets published from [!DNL AEM] to [!DNL Brand Portal], or by licensing these assets for conditional use. [!DNL Brand Portal] Vous pouvez également spécifier une date d'expiration pour les liens aux ressources partagées.[!DNL Brand Portal]

Read on to know how the assets are secured on [!DNL Brand Portal] and understand the associated usage permissions.

## Expiration de ressources {#asset-expiration}

L’expiration de ressources est une façon efficace de contrôler l’utilisation des ressources approuvées sur Brand Portal à travers une organisation. All the assets published from [!DNL AEM] Assets to Brand Portal can have an expiration date, which restricts the usage of these assets by different user roles.

### Autorisations d’utilisation liées aux ressources expirées {#usage-permissions-expired-assets}

In [!DNL Brand Portal], Administrators can view, download, and add expired assets to collections. En revanche, les éditeurs et les observateurs peuvent seulement afficher et ajouter des ressources expirées aux collections.

Administrators can publish expired assets from [!DNL AEM] Assets to [!DNL Brand Portal]. Cependant, les ressources expirées ne peuvent pas être partagées par l’intermédiaire d’un lien à partir de [!DNL Brand Portal]. If you select any expired asset from a folder containing both expired and non-expired assets, the **[!UICONTROL Share Link]** action is not available. Toutefois, si vous sélectionnez un dossier contenant des ressources expirées et non expirées, les actions [!UICONTROL Partager] et **[!UICONTROL Partager le lien]** sont disponibles.

>[!NOTE]
>
>Un dossier peut toujours être partagé sous forme de lien, même s'il contient des ressources expirées. Dans ce cas, le lien ne répertorie pas les ressources expirées et seuls les fichiers non expirés sont partagés.

Le tableau suivant montre les autorisations d’utilisation des ressources expirées :

|  | **Partager le lien** | **Téléchargement** | **Propriétés** | **Ajouter à la collection** | **Supprimer** |
|---|---|---|---|---|---|
| **Administrateur** | Non disponible | Disponible | Disponible | Disponible | Disponible |
| **Éditeur** | Non disponible | Non disponible | Disponible | Disponible | Non disponible |
| **Observateur** | Non disponible | Non disponible | Disponible | Disponible | Non disponible |
| **Utilisateur invité** | Non disponible | Non disponible | Disponible | Disponible | Non disponible |

>[!NOTE]
>
>Si les lecteurs et les éditeurs téléchargent un dossier contenant des fichiers expirés et non expirés, seuls les fichiers non expirés sont téléchargés. Si un dossier contient seulement des ressources expirées, un dossier vide est téléchargé.

### État d’expiration des ressources {#expiration-status-of-assets}

Vous pouvez voir l’état d’expiration des ressources dans leur mode Carte. Un drapeau rouge sur la carte indique que la ressource a expiré.

![](assets/expired_assets_cardview.png)

>[!NOTE]
>
>Les modes Liste et Colonnes n’indiquent pas l’état d’expiration des ressources.

## Expiration des liens de ressources {#asset-link-expiration}

While sharing assets through links, Administrators and Editors can set a date and time of expiration using the **[!UICONTROL Expiration]** field in the **[!UICONTROL Link Sharing]** dialog box. L'expiration par défaut du lien est de sept jours à compter de la date de partage du lien.

![](assets/asset-link-sharing.png)

It ensures that assets shared as links expire at the date and time set by [!DNL Brand Portal] Administrators and Editors, and can no longer be viewed and downloaded beyond the expiration date. Comme les ressources partagées via des liens peuvent également être visualisées par des utilisateurs externes qui ne font pas partie de l'organisation, en spécifiant l'expiration, vous pouvez vous assurer que les ressources approuvées sont protégées et non exposées à des entités inconnues au-delà d'une heure spécifiée.

For more information about link sharing, refer to [Share assets as a link](../using/brand-portal-link-share.md).

## Ressources sous licence {#licensed-assets}

Les ressources sous licence sont sujettes à l’acceptation d’un accord de licence avant leur téléchargement à partir de Brand Portal. This agreement for licensed assets comes when you directly download the asset from [!DNL Brand Portal] or via a shared link. Qu’elles soient ou non expirées, les ressources protégées par une licence peuvent être affichées par tous les utilisateurs. Cependant, le téléchargement et l’utilisation des ressources sous licence expirées sont limités. Pour connaître le comportement des ressources sous licence expirées et des activités permises en fonction des rôles d’utilisateur, voir [Autorisations d’utilisation des ressources expirées](../using/manage-digital-rights-of-assets.md#usage-permissions-expired-assets).

License-protected assets have [license agreement attached](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) to them, which is done by setting asset's [metadata property](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) in [!DNL AEM] Assets.

If you choose to download license-protected asset(s), you are redirected to [!UICONTROL Copyright Management] page.

![](assets/asset-copyright-mgmt.png)

Vous devez y sélectionner la ressource à télécharger et accepter l’accord de licence associé. If you do not accept the license agreement, the **[!UICONTROL Download]** button is not enabled.

![](assets/licensed-asset-download-2.png)

Si la sélection contient plusieurs ressources protégées, sélectionnez-en une à la fois, acceptez le contrat de licence et procédez au téléchargement de la ressource.

## Génération d’un rapport sur les ressources expirées {#generate-report-about-expired-assets}

Les administrateurs peuvent générer et télécharger un rapport répertoriant toutes les ressources expirées dans une période spécifique. Ce rapport contient des informations détaillées, telles que la taille, le type, le chemin spécifiant l'emplacement de la ressource dans la hiérarchie des ressources, quand la ressource a expiré, et quand la ressource a été publiée— à propos des ressources expirées. Les colonnes de ce rapport peuvent être personnalisées pour afficher plus de données selon les besoins des utilisateurs.

![](assets/assets-expired.png)

For more information about the reports feature, refer [Work with reports](../using/brand-portal-reports.md#work-with-reports).
