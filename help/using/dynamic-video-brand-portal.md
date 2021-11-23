---
title: Prise en charge de la vidéo dynamique sur Brand Portal
seo-title: Dynamic video support on Brand Portal
description: Prise en charge de la vidéo dynamique sur Brand Portal
seo-description: Dynamic video support on Brand Portal
uuid: a3502a4d-3971-4ea4-953c-44ba04446269
contentOwner: mgulati
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: download-install
discoiquuid: e18d992a-a3b5-45f2-9696-8161993213ee
exl-id: 08d6a0fb-061e-4bef-b8e2-bb8522e7482e
source-git-commit: 8924ff9c78c065895dd0f8d1099a5488b34a34e2
workflow-type: tm+mt
source-wordcount: '1250'
ht-degree: 56%

---

# Prise en charge de la vidéo dynamique sur Brand Portal {#dynamic-video-support-on-brand-portal}

Prévisualisez et lisez des vidéos de manière adaptative sur Brand Portal grâce à la prise en charge de Dynamic Media. Téléchargez également les rendus dynamiques à partir du portail et des liens partagés.
Les utilisateurs de Brand Portal peuvent effectuer les opérations suivantes :

* prévisualiser des vidéos sur la page des détails de la ressource, en mode Carte et sur la page d’aperçu du partage de liens ;
* lire des codes vidéo sur la page des détails de la ressource ;
* afficher des rendus dynamiques dans l’onglet Rendus de la page des détails de la ressource ;
* télécharger des codes vidéo et des dossiers contenant des vidéos.

>[!NOTE]
>
>Pour utiliser des vidéos et les publier sur Brand Portal, vérifiez que votre instance de création Experience Manager est configurée sur le mode hybride Dynamic Media ou le mode Dynamic Media **[!DNL Scene7]**.

Pour prévisualiser, lire et télécharger des vidéos, Brand Portal expose les deux configurations suivantes aux administrateurs :

* [Configuration hybride Dynamic Media](#configure-dm-hybrid-settings)
Si l’instance d’auteur Experience Manager est en cours d’exécution sur le mode hybride Dynamic Media.
* [Configuration [!DNL Scene7] Dynamic Media](#configure-dm-scene7-settings)
Si l’instance d’auteur Experience Manager est en cours d’exécution en mode Dynamic Media **[!DNL Scene7]**.
Définissez l’une de ces configurations selon les configurations définies dans votre instance d’auteur Experience Manager avec laquelle le client Brand Portal est répliqué.

>[!NOTE]
>
>Les vidéos dynamiques ne sont pas prises en charge sur les clients Brand Portal configurés avec l’auteur Experience Manager s’exécutant sur **[!UICONTROL Scene7Connect]** mode d’exécution.

## Comment les vidéos dynamiques sont-elles lues ? {#how-are-dynamic-videos-played}

![Les codes vidéo sont récupérés à partir du cloud](assets/VideoEncodes.png)

Si les configurations Dynamic Media ([hybrides](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) ou [[!DNL Scene7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings)) sont définies sur Brand Portal, les rendus dynamiques sont récupérés à partir du serveur **[!DNL Scene7]**. Les codages vidéo sont donc prévisualisés et lus sans retard ni distorsion.

Comme les codes vidéo ne sont pas stockés dans le référentiel Brand Portal et sont récupérés à partir de **[!DNL Scene7]** , assurez-vous que les configurations Dynamic Media sur l’instance d’auteur Adobe Experience Manager et Brand Portal sont identiques.

>[!NOTE]
>
>Les visionneuses vidéo et les paramètres prédéfinis de visionneuses ne sont pas pris en charge dans Brand Portal. Les vidéos sont prévisualisées et lues sur les visionneuses par défaut dans Brand Portal.

## Prérequis {#prerequisites}

Pour utiliser des vidéos dynamiques sur Brand Portal, veillez à :

* **Démarrer l’auteur Experience Manager en mode Dynamic Media**
Démarrez l’instance d’auteur du Experience Manager (avec laquelle Brand Portal est configuré) dans [Dynamic Media - [!DNL Scene7] mode](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dms7.html?lang=en#enabling-dynamic-media-in-scene-mode) ou [Dynamic Media - mode hybride](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dynamic.html?lang=fr) ou
* **Configuration des Cloud Services Dynamic Media sur l’auteur du Experience Manager**
En fonction du mode Dynamic Media (mode Scene7 ou mode hybride) sur lequel l’auteur du Experience Manager s’exécute, définissez [Cloud Services Dynamic Media ([!DNL Scene7] mode)](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dms7.html?lang=fr?lang=en#configuring-dynamic-media-cloud-services) ou [Cloud Services Dynamic Media (mode hybride)](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dynamic.html?lang=en#configuring-dynamic-media-cloud-services) sur l’auteur Experience Manager depuis **Outils** | **Cloud Services** | **Dynamic Media**.
* **Configuration de Dynamic Media sur Brand Portal**
Selon les configurations cloud Dynamic Media sur l’auteur Experience Manager, configurez [Paramètres Dynamic Media](#configure-dm-hybrid-settings) ou [[!DNL Scene7] paramètres](#configure-dm-scene7-settings) à partir des outils d’administration de Brand Portal.
Assurez-vous que [clients Brand Portal distincts](#separate-tenants) sont utilisées pour les instances d’auteur de Experience Manager configurées dans Dynamic Media - **[!UICONTROL Scene7]** et Dynamic Media - mode hybride. Surtout si vous utilisez les fonctionnalités de Dynamic Media **[!UICONTROL S7]** et Dynamic Media hybride.
* **Publication de dossiers avec des codes vidéo appliqués à Brand Portal**
Appliquer [encodages vidéo](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/video-profiles.html?lang=fr) et publier le dossier contenant les ressources multimédias enrichies de l’instance d’auteur de Experience Manager sur Brand Portal.
* **Mettre sur liste blanche les adresses IP sortantes dans SPS si l’aperçu sécurisé est activé**
En cas d’utilisation de Dynamic Media **[!DNL Scene7]** (avec l’[aperçu sécurisé activé](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html?lang=fr) pour une entreprise), il est conseillé à l’**[!DNL Scene7]** administrateur de l’entreprise[ de mettre les adresses IP sortantes publiques sur liste blanche](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html?lang=fr#testing-the-secure-testing-service) pour les zones géographiques respectives utilisant l’interface utilisateur Flash de SPS (**[!UICONTROL Scene7]** Publishing System).
Les adresses IP sortantes sont les suivantes :

| **Zone géographique** | **Adresse IP sortante** |
|--- |--- |
| N/A | 130.248.160.68,  20.94.203.130 |
| EMEA | 185.34.189.3,  51.132.146.75 |
| APAC | 63.140.44.54 |

Pour mettre l’une de ces adresses IP sortantes sur liste blanche, voir [Préparation de votre compte pour un test sécurisé](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).

## Meilleures pratiques

Pour vérifier que vos ressources vidéo dynamiques sont prévisualisées, lues et téléchargées depuis Brand Portal (et les liens partagés), suivez ces pratiques :

### Séparez les clients pour Dynamic Media - Scene7 et Dynamic Media - Modes hybrides {#separate-tenants}

Si vous utilisez Dynamic Media - **[!DNL Scene7]** Mode et Dynamic Media - Fonctionnalités du mode hybride, utilisez différents clients Brand Portal pour les instances d’auteur de Experience Manager configurées avec Dynamic Media - **[!DNL Scene7]** et Dynamic Media - Modes hybrides.


![Mappage un-à-un Auteur et Brand Portal](assets/BPDynamicMedia.png)

### Mêmes détails de configuration sur l’instance d’auteur du Experience Manager et Brand Portal

Assurez-vous que les détails de configuration sont identiques dans Brand Portal et **[!UICONTROL Configuration du cloud de Experience Manager]**. Les mêmes détails de configuration sont les suivants :

* **[!UICONTROL Titre]**
* **[!UICONTROL ID d’enregistrement]**
* **[!UICONTROL URL du service vidéo]** in **[!UICONTROL Dynamic Media - mode hybride]**
* **[!UICONTROL Titre]**
* Informations d’identification (**[!UICONTROL Email]** et mot de passe)
* **[!UICONTROL Zone géographique]**
* **[!UICONTROL Société]** dans Dynamic Media - **[!DNL Scene7]** mode

### Mise sur liste blanche des adresses IP sortantes publiques pour le mode Scene7 Dynamic Media

Si le mode **[!UICONTROL Scene7]** de Dynamic Media avec l’[aperçu sécurisé activé](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) est utilisé pour diffuser des ressources vidéo sur Brand Portal, **[!UICONTROL Scene7]** crée un serveur d’images dédié pour les environnements d’évaluation ou les applications internes. Toute requête à ce serveur vérifie l’adresse IP d’origine. Si la requête entrante ne figure pas dans la liste approuvée des adresses IP, une réponse d’échec est renvoyée.
Le **[!UICONTROL Scene7]** L’administrateur de l’entreprise configure donc une liste approuvée d’adresses IP pour le **[!UICONTROL Test sécurisé]** environnement, par **[!UICONTROL SPS]** (Scene7 Publishing System) IU Flash. Vérifiez que l’adresse IP sortante pour votre zone géographique respective (parmi les suivantes) est ajoutée à cette liste approuvée.
Pour mettre l’une de ces adresses IP sortantes sur liste blanche, voir [Préparation de votre compte pour un test sécurisé](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).
Les adresses IP sortantes sont les suivantes :

| **Zone géographique** | **Adresse IP sortante** |
|--- |--- |
| N/A | 130.248.160.66,  52.151.32.108 |
| EMEA | 185.34.189.1 |
| APAC | 63.140.44.54 |

## Configuration des paramètres Dynamic Media (hybride) {#configure-dm-hybrid-settings}

Si l’instance d’auteur du Experience Manager est en cours d’exécution en mode hybride Dynamic Media, utilisez **[!UICONTROL Vidéo]** à partir du panneau des outils d’administration pour configurer les paramètres de la passerelle Dynamic Media.

>[!NOTE]
>
>Les [profils de codage vidéo](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/video-profiles.html) ne sont pas publiés sur Brand Portal, mais sont récupérés du serveur **[!UICONTROL Scene7]**. Par conséquent, pour que les codes vidéo soient lus correctement dans Brand Portal, assurez-vous que les détails de configuration sont identiques au [Cloud Services Dynamic Media ([!DNL Scene7] mode)](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dms7.html?lang=en#configuring-dynamic-media-cloud-services) dans votre instance d’auteur de Experience Manager.

Pour définir les configurations Dynamic Media sur des clients Brand Portal :

1. Sélectionnez le logo du Experience Manager afin d’accéder aux outils d’administration dans la barre d’outils supérieure, dans Brand Portal.
1. Dans le panneau des outils d’administration, sélectionnez la vignette **[!UICONTROL Vidéo]**.

   ![Configuration du mode hybride Dynamic Media sur Brand Portal](assets/DMHybrid-Video.png)

   La page **[!UICONTROL Modifier la configuration Dynamic Media]** s’ouvre.

   ![Configuration du mode hybride Dynamic Media sur Brand Portal](assets/edit-dynamic-media-config.png)

1. Spécifiez l’**[!UICONTROL ID d’enregistrement]** et l’**[!UICONTROL URL du service vidéo]** (URL de la passerelle Dynamic Media). Assurez-vous que ces détails sont identiques à ceux de la section **[!UICONTROL Outils > Cloud Services]** dans votre instance d’auteur de Experience Manager.
1. Cliquez sur **Enregistrer** pour enregistrer la configuration.

## Configuration des paramètres de Scene7 Dynamic Media {#configure-dm-scene7-settings}

Si l’instance d’auteur du Experience Manager est en cours d’exécution sur Dynamic Media- **[!UICONTROL Scene7]** mode, puis utilisez **[!UICONTROL Configuration Dynamic Media]** à partir du panneau des outils d’administration pour configurer **[!UICONTROL Scene7]** paramètres du serveur.

Pour définir les configurations Dynamic Media **[!UICONTROL Scene7]** sur des clients Brand Portal :

1. Sélectionnez le logo du Experience Manager afin d’accéder aux outils d’administration dans la barre d’outils supérieure, dans Brand Portal.

2. Dans le panneau Outils d’administration, sélectionnez la vignette **[!UICONTROL Configuration Dynamic Media]**.

   ![Configuration de Dynamic Media [!UICONTROL Scene7]sur Brand Portal](assets/DMS7-Tile.png)

   La page **[!UICONTROL Modifier la configuration Dynamic Media]** s’ouvre.

   ![Configuration de Scene7 sur Brand Portal](assets/S7Config.png)

3. Fournissez les détails suivants :

   * **[!UICONTROL Titre]**
   * Informations d’identification (**[!UICONTROL ID de message électronique]** et **[!UICONTROL Mot de passe]**) pour accéder au serveur Scene7.
   * **[!UICONTROL Zone géographique]**

   Assurez-vous que ces valeurs sont identiques à celles trouvées dans votre instance d’auteur de Experience Manager.

4. Sélectionnez **[!UICONTROL Connexion à Dynamic Media]**.

5. Indiquez le **[!UICONTROL nom de la société]** et **[!UICONTROL enregistrez]** la configuration.
