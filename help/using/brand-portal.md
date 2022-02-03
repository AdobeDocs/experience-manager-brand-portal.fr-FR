---
title: Aperçu d’Experience Manager Assets Brand Portal
seo-title: Overview of Experience Manager Assets Brand Portal
description: Experience Manager Assets Brand Portal permet d’acquérir, de contrôler et de distribuer facilement et en toute sécurité des ressources créatives destinées à des tiers externes et aux collaborateurs de l’entreprise sur différents appareils.
seo-description: Experience Manager Assets Brand Portal can help you easily acquire, control, and securely distribute approved creative assets to external parties and internal business users across devices.
uuid: b1e54d03-eb2e-488e-af4d-bae817dd135a
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: introduction
discoiquuid: 6aefa298-4728-4b8e-a85b-e419ee37f2f4
exl-id: 0f2c45e4-416e-451a-905b-06c5e42a9272
source-git-commit: 12187c4a98e1541be27b06eefedb1b654c5fb083
workflow-type: tm+mt
source-wordcount: '1528'
ht-degree: 100%

---

# Aperçu d’Experience Manager Assets Brand Portal {#overview-of-aem-assets-brand-portal}

En tant que marketeur, vous devez parfois collaborer avec des partenaires de distribution et des collaborateurs de l’entreprise pour créer, gérer et diffuser rapidement du contenu numérique pertinent à vos clients. La diffusion au bon moment de contenu pertinent tout le long du parcours client est essentielle pour accroître la demande, la conversion, l’engagement et la fidélisation des clients.

Il est toutefois difficile de développer des solutions qui permettent le partage efficace et sécurisé de logos de la marque, d’instructions, de ressources de campagne ou de clichés de produit avec des équipes internes, des partenaires et des revendeurs.

**Adobe Experience Manager (AEM) Assets Brand Portal** est axé sur la nécessité pour le marketeur de collaborer efficacement avec les utilisateurs de Brand Portal répartis dans le monde entier, en offrant des fonctionnalités de distribution et de contribution aux ressources.

La distribution des ressources permet d’acquérir, de contrôler et de distribuer facilement et en toute sécurité des ressources créatives destinées à des tiers externes et aux collaborateurs de l’entreprise sur différents appareils. La contribution aux ressources permet aux utilisateurs de Brand Portal de charger des ressources sur Brand Portal et de les publier sur Experience Manager Assets, sans avoir à accéder à l’environnement de création. La fonction de contribution est appelée **Approvisionnement des ressources dans Brand Portal**. Ces deux fonctionnalités améliorent l’expérience globale en matière de distribution et de contribution aux ressources des utilisateurs de Brand Portal (agences/équipes externes), accélèrent le délai de mise sur le marché des ressources et réduisent le risque de non-conformité et d’accès non autorisé.
Voir [Approvisionnement des ressources dans Brand Portal](brand-portal-asset-sourcing.md).

L’environnement de portail de type navigateur permet de télécharger, parcourir, rechercher, prévisualiser et exporter facilement des ressources dans des formats approuvés.

## Configuration d’Experience Manager Assets avec Brand Portal {#configure-brand-portal}

La configuration d’Adobe Experience Manager Assets avec Brand Portal permet aux utilisateurs de Brand Portal de bénéficier de fonctions de publication, de distribution et de contribution des ressources.

>[!NOTE]
>
>La configuration d’Experience Manager Assets avec Brand Portal est prise en charge dans Experience Manager Assets as a Cloud Service, Experience Manager Assets 6.3 et les versions ultérieures.

Experience Manager Assets as a Cloud Service est automatiquement configuré avec Brand Portal en activant celui-ci à partir de Cloud Manager. Le workflow d’activation crée les configurations requises en arrière-plan et active Brand Portal sur la même organisation IMS qu’Experience Manager Assets as a Cloud Service.

En revanche, Experience Manager Assets (On-Premise et Managed Service) est configuré avec Brand Portal à l’aide d’Adobe Developer Console qui fournit un jeton Adobe Identity Management Services (IMS) pour l’autorisation du client Brand Portal.

Pour plus d’informations, consultez [Configuration d’Experience Manager Assets avec Brand Portal](../using/configure-aem-assets-with-brand-portal.md).

## Différents types d’utilisateurs de Brand Portal {#Personas}

Brand Portal prend en charge les rôles utilisateur suivants :

* Utilisateur invité
* Observateur
* Éditeur
* Administrateur

Le tableau suivant répertorie les tâches que peuvent réaliser les utilisateurs qui disposent de ces rôles :

|  | **Parcourir** | **Rechercher** | **Télécharger** | **Partage de dossiers** | **Partage d’une collection** | **Partager des ressources en tant que lien** | **Accéder aux outils d’administration** |
|--- |--- |--- |--- |--- |--- |--- |--- |
| **Utilisateur invité** | ✓* | ✓* | ✓* | x | x | x | x |
| **Observateur** | ✓ | ✓ | ✓ | x | x | x | x |
| **Éditeur** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | x |
| **Administrateur** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |

>[!NOTE]
>
>Les utilisateurs invités peuvent explorer des ressources, y accéder et en rechercher dans les dossiers et collections publics uniquement.

<!--
&#42; Viewer users can access and download the public assets shared with them, and can add these assets to create their own collections.

>[!NOTE]
>
>There is a known issue that the share link for collections is currently visible to the viewer users. The viewer users does not have the privilege to add users to create a share link. This issue will be fixed in the upcoming release, the option to share link for the collections will not be available to the viewer users.
-->

### Utilisateur invité {#guest-user}

Tout utilisateur disposant d’un accès limité aux ressources sur Brand Portal sans passer par une authentification est un utilisateur invité. La session d’invité permet aux utilisateurs d’accéder aux dossiers et collections publics. En tant qu’utilisateur invité, vous pouvez explorer les détails des ressources et bénéficier d’une vue complète sur les ressources des membres des dossiers et collections publics. Vous pouvez rechercher, télécharger et ajouter des ressources publiques à une collection [!UICONTROL Lightbox].

La session d’invité vous empêche toutefois de créer des collections et des recherches enregistrées, et de les partager. Lors d’une session d’invité, les utilisateurs ne peuvent ni accéder aux paramètres des dossiers et des collections, ni partager des ressources sous la forme de lien. Voici la liste des tâches que peut réaliser un utilisateur invité :

* [Exploration et accès aux ressources publiques](browse-assets-brand-portal.md)

* [Recherche parmi les ressources publiques](brand-portal-searching.md)

* [Téléchargement de ressources publiques](download-assets.md)

* [Ajout de ressources à [!UICONTROL Lightbox]](brand-portal-light-box.md#add-assets-to-lightbox)

### Observateur {#viewer}

Dans Brand Portal, un utilisateur standard est généralement un utilisateur qui dispose du rôle Visualisateur. Un utilisateur qui dispose de ce rôle peut accéder aux dossiers, aux collections et aux ressources autorisés. L’utilisateur peut également parcourir, prévisualiser, télécharger et exporter des ressources (rendus d’origine ou spécifiques), configurer des paramètres de compte et rechercher des ressources. Voici la liste des tâches que peut réaliser un observateur :

* [Exploration des ressources](browse-assets-brand-portal.md)

* [Recherche de ressources](brand-portal-searching.md)

* [Téléchargement de ressources](download-assets.md)

### Éditeur {#editor}

Un utilisateur qui dispose du rôle d’éditeur peut effectuer toutes les tâches d’un observateur. En complément, il peut visualiser les fichiers et dossiers partagés par un administrateur. L’utilisateur qui dispose du rôle d’éditeur peut également partager du contenu (fichiers, dossiers, collections) avec d’autres personnes.

En plus des tâches d’un observateur, un éditeur peut effectuer les tâches suivantes :

* [Partage de dossiers](brand-portal-sharing-folders.md)

* [Partage d’une collection](brand-portal-share-collection.md)

* [Partage de ressources en tant que lien](brand-portal-link-share.md)

### Administrateur {#administrator}

Un administrateur comprend un utilisateur désigné comme administrateur système ou administrateur de produit Brand Portal dans [!UICONTROL Admin Console]. Un administrateur peut ajouter et supprimer des administrateurs système et des utilisateurs, définir des paramètres prédéfinis, envoyer des e-mails aux utilisateurs et afficher des rapports sur l’utilisation et le stockage du portail.

Un administrateur peut effectuer toutes les tâches exécutées par un éditeur, ainsi que les tâches suivantes :

* [Gestion des utilisateurs, des groupes et des rôles utilisateur](brand-portal-adding-users.md)

* [Personnalisation du papier peint, des en-têtes de page et des e-mails](brand-portal-branding.md)

* [Utilisation des facettes de recherche personnalisée](brand-portal-search-facets.md)

* [Utilisation du formulaire de schéma de métadonnées](brand-portal-metadata-schemas.md)

* [Application de paramètres d’image prédéfinis ou de rendus dynamiques](brand-portal-image-presets.md)

* [Utilisation des rapports](brand-portal-reports.md)

En plus des tâches mentionnées ci-dessus, un auteur dans AEM Assets peut effectuer les tâches suivantes :

* [Configuration d’AEM Assets avec Brand Portal](../using/configure-aem-assets-with-brand-portal.md)

* [Publication de dossiers sur Brand Portal](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/brand-portal-publish-folder.html?lang=fr)

* [Publication de collections sur Brand Portal](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/brand-portal-publish-collection.html?lang=fr)

## Autre alias pour l’URL de Brand Portal {#tenant-alias-for-portal-url}

À partir de Brand Portal 6.4.3, les entreprises peuvent avoir une autre URL (alias) pour l’URL existante de leur client Brand Portal. L’URL d’alias peut être créée avec un autre préfixe dans l’URL.\
Notez que seul le préfixe de l’URL Brand Portal peut être personnalisé et non l’URL entière. Par exemple, une entreprise avec le domaine existant `geomettrix.brand-portal.adobe.com` peut demander et obtenir la création de `geomettrixinc.brand-portal.adobe.com`.

Cependant, l’instance d’auteur AEM peut uniquement être [configurée](../using/configure-aem-assets-with-brand-portal.md) avec l’URL d’ID du client et non avec l’URL (alternative) d’alias de client.

>[!NOTE]
>
>Pour obtenir un alias pour le nom du client dans l’URL de portail existante, les organisations doivent solliciter la création d’un alias de client auprès de le service clientèle. Cette demande est traitée en vérifiant d’abord si l’alias est disponible puis en le créant.
>
>Pour remplacer ou supprimer l’ancien alias, le même processus doit être suivi.

## Demande d’accès à Brand Portal {#request-access-to-brand-portal}

Les utilisateurs peuvent demander l’accès à Brand Portal depuis l’écran de connexion. Ces demandes sont envoyées aux administrateurs de Brand Portal qui accordent l’accès aux utilisateurs via Adobe [!UICONTROL Admin Console]. Une fois l’accès accordé, les utilisateurs reçoivent une notification par e-mail.

Pour demander l’accès, procédez comme suit :

1. Sur la page de connexion de Brand Portal, sélectionnez **[!UICONTROL Cliquez ici]** en regard de **[!UICONTROL Besoin d’un accès ?]**. En revanche, pour créer une session d’invité, sélectionnez **[!UICONTROL Cliquez ici]** en regard de **[!UICONTROL Accès d’invité ?]**.

   ![Écran de connexion de Brand Portal](assets/bp-login-requestaccess.png)

   La page [!UICONTROL Demander l’accès] s’affiche.

1. Pour pouvoir demander l’accès au portail Brand Portal d’une entreprise, vous devez disposer d’un [!UICONTROL Adobe ID], d’un [!UICONTROL Enterprise ID] ou d’un [!UICONTROL Federated ID] valide.

   Dans la page [!UICONTROL Demander l’accès], connectez-vous à l’aide de votre ID (scénario 1) ou créez un [!UICONTROL Adobe ID] (scénario 2) :

   ![[!UICONTROL Demander l’accès]](assets/bplogin_request_access_2.png)

   **Scénario 1**

   1. Si vous disposez d’un [!UICONTROL Adobe ID], d’un [!UICONTROL Enterprise ID] ou d’un [!UICONTROL Federated ID], cliquez sur **[!UICONTROL Se connecter]**.
La page [!UICONTROL Se connecter] s’affiche.

   1. Saisissez votre [!UICONTROL Adobe ID], puis cliquez sur **[!UICONTROL Se connecter]**.

      ![Connexion à Adobe](assets/bplogin_request_access_3.png)
   Vous êtes redirigé vers la page [!UICONTROL Demander l’accès].

   **Scénario 2**

   1. Si vous ne possédez pas d’[!UICONTROL Adobe ID], pour en créer un, cliquez sur **[!UICONTROL Obtenir un Adobe ID]** dans la page [!UICONTROL Demander l’accès].
La page [!UICONTROL Se connecter] s’affiche.
   1. Cliquez sur **[!UICONTROL Obtenir un Adobe ID]**.
La page [!UICONTROL S’inscrire] s’affiche.
   1. Saisissez vos nom et prénom, e-mail et mot de passe.
   1. Sélectionnez **[!UICONTROL S’inscrire]**.

      ![](assets/bplogin_request_access_5.png)
   Vous êtes redirigé vers la page [!UICONTROL Demander l’accès].

1. La page suivante affiche vos nom et e-mail utilisés pour la demande d’accès. Faites part de vos commentaires à l’administrateur, puis cliquez sur **[!UICONTROL Envoyer]**.

   ![](assets/bplogin-request-access.png)

## Les administrateurs de produit accordent les accès {#grant-access-to-brand-portal}

Les administrateurs de produit Brand Portal reçoivent les demandes d’accès dans leur zone de notification de Brand Portal et par e-mail dans leur boîte de réception.

![Notification de demande d’accès](assets/bplogin_request_access_7.png)

Pour accorder un accès, les administrateurs de produit doivent cliquer sur la notification correspondante dans la zone de notification de Brand Portal, puis sur **[!UICONTROL Accorder l’accès]**.
Les administrateurs de produit peuvent aussi suivre le lien contenu dans l’e-mail de demande d’accès afin d’accéder à Adobe [!UICONTROL Admin Console] et d’ajouter l’utilisateur à la configuration de produit adéquate.

Vous êtes redirigé vers la page d’accueil d’[Adobe [!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview). Utilisez Adobe [!UICONTROL Admin Console] pour créer des utilisateurs et les affecter à des profils de produit (auparavant appelés configurations de produit), qui s’affichent sous la forme de groupes dans Brand Portal. Pour plus d’informations sur l’ajout d’utilisateurs dans [!UICONTROL Admin Console], voir [Ajout d’un utilisateur](brand-portal-adding-users.md#add-a-user) (suivez les étapes 4 à 7 de la procédure pour ajouter un utilisateur).

## Langues de Brand Portal {#brand-portal-language}

Vous pouvez modifier la langue de Brand Portal à partir des [!UICONTROL paramètres d’Adobe Experience Cloud].

![Notification de demande d’accès](assets/BPLang.png)

Pour modifier la langue :

1. Sélectionnez [!UICONTROL Utilisateur] > [!UICONTROL Modifier le profil] dans le menu supérieur.

   ![Modifier le profil](assets/EditBPProfile.png)

1. Sur la page [!UICONTROL Paramètres Adobe Experience Cloud], sélectionnez une langue dans le menu déroulant [!UICONTROL Langue].

## Notification de maintenance de Brand Portal {#brand-portal-maintenance-notification}

Avant l’arrêt de Brand Portal pour maintenance, une notification s’affiche sous la forme d’une bannière une fois que vous êtes connecté à Brand Portal. Exemple de notification :

![](assets/bp_maintenance_notification.png)

Vous pouvez ignorer cette notification et continuer à utiliser Brand Portal. Cette notification apparaît dans chaque nouvelle session.

## Version et informations système {#release-and-system-information}

* [Nouveautés](whats-new.md)
* [Notes de mise à jour](brand-portal-release-notes.md)
* [Formats de fichiers pris en charge](brand-portal-supported-formats.md)

## Ressources connexes {#related-resources}

<!--
* [Adobe Customer Support]()
-->

* [Forums AEM](https://experienceleaguecommunities.adobe.com/t5/adobe-experience-manager/ct-p/adobe-experience-manager-community)
