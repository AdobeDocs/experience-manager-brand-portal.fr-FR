---
title: Présentation d’AEM Assets Brand Portal
seo-title: Présentation d’AEM Assets Brand Portal
description: AEM Assets Brand Portal permet d’acquérir, de contrôler et de distribuer facilement et en toute sécurité des ressources créatives destinées à des tiers externes et aux collaborateurs de l’entreprise sur différents appareils.
seo-description: AEM Assets Brand Portal permet d’acquérir, de contrôler et de distribuer facilement et en toute sécurité des ressources créatives destinées à des tiers externes et aux collaborateurs de l’entreprise sur différents appareils.
uuid: b 1 e 54 d 03-eb 2 e -488 e-af 4 d-bae 817 dd 135 a
content-type: référence
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
topic-tags: introduction
discoiquuid: 6 aefa 298-4728-4 b 8 e-a 85 b-e 419 ee 37 f 2 f 4
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Présentation d’AEM Assets Brand Portal {#overview-of-aem-assets-brand-portal}

En tant que spécialiste du marketing, il est parfois nécessaire de collaborer avec les partenaires de canaux et les utilisateurs internes pour créer, gérer et diffuser rapidement du contenu numérique pertinent aux clients. La diffusion au bon moment de contenu pertinent tout le long du parcours client est essentielle pour accroître la demande, la conversion, l’engagement et la fidélisation des clients.

Il est toutefois difficile de développer des solutions qui permettent le partage efficace et en toute sécurité de logos de la marque, d’instructions, de ressources de campagne ou de clichés de produit avec des équipes internes, des partenaires et des revendeurs.

**Adobe Experience Manager (AEM) Assets Brand Portal permet d’acquérir, de contrôler et de distribuer facilement et en toute sécurité des ressources créatives destinées à des tiers externes et aux collaborateurs de l’entreprise sur différents appareils.** Brand Portal améliore l’efficacité du partage des ressources, accélère la mise sur le marché des ressources et réduit les risques de non-conformité et d’accès non autorisé.

L'environnement de portail basé sur un navigateur vous permet de télécharger, parcourir, rechercher, prévisualiser et exporter facilement des fichiers dans des formats approuvés.

## Utilisateurs de l'utilisateur dans Brand Portal {#Personas}

Le portail de marque prend en charge les rôles utilisateur suivants :

* Utilisateur invité
* Visualisateur
* Éditeur
* Administrateur

Le tableau suivant répertorie les tâches que peuvent réaliser les utilisateurs qui disposent de ces rôles :

|  | **Parcourir** | **Recherche** | **Téléchargement** | **Partager des dossiers** | **Partager une collection** | **Partager de ressources en tant que lien** | **Accéder aux outils d’administration** |
|--- |--- |--- |--- |--- |--- |--- |--- |
| **Utilisateur invité** | ✓* | ✓* | ✓* | x | x | x | x |
| **Visualisateur** | ✓ | ✓ | ✓ | x | x | x | x |
| **Éditeur** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | x |
| **Administrateur** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |

* Les utilisateurs invités peuvent explorer, accéder et effectuer des recherches dans les dossiers et collections publics uniquement.

### Utilisateur invité {#guest-user}

Tout utilisateur disposant d’un accès limité aux ressources sur Brand Portal sans passer par une authentification est un utilisateur invité. La session d'invités permet aux utilisateurs d'accéder aux dossiers publics et aux collections. En tant qu'utilisateur invité, vous pouvez parcourir les détails des ressources et avoir une vue complète des ressources des membres de dossiers publics et de collections. You can search, download, and add public assets to [!UICONTROL Lightbox] collection.

La session d’invité vous empêche toutefois de créer des collections et des recherches enregistrées et de les partager. Lors d’une session d’invité,  les utilisateurs ne peuvent ni accéder aux paramètres des dossiers et collections, ni partager des ressources sous la forme de lien. Voici la liste des tâches qu'un utilisateur invité peut effectuer :

[Exploration et accès aux ressources publiques](browse-assets-brand-portal.md)

[Recherche parmi les ressources publiques](brand-portal-searching.md)

[Téléchargement de ressources publiques](brand-portal-download-users.md)

[Ajout de ressources à [! UICONPREVLIGHTBOX]](brand-portal-light-box.md#add-assets-to-lightbox)

### Observateur {#viewer}

Dans Brand Portal, un utilisateur standard est généralement un utilisateur qui dispose du rôle Visualisateur. Un utilisateur qui dispose de ce rôle peut accéder aux fichiers, aux collections et aux ressources autorisés. L’utilisateur peut également parcourir, prévisualiser, télécharger et exporter des ressources (rendus d’origine ou spécifiques), configurer des paramètres de compte et rechercher des ressources. Voici la liste des tâches que peut réaliser un visualisateur :

[Exploration des ressources](browse-assets-brand-portal.md)

[Recherche de ressources](brand-portal-searching.md)

[Téléchargement de ressources](brand-portal-download-users.md)

### Éditeur {#editor}

Un utilisateur qui dispose du rôle Éditeur peut effectuer toutes les tâches d’un visualisateur. En outre, il peut visualiser les fichiers et dossiers partagés par un administrateur. L’utilisateur qui dispose du rôle Éditeur peut également partager du contenu (fichiers, dossiers, collections) avec d’autres personnes.

En plus des tâches d’un visualisateur, un éditeur peut effectuer les tâches suivantes :

[Partage de dossiers](brand-portal-sharing-folders.md)

[Partager une collection](brand-portal-share-collection.md)

[Partager de ressources en tant que lien](brand-portal-link-share.md)

### Administrateur {#administrator}

An administrator includes a user marked as system administrator or Brand Portal product administrator in [!UICONTROL Admin Console]. Un administrateur peut ajouter et supprimer des administrateurs système et des utilisateurs, définir des paramètres prédéfinis, envoyer des e-mails aux utilisateurs et afficher des rapports sur l’utilisation et le stockage du portail.

Un administrateur peut effectuer toutes les tâches qu'un éditeur peut effectuer pour effectuer les tâches supplémentaires suivantes :

[Gestion des utilisateurs, des groupes et des rôles utilisateur](brand-portal-adding-users.md)

[Personnalisation du papier peint, des en-têtes de page et des e-mails](brand-portal-branding.md)

[Utilisation des facettes de recherche personnalisée](brand-portal-search-facets.md)

[Utilisation du formulaire de schéma de métadonnées](brand-portal-metadata-schemas.md)

[Application de paramètres d’image prédéfinis ou de rendus dynamiques](brand-portal-image-presets.md)

[Utilisation des rapports](brand-portal-reports.md)

En plus des tâches mentionnées ci-dessus, un auteur dans AEM Assets peut effectuer les tâches suivantes :

[Configuration de l’intégration d’AEM Assets avec Brand Portal](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html)

[Publication de dossiers sur Brand Portal](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-publish-folder.html)

[Publication de collections sur Brand Portal](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-publish-collection.html)

## Alias alternatif pour l'URL de Portal Portal {#tenant-alias-for-portal-url}

A partir de la version 6.4.3 de Brand Portal, les organisations peuvent avoir une URL alternative (alias) pour l'URL existante de leur client de portail de marque. Vous pouvez créer l'URL d'alias en utilisant un autre préfixe dans l'URL.\
Notez que seul le préfixe de l’URL Brand Portal peut être adapté aux besoins du client, et non l’URL entière. For example, an organization with existing domain **[!UICONTROL geomettrix.brand-portal.adobe.com]** can get **[!UICONTROL geomettrixinc.brand-portal.adobe.com]** created on request.

Cependant, l’instance d’auteur AEM peut uniquement être [configurée](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html) avec l’URL d’ID client et non avec l’URL (alternative) d’alias de client.

>[!NOTE]
>
>Pour obtenir un alias pour le nom du client dans l’URL de portail existante, les organisations doivent solliciter la création d’un alias de client auprès de l’assistance Adobe. Cette demande est traitée en vérifiant d’abord si l’alias est disponible puis en le créant.
>
>Pour remplacer ou supprimer l’ancien alias, le même processus doit être suivi.

## Demande d’accès à Brand Portal {#request-access-to-brand-portal}

Les utilisateurs peuvent demander l’accès à Brand Portal depuis l’écran de connexion. These requests are sent to Brand Portal administrators, who grant access to users through the Adobe [!UICONTROL Admin Console]. Une fois l’accès accordé, les utilisateurs reçoivent une notification par e-mail.

Pour demander l’accès, procédez comme suit :

1. From the Brand Portal login page, select **[!UICONTROL Click here]** corresponding to **[!UICONTROL Need Access?]**. However, to enter the guest session, select the **[!UICONTROL Click here]** corresponding to **[!UICONTROL Guest Access?]**.

   ![Écran de connexion de Brand Portal](assets/bp-login-requestaccess.png)

   La page [!UICONTROL Demander l’accès] s’affiche.

2. To request access to an organization’s Brand Portal, you must have a valid [!UICONTROL Adobe ID], [!UICONTROL Enterprise ID], or [!UICONTROL Federated ID].

   In the [!UICONTROL Request Access] page, sign in using your ID (scenario 1) or create an [!UICONTROL Adobe ID] (scenario 2):
   ![[!UICONTROL Demande d'accès]](assets/bplogin_request_access_2.png)

   **Scénario 1**
   1. If you have an [!UICONTROL Adobe ID], [!UICONTROL Enterprise ID], or [!UICONTROL Federated ID], click **[!UICONTROL Sign In]**.
The [!UICONTROL Sign in] page opens.
   2. Provide your [!UICONTROL Adobe ID] credentials and click **[!UICONTROL Sign in]**.
      ![Adobe sign in](assets/bplogin_request_access_3.png)
   You are redirected to the [!UICONTROL Request Access] page.
   **Scénario 2**
   1. If you do not have an [!UICONTROL Adobe ID], to create one, click **[!UICONTROL Get an Adobe ID]** from the [!UICONTROL Request Access] page.
The [!UICONTROL Sign in] page opens.
   2. Click **[!UICONTROL Get an Adobe ID]**.
The [!UICONTROL Sign up] page opens.
   3. Saisissez vos nom et prénom, e-mail et mot de passe.
   4. Sélectionnez **[!UICONTROL S'inscrire]**.
      ![](assets/bplogin_request_access_5.png)
   You are redirected to the [!UICONTROL Request Access] page.

3. La page suivante affiche votre nom et votre ID d'adresse électronique utilisés pour demander l'accès. Faites part de vos commentaires à l’administrateur, puis cliquez sur **[!UICONTROL Envoyer]**.

   ![](assets/bplogin-request-access.png)

## Les administrateurs de produit donnent accès {#grant-access-to-brand-portal}

Les administrateurs du produit de portail de marque reçoivent des demandes d'accès dans leur zone de notification de portail de marque et par courrier électronique dans leur boîte de réception.

![Accéder à la notification demandée](assets/bplogin_request_access_7.png)

To grant access, product administrators need to click the relevant notification in Brand Portal notification area and then click **[!UICONTROL Grant Access]**.
Alternatively, product administrators can follow the link provided in the access request email to visit Adobe [!UICONTROL Admin Console] and add the user to the relevant product configuration.
![](assets/bplogin_request_access_8.png)

You are redirected to the [Adobe [!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview) home page. Use Adobe [!UICONTROL Admin Console] to create users and assign them to product profiles (formerly known as product configurations), which show as groups in Brand Portal. For more information about adding users in [!UICONTROL Admin Console], see [Add a user](brand-portal-adding-users.md#add-a-user) (follow Steps 4-7 in the procedure to add a user).

## Notification de maintenance de Brand Portal {#brand-portal-maintenance-notification}

Avant l’arrêt de Brand Portal pour maintenance, une notification s’affiche sous la forme d’une bannière une fois que vous êtes connecté à Brand Portal. Exemple de notification :

![](assets/bp_maintenance_notification.png)

Vous pouvez ignorer cette notification et continuer à utiliser Brand Portal. Cette notification s'affiche à chaque nouvelle session.

## Version et informations système {#release-and-system-information}

<!--* [What's new](../using/whats-new.md)-->
* [Notes de mise à jour](brand-portal-release-notes.md)
* [Formats de fichiers pris en charge](brand-portal-supported-formats.md)

## Ressources connexes {#related-resources}

* [Assistance clientèle d’Adobe](https://helpx.adobe.com/marketing-cloud/contact-support.html)
* [Forums AEM](https://www.adobe.com/go/aod_forums_en)