---
title: Partage de dossiers
description: Brand Portal nécessite que les ressources soient publiées à partir d’une instance de création Experience Manager Assets préconfigurée. Les utilisateurs non administrateurs peuvent accéder aux ressources publiées uniquement s’ils sont configurés lors de la configuration de la réplication avec Experience Manager. Les ressources doivent également être partagées avec ces utilisateurs.
content-type: reference
topic-tags: sharing
products: SG_EXPERIENCEMANAGER/Brand_Portal
exl-id: d28cf927-60e8-437e-9cba-92f7e19020e7
TQID: https://experienceleague.adobe.com/zcuaWI7GsV39hpBMfzoB9Oiep5IVgmmfz79J-cOm32g
product_v2:
  - id: d09181b5-a36a-43de-ba01-36641440bc43
  - id: fd1f54a9-f50c-467d-8956-cebbaf4f3eb8
feature_v2:
  - id: da0dfbce-df02-4f8b-b32d-a4e3b1d05085
subfeature_v2:
  - id: e00c7c12-7035-41fe-ad76-1ec82c8c3f01
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: e48edcb1ed5d76686794f7a7ed6389c7f4ab1ed3
workflow-type: tm+mt
source-wordcount: 1108
ht-degree: 54%

---

# Partage de dossiers sur Brand Portal {#share-folders}

Les ressources doivent être publiées sur Brand Portal à partir d’une instance de création Experience Manager préconfigurée, car Brand Portal ne prend pas en charge l’ingestion des ressources.

## Workflow de partage de dossiers dans Brand Portal {#folder-sharing-workflow-in-brand-portal}

La section suivante décrit le workflow de partage de dossiers et l’accès utilisateur :

* Par défaut, tous les dossiers publiés depuis Experience Manager Assets sur Brand Portal ne sont visibles que par l’administrateur de Brand Portal, sauf s’ils ont été désignés comme publics lors de la configuration de la réplication.
* L’administrateur utilise la console **[!UICONTROL Propriétés du dossier]** pour partager un dossier avec des utilisateurs ou des groupes sélectionnés. Seuls les utilisateurs ou les groupes avec lesquels le dossier est partagé peuvent voir le dossier après s’être connectés à Brand Portal. Le dossier n’est pas visible par les autres utilisateurs.
* L’administrateur peut également choisir de rendre un dossier public en cochant la case **[!UICONTROL Dossier public]** dans la console **[!UICONTROL Propriétés du dossier]**. Un dossier public est visible par tous les utilisateurs.

* Indépendamment des rôles et des privilèges utilisateur, lorsque des utilisateurs se connectent à Brand Portal, ils voient tous les dossiers publics et les dossiers partagés directement avec eux ou avec un groupe auquel ils appartiennent. Les dossiers privés ou les dossiers partagés avec d’autres utilisateurs ne sont pas visibles par tous les utilisateurs.

### Partage de dossiers avec des groupes d’utilisateurs sur Brand Portal {#sharing-folders-with-user-groups-on-brand-portal}

Les droits d’accès aux ressources d’un dossier dépendent des droits d’accès à son dossier parent, indépendamment des paramètres des dossiers enfants. Les [ACL](https://experienceleague.adobe.com/fr/docs/experience-manager-65/content/security/security) d’AEM régissent ce comportement, les dossiers enfants héritant des ACL de leurs dossiers parents. Supposons, par exemple, que le dossier A contienne le dossier B, qui contient le dossier C. Un groupe d’utilisateurs (ou plusieurs utilisateurs) disposant de droits d’accès sur le dossier A dispose alors des mêmes droits d’accès sur le dossier B et le dossier C. Le dossier B étant le dossier enfant de A hérite de ses listes de contrôle d’accès, et le dossier C étant le dossier enfant de B hérite de ses listes de contrôle d’accès.

De même, les groupes d’utilisateurs (ou utilisateurs) disposant d’autorisations pour accéder uniquement au dossier B disposent des mêmes autorisations d’accès sur le dossier C, mais pas sur le dossier A. Adobe recommande d’organiser le contenu de sorte que les ressources les plus exposées soient placées dans des dossiers enfants, ce qui permet de restreindre l’accès des dossiers enfants jusqu’au dossier racine.

### Publication de dossier public {#public-folder-publish}

Les utilisateurs non administrateurs (tels que les éditeurs et les observateurs) ne peuvent accéder aux ressources publiées d’AEM Assets vers Brand Portal que si l’option **[!UICONTROL Publication de dossier public]** est sélectionnée lors de la configuration de la réplication Brand Portal.

![](assets/assetbpreplication.png)

Si l’option **[!UICONTROL Publication de dossier public]** est désactivée, les administrateurs doivent partager ces ressources spécifiquement avec des utilisateurs non administrateurs à l’aide de la fonctionnalité de partage.

>[!NOTE]
>
>L’option permettant d’activer la **[!UICONTROL publication de dossier public]** est disponible dans AEM à 6.3.2.1.

## Accès aux dossiers partagés {#access-to-shared-folders}

Le tableau suivant décrit les droits d’accès et les droits de partage ou d’annulation du partage de ressources pour divers rôles utilisateur :

|               | Accès à tous les dossiers publiés d’AEM Assets vers Brand Portal | Accès aux dossiers partagés | Partager ou annuler le partage des droits de dossier |
|---------------|-----------|-----------|------------|
| Administrateur | Oui | Oui | Oui |
| Éditeur | Non* | Oui, uniquement s’il est partagé avec eux ou avec le groupe auquel ils appartiennent | Oui, uniquement pour les dossiers partagés avec eux ou avec le groupe auquel ils appartiennent. |
| Observateur | Non* | Oui, uniquement s’il est partagé avec eux ou avec le groupe auquel ils appartiennent | Non |
| Utilisateur visiteur | Non* | Oui, uniquement s’il est partagé avec eux ou avec le groupe auquel ils appartiennent | Non |

>[!NOTE]
>
>Par défaut, l’option **[!UICONTROL Publication de dossier public]** est désactivée lors de la configuration de la réplication de Brand Portal avec un auteur AEM. Si cette option est activée, les dossiers publiés sur Brand Portal sont accessibles par défaut à tous les utilisateurs (y compris les utilisateurs non-administrateurs).

### Accès des utilisateurs non-administrateurs aux dossiers partagés {#non-admin-user-access-to-shared-folders}

Les utilisateurs non-administrateurs ne peuvent accéder qu’aux dossiers partagés avec eux sur Brand Portal. Toutefois, l’affichage de ces dossiers sur le portail lors de la connexion dépend des paramètres de la configuration **[!UICONTROL Activer la hiérarchie de dossiers]**.

**Si la configuration est désactivée**

Les utilisateurs non-administrateurs peuvent voir tous les dossiers partagés avec eux sur la page de destination lors de la connexion au Brand Portal.

![](assets/disabled-folder-hierarchy1-1.png)

**Si la configuration est activée**

Les utilisateurs non-administrateurs voient l’arborescence de dossiers (à partir du dossier racine) et les dossiers partagés organisés dans leurs dossiers parents respectifs, lors de leur connexion à Brand Portal.

Ces dossiers parents sont des dossiers virtuels sur lesquels aucune action ne peut être effectuée. Vous pouvez identifier ces dossiers virtuels grâce à leur icône de cadenas.

Aucune tâche d’action n’est visible lorsque vous les survolez ou les sélectionnez en **[!UICONTROL mode Carte]**, à la différence des dossiers partagés. Le bouton **[!UICONTROL Aperçu]** s’affiche lors de la sélection d’un dossier virtuel dans la vue **[!UICONTROL Colonnes]** et **[!UICONTROL Liste]**.

>[!NOTE]
>
>Notez que la miniature par défaut des dossiers virtuels est l’image de miniature du premier dossier partagé.

![](assets/enabled-hierarchy1-1.png) ![](assets/hierarchy1-nonadmin-1.png) ![](assets/hierarchy-nonadmin-1.png) ![](assets/hierarchy2-nonadmin-1.png)

## Partage de dossiers {#how-to-share-folders}

Pour partager un dossier avec des utilisateurs sur Brand Portal, suivez ces étapes :

1. Cliquez sur l’icône de recouvrement située à gauche, puis sélectionnez **[!UICONTROL Navigation]**.

   ![](assets/selectorrail.png)

1. Dans le rail latéral sur la gauche, sélectionnez **[!UICONTROL Fichiers]**.

   ![](assets/access_files.png)

1. Dans l’interface de Brand Portal, sélectionnez le dossier que vous souhaitez partager.

   ![](assets/share-folders.png)

1. Dans la barre d’outils supérieure, sélectionnez **[!UICONTROL Partager]**.

   ![](assets/share_icon.png)

   La console [!UICONTROL Propriétés du dossier] s’affiche.

   ![](assets/folder_properties.png)

1. Dans la console **[!UICONTROL Propriétés du dossier]**, spécifiez le titre du dossier dans le champ **[!UICONTROL Titre du dossier]** si vous ne souhaitez pas que le nom par défaut s’affiche pour les utilisateurs.
1. Dans la liste **[!UICONTROL Ajouter un utilisateur]**, sélectionnez les utilisateurs ou les groupes avec lesquels vous souhaitez partager le dossier et cliquez sur **[!UICONTROL Ajouter]**.
Pour partager le dossier uniquement avec les utilisateurs invités, et aucun autre utilisateur, sélectionnez **[!UICONTROL Utilisateurs anonymes]** dans le menu déroulant **[!UICONTROL Membres]**.

   ![](assets/only-anonymous.png)

   >[!NOTE]
   >
   >Pour que le dossier soit disponible pour tous les utilisateurs, quel que soit le groupe auquel ils appartiennent et leur rôle, rendez-le public en activant la case à cocher **[!UICONTROL Dossier public]**.

1. Si nécessaire, cliquez sur **[!UICONTROL Modifier la miniature]** pour modifier l’image de miniature du dossier.
1. Cliquez sur **[!UICONTROL Enregistrer]**.

1. Pour accéder au dossier partagé, connectez-vous à Brand Portal à l’aide des informations d’identification de l’utilisateur avec lequel vous avez partagé le dossier. Examinez le dossier partagé dans l’interface.

## Annulation du partage de dossiers {#unshare-the-folders}

Pour annuler le partage d’un dossier précédemment partagé, procédez comme suit :

1. Dans l’interface de Brand Portal, sélectionnez le dossier dont vous souhaitez annuler le partage.

   ![](assets/share-folders-1.png)

1. Dans la barre d’outils supérieure, cliquez sur **[!UICONTROL Partager]**.
1. Dans la console **[!UICONTROL Propriétés du dossier]**, sous **[!UICONTROL Membres]**, cliquez sur le symbole **[!UICONTROL x]** situé en regard d’un utilisateur pour le supprimer de la liste des utilisateurs avec lesquels vous avez partagé le dossier.

   ![](assets/folder_propertiesunshare.png)

1. Dans la boîte de message d’avertissement, cliquez sur **[!UICONTROL Confirmer]** pour confirmer l’annulation du partage.
Cliquez sur **[!UICONTROL Enregistrer]**.

1. Connectez-vous à Brand Portal avec les informations d’identification de l’utilisateur que vous avez supprimé de la liste de partage. Le dossier n’est plus disponible dans l’interface Brand Portal de l’utilisateur.
