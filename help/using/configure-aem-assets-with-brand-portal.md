---
title: Configuration d’AEM Assets avec Brand Portal
seo-title: Configuration d’AEM Assets avec Brand Portal
description: Découvrez comment configurer AEM Assets avec Brand Portal.
seo-description: Découvrez comment configurer AEM Assets avec Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: de21e84b93a657570db2024c2ceba58704ba5844
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 59%

---


# Configuration d’AEM Assets avec Brand Portal {#configure-integration}

La configuration de Adobe Experience Manager Assets en tant que Cloud Service avec Adobe Experience Manager Assets Brand Portal permet de publier et de distribuer des fichiers avec les utilisateurs du portail de marques. En revanche, la configuration de AEM 6.3 (et versions ultérieures) avec le portail de marque permet aux utilisateurs du portail de marque de publier des fichiers, de distribuer des fichiers et de contribuer aux fichiers.

Adobe Experience Manager Assets est configuré avec Brand Portal via Adobe Developer Console, qui fournit un jeton IMS (Adobe Identity Management Services) pour l’autorisation de votre locataire du portail Marque.

>[!NOTE]
>
>***Pour AEM Assets 6.3 et versions ultérieures***
>
>Auparavant, le portail de marque était configuré dans une interface classique via la passerelle OAuth héritée, qui utilise l’échange JSON Web token (JWT) pour obtenir un jeton IMS pour autorisation.
>
>La configuration via application OAuth héritée n’est plus prise en charge à partir du 6 avril 2020 et est remplacée par la configuration via Adobe Developer Console.


>[!TIP]
>
>***Pour les clients existants uniquement***
>
>La configuration de passerelle OAuth héritée continuera à fonctionner pour les clients existants.
>
>Si vous rencontrez des problèmes avec la configuration héritée de la passerelle OAuth, supprimez la configuration existante et créez une configuration via Adobe Developer Console.


Les étapes de configuration d’AEM Assets avec Brand Portal sont différentes selon la version de votre AEM et selon que vous configurez pour la première fois ou mettez à niveau les configurations existantes :

| **Version d’AEM** | **Nouvelle configuration** | **Mise à niveau de la configuration** |
|---|---|---|
| **AEM Assets as a Cloud Service** | [Création d’une configuration](https://docs.adobe.com/content/help/fr-FR/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM 6.5 (6.5.4.0 et versions ultérieures)** | [Création d’une configuration](https://docs.adobe.com/content/help/fr-FR/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Mise à niveau de la configuration](https://docs.adobe.com/content/help/fr-FR/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
| **AEM 6.4 (6.4.8.0 et versions ultérieures)** | [Création d’une configuration](https://docs.adobe.com/content/help/fr-FR/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Mise à niveau de la configuration](https://docs.adobe.com/content/help/fr-FR/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) |
| **AEM 6.3 (6.3.3.8 et versions ultérieures)** | [Création d’une configuration](https://helpx.adobe.com/fr/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [Mise à niveau de la configuration](https://helpx.adobe.com/fr/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6.2** | Contacter le support technique | Contacter le support technique |


