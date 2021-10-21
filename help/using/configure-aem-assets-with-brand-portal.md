---
title: Configuration d’Experience Manager Assets avec Brand Portal
seo-title: Configure Experience Manager Assets with Brand Portal
description: Découvrez comment configurer Experience Manager Assets avec Brand Portal.
seo-description: Get an insight into configuring Experience Manager Assets with Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
role: Admin
exl-id: 261c0e84-6b3d-459c-b6b9-a9af106d6943
source-git-commit: 5503a34f4896816bf991216b457cd824707ae5ed
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Configuration d’Experience Manager Assets avec Brand Portal {#configure-integration}

La configuration d’Adobe Experience Manager Assets avec Brand Portal permet aux utilisateurs de Brand Portal de bénéficier de fonctions de publication, de distribution et de contribution des ressources. Il permet aux utilisateurs d’Experience Manager Assets de publier et de distribuer des ressources aux utilisateurs de Brand Portal. Les utilisateurs de Brand Portal peuvent accéder aux ressources partagées et y contribuer en chargeant de nouvelles ressources dans les dossiers de contribution de ressources et en les republiant dans Experience Manager Assets.

La configuration d’Experience Manager Assets avec Brand Portal est prise en charge sur :

* Experience Manager Assets as a Cloud Service
* Experience Manager Assets (On-Premise et Managed Service) version 6.3 et ultérieures

Experience Manager Assets as a Cloud Service est automatiquement configuré avec Brand Portal en activant celui-ci à partir de Cloud Manager. Le workflow d’activation crée les configurations requises en arrière-plan et active Brand Portal sur la même organisation IMS qu’Experience Manager Assets as a Cloud Service.

En revanche, Experience Manager Assets (On-Premise et Managed Service) est configuré avec Brand Portal à l’aide d’Adobe Developer Console qui fournit un jeton Adobe Identity Management Services (IMS) pour l’autorisation du client Brand Portal.

>[!NOTE]
>
>***Pour Experience Manager Assets 6.3 et les versions ultérieures***
>
>Auparavant, Brand Portal était configuré dans l’interface classique via la passerelle OAuth héritée, qui fait appel à l’échange de jetons web JSON (JWT) pour obtenir un jeton IMS en vue de l’autorisation.
>
>La configuration via application OAuth héritée n’est plus prise en charge à partir du 6 avril 2020 et est remplacée par la configuration via Adobe Developer Console.


>[!TIP]
>
>***Pour les clients existants uniquement (On-Premise et Managed Service)***
>
>La configuration de passerelle OAuth héritée continuera à fonctionner pour les clients existants.
>
>Si vous rencontrez des problèmes avec la configuration héritée de la passerelle OAuth, supprimez la configuration existante et créez une configuration via Adobe Developer Console.

Les étapes de configuration d’AEM Assets avec Brand Portal sont différentes selon votre version d’AEM et selon que vous effectuez une configuration pour la première fois ou une mise à niveau des configurations existantes :

| **Version d’AEM** | **Nouvelle configuration** | **Mise à niveau de la configuration** |
|---|---|---|
| **AEM Assets as a Cloud Service** | [Activer Brand Portal](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html?lang=fr) | - |
| **AEM 6.5 (6.5.4.0 et versions ultérieures)** | [Création d’une configuration](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html?lang=fr) | [Mise à niveau de la configuration](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html?lang=fr#upgrade-integration-65) |
| **AEM 6.4 (6.4.8.0 et versions ultérieures)** | [Création d’une configuration](https://experienceleague.adobe.com/docs/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html?lang=fr) | [Mise à niveau de la configuration](https://experienceleague.adobe.com/docs/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html?lang=fr#upgrade-integration-64) |
| **AEM 6.3 (6.3.3.8 et versions ultérieures)** | [Création d’une configuration](https://helpx.adobe.com/fr/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [Mise à niveau de la configuration](https://helpx.adobe.com/fr/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6.2** | Contactez le service clientèle | Contactez le service clientèle |
