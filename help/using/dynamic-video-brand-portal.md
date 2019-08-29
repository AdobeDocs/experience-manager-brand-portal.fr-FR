---
title: Prise en charge de la vidéo dynamique sur Brand Portal
seo-title: Prise en charge de la vidéo dynamique sur Brand Portal
description: Prise en charge de la vidéo dynamique sur Brand Portal
seo-description: Prise en charge de la vidéo dynamique sur Brand Portal
uuid: a 3502 a 4 d -3971-4 ea 4-953 c -44 ba 04446269
contentOwner: mgulati
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
content-type: référence
topic-tags: téléchargement-install
discoiquuid: e 18 d 992 a-a 3 b 5-45 f 2-9696-8161993213 ee
translation-type: tm+mt
source-git-commit: 770c353b1143d879280df310012ce9d4d30b40c9

---


# Prise en charge de la vidéo dynamique sur Brand Portal {#dynamic-video-support-on-brand-portal}

Preview and play videos adaptively on [!DNL Brand Portal] with Dynamic Media support. Téléchargez également les rendus dynamiques depuis le portail et les liens partagés.
[!DNL Brand Portal] les utilisateurs peuvent :

* prévisualiser des vidéos sur la page des détails de la ressource, en mode Carte et sur la page d’aperçu du partage de liens ;
* lire des codes vidéo sur la page des détails de la ressource ;
* afficher des rendus dynamiques dans l’onglet Rendus de la page des détails de la ressource ;
* télécharger des codes vidéo et des dossiers contenant des vidéos.

>[!NOTE]
>
>To work with videos and to publish them to [!DNL Brand Portal], make sure that your [!DNL AEM] Author instance is set up either on Dynamic Media Hybrid mode or Dynamic Media [!DNL Scene 7] mode.

To preview, play, and download videos, [!DNL Brand Portal] exposes the following two configurations to administrators:

* [Configuration
hybride Media hybride](#configure-dm-hybrid-settings)si l'instance [!DNL AEM] Auteur est en cours d'exécution sur le mode Hybrid Media hybride.
* [Contenu multimédia dynamique [! Configuration
DNL Scene 7]](#configure-dm-scene7-settings)si l'instance [!DNL AEM] Auteur est en cours d'exécution sur le[!DNL Scene 7] mode multimédia dynamique.
Set either of these configurations based on the configurations you set in your [!DNL AEM] Author instance with which [!DNL Brand Portal] tenant is replicated.

>[!NOTE]
>
>Dynamic videos are not supported on [!DNL Brand Portal] tenants integrated with [!DNL AEM] Author running on [!UICONTROL Scene7Connect] runmode.

## How are dynamic videos played? {#how-are-dynamic-videos-played}

![Les codes vidéo sont récupérés à partir du cloud](assets/VideoEncodes.png)

If Dynamic Media configurations ([Hybrid](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) or [[!DNL Scene 7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings) configurations) are set up on [!DNL Brand Portal], the dynamic renditions are fetched from [!DNL Scene 7] server. Les codes vidéo sont donc prévisualisés et lus sans retard ni distorsion.

As video encodes are not stored in [!DNL Brand Portal] repository and are fetched from [!DNL Scene 7] server, ensure that the Dynamic Media configurations on [!DNL AEM] Author Instance and [!DNL Brand Portal] are the same.

>[!NOTE]
>
>Les visionneuses vidéo et les paramètres prédéfinis de visionneuses ne sont pas pris en charge dans [!DNL Brand Portal]. Les vidéos sont prévisualisées et lues sur les visionneuses par défaut dans [!DNL Brand Portal].

## Conditions préalables {#prerequisites}

To work with dynamic videos on [!DNL Brand Portal], make sure to:

* **Démarrage[!DNL AEM]de l'auteur sur le mode
DM (Dynamic Media)** Démarrer l'instance [!DNL AEM] d'auteur (avec laquelle [!DNL Brand Portal] est intégré) soit sur [le mode](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#EnablingDynamicMedia) Hybrid Media hybride, soit [sur Dynamic Media [! DNL Scene 7]](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#EnablingDynamicMediainScene7mode).
* **Configuration des services Cloud Dynamic Media sur[!DNL AEM]l'auteur**
en fonction du mode [!DNL AEM] Média dynamique en cours d'exécution sur, définissez les services Cloud de médias [dynamiques](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#ConfiguringDynamicMediaCloudServices) ou [[! ! DNL Scene 7] Services Cloud](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) sur [!DNL AEM] l'auteur à partir **d'outils** | **Services Cloud** | **Contenu multimédia dynamique**.
* **Configuration du contenu multimédia dynamique sur le portail**
de marque en fonction des configurations de cloud de médias dynamiques sur [!DNL AEM] l'auteur, configuration [des paramètres de médias dynamiques](#configure-dm-hybrid-settings) ou [[! Paramètres DNL Scene 7](#configure-dm-scene7-settings) de [!DNL Brand Portal] l'administration.
Assurez-vous de [bien séparer [! Les clients DNL Brand Portal] sont](#separate-tenants) utilisés pour [!DNL AEM] les instances d'auteur configurées avec les modes Dynamic Media Hybride et Dynamic Media [!UICONTROL Scene 7] , si vous utilisez des fonctionnalités de Dynamic Media Hybrid et de Dynamic Media [!UICONTROL S 7].
* **Publiez les dossiers avec des codages vidéo appliqués au portail
de marque** Appliquez [des encodages](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) vidéo et publiez le dossier contenant des ressources multimédias enrichies depuis [!DNL AEM] l'instance Auteur.[!DNL Brand Portal]
* **La liste blanche Egalise les IPS dans SPS si l'aperçu sécurisé est activé** Si l'option Média dynamique est[!DNL Scene 7] activée
(avec [l'option d'aperçu sécurisé activée](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) pour une entreprise), il est conseillé aux administrateurs [!DNL Scene 7] d'entreprise [de liste blanche des adresses IP](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) d'egalisation publique pour les régions respectives utilisant SPS ([!UICONTROL Scene 7] Publishing System) Flash UI.
 Les adresses IP sortantes sont les suivantes :

| **Région géographique** | **Adresse IP sortante** |
|--- |--- |
| s.o. | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

To whitelist either of these egress IPs, see [prepare your account for secure testing service](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).

## Meilleures pratiques

To ensure that your dynamic video assets are successfully previewed, played, and downloaded from [!DNL Brand Portal] (and shared links), follow these practices:

### Clients distincts pour les modes Multimédia dynamique et Média dynamique Scene 7 {#separate-tenants}

Si vous utilisez les fonctions Dynamic Media [!DNL Scene 7] et Dynamic Media Hybride, il est conseillé d'utiliser différents [!DNL Brand Portal] locataires pour [!DNL AEM] les instances Auteur configurées avec [!DNL Scene 7] les modes Dynamic Media Hybride et Dynamic Media.
![Mappage un-à-un Auteur et Brand Portal](assets/BPDynamicMedia.png)

### Même détails de configuration sur l'instance d'auteur AEM et le portail de marque

Assurez-vous que les détails de configuration, tels que Titre, ID d'enregistrement, URL du service vidéo (dans Dynamic Media Hybride) et Titre, informations d'identification (Courriel et Mot de passe), Région, Société (dans le contenu multimédia [!DNL Scene 7]dynamique)-sont identiques dans la configuration [!DNL Brand Portal] de [!DNL AEM] cloud et de cloud.

### Liste blanche de l'egalisation publique des ips pour le mode Scene 7 Dynamic Media

Si l'option d'aperçu sécurisé Scene 7 est [activée pour](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html)servir des fichiers vidéo, [!DNL Brand Portal]Scene 7 établit un serveur d'images dédié pour les environnements d'évaluation ou les applications internes. Toute requête à ce serveur vérifie l’adresse IP d’origine. Si la requête entrante ne figure pas dans la liste approuvée des adresses IP, une réponse d’échec est renvoyée.
L'administrateur d'entreprise Scene 7 configure par conséquent une liste approuvée d'adresses IP pour l'environnement Secure Testing de leur entreprise, via SPS (Scene -7 Publishing System) Flash UI. Vérifiez que l’adresse IP sortante pour votre région géographique respective (parmi les suivantes) est ajoutée à cette liste approuvée.
To whitelist either of these egress IPs, see [prepare your account for secure testing service](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).
Les adresses IP egales sont les suivantes :

| **Région géographique** | **Adresse IP sortante** |
|--- |--- |
| s.o. | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

## Configuration des paramètres Dynamic Media (hybride){#configure-dm-hybrid-settings}

If [!DNL AEM] Author instance is running on dynamic media hybrid mode, then use Video tile from administrative tools panel to configure Dynamic Media gateway settings.
>[!NOTE]
>
>The [video encoding profiles](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) are not published to [!DNL Brand Portal], instead are fetched from the Scene 7 server. Therefore, for video encodes to be played successfully in [!DNL Brand Portal], ensure that the configuration details are the same as the [Scene7 cloud configuration](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) in your [!DNL AEM] Author instance.
To set up Dynamic Media configurations on [!DNL Brand Portal] tenants:

1. Select the [!DNL AEM] logo to access administrative tools from the toolbar at the top, in [!DNL Brand Portal].

2. From the administrative tools panel, select the **Video** tile.
   ![Configuration du mode hybride Dynamic Media sur Brand Portal](assets/DMHybrid-Video.png)
   **La page Modifier la configuration** du média dynamique s'ouvre.
   ![Configuration du mode hybride Dynamic Media sur Brand Portal](assets/edit-dynamic-media-config.png)

3. Specify **Registration ID** and **Video Service URL** (DM-Gateway URL). Make sure these details are the same as those in **Tools** &gt; **Cloud Services** in your [!DNL AEM] Author instance.

4. Cliquez sur **Enregistrer** pour enregistrer la configuration.

## Configuration des paramètres de Scene 7 Dynamic Media {#configure-dm-scene7-settings}

If [!DNL AEM] Author instance is running on Dynamic Media- [!UICONTROL Scene 7] mode, then use **Dynamic Media Configuration** tile from administrative tools panel to configure the [!UICONTROL Scene 7] server settings.

To set up Dynamic Media [!UICONTROL Scene 7] configurations on [!DNL Brand Portal] tenants:

1. Select the [!DNL AEM] logo to access administrative tools from the toolbar at the top, in [!DNL Brand Portal].

2. From the administrative tools panel, select the **Dynamic Media Configuration** tile.
   ![La configuration de Scene 7 sur la page [!DNL Brand Portal]](assets/DMS7-Tile.png)Modifier la configuration du média dynamique s'ouvre.
   ![Configuration de Scene 7 sur [!DNL Brand Portal]](assets/S7Config.png)

3. Fournissez les détails suivants :
   * Titre
   * Informations d’identification (e-mail et mot de passe) pour accéder au serveur Scene 7.
   * Région
Make sure these values are the same as those in your [!DNL AEM] Author instance.

4. Sélectionnez **Connexion à Dynamic Media**.

5. Provide the **Company name**, and **Save** the configuration.
