---
title: Ressource dans le portail de marque
seo-title: Ressource dans le portail de marque
description: Découvrez la fonctionnalité d’origine des ressources disponible sur le portail des ressources d’Adobe Experience Manager.
seo-description: Découvrez la fonctionnalité d’origine des ressources disponible sur le portail des ressources d’Adobe Experience Manager.
uuid: null
content-type: référencereference
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: 413a6bd17d689d0af0cce20bbd7dedb6ae3cf9b5

---


# Présentation de l’approvisionnement en ressources {#overview-asset-sourcing-in-bp}

**La fonctionnalité d’origine des** ressources permet aux utilisateurs d’AEM (administrateurs/non-administrateurs) de créer de nouveaux dossiers avec une propriété de contribution **des** ressources supplémentaire, en veillant à ce que le nouveau dossier créé soit ouvert à l’envoi des ressources par les utilisateurs du portail de marque. Cela déclenche automatiquement un flux de travail qui crée deux sous-dossiers supplémentaires, appelés **PARTAGÉS** et **NOUVEAU**, dans le dossier de **contribution** nouvellement créé. L’administrateur AEM définit ensuite les exigences en téléchargeant un résumé sur les types de ressources à ajouter au dossier de contributions, ainsi qu’un ensemble de ressources de base, dans le dossier **PARTAGÉ** afin de s’assurer que les utilisateurs de BP disposent des informations de référence dont ils ont besoin. L’administrateur peut alors octroyer aux utilisateurs actifs du portail de marque l’accès au dossier de contributions avant de publier le dossier de **contributions** nouvellement créé sur le portail de marques. Une fois que l’utilisateur a fini d’ajouter du contenu dans le dossier **NEW** , il peut publier le dossier des contributions dans l’environnement d’auteur AEM. Veuillez noter que l’importation peut prendre quelques minutes et refléter le contenu récemment publié dans les ressources AEM.

En outre, toutes les fonctionnalités existantes restent inchangées. Les utilisateurs du portail de marque peuvent afficher, rechercher et télécharger des fichiers à partir du dossier des contributions et des autres dossiers autorisés. Les administrateurs peuvent également partager le dossier des contributions, modifier les propriétés et ajouter des ressources aux collections.

>[!NOTE]
>
>La recherche de ressources dans le portail de marque est prise en charge sur AEM 6.5.2.0 et versions ultérieures.
>
>Cette fonctionnalité n’est pas prise en charge dans les versions antérieures - AEM 6.3 et AEM 6.4.
>
>Contactez l’assistance d’Adobe pour mettre à niveau votre instance AEM vers la dernière version d’AEM prise en charge.

![](assets/asset-sourcing.png)

## Voir également {#reference-articles}

**Pour les administrateurs**
* [Configuration de l’approvisionnement en ressources dans AEM](brand-portal-enable-asset-sourcing.md)
* [Télécharger la liste des utilisateurs du portail de marque](brand-portal-upload-user-list.md)
* [Configuration du dossier des contributions](brand-portal-contribution-folder.md)
* [Téléchargement des fichiers de ligne de base dans le dossier de contributions](brand-portal-upload-baseline-assets.md)
* [Publier le dossier de contribution sur le portail de marque](brand-portal-publish-contribution-folder-to-brand-portal.md)

**Pour les utilisateurs du portail de marque**
* [Télécharger les ressources requises](brand-portal-download-asset-requirements.md)
* [Téléchargement de nouveaux fichiers dans le dossier de contributions](brand-portal-upload-assets-to-contribution-folder.md)
* [Publier le dossier de contributions dans AEM Assets](brand-portal-publish-contribution-folder-to-aem-assets.md)
