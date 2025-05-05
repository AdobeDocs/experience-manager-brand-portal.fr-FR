---
title: Configuration d’Experience Manager Assets avec Brand Portal
description: Découvrez comment configurer Experience Manager Assets avec Brand Portal.
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
role: Admin
exl-id: 261c0e84-6b3d-459c-b6b9-a9af106d6943
source-git-commit: 32a67abf466dd3bf635b851b02377ed23591915e
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 60%

---

# Configuration d’Experience Manager Assets avec Brand Portal {#configure-integration}

La configuration d’Adobe Experience Manager Assets avec Brand Portal permet aux utilisateurs de Brand Portal de bénéficier de fonctions de publication, de distribution et de contribution des ressources. Il permet aux utilisateurs de Experience Manager Assets de publier et de distribuer des ressources avec les utilisateurs de Brand Portal. Les utilisateurs de Brand Portal peuvent accéder aux ressources partagées et y contribuer en chargeant de nouvelles ressources dans les dossiers de contribution de ressources et en les republiant dans Experience Manager Assets.

La configuration d’Experience Manager Assets avec Brand Portal est prise en charge sur :

* Experience Manager Assets as a Cloud Service
* Experience Manager Assets (On-Premise et Managed Service) version 6.5 et ultérieures

Experience Manager Assets as a Cloud Service est automatiquement configuré avec Brand Portal en activant celui-ci à partir de Cloud Manager. Le workflow d’activation crée les configurations requises en arrière-plan et active Brand Portal sur la même organisation IMS qu’Experience Manager Assets as a Cloud Service.

Alors que Experience Manager Assets (on-premise et managed service) est configuré manuellement avec Brand Portal à l’aide de Adobe Developer Console, qui fournit un jeton Adobe Identity Management Services (IMS) pour autoriser le client Brand Portal.

>[!NOTE]
>
>***Pour Experience Manager Assets, 6.5 et versions ultérieures***
>
>Auparavant, l’interface classique configurait Brand Portal à l’aide de la passerelle OAuth héritée, qui utilise l’exchange JSON Web Token (JWT) pour obtenir un jeton IMS en vue de l’autorisation.
>
>La configuration par le biais d’OAuth hérité n’est plus prise en charge à partir du 6 avril 2020 et est remplacée par la configuration par Adobe Developer Console.


>[!TIP]
>
>***Pour les clients existants uniquement (On-Premise et Managed Service)***
>
>La configuration héritée de la passerelle OAuth continue de fonctionner pour les clients existants.
>
>Si vous rencontrez des problèmes avec la configuration de la passerelle OAuth héritée, supprimez la configuration existante et créez une configuration à l’aide de Adobe Developer Console.

Les étapes de configuration d’AEM Assets avec Brand Portal sont différentes selon votre version d’AEM et selon que vous effectuez une configuration pour la première fois ou une mise à niveau des configurations existantes :

| **Version d’AEM** | **Nouvelle configuration** | **Mise à niveau de la configuration** |
|---|---|---|
| **AEM Assets as a Cloud Service** | [Activer Brand Portal](https://experienceleague.adobe.com/fr/docs/experience-manager-cloud-service/content/assets/brand-portal/configure-aem-assets-with-brand-portal) | - |
| **AEM 6.5 (6.5.4.0 et versions ultérieures)** | [Création d’une configuration](https://experienceleague.adobe.com/fr/docs/experience-manager-65/content/assets/brandportal/configure-aem-assets-with-brand-portal) | [Mise à niveau de la configuration](https://experienceleague.adobe.com/fr/docs/experience-manager-65/content/assets/brandportal/configure-aem-assets-with-brand-portal#upgrade-integration-65) |
