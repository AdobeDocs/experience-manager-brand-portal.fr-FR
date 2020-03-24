---
title: Configuration d’AEM Assets avec Brand Portal
seo-title: Configuration d’AEM Assets avec Brand Portal
description: Découvrez comment configurer AEM Assets avec Brand Portal.
seo-description: Découvrez comment configurer AEM Assets avec Brand Portal.
uuid: null
content-type: reference
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: ht
source-git-commit: 58110f1635a9e74340d4a8901e86c0c6a99cf4e2

---


# Configuration d’AEM Assets avec Brand Portal {#configure-integration}

Adobe Experience Manager (AEM) Assets est configuré avec Brand Portal via Adobe I/O, qui fournit un jeton IMS pour autoriser votre client Brand Portal. La configuration permet les fonctions de publication, de distribution et de contribution des ressources pour les utilisateurs de Brand Portal.

>[!NOTE]
>
>Auparavant, Brand Portal était configuré dans l’interface utilisateur classique via la passerelle OAuth héritée, qui fait appel à l’échange de jetons JWT pour obtenir un jeton d’accès IMS en vue de l’autorisation.
>
>La configuration via application OAuth héritée n’est plus prise en charge à partir du 6 avril 2020 et est remplacée par la configuration via Adobe I/O.
>
>Si vous êtes déjà un utilisateur de Brand Portal avec une configuration sur passerelle OAuth héritée, il est recommandé de supprimer les configurations existantes et de créer une configuration sur Adobe I/O.
>
>Toutefois, les configurations existantes continueront à fonctionner si vous ne les modifiez pas.

Les étapes de configuration d’AEM Assets avec Brand Portal sont différentes selon votre version d’AEM et selon que vous effectuez une configuration pour la première fois ou une mise à niveau des configurations existantes :

| **Version d’AEM** | **Nouvelle configuration** | **Mise à niveau de la configuration** |
|---|---|---|
| **AEM 6.5 (6.5.4.0 et versions ultérieures)** | [Création d’une configuration](https://docs.adobe.com/content/help/fr-FR/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Mise à niveau de la configuration](https://docs.adobe.com/content/help/fr-FR/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
| **AEM 6.4 (6.4.8.0 et versions ultérieures)** | [Création d’une configuration](https://docs.adobe.com/content/help/fr-FR/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Mise à niveau de la configuration](https://docs.adobe.com/content/help/fr-FR/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) |
| **AEM 6.3 (6.3.3.8 et versions ultérieures)** | [Création d’une configuration](https://helpx.adobe.com/fr/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [Mise à niveau de la configuration](https://helpx.adobe.com/fr/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6.2** | Contacter le support technique | Contacter le support technique |


<!--
   Comment Type: draft

   <li> </li>
   -->

<!--
   Comment Type: draft

   <li>Step text</li>
   -->
