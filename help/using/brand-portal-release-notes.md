---
title: Notes de mise à jour
seo-title: Notes de mise à jour
description: Découvrez les fonctionnalités, les améliorations, les problèmes critiques résolus et les problèmes connus de la version Adobe Experience Manager Assets Brand Portal 6.4.6.2.
seo-description: Découvrez les améliorations, les problèmes critiques résolus et les problèmes connus de la version Adobe Experience Manager Assets Brand Portal 6.4.6.2.
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
translation-type: tm+mt
source-git-commit: b41f86824afd5be043c7b91035b01b71fdb69a26
workflow-type: tm+mt
source-wordcount: '789'
ht-degree: 100%

---


# Notes de mise à jour {#release-notes}

Découvrez les fonctionnalités, les améliorations, les problèmes critiques résolus et les problèmes connus de la version Adobe Experience Manager Assets Brand Portal 6.4.6.2.

## Informations sur la version {#release-information}

| Produit | Adobe Experience Manager Assets Brand Portal |
|---|---|
| Version | 6.4.6.2 |
| Date | juin 2020 |

## Présentation {#overview}

Adobe Experience Manager (AEM) Assets Brand Portal permet d’acquérir, de contrôler et de distribuer facilement et en toute sécurité des ressources créatives approuvées destinées à des tiers externes et aux collaborateurs de l’entreprise sur différents appareils. Brand Portal améliore l’efficacité du partage des ressources, accélère la mise sur le marché des ressources et réduit les risques de non-conformité et d’accès non autorisé. Brand Portal permet aux utilisateurs de parcourir, rechercher, prévisualiser, télécharger et exporter des ressources dans des formats approuvés, à tout moment et n’importe où.

## Nouveautés de la version 6.4.6.2 {#what-s-new-in-6462}

### Problèmes critiques résolus {#critical-issues-fixed-6462}

Cette version comprend des correctifs pour les problèmes critiques suivants :

* La suppression d’un schéma de métadonnées publié de Brand Portal entraîne une erreur.

* Si l’administrateur configure Experience Manager Assets 6.5.4 avec Brand Portal via Adobe Developer Console, l’utilisateur de Brand Portal ne peut pas publier les ressources du dossier de contribution de Brand Portal vers Experience Manager.

* La duplication de réplication des dossiers parents provoque des conflits.

* L’utilisateur ne peut pas générer de rapport de partage des liens.

* L’utilisateur peut copier des secrets MAC pour un point d’entrée Brand Portal à l’aide de la commande copyPage.

* Réindexation provoquée par les cqTags sur le clone VA5.


### Problèmes connus {#known-issues-6462}

Cette version présente les problèmes connus suivants :

* Si un dossier de la hiérarchie est renommé à partir d’AEM Assets et que le dossier imbriqué contenant une ressource est publié sur Brand Portal, le titre du dossier n’est pas mis à jour dans Brand Portal tant que le dossier racine n’a pas été republié.


## Nouveautés de la version 6.4.6 {#what-s-new-in-646}

### Nouvelles fonctionnalités {#new-feature}

Cette version comprend les nouvelles fonctionnalités suivantes :

* Captcha pour la connexion des invités à Brand Portal. Pour plus d’informations, voir [Accès des invités à Brand Portal](../using/guest-access.md).

* Brand Portal est désormais pris en charge par AEM Assets Cloud Service. Vous pouvez configurer AEM Assets Cloud Service avec Brand Portal pour partager et distribuer des ressources avec les utilisateurs de Brand Portal.
Pour plus d’informations, voir [Configuration d’AEM Assets Cloud Service avec Brand Portal](https://docs.adobe.com/content/help/fr-FR/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html).

### Améliorations {#enhancements-646}

Cette version de Brand Portal comprend les améliorations suivantes :

* Dans AEM 6.3 et versions ultérieures, le canal d’autorisation entre AEM Assets et Brand Portal a été modifié. AEM Assets est désormais configuré avec Brand Portal via Adobe Developer Console, qui fournit un jeton IMS pour autoriser votre client Brand Portal.

>[!NOTE]
>
>La configuration via application OAuth héritée n’est plus prise en charge à partir du 6 avril 2020 et est remplacée par la configuration via Adobe Developer Console.

>[!TIP]
>
>***Pour les clients existants uniquement***
>
>La configuration de passerelle OAuth héritée continuera à fonctionner pour les clients existants.
>
>Si vous rencontrez des problèmes avec la configuration héritée de la passerelle OAuth, supprimez la configuration existante et créez une configuration via Adobe Developer Console.

Pour plus d’informations, voir [Configuration d’AEM Assets avec Brand Portal](configure-aem-assets-with-brand-portal.md).

### Problèmes critiques résolus {#critical-issues-fixed}

Cette version comprend des correctifs pour les problèmes critiques suivants :

* Les valeurs du menu déroulant Schéma de métadonnées ne sont pas visibles dans les propriétés des ressources.

* Le sous-schéma de métadonnées n’affiche pas les onglets basés sur le type MIME dans les propriétés des ressources.

* L’annulation de la publication d’un schéma de métadonnées renvoie un message d’erreur bien que le schéma soit supprimé du serveur principal.

* L’image d’aperçu ne s’affiche pas pour une ressource publiée.

* L’utilisateur ne peut pas publier ni annuler la publication de ressources dont le nom contient une apostrophe.

* Les termes et conditions ne s’affichent pas lors du téléchargement de plusieurs ressources.

* Des vulnérabilités mineures de sécurité ont été corrigées.

### Problèmes connus {#known-issues}

Cette version présente les problèmes connus suivants :

* Les utilisateurs de Brand Portal ne peuvent pas publier les ressources du dossier de contribution dans AEM Assets après mise à niveau vers Adobe Developer Console sur AEM 6.5.4.

   Ce problème sera corrigé dans le prochain Service Pack 6.5.5.

   Pour une solution immédiate sur AEM 6.5.4, il est recommandé de [télécharger le correctif](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) et de l’installer sur votre instance d’auteur.

* L’option d’exclusion des rendus système ne fonctionne pas correctement lors du téléchargement d’une ressource.


## Langues {#languages}

L’interface utilisateur de Brand Portal est disponible dans les langues suivantes :

* Anglais
* Allemand
* Français
* Espagnol
* Italien
* Brésilien        Portugais
* Japonais
* Chinois simplifié
* Coréen

## Plates-formes certifiées        {#certified-platforms}

Pour vérifier quelles sont les plates-formes certifiées pour exécuter cette version de Brand Portal, reportez-vous à la colonne **Prise en charge de l’interface utilisateur optimisée pour les écrans tactiles** du tableau **Navigateurs pris en charge pour l’interface utilisateur de création** dans la section [Exigences techniques](https://helpx.adobe.com/fr/experience-manager/6-4/sites/deploying/using/technical-requirements.html).

## Liens {#links}

* [Page du produit Adobe Experience Manager sur adobe.com](http://www.adobe.com/fr/marketing-cloud/experience-manager.html)
* [Documentation Assets Brand Portal](https://helpx.adobe.com/fr/experience-manager/brand-portal/user-guide.html)

## Assistance technique et accès au produit (sites à accès limité) {#product-access-and-support-restricted-sites}

Ces sites sont réservés aux clients. Si vous êtes client et avez besoin d’un accès, contactez votre responsable de compte Adobe.

* [https://daycare.day.com](https://daycare.day.com)

* [Accès aux produits](https://login.marketing.adobe.com)

* [Assistance clientèle d’Adobe](https://helpx.adobe.com/fr/contact.html)
