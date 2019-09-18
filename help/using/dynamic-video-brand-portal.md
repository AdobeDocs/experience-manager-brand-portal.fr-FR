---
title: Prise en charge de la vidéo dynamique sur Brand Portal
seo-title: Prise en charge de la vidéo dynamique sur Brand Portal
description: Prise en charge de la vidéo dynamique sur Brand Portal
seo-description: Prise en charge de la vidéo dynamique sur Brand Portal
uuid: a3502a4d-3971-4ea4-953c-44ba04446269
contentOwner: mgulati
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: référencereference
topic-tags: download-install
discoiquuid: e18d992a-a3b5-45f2-9696-8161993213ee
translation-type: tm+mt
source-git-commit: d584ccb4d50f62ec70dabc39be2b17acaba47140

---


# Prise en charge de la vidéo dynamique sur Brand Portal {#dynamic-video-support-on-brand-portal}

Prévisualisez et lisez des vidéos de manière adaptative sur Brand Portal grâce à la prise en charge de Dynamic Media. Téléchargez également les rendus dynamiques à partir du portail et des liens partagés.
 Les utilisateurs de Brand Portal peuvent effectuer les opérations suivantes :

* prévisualiser des vidéos sur la page des détails de la ressource, en mode Carte et sur la page d’aperçu du partage de liens ;
* lire des codes vidéo sur la page des détails de la ressource ;
* afficher des rendus dynamiques dans l’onglet Rendus de la page des détails de la ressource ;
* télécharger des codes vidéo et des dossiers contenant des vidéos.

>[!NOTE]
>
>To work with videos and to publish them to Brand Portal, make sure that your AEM Author instance is set up either on Dynamic Media Hybrid mode or Dynamic Media [!DNL Scene 7] mode.

Pour prévisualiser, lire et télécharger des vidéos, Brand Portal expose les deux configurations suivantes aux administrateurs :

* [Configuration](#configure-dm-hybrid-settings)hybride média dynamique Si l’instance Auteur AEM est en cours d’exécution en mode hybride média dynamique.
* [Configuration](#configure-dm-scene7-settings)du média dynamique [!DNL Scene7] si l’instance d’auteur AEM est en cours d’exécution en mode multimédia[!DNL Scene 7] dynamique.
Définissez l’une de ces configurations selon les configurations définies dans votre instance d’auteur AEM avec laquelle le client Brand Portal est répliqué.

>[!NOTE]
>
>Dynamic videos are not supported on Brand Portal tenants integrated with AEM Author running on [!UICONTROL Scene7Connect] runmode.

## Comment les vidéos dynamiques sont-elles lues ?{#how-are-dynamic-videos-played}

![Les codes vidéo sont récupérés à partir du cloud](assets/VideoEncodes.png)

If Dynamic Media configurations ([Hybrid](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) or [[!DNL Scene 7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings) configurations) are set up on Brand Portal, the dynamic renditions are fetched from [!DNL Scene 7] server. Les codes vidéo sont donc prévisualisés et lus sans retard ni distorsion.

As video encodes are not stored in Brand Portal repository and are fetched from [!DNL Scene 7] server, ensure that the Dynamic Media configurations on AEM Author Instance and Brand Portal are the same.

>[!NOTE]
>
>Les visionneuses vidéo et les paramètres prédéfinis de visionneuses ne sont pas pris en charge dans Brand Portal. Les vidéos sont prévisualisées et lues sur les visionneuses par défaut dans Brand Portal.

## Conditions préalables {#prerequisites}

Pour utiliser des vidéos dynamiques sur Brand Portal, veillez à :

* **Démarrez AEM Author en mode** DM (Contenu multimédia dynamique) Démarrez l’instance AEM Author (avec laquelle le portail de marque est intégré) en mode [hybride](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#EnablingDynamicMedia) Contenu multimédia ou en mode [Contenu multimédia](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#EnablingDynamicMediainScene7mode)dynamique [!DNL Scene7].
* **Configuration des services de cloud de médias dynamiques sur AEM Author** en fonction du mode de média dynamique sur lequel AEM Author est en cours d’exécution, définissez les services [de cloud de médias](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#ConfiguringDynamicMediaCloudServices) dynamiques ou les services [de cloud](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) [!DNL Scene7] sur AEM Author à partir des **outils** .| Services **** Cloud| Contenu multimédia **dynamique**.
* **Configurez Contenu multimédia dynamique sur le portail** de marque en fonction des configurations du cloud Contenu multimédia dynamique dans AEM Author, configurez les paramètres [Contenu multimédia](#configure-dm-hybrid-settings) dynamique ou les paramètres [](#configure-dm-scene7-settings) [!DNL Scene7] à partir des outils d’administration du portail de marque.
Make sure that [separate Brand Portal tenants](#separate-tenants) are used for AEM Author instances configured with Dynamic Media Hybrid and Dynamic Media [!UICONTROL Scene7] modes, if you are using functionalities of Dynamic Media Hybrid and Dynamic Media [!UICONTROL S7].
* **Publiez des dossiers avec des encodages vidéo appliqués au portail** de marque Appliquez des codages [](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) vidéo et publiez le dossier contenant des fichiers de média enrichi de l’instance Auteur AEM vers le portail de marque.
* **Les adresses IP d’entrée de liste blanche dans SPS si l’aperçu sécurisé est activé** Si vous utilisez Contenu multimédia dynamique[!DNL Scene 7] (avec l’aperçu [sécurisé activé](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) pour une entreprise), il est conseillé aux administrateurs [!DNL Scene 7] d’entreprise d’ [autoriser le public à accéder aux adresses IP](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) d’entrée pour les régions respectives à l’aide de l’interface utilisateur Flash de SPS (Scene 7 Publishing System).

Les adresses IP sortantes sont les suivantes :

| **RégionZone géographique** | **Adresse IP sortante** |
|--- |--- |
| N/A | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

To whitelist either of these egress IPs, see [prepare your account for secure testing service](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).

## Meilleures pratiques

Pour vérifier que vos ressources vidéo dynamiques sont prévisualisées, lues et téléchargées depuis Brand Portal (et les liens partagés), suivez ces pratiques :

### Sséparezr les clients pour les modes hybride Dynamic Media et Scene  7 Dynamic Media {#separate-tenants}

If you are using both Dynamic Media [!DNL Scene 7] and Dynamic Media Hybrid features, it is advised that you use different Brand Portal tenants for AEM Author instances configured with Dynamic Media Hybrid and Dynamic Media [!DNL Scene 7] modes.

![Mappage un-à-un Auteur et Brand Portal](assets/BPDynamicMedia.png)

### Même détails de configuration sur l’'instance d’'auteur AEM et Brand  Portal

Ensure that the configuration details–such as [!UICONTROL Title], [!UICONTROL Registration ID], [!UICONTROL Video Service URL] (in [!UICONTROL Dynamic Media Hybrid]) and [!UICONTROL Title], credentials ([!UICONTROL Email] and Password), [!UICONTROL Region], [!UICONTROL Company] (in Dynamic Media [!DNL Scene 7])–are the same in Brand Portal and [!UICONTROL AEM cloud configuration].

### Mettre sur liste blanche les adresses IP sortantes publiques pour le mode Scene  7 Dynamic Media

If Dynamic Media [!UICONTROL Scene 7]–having [secure preview enabled](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html)–is used to serve video assets to Brand Portal, then [!UICONTROL Scene 7] establishes a dedicated image server for staging environments or internal applications. Toute requête à ce serveur vérifie l’adresse IP d’origine. Si la requête entrante ne figure pas dans la liste approuvée des adresses IP, une réponse d’échec est renvoyée.
The [!UICONTROL Scene-7] Company Administrator, therefore, configures an approved list of IP addresses for their company’s [!UICONTROL Secure Testing] environment, through [!UICONTROL SPS] (Scene-7 Publishing System) flash UI. Vérifiez que l’adresse IP sortante pour votre régionzone géographique respective (parmi les suivantes) est ajoutée à cette liste approuvée.
To whitelist either of these egress IPs, see [prepare your account for secure testing service](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).
Les adresses IP sortantes sont les suivantes :

| **RégionZone géographique** | **Adresse IP sortante** |
|--- |--- |
| N/A | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

## Configuration des paramètres Dynamic Media (hybride){#configure-dm-hybrid-settings}

If AEM Author instance is running on dynamic media hybrid mode, then use [!UICONTROL Video] tile from administrative tools panel to configure Dynamic Media gateway settings.
>[!NOTE]
>
>The [video encoding profiles](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) are not published to Brand Portal, instead are fetched from the [!UICONTROL Scene 7] server. Therefore, for video encodes to be played successfully in Brand Portal, ensure that the configuration details are the same as the [[!UICONTROL Scene7 cloud configuration]](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) in your AEM Author instance.
Pour définir les configurations Dynamic Media sur des clients Brand Portal :

1. Dans Brand Portal, sélectionnez le logo AEM pour accéder aux outils d’administration dans la barre d’outils supérieure.

2. From the administrative tools panel, select the **[!UICONTROL Video]** tile.<br />
   ![Configuration du mode hybride Dynamic Media sur Brand Portal](assets/DMHybrid-Video.png)
   **[!UICONTROL La page Modifier la configuration Dynamic Media]** s’ouvre.<br />
   ![Configuration du mode hybride Dynamic Media sur Brand Portal](assets/edit-dynamic-media-config.png)

3. Specify **[!UICONTROL Registration ID]** and **[!UICONTROL Video Service URL]** (DM-Gateway URL). Vérifiez que ces détails sont identiques à ceux dans **[!UICONTROL Outils &gt; Services cloud]dans votre instance d’auteur AEM.**

4. Cliquez sur **Enregistrer** pour enregistrer la configuration.

## Configuration des paramètres de Scene 7 Dynamic Media {#configure-dm-scene7-settings}

If AEM Author instance is running on Dynamic Media- [!UICONTROL Scene 7] mode, then use **[!UICONTROL Dynamic Media Configuration]** tile from administrative tools panel to configure the [!UICONTROL Scene 7] server settings.

To set up Dynamic Media [!UICONTROL Scene 7] configurations on Brand Portal tenants:

1. Dans Brand Portal, sélectionnez le logo AEM pour accéder aux outils d’administration dans la barre d’outils supérieure.

2. From the administrative tools panel, select the **[!UICONTROL Dynamic Media Configuration]** tile.<br />
   ![[!UICONTROL Configuration de Scene 7 Dynamic Media sur Brand Portal]](assets/DMS7-Tile.png)
   La page [!UICONTROL Modifier la configuration Dynamic Media] s’ouvre.<br />
   ![Configuration de Scene 7 sur Brand Portal](assets/S7Config.png)

3. Fournissez les détails suivants :
   * [!UICONTROL Titre]
   * Credentials ([!UICONTROL Email ID] and [!UICONTROL Password]) to access the Scene 7 server
   * [!UICONTROL Région]Assurez-vous que ces valeurs sont identiques à celles de votre instance d’auteur AEM.

4. Sélectionnez **[!UICONTROL Connexion à Dynamic Media]**.

5. Indiquez le **[!UICONTROL nom de la société]** et **eEnregistrez] la configuration.[!UICONTROL **
