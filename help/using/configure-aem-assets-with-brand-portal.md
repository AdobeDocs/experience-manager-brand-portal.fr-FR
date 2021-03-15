---
title: Configuration d’AEM Assets avec Brand Portal
seo-title: Configuration d’AEM Assets avec Brand Portal
description: Découvrez comment configurer AEM Assets avec Brand Portal.
seo-description: Découvrez comment configurer AEM Assets avec Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: 59eeaedd7f66a0a5affa53f82f3ebbb2bcea535d
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 59%

---


# Configuration d’AEM Assets avec Brand Portal {#configure-integration}

La configuration des ressources Adobe Experience Manager avec le portail de marques permet aux utilisateurs du portail de marques de publier des fichiers, de les distribuer et de leur proposer des fonctions de contribution. Il permet aux utilisateurs de AEM Assets de publier et de distribuer des fichiers avec les utilisateurs du portail de marque. Les utilisateurs du portail de marque peuvent accéder aux ressources partagées et y contribuer en téléchargeant de nouveaux fichiers dans les dossiers de contributions et en les republiant dans AEM Assets.

La configuration de AEM Assets avec Brand Portal est prise en charge sur :
* AEM Assets as a Cloud Service
* AEM Assets (sur site et service géré) version 6.3 et ultérieure

AEM Assets en tant que Cloud Service est automatiquement configuré avec le portail des marques en activant le portail des marques à partir de Cloud Manager. Le processus d’activation crée les configurations requises à l’arrière-plan et active Brand Portal sur la même organisation IMS que l’instance de Cloud Service dans la AEM Assets.

En revanche, AEM Assets (sur site et service géré) est configuré manuellement avec Brand Portal à l’aide d’Adobe Developer Console, qui achète un jeton Adobe Identity Management Services (IMS) pour l’autorisation du locataire du portail Marque.

>[!NOTE]
>
>***Pour AEM Assets 6.3 et versions ultérieures***
>
>Auparavant, Brand Portal était configuré dans l’interface classique via la passerelle OAuth héritée, qui fait appel à l’échange de jetons web JSON (JWT) pour obtenir un jeton IMS en vue de l’autorisation.
>
>La configuration via application OAuth héritée n’est plus prise en charge à partir du 6 avril 2020 et est remplacée par la configuration via Adobe Developer Console.


>[!TIP]
>
>***Pour les clients existants uniquement (sur site et service géré)***
>
>La configuration de passerelle OAuth héritée continuera à fonctionner pour les clients existants.
>
>Si vous rencontrez des problèmes avec la configuration héritée de la passerelle OAuth, supprimez la configuration existante et créez une configuration via Adobe Developer Console.

Les étapes de configuration d’AEM Assets avec Brand Portal sont différentes selon votre version d’AEM et selon que vous effectuez une configuration pour la première fois ou une mise à niveau des configurations existantes :

| **Version d’AEM** | **Nouvelle configuration** | **Mise à niveau de la configuration** |
|---|---|---|
| **AEM Assets as a Cloud Service** | [Activer Brand Portal](https://docs.adobe.com/content/help/fr-FR/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM 6.5 (6.5.4.0 et versions ultérieures)** | [Création d’une configuration](https://docs.adobe.com/content/help/fr-FR/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Mise à niveau de la configuration](https://docs.adobe.com/content/help/fr-FR/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
| **AEM 6.4 (6.4.8.0 et versions ultérieures)** | [Création d’une configuration](https://docs.adobe.com/content/help/fr-FR/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Mise à niveau de la configuration](https://docs.adobe.com/content/help/fr-FR/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) |
| **AEM 6.3 (6.3.3.8 et versions ultérieures)** | [Création d’une configuration](https://helpx.adobe.com/fr/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [Mise à niveau de la configuration](https://helpx.adobe.com/fr/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6.2** | Contacter le support technique | Contacter le support technique |
