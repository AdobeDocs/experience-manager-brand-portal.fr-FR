---
title: Approvisionnement des ressources dans Brand Portal
seo-title: Approvisionnement des ressources dans Brand Portal
description: Découvrez la fonctionnalité d’approvisionnement des ressources disponible dans Adobe Experience Manager Assets Brand Portal.
seo-description: Découvrez la fonctionnalité d’approvisionnement des ressources disponible dans Adobe Experience Manager Assets Brand Portal.
uuid: null
content-type: reference
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: ht
source-git-commit: 413a6bd17d689d0af0cce20bbd7dedb6ae3cf9b5

---


# Présentation de l’approvisionnement des ressources {#overview-asset-sourcing-in-bp}

L’**approvisionnement des ressources** permet aux utilisateurs d’AEM (administrateurs/non-administrateurs) de créer des dossiers avec une propriété **Contribution des ressources** supplémentaire, en s’assurant que les nouveaux dossiers s’ouvrent lorsque des utilisateurs Brand Portal envoient des ressources. Cela déclenche automatiquement un workflow qui crée deux sous-dossiers supplémentaires, appelés **SHARED** et **NEW**, dans le dossier **Contribution** nouvellement créé. L’administrateur d’AEM définit ensuite les exigences en chargeant un résumé relatif aux types de ressources à ajouter au dossier de contribution, ainsi qu’un ensemble de ressources de base, dans le dossier **SHARED**, afin de s’assurer que les utilisateurs de Brand Portal disposent des informations de référence dont ils ont besoin. L’administrateur peut alors octroyer aux utilisateurs actifs de Brand Portal l’accès au dossier de contribution avant de publier le nouveau dossier **Contribution** sur Brand Portal. Dès que l’utilisateur a fini d’ajouter du contenu dans le dossier **NEW**, il peut republier le dossier de contribution dans l’environnement AEM Author. Notez que l’importation du nouveau contenu publié dans AEM Assets et la prise en compte de cette opération peuvent prendre quelques minutes.

En outre, toutes les fonctionnalités existantes restent inchangées. Les utilisateurs de Brand Portal peuvent afficher, rechercher et télécharger des ressources à partir du dossier de contribution, ainsi que des autres dossiers autorisés. Quant aux administrateurs, ils peuvent partager le dossier de contribution de manière plus avancée, modifier les propriétés et ajouter des ressources aux collections.

>[!NOTE]
>
>L’approvisionnement des ressources dans Brand Portal est pris en charge dans AEM 6.5.2.0 et versions ultérieures.
>
>Cette fonctionnalité n’est pas prise en charge dans les versions antérieures : AEM 6.3 et AEM 6.4.
>
>Contactez l’assistance Adobe pour mettre à niveau votre instance d’AEM vers la dernière version d’AEM prise en charge.

![](assets/asset-sourcing.png)

## Voir également {#reference-articles}

**Pour les administrateurs**
* [Configuration de l’approvisionnement des ressources dans AEM](brand-portal-enable-asset-sourcing.md)
* [Chargement de la liste des utilisateurs de Brand Portal](brand-portal-upload-user-list.md)
* [Configuration du dossier de contribution](brand-portal-contribution-folder.md)
* [Chargement de ressources de base dans le dossier de contribution](brand-portal-upload-baseline-assets.md)
* [Publication du dossier de contribution sur Brand Portal](brand-portal-publish-contribution-folder-to-brand-portal.md)

**Pour les utilisateurs de Brand Portal**
* [Téléchargement des exigences en matière de ressources](brand-portal-download-asset-requirements.md)
* [Chargement de nouvelles ressources dans le dossier de contribution](brand-portal-upload-assets-to-contribution-folder.md)
* [Publication du dossier de contribution sur AEM Assets](brand-portal-publish-contribution-folder-to-aem-assets.md)
