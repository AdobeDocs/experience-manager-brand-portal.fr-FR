---
title: Configuration des ressources AEM avec le portail de marque
seo-title: Configuration des ressources AEM avec le portail de marque
description: Découvrez comment configurer AEM Assets avec Brand Portal.
seo-description: Découvrez comment configurer AEM Assets avec Brand Portal.
uuid: null
content-type: reference
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: eba4ee138d4f594c4c446a3cc8941f04fd46902c

---


# Configure AEM Assets with Brand Portal {#configure-integration}

Les ressources d’Adobe Experience Manager (AEM) sont configurées avec le portail de marques via les E/S Adobe, qui obtiennent un jeton IMS pour l’autorisation de votre locataire du portail de marques. La configuration active les fonctions de publication, de distribution et de contribution des ressources pour les utilisateurs du portail de marque.

>[!NOTE]
>
>Auparavant, Brand Portal était configuré dans l’interface utilisateur classique via la passerelle OAuth héritée, qui fait appel à l’échange de jetons JWT pour obtenir un jeton d’accès IMS en vue de l’autorisation.
>
>La configuration via OAuth héritée n’est plus prise en charge à partir du 6 avril 2020 et est remplacée par la configuration via les E/S Adobe.
>
>Si vous êtes déjà un utilisateur du portail de marque avec une configuration sur la passerelle OAuth héritée, il est recommandé de supprimer les configurations existantes et de créer une nouvelle configuration sur les E/S Adobe.
>
>Cependant, la configuration existante continuera à fonctionner si vous ne modifiez pas les configurations.

Les étapes de configuration des ressources AEM avec le portail de marque sont différentes selon votre version AEM et selon que vous effectuez une configuration pour la première fois ou une mise à niveau des configurations existantes :

| **Version d’AEM** | **Nouvelle configuration** | **Configuration de la mise à niveau** |
|---|---|---|
| **AEM 6.5 (6.5.4.0 et versions ultérieures)** | [Créer une configuration](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Configuration de la mise à niveau](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#Upgradeconfiguration) |
| **AEM 6.4 (6.4.8.0 et versions ultérieures)** | [Créer une configuration](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Configuration de la mise à niveau](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#Upgradeconfiguration) |
| **AEM 6.3 (6.3.3.8 et versions ultérieures)** | [Créer une configuration](https://helpx.adobe.com/in/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [Configuration de la mise à niveau](https://helpx.adobe.com/in/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6.2** | Contacter le support technique | Contacter le support technique |


<!--
   Comment Type: draft

   <li> </li>
   -->

<!--
   Comment Type: draft

   <li>Step text</li>
   -->
