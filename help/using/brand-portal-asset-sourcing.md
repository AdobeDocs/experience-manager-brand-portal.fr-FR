---
title: Approvisionnement des ressources dans Brand Portal
seo-title: Approvisionnement des ressources dans Brand Portal
description: Découvrez la fonctionnalité d’approvisionnement des ressources disponible dans Adobe Experience Manager Assets Brand Portal.
seo-description: Découvrez la fonctionnalité d’approvisionnement des ressources disponible dans Adobe Experience Manager Assets Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
product: experience-manager
sub-product: ressources
feature: brand-portal
topics: collaboration, content-velocity, sharing
doc-type: feature-video
activity: use
audience: author, marketer
version: 6.5
kt: 3838
translation-type: ht
source-git-commit: ca71b51ea51a92f23fc4c7d6682f73c4c204a5f2

---


# Présentation de l’approvisionnement des ressources {#overview-asset-sourcing-in-bp}

L’**approvisionnement des ressources** permet aux utilisateurs d’AEM (administrateurs/non-administrateurs) de créer des dossiers avec une propriété **Contribution des ressources** supplémentaire, en s’assurant que les nouveaux dossiers s’ouvrent lorsque des utilisateurs Brand Portal envoient des ressources. Cela déclenche automatiquement un workflow qui crée deux sous-dossiers supplémentaires, appelés **SHARED** et **NEW**, dans le dossier **Contribution** nouvellement créé. L’administrateur d’AEM définit ensuite les exigences en chargeant un résumé relatif aux types de ressources à ajouter au dossier de contribution, ainsi qu’un ensemble de ressources de base, dans le dossier **SHARED**, afin de s’assurer que les utilisateurs de Brand Portal disposent des informations de référence dont ils ont besoin. L’administrateur peut alors octroyer aux utilisateurs actifs de Brand Portal l’accès au dossier de contribution avant de publier le nouveau dossier **Contribution** sur Brand Portal. Dès que l’utilisateur a fini d’ajouter du contenu dans le dossier **NEW**, il peut republier le dossier de contribution dans l’environnement AEM Author. Notez que l’importation du nouveau contenu publié dans AEM Assets et la prise en compte de cette opération peuvent prendre quelques minutes.

En outre, toutes les fonctionnalités existantes restent inchangées. Les utilisateurs de Brand Portal peuvent afficher, rechercher et télécharger des ressources à partir du dossier de contribution, ainsi que des autres dossiers autorisés. Quant aux administrateurs, ils peuvent partager le dossier de contribution de manière plus avancée, modifier les propriétés et ajouter des ressources aux collections.

>[!VIDEO](https://video.tv.adobe.com/v/29365/?quality=12&captions=fre_fr)

>[!NOTE]
>
>L’approvisionnement des ressources dans Brand Portal est pris en charge dans AEM 6.5.2.0 et versions ultérieures.
>
>Cette fonctionnalité n’est pas prise en charge dans les versions antérieures : AEM 6.3 et AEM 6.4.
>
>Contactez l’assistance Adobe pour mettre à niveau votre instance d’AEM vers la dernière version d’AEM prise en charge.

![Approvisionnement des ressources dans Brand Portal](assets/asset-sourcing.png)


>[!NOTE]
>
>Si vous êtes un utilisateur d’AEM 6.5.4, la fonctionnalité d’approvisionnement des ressources continuera à fonctionner sur l’« intégration OAuth héritée ».
>
>Toutefois, les utilisateurs de Brand Portal ne peuvent pas publier les ressources du dossier de contribution dans AEM Assets après mise à niveau vers Adobe I/O sur AEM 6.5.4.
>
>Ce problème sera corrigé dans le prochain Service Pack AEM 6.5.5.
>
>Pour une solution immédiate sur AEM 6.5.4, il est recommandé de [télécharger le correctif](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) et de l’installer sur votre instance d’auteur.


## Conditions préalables {#prerequisites}

* AEM 6.5.0.2 ou version ultérieure.
* Vérifiez que votre instance d’AEM Assets est configurée avec Brand Portal. Voir [Configuration d’AEM Assets avec Brand Portal](../using/configure-aem-assets-with-brand-portal.md).

## Voir également {#reference-articles}

**Pour les administrateurs**

* [Configuration de l’approvisionnement des ressources dans AEM](brand-portal-configure-asset-sourcing.md)
* [Chargement de la liste des utilisateurs de Brand Portal](brand-portal-configure-asset-sourcing.md)
* [Configuration du dossier de contribution](brand-portal-contribution-folder.md)
* [Chargement de ressources de base dans le dossier de contribution](brand-portal-upload-baseline-assets.md)
* [Publication du dossier de contribution sur Brand Portal](brand-portal-publish-contribution-folder-to-brand-portal.md)

**Pour les utilisateurs de Brand Portal**

* [Téléchargement des exigences en matière de ressources](brand-portal-download-asset-requirements.md)
* [Chargement de nouvelles ressources dans le dossier de contribution](brand-portal-upload-assets-to-contribution-folder.md)
* [Publication du dossier de contribution sur AEM Assets](brand-portal-publish-contribution-folder-to-aem-assets.md)
