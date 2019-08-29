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
source-git-commit: 770c353b1143d879280df310012ce9d4d30b40c9

---


# Présentation d’AEM Assets Brand Portal {#overview-of-aem-assets-brand-portal}

En tant que spécialiste du marketing, il est parfois nécessaire de collaborer avec les partenaires de canaux et les utilisateurs internes pour créer, gérer et diffuser rapidement du contenu numérique pertinent aux clients. La diffusion au bon moment de contenu pertinent tout le long du parcours client est essentielle pour accroître la demande, la conversion, l’engagement et la fidélisation des clients.

Il est toutefois difficile de développer des solutions qui permettent le partage efficace et en toute sécurité de logos de la marque, d’instructions, de ressources de campagne ou de clichés de produit avec des équipes internes, des partenaires et des revendeurs.

**[!DNL Adobe Experience Manager (AEM) Assets Brand Portal]** permet d’acquérir, de contrôler et de distribuer facilement et en toute sécurité des ressources créatives destinées à des tiers externes et aux collaborateurs de l’entreprise sur différents appareils. Brand Portal améliore l’efficacité du partage des ressources, accélère la mise sur le marché des ressources et réduit les risques de non-conformité et d’accès non autorisé.

L'environnement de portail basé sur un navigateur vous permet de télécharger, parcourir, rechercher, prévisualiser et exporter facilement des fichiers dans des formats approuvés.

## Utilisateurs de l'utilisateur dans Brand Portal {#Personas}

[!DNL Brand Portal] prend en charge les rôles utilisateur suivants :

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

Any user having limited access to assets on [!DNL Brand Portal] without undergoing authentication is a guest user. La session d'invités permet aux utilisateurs d'accéder aux dossiers publics et aux collections. En tant qu'utilisateur invité, vous pouvez parcourir les détails des ressources et avoir une vue complète des ressources des membres de dossiers publics et de collections. You can search, download, and add public assets to [!UICONTROL lightbox collection].

La session d’invité vous empêche toutefois de créer des collections et des recherches enregistrées et de les partager. Lors d’une session d’invité,  les utilisateurs ne peuvent ni accéder aux paramètres des dossiers et collections, ni partager des ressources sous la forme de lien. Voici la liste des tâches qu'un utilisateur invité peut effectuer :

[Exploration et accès aux ressources publiques](browse-assets-brand-portal.md)

[Recherche parmi les ressources publiques](brand-portal-searching.md)

[Téléchargement de ressources publiques](brand-portal-download-users.md)

[Ajout de ressources à [! UICONTROL lightbox]](brand-portal-light-box.md#add-assets-to-lightbox)

### Observateur {#viewer}

A standard user in [!DNL Brand Portal] is typically a user with the role of Viewer. Un utilisateur qui dispose de ce rôle peut accéder aux fichiers, aux collections et aux ressources autorisés. L’utilisateur peut également parcourir, prévisualiser, télécharger et exporter des ressources (rendus d’origine ou spécifiques), configurer des paramètres de compte et rechercher des ressources. Voici la liste des tâches que peut réaliser un visualisateur :

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

An administrator includes a user marked as system administrator or [!DNL Brand Portal] product administrator in [!UICONTROL Admin Console]. Un administrateur peut ajouter et supprimer des administrateurs système et des utilisateurs, définir des paramètres prédéfinis, envoyer des e-mails aux utilisateurs et afficher des rapports sur l’utilisation et le stockage du portail.

Un administrateur peut effectuer toutes les tâches exécutées par un éditeur, ainsi que les tâches suivantes :

[Gestion des utilisateurs, des groupes et des rôles utilisateur](brand-portal-adding-users.md)

[Personnalisation du papier peint, des en-têtes de page et des e-mails](brand-portal-branding.md)

[Utilisation des facettes de recherche personnalisée](brand-portal-search-facets.md)

[Utilisation du formulaire de schéma de métadonnées](brand-portal-metadata-schemas.md)

[Application de paramètres d’image prédéfinis ou de rendus dynamiques](brand-portal-image-presets.md)

[Utilisation des rapports](brand-portal-reports.md)

In addition to the above tasks, an Author in [!DNL AEM Assets] can perform the following tasks:

[Configurer [! Intégration DNL Assets] intégration avec [! DNL Brand Portal]](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html)

[Publication des dossiers vers [! DNL Brand Portal]](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-publish-folder.html)

[Publier des collections dans [! DNL Brand Portal]](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-publish-collection.html)

## Alias alternatif pour l'URL de Portal Portal {#tenant-alias-for-portal-url}

[!DNL Brand Portal] 6.4.3, les organisations peuvent avoir une URL alternative (alias) pour l'URL existante de leur [!DNL Brand Portal] client. Vous pouvez créer l'URL d'alias en utilisant un autre préfixe dans l'URL.\
Note that only the prefix of the [!DNL Brand Portal] URL can be customized and not the entire URL. For example, an organization with existing domain **[!UICONTROL geomettrix.brand-portal.adobe.com]** can get **[!UICONTROL geomettrixinc.brand-portal.adobe.com]** created on request.

However, **[!DNL AEM] Author instance can be [configured](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html) only with the tenant id URL and not with tenant alias (alternate) URL.

>[!NOTE]
>
>To get an alias for tenant name in existing portal URL, organizations need to contact **[!DNL Adobe support] with a new tenant alias creation request. Cette demande est traitée en vérifiant d’abord si l’alias est disponible puis en le créant.
>
>Pour remplacer ou supprimer l’ancien alias, le même processus doit être suivi.

## Demande d’accès à Brand Portal {#request-access-to-brand-portal}

Users can request access to [!DNL Brand Portal] from the login screen. These requests are sent to [!DNL Brand Portal] administrators, who grant access to users through the Adobe Admin Console. Une fois l’accès accordé, les utilisateurs reçoivent une notification par e-mail.

Pour demander l’accès, procédez comme suit :

1. From the [!DNL Brand Portal] login page, select the **Click here** corresponding to **Need Access?**. However, to enter the guest session, select the **Click here** corresponding to **Guest Access?**.

   ![Écran de connexion de Brand Portal](assets/bp-login-requestaccess.png)

   La page **Demander l’accès** s’affiche.

2. To be able to request access to an organization’s [!DNL Brand Portal], you must have a valid [!UICONTROL Adobe ID], [!UICONTROL Enterprise ID], or [!UICONTROL Federated ID].

   In the **Request Access** page, sign in using your ID (scenario 1) or create an [!UICONTROL Adobe ID] (scenario 2):
   ![Demande d'accès](assets/bplogin_request_access_2.png)

   **Scénario 1**
   1. If you have an [!UICONTROL Adobe ID], [!UICONTROL Enterprise ID], or [!UICONTROL Federated ID], click **Sign In**.
The **Sign in** page opens.
   2. Provide your [!UICONTROL Adobe ID] credentials and click **Sign in**.
      ![Adobe sign in](assets/bplogin_request_access_3.png)
   You are redirected to the **Request Access** page.
   **Scénario 2**
   1. If you do not have an [!UICONTROL Adobe ID], to create one, click **Get an Adobe ID** from the **Request Access** page.
The **Sign in** page opens.
   2. Click **Get an Adobe ID**.
The **Sign up** page opens.
   3. Saisissez vos nom et prénom, e-mail et mot de passe. Click **Sign up**.
      ![](assets/bplogin_request_access_5.png)
   You are redirected to the **Request Access** page.

3. La page suivante affiche votre nom et votre ID d'adresse électronique utilisés pour demander l'accès. Faites part de vos commentaires à l’administrateur, puis cliquez sur **Envoyer**.

   ![](assets/bplogin-request-access.png)

## Les administrateurs de produit donnent accès {#grant-access-to-brand-portal}

[!DNL Brand Portal] les administrateurs de produit reçoivent les demandes d'accès dans leur zone [!DNL Brand Portal] de notification et par courrier électronique dans leur boîte de réception.

![Accéder à la notification demandée](assets/bplogin_request_access_7.png)

Pour accorder l'accès, les administrateurs de produit doivent cliquer sur la notification appropriée dans [!DNL Brand Portal] la zone de notification, puis sur **Octroyer l'accès**.
Alternatively, product administrators can follow the link provided in the access request email to visit [!DNL Adobe Admin Console] and add the user to the relevant product configuration.
![](assets/bplogin_request_access_8.png)

You are redirected to the [[!DNL Adobe Admin Console]](https://adminconsole.adobe.com/enterprise/overview) home page. Use [!DNL Adobe Admin Console] to create users and assign them to product profiles (formerly known as product configurations), which show as groups in [!DNL Brand Portal]. For more information about adding users in [!DNL Admin Console], see [Add a user](brand-portal-adding-users.md#add-a-user) (follow Steps 4-7 in the procedure to add a user).

## Notification de maintenance de Brand Portal {#brand-portal-maintenance-notification}

Before [!DNL Brand Portal] is scheduled to go down for maintenance, a notification is displayed as a banner after you log in to [!DNL Brand Portal]. Exemple de notification :

![](assets/bp_maintenance_notification.png)

Vous pouvez ignorer cette notification et continuer à utiliser [!DNL Brand Portal]. Cette notification s'affiche à chaque nouvelle session.

## Version et informations système {#release-and-system-information}

<!--* [What's new](../using/whats-new.md)-->
* [Notes de mise à jour](brand-portal-release-notes.md)
* [Formats de fichiers pris en charge](brand-portal-supported-formats.md)

## Ressources connexes {#related-resources}

* [Assistance clientèle d’Adobe](https://helpx.adobe.com/marketing-cloud/contact-support.html)
* [Forums AEM](https://www.adobe.com/go/aod_forums_en)