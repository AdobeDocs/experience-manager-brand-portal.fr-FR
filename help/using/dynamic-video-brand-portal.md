---
title: Prise en charge de la vidéo dynamique sur Brand Portal
seo-title: Prise en charge de la vidéo dynamique sur Brand Portal
description: Prise en charge de la vidéo dynamique sur Brand Portal
seo-description: 'Prise en charge de la vidéo dynamique sur Brand Portal  '
uuid: a3502a4d-3971-4ea4-953c-44ba04446269
contentOwner: mgulati
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: download-install
discoiquuid: e18d992a-a3b5-45f2-9696-8161993213ee
translation-type: tm+mt
source-git-commit: eab0a56cfe03d13485386ddc60400ed458198950
workflow-type: tm+mt
source-wordcount: '1209'
ht-degree: 93%

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
>Pour utiliser des vidéos et les publier sur Brand Portal, vérifiez que votre instance AEM Author est configurée sur le mode hybride Dynamic Media ou le mode Dynamic Media **[!DNL Scene 7]**.

Pour prévisualiser, lire et télécharger des vidéos, Brand Portal expose les deux configurations suivantes aux administrateurs :

* [Configuration hybride Dynamic Media](#configure-dm-hybrid-settings) Si l’instance AEM Author est en cours d’exécution sur le mode hybride Dynamic Media.

* [Configuration [!DNL Scene 7] Dynamic Media](#configure-dm-scene7-settings)
Si l’instance d’auteur AEM est en cours d’exécution en mode Dynamic Media **[!DNL Scene 7]**.
Définissez l’une de ces configurations selon les configurations définies dans votre instance d’auteur AEM avec laquelle le client Brand Portal est répliqué.

>[!NOTE]
>
>Les vidéos dynamiques ne sont pas prises en charge sur les clients Brand Portal configurés avec une instance d’auteur AEM s’exécutant en mode **[!UICONTROL Scene7Connect]**.

## Comment les vidéos dynamiques sont-elles lues ?{#how-are-dynamic-videos-played}

![Les codes vidéo sont récupérés à partir du cloud](assets/VideoEncodes.png)

Si les configurations Dynamic Media ([hybride](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) ou [[!DNL Scene 7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings)) sont définies sur Brand Portal, les rendus dynamiques sont récupérés à partir du serveur **[!DNL Scene 7]**. Les codages vidéo sont donc prévisualisés et lus sans retard ni distorsion.

Comme les codages vidéo ne sont pas stockés dans le référentiel Brand Portal et sont récupérés à partir du serveur **[!DNL Scene 7]**, vérifiez que les configurations Dynamic Media sur l’instance AEM Author et sur Brand Portal sont identiques.

>[!NOTE]
>
>Les visionneuses vidéo et les paramètres prédéfinis de visionneuses ne sont pas pris en charge dans Brand Portal. Les vidéos sont prévisualisées et lues sur les visionneuses par défaut dans Brand Portal.

## Conditions préalables {#prerequisites}

Pour utiliser des vidéos dynamiques sur Brand Portal, veillez à :

* **Démarrer l’auteur AEM en mode DM (Dynamic Media)**
Démarrez l’instance d’auteur AEM (avec laquelle Brand Portal est configuré) en [mode hybride Dynamic Media](https://helpx.adobe.com/fr/experience-manager/6-5/assets/using/config-dynamic.html#EnablingDynamicMedia) ou en [mode Dynamic Media [!DNL Scene 7] ](https://helpx.adobe.com/fr/experience-manager/6-5/assets/using/config-dms7.html#EnablingDynamicMediainScene7mode).
* **Configurer Dynamic Media Cloud Services sur l’auteur AEM**
En fonction du mode Dynamic Media dans lequel l’auteur AEM s’exécute, définissez soit [Dynamic Media Cloud Services](https://helpx.adobe.com/fr/experience-manager/6-5/assets/using/config-dynamic.html#ConfiguringDynamicMediaCloudServices), soit [[!DNL Scene 7] Cloud Services](https://helpx.adobe.com/fr/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) sur l’auteur AEM depuis **Outils** | **Services cloud** | **Dynamic Media**.
* **Configurer Dynamic Media sur Brand Portal**
Selon les configurations cloud de Dynamic Media sur l’auteur AEM, configurez les [paramètres Dynamic Media](#configure-dm-hybrid-settings) ou les [[!DNL Scene 7] paramètres](#configure-dm-scene7-settings) à partir des outils d’administration de Brand Portal.
Assurez-vous de bien [séparer les clients Brand Portal](#separate-tenants) utilisés pour les instances d’auteur AEM configurées en modes hybride et **[!UICONTROL Scene 7]** de Dynamic Media, si vous utilisez des fonctionnalités des modes hybride et **[!UICONTROL S7]** de Dynamic Media.
* **Publier des dossiers avec des codes vidéo appliqués à Brand Portal**
Appliquez des [codes vidéo](https://helpx.adobe.com/fr/experience-manager/6-5/assets/using/video-profiles.html) et publiez le dossier contenant des ressources multimédias enrichies depuis l’instance d’auteur AEM sur Brand Portal.
* **Placer sur l&#39;liste autorisée les adresses IP de sortie dans SPS si la prévisualisation sécurisée est activée** Si vous utilisez Dynamic Media-**[!DNL Scene 7]** (avec la prévisualisation [sécurisée activée](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) pour une société), il est conseillé à l’administrateur **[!DNL Scene 7]** de la société de [placer sur l&#39;liste autorisée les adresses IP](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) publiques d’évacuation pour les régions respectives à l’aide de l’interface utilisateur Flash de SPS (Scene 7 Publishing System).
****
Les adresses IP sortantes sont les suivantes :

| **Zone géographique** | **Adresse IP sortante** |
|--- |--- |
| N/A | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

To allowlist either of these egress IPs, see [prepare your account for secure testing service](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).

## Meilleures pratiques

Pour vérifier que vos ressources vidéo dynamiques sont prévisualisées, lues et téléchargées depuis Brand Portal (et les liens partagés), suivez ces pratiques :

### Séparez les clients pour les modes hybride Dynamic Media et Scene 7 Dynamic Media {#separate-tenants}

Si vous utilisez les fonctionnalités Dynamic Media **[!DNL Scene 7]** et hybride, il est conseillé d’utiliser des clients Brand Portal différents pour les instances AEM Author configurées en modes hybride et **[!DNL Scene 7]**.<br />

![Mappage un-à-un Auteur et Brand Portal](assets/BPDynamicMedia.png)

### Même détails de configuration sur l’instance d’auteur AEM et Brand Portal

Assurez-vous que les informations de configuration, telles que **[!UICONTROL Titre]**, **[!UICONTROL ID d’enregistrement]**, **[!UICONTROL URL du service vidéo]** (dans le mode **[!UICONTROL Dynamic Media Hybride]**) et **[!UICONTROL Titre]**, Infos de connexion (**[!UICONTROL E-mail]** et Mot de passe), **[!UICONTROL Région]**, **[!UICONTROL Société]** (dans Dynamic Media **[!DNL Scene 7]**)–sont identiques dans la configuration cloud Brand Portal et **[!UICONTROL AEM]**.

### Placer sur l&#39;liste autorisée les adresses IP publiques de sortie pour le mode Dynamic Media Scene7

Si le mode **[!UICONTROL Scene 7]** de Dynamic Media avec l’[aperçu sécurisé activé](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) est utilisé pour diffuser des ressources vidéo sur Brand Portal, **[!UICONTROL Scene 7]** crée un serveur d’images dédié pour les environnements d’évaluation ou les applications internes. Toute requête à ce serveur vérifie l’adresse IP d’origine. Si la requête entrante ne figure pas dans la liste approuvée des adresses IP, une réponse d’échec est renvoyée.
L’administrateur d’entreprise **[!UICONTROL Scene-7]** configure par conséquent une liste approuvée d’adresses IP pour l’environnement de **[!UICONTROL test sécurisé]** de la société via l’IU Flash de **[!UICONTROL SPS]** (Scene-7 Publishing System). Vérifiez que l’adresse IP sortante pour votre zone géographique respective (parmi les suivantes) est ajoutée à cette liste approuvée.
To allowlist either of these egress IPs, see [prepare your account for secure testing service](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).
Les adresses IP sortantes sont les suivantes :

| **Zone géographique** | **Adresse IP sortante** |
|--- |--- |
| N/A | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

## Configuration des paramètres Dynamic Media (hybride){#configure-dm-hybrid-settings}

Si l’instance AEM Author s’exécute dans le mode hybride de Dynamic Media, utilisez la vignette **[!UICONTROL Vidéo]** dans le panneau Outils d’administration pour configurer les paramètres de la passerelle Dynamic Media.
>[!NOTE]
>
>Les [profils de codage vidéo](https://helpx.adobe.com/fr/experience-manager/6-5/assets/using/video-profiles.html) ne sont pas publiés sur Brand Portal, mais sont récupérés du serveur **[!UICONTROL Scene 7]**. Par conséquent, pour que les codes vidéo soient lus correctement dans Brand Portal, assurez-vous que les détails de configuration sont identiques à la [[!UICONTROL configuration cloud Scene 7]](https://helpx.adobe.com/fr/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) dans votre instance d’auteur AEM.
Pour définir les configurations Dynamic Media sur des clients Brand Portal :

1. Dans Brand Portal, sélectionnez le logo AEM pour accéder aux outils d’administration dans la barre d’outils supérieure.

2. Dans le panneau des outils d’administration, sélectionnez la vignette **[!UICONTROL Vidéo]**.<br />

   ![Configuration du mode hybride Dynamic Media sur Brand Portal](assets/DMHybrid-Video.png)
   La page **[!UICONTROL Modifier la configuration Dynamic Media]** s’ouvre.<br />
   ![Configuration du mode hybride Dynamic Media sur Brand Portal](assets/edit-dynamic-media-config.png)

3. Spécifiez l’**[!UICONTROL ID d’enregistrement]** et l’**[!UICONTROL URL du service vidéo]** (URL de la passerelle Dynamic Media). Vérifiez que ces détails sont identiques à ceux figurant dans **[!UICONTROL Outils > Cloud Services]** dans votre instance d’auteur AEM.

4. Cliquez sur **Enregistrer** pour enregistrer la configuration.

## Configuration des paramètres de Scene 7 Dynamic Media {#configure-dm-scene7-settings}

Si l’instance AEM Author s’exécute dans le mode **[!UICONTROL Scene 7]** de Dynamic Media, utilisez la vignette **[!UICONTROL Configuration Dynamic Media]** dans le panneau des outils d’administration pour configurer les paramètres du serveur **[!UICONTROL Scene 7]**.

Pour définir les configurations Dynamic Media **[!UICONTROL Scene 7]** sur des clients Brand Portal :

1. Dans Brand Portal, sélectionnez le logo AEM pour accéder aux outils d’administration dans la barre d’outils supérieure.

2. Dans le panneau Outils d’administration, sélectionnez la vignette **[!UICONTROL Configuration Dynamic Media]**.<br />
   ![Configuration de Dynamic Media [!UICONTROL Scene 7]sur Brand Portal](assets/DMS7-Tile.png)
   La page **[!UICONTROL Modifier la configuration Dynamic Media]** s’ouvre.<br />
   ![Configuration de Scene 7 sur Brand Portal](assets/S7Config.png)

3. Fournissez les détails suivants :
   * **[!UICONTROL Titre]**
   * Informations d’identification (**[!UICONTROL ID de message électronique]** et **[!UICONTROL Mot de passe]**) pour accéder au serveur Scene 7.
   * **[!UICONTROL Région]**
Vérifiez que ces valeurs sont identiques à celles de votre instance AEM Author.

4. Sélectionnez **[!UICONTROL Connexion à Dynamic Media]**.

5. Indiquez le **[!UICONTROL nom de la société]** et **[!UICONTROL enregistrez]** la configuration.
