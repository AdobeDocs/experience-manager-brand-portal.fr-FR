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
source-git-commit: b41f86824afd5be043c7b91035b01b71fdb69a26
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 100%

---


# Configuration d’AEM Assets avec Brand Portal {#configure-integration}

Adobe Experience Manager (AEM) Assets est configuré avec Brand Portal via Adobe Developer Console, qui fournit un jeton IMS pour autoriser votre client Brand Portal. Brand Portal est désormais pris en charge sur AEM Assets Cloud Service, AEM Assets 6.3 et versions ultérieures.

La configuration d’AEM Assets Cloud Service avec Brand Portal vous permet de publier et de distribuer des ressources avec les utilisateurs de Brand Portal. En revanche, la configuration de Brand Portal sur AEM 6.3 (et versions ultérieures) permet aux utilisateurs de Brand Portal de bénéficier de fonctions de publication, de distribution et de contribution des ressources.

>[!NOTE]
>
>***Pour AEM Assets 6.3 et versions ultérieures***
>
>Auparavant, Brand Portal était configuré dans l’interface utilisateur classique via la passerelle OAuth héritée, qui fait appel à l’échange de jetons JWT pour obtenir un jeton d’accès IMS en vue de l’autorisation.
>
>La configuration via application OAuth héritée n’est plus prise en charge à partir du 6 avril 2020 et est remplacée par la configuration via Adobe Developer Console.

>[!TIP]
>
>***Pour les clients existants uniquement***
>
>La configuration de passerelle OAuth héritée continuera à fonctionner pour les clients existants.
>
>Si vous rencontrez des problèmes avec la configuration héritée de la passerelle OAuth, supprimez la configuration existante et créez une configuration via Adobe Developer Console.

Les étapes de configuration d’AEM Assets avec Brand Portal sont différentes selon votre version d’AEM et selon que vous effectuez une configuration pour la première fois ou une mise à niveau des configurations existantes :

| **Version d’AEM** | **Nouvelle configuration** | **Mise à niveau de la configuration** |
|---|---|---|
| **AEM Assets as a Cloud Service** | [Création d’une configuration](https://docs.adobe.com/content/help/fr-FR/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM 6.5 (6.5.4.0 et versions ultérieures)** | [Création d’une configuration](https://docs.adobe.com/content/help/fr-FR/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Mise à niveau de la configuration](https://docs.adobe.com/content/help/fr-FR/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
| **AEM 6.4 (6.4.8.0 et versions ultérieures)** | [Création d’une configuration](https://docs.adobe.com/content/help/fr-FR/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Mise à niveau de la configuration](https://docs.adobe.com/content/help/fr-FR/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) |
| **AEM 6.3 (6.3.3.8 et versions ultérieures)** | [Création d’une configuration](https://helpx.adobe.com/fr/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [Mise à niveau de la configuration](https://helpx.adobe.com/fr/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6.2** | Contacter le support technique | Contacter le support technique |


