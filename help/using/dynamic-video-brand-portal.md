---
title: Prise en charge de la vidéo dynamique sur Brand Portal
description: Prise en charge de la vidéo dynamique sur Brand Portal
contentOwner: mgulati
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: download-install
exl-id: 08d6a0fb-061e-4bef-b8e2-bb8522e7482e
source-git-commit: e2e007550b557e790533204d49271c90b3b8647d
workflow-type: tm+mt
source-wordcount: '1194'
ht-degree: 46%

---

# Prise en charge de la vidéo dynamique sur Brand Portal {#dynamic-video-support-on-brand-portal}

Prévisualisez et lisez des vidéos de manière adaptative sur Brand Portal grâce à la prise en charge de Dynamic Media. Téléchargez également les rendus dynamiques à partir du portail et des liens partagés.
Les utilisateurs de Brand Portal peuvent effectuer les opérations suivantes :

* Prévisualisez des vidéos dans la page Détails de la ressource, le mode Carte et la page d’aperçu du partage de lien.
* Lire les codes vidéo sur la page Détails de la ressource.
* Affichez les rendus dynamiques dans l’onglet Rendus de la page Détails de la ressource.
* Télécharger des codes vidéo et des dossiers contenant des vidéos.

>[!NOTE]
>
>Pour utiliser des vidéos et les publier dans Brand Portal, assurez-vous que votre instance d’auteur Experience Manager est configurée en mode hybride Dynamic Media ou en mode Dynamic Media **[!DNL Scene7]**.

Pour prévisualiser, lire et télécharger des vidéos, Brand Portal expose les deux configurations suivantes aux administrateurs :

* [Configuration hybride Dynamic Media](#configure-dm-hybrid-settings)
Si l’instance d’auteur Experience Manager est en cours d’exécution en mode hybride Dynamic Media.
* [Dynamic Media [!DNL Scene7] configuration](#configure-dm-scene7-settings)
Si l’instance d’auteur Experience Manager est en cours d’exécution en mode Dynamic Media - **[!DNL Scene7]** .
Définissez l’une de ces configurations en fonction des configurations définies dans votre instance d’auteur Experience Manager avec laquelle le client Brand Portal est répliqué.

>[!NOTE]
>
>Les vidéos dynamiques ne sont pas prises en charge sur les clients Brand Portal configurés avec l’auteur Experience Manager s’exécutant en mode d’exécution **[!UICONTROL Scene7 Connect]**.

## Comment les vidéos dynamiques sont-elles lues ? {#how-are-dynamic-videos-played}

![Les codes vidéo sont récupérés à partir du cloud](assets/VideoEncodes.png)

Si des configurations Dynamic Media ([Hybrid](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) ou [[!DNL Scene7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings)) sont configurées sur Brand Portal, les rendus dynamiques sont récupérés à partir du serveur **[!DNL Scene7]**. Les codages vidéo sont donc prévisualisés et lus sans retard ni distorsion.

Le référentiel Brand Portal ne stocke pas de codes vidéo et les récupère du serveur **[!DNL Scene7]**. Assurez-vous que les configurations Dynamic Media sur l’instance d’auteur Adobe Experience Manager et sur Brand Portal sont identiques.

>[!NOTE]
>
>Les visionneuses vidéo et leurs paramètres prédéfinis ne sont pas pris en charge dans Brand Portal. Les vidéos sont prévisualisées et lues sur les visionneuses par défaut dans Brand Portal.

## Prérequis {#prerequisites}

Pour utiliser des vidéos dynamiques sur Brand Portal, veillez à :

* **Démarrer l’auteur Experience Manager en mode Dynamic Media**

  Démarrez l’instance d’auteur Experience Manager (avec laquelle Brand Portal est configuré) dans [Dynamic Media - [!DNL Scene7] mode](https://experienceleague.adobe.com/fr/docs/experience-manager-65/content/assets/dynamic/config-dms7#enabling-dynamic-media-in-scene-mode) ou dans [Dynamic Media - mode hybride](https://experienceleague.adobe.com/fr/docs/experience-manager-65/content/assets/dynamic/config-dynamic) ou

* **Configuration de Cloud Service Dynamic Media sur l’instance d’auteur Experience Manager**

  En fonction du mode Dynamic Media (mode Scene7 ou mode hybride) sur lequel l’auteur Experience Manager s’exécute, définissez [Cloud Service Dynamic Media ([!DNL Scene7])](https://experienceleague.adobe.com/fr/docs/experience-manager-65/content/assets/dynamic/config-dms7#configuring-dynamic-media-cloud-services) ou [Cloud Service Dynamic Media (mode hybride)](https://experienceleague.adobe.com/fr/docs/experience-manager-65/content/assets/dynamic/config-dms7#configuring-dynamic-media-cloud-services) sur l’auteur Experience Manager à partir de **outils** | **Cloud Service** | **Dynamic Media**.

* **Configurer Dynamic Media sur Brand Portal**

  En fonction des configurations du cloud Dynamic Media sur l’auteur Experience Manager, configurez les [paramètres Dynamic Media](#configure-dm-hybrid-settings) ou [[!DNL Scene7] paramètres](#configure-dm-scene7-settings) à partir des outils d’administration Brand Portal.

  Assurez-vous que des [clients Brand Portal distincts](#separate-tenants) soient utilisées pour les instances de création Experience Manager Author configurées dans le mode Dynamic Media - **[!UICONTROL Scene7]** et Dynamic Media - mode hybride. Si vous utilisez les fonctionnalités de Dynamic Media **[!UICONTROL S7]** et de Dynamic Media Hybrid, cette approche est particulièrement importante.

* **Dossiers Publish avec codage vidéo appliqués à Brand Portal**

  Appliquez les [codages vidéo](https://experienceleague.adobe.com/fr/docs/experience-manager-65/content/assets/dynamic/video-profiles) et publiez le dossier contenant des ressources multimédias enrichies de l’instance d’auteur Experience Manager vers Brand Portal.

* **Placer sur la liste autorisée les adresses IP sortantes dans SPS si l’aperçu sécurisé est activé**

  Si vous utilisez Dynamic Media-**[!DNL Scene7]** (avec [l’aperçu sécurisé activé](https://experienceleague.adobe.com/fr/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public) pour une entreprise), il est conseillé à l’ **[!DNL Scene7]** administrateur de l’entreprise [de placer sur la liste autorisée les adresses IP sortantes publiques](https://experienceleague.adobe.com/fr/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public#testing-the-secure-testing-service) pour les régions respectives utilisant SPS (**[!UICONTROL Scene7]** Publishing System) de l’interface utilisateur Flash.

  Les adresses IP sortantes sont les suivantes :

  | **Zone géographique** | **Adresse IP de sortie** |
  |--- |--- |
  | N/A | 130.248.160.68, 20.94.203.130 |
  | EMEA | 185.34.189.3, 51.132.146.75 |
  | APAC | 63.140.44.54 |

  Pour placer sur la liste autorisée l’une de ces adresses IP sortantes, voir [Préparation de votre compte pour un service de test sécurisé](https://experienceleague.adobe.com/fr/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public#testing-the-secure-testing-service).

## Bonnes pratiques

Assurez-vous que les ressources vidéo dynamiques sont prévisualisées, lues et téléchargées correctement à partir de Brand Portal (et des liens partagés). Suivez les pratiques suivantes :

### Séparez les clients pour les modes Dynamic Media - Scene7 et Dynamic Media - Hybride {#separate-tenants}

Si vous utilisez les fonctionnalités du mode Dynamic Media - **[!DNL Scene7]** et Dynamic Media - Hybride, utilisez différents clients Brand Portal pour les instances de création Experience Manager Author configurées avec les modes Dynamic Media - **[!DNL Scene7]** et Dynamic Media - Hybride.


![Mappage un-à-un Auteur et Brand Portal](assets/BPDynamicMedia.png)

### Détails de configuration identiques sur l’instance de création Experience Manager Author et Brand Portal

Assurez-vous que les détails de la configuration soient identiques dans Brand Portal et dans la **[!UICONTROL Configuration Cloud Experience Manager]**. Les détails identiques de la configuration sont les suivants :

* **[!UICONTROL Titre]**
* **[!UICONTROL ID d’enregistrement]**
* **[!UICONTROL URL du service vidéo]** en mode **[!UICONTROL Dynamic Media - Hybride]**
* **[!UICONTROL Titre]**
* Informations d’identification (**[!UICONTROL E-mail]** et mot de passe)
* **[!UICONTROL Zone géographique]**
* **[!UICONTROL Société]** en mode Dynamic Media - **[!DNL Scene7]**

### Mise sur liste blanche des adresses IP sortantes publiques pour le mode Scene7 Dynamic Media

Si Dynamic Media **[!UICONTROL Scene7]** - dont l’ [ aperçu sécurisé est activé](https://experienceleague.adobe.com/fr/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public) - est utilisé pour diffuser des ressources vidéo vers Brand Portal, **[!UICONTROL Scene7]** crée un serveur d’images dédié pour les environnements d’évaluation ou les applications internes. Toute requête à ce serveur vérifie l’adresse IP d’origine. Si la requête entrante ne figure pas dans la liste approuvée des adresses IP, une réponse d’échec est renvoyée.
L’administrateur de la société **[!UICONTROL Scene7]** configure par conséquent une liste approuvée d’adresses IP pour l’environnement de **[!UICONTROL test sécurisé]** de sa société, par le biais de l’interface utilisateur Flash **[!UICONTROL SPS]** (Scene7 Publishing System). Vérifiez que l’adresse IP sortante pour votre zone géographique respective (parmi les suivantes) est ajoutée à cette liste approuvée.
Pour placer sur la liste autorisée l’une de ces adresses IP sortantes, voir [Préparation de votre compte pour un service de test sécurisé](https://experienceleague.adobe.com/fr/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public#testing-the-secure-testing-service).
Les adresses IP sortantes sont les suivantes :

| **Zone géographique** | **Adresse IP de sortie** |
|--- |--- |
| N/A | 130.248.160.68, 20.94.203.130 |
| EMEA | 51.132.146.75, 130.248.244.202, 130.248.244.203, 130.248.244.204, 130.248.244.210, 130.248.244.211, 130.248.244.212 |
| APAC | 63.140.44.54 |

## Configuration des paramètres Dynamic Media (hybride) {#configure-dm-hybrid-settings}

Si l’instance d’auteur Experience Manager s’exécute en mode hybride Dynamic Media, utilisez la vignette **[!UICONTROL Vidéo]** du panneau des outils d’administration pour configurer les paramètres de la passerelle Dynamic Media.

>[!NOTE]
>
>Les [profils de codage vidéo](https://experienceleague.adobe.com/fr/docs/experience-manager-65/content/assets/dynamic/video-profiles) ne sont pas publiés sur Brand Portal. Ils sont récupérés à la place à partir du serveur **[!UICONTROL Scene7]**. Par conséquent, pour que les codes vidéo soient lus correctement dans Brand Portal, assurez-vous que les détails de configuration soient identiques à ceux de [Dynamic Media Cloud Services (mode [!DNL Scene7])](https://experienceleague.adobe.com/fr/docs/experience-manager-65/content/assets/dynamic/config-dms7#configuring-dynamic-media-cloud-services) dans votre instance Experience Manager Author.

Pour définir les configurations Dynamic Media sur des clients Brand Portal :

1. Sélectionnez le logo de l’Experience Manager pour accéder aux outils d’administration dans la barre d’outils supérieure de Brand Portal.
1. Dans le panneau des outils d’administration, sélectionnez la vignette **[!UICONTROL Vidéo]**.

   ![Configuration du mode hybride Dynamic Media sur Brand Portal](assets/DMHybrid-Video.png)

   La page **[!UICONTROL Modifier la configuration Dynamic Media]** s’ouvre.

   ![Configuration du mode hybride Dynamic Media sur Brand Portal](assets/edit-dynamic-media-config.png)

1. Spécifiez l’**[!UICONTROL ID d’enregistrement]** et l’**[!UICONTROL URL du service vidéo]** (URL de la passerelle Dynamic Media). Assurez-vous que ces détails soient identiques à ceux figurant dans **[!UICONTROL Outils > Cloud Services]** dans votre instance Experience Manager Author.
1. Cliquez sur **Enregistrer** pour enregistrer la configuration.

## Configuration des paramètres de Scene7 Dynamic Media {#configure-dm-scene7-settings}

Si l’instance d’auteur Experience Manager est en cours d’exécution en mode Dynamic Media **[!UICONTROL Scene7]**, utilisez la vignette **[!UICONTROL Configuration Dynamic Media]** du panneau des outils d’administration pour configurer les paramètres du serveur **[!UICONTROL Scene7]**.

Pour définir les configurations Dynamic Media **[!UICONTROL Scene7]** sur des clients Brand Portal :

1. Sélectionnez le logo de l’Experience Manager pour accéder aux outils d’administration dans la barre d’outils supérieure de Brand Portal.

2. Dans le panneau Outils d’administration, sélectionnez la vignette **[!UICONTROL Configuration Dynamic Media]**.

   ![Configuration de Dynamic Media [!UICONTROL Scene7]sur Brand Portal](assets/DMS7-Tile.png)

   La page **[!UICONTROL Modifier la configuration Dynamic Media]** s’ouvre.

   ![Configuration de Scene7 sur Brand Portal](assets/S7Config.png)

3. Fournissez les détails suivants :

   * **[!UICONTROL Titre]**
   * Informations d’identification (**[!UICONTROL ID de message électronique]** et **[!UICONTROL Mot de passe]**) pour accéder au serveur Scene7.
   * **[!UICONTROL Zone géographique]**

   Assurez-vous que ces valeurs soient identiques à celles qui se trouvent dans votre instance Experience Manager Author.

4. Sélectionnez **[!UICONTROL Connexion à Dynamic Media]**.

5. Indiquez le **[!UICONTROL nom de la société]** et **[!UICONTROL enregistrez]** la configuration.
