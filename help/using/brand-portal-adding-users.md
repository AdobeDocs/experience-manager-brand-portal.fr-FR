---
title: Gestion des utilisateurs, des groupes et des rôles utilisateur
description: Découvrez comment les administrateurs peuvent utiliser Adobe Admin Console pour créer des utilisateurs et des profils de produits Brand Portal, et gérer leurs rôles à l’aide de l’interface utilisateur de Brand Portal. Ce privilège n’est pas disponible pour les observateurs et les éditeurs.
content-type: reference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
role: Admin
exl-id: 35b1fd75-f9e4-4145-80bd-84de091f8b2b
TQID: https://experienceleague.adobe.com/CxUuu1tgxUNjW4TD-vgW-LGn2y9-4avL-mc9eykqBQM
product_v2: id: d09181b5-a36a-43de-ba01-36641440bc43id: fd1f54a9-f50c-467d-8956-cebbaf4f3eb8
feature_v2: id: cda65036-5305-4f01-89da-9b3506ae8c50id: da0dfbce-df02-4f8b-b32d-a4e3b1d05085
subfeature_v2: id: e00c7c12-7035-41fe-ad76-1ec82c8c3f01
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e48edcb1ed5d76686794f7a7ed6389c7f4ab1ed3
workflow-type: tm+mt
source-wordcount: 2233
ht-degree: 57%

---

# Gestion des utilisateurs, des groupes et des rôles utilisateur {#manage-users-groups-and-user-roles}

Les administrateurs peuvent utiliser Adobe Admin Console pour créer des utilisateurs et des profils de produits Experience Manager Assets Brand Portal, et gérer leurs rôles à l’aide de l’interface utilisateur de Brand Portal. Ce privilège n’est pas disponible pour les observateurs et les éditeurs.

Dans [[!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview), vous pouvez visualiser tous les produits associés à votre entreprise. Un produit peut être n’importe quelle solution Experience Cloud (Adobe Analytics, Adobe Target ou Experience Manager Assets Brand Portal, par exemple). Choisissez le produit AEM Brand Portal et créez des profils de produit.

<!--
Comment Type: draft

<note type="note">
<p>Product profiles (formerly known as product configurations*). </p>
<p>* The nomenclature has changed from product configurations to Product Profiles in the new Adobe Admin Console.</p>
</note>
-->
![](assets/create-user-group.png)

Ces profils de produit sont synchronisés avec l’interface utilisateur de Brand Portal toutes les 8 heures et visibles en tant que groupes dans Brand Portal. Une fois que vous avez ajouté des utilisateurs, créé des profils de produit et ajouté des utilisateurs à ces profils de produit, vous pouvez affecter des rôles aux utilisateurs et aux groupes dans Brand Portal.

>[!NOTE]
>
>Pour créer des groupes dans Brand Portal, dans [!UICONTROL Admin Console], utilisez **[!UICONTROL Produits > Profils de produit]** au lieu de la page **[!UICONTROL Utilisateur > Groupes d’utilisateurs]**. Dans Adobe [!UICONTROL Admin Console], les profils de produit servent à créer des groupes dans Brand Portal.

## Ajout d’un utilisateur {#add-a-user}

Si vous êtes administrateur de produit, utilisez Adobe [[!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview) pour créer des utilisateurs et les affecter à des profils de produit (*anciennement appelés configurations de produit*), qui s’affichent sous la forme de groupes dans Brand Portal. Vous pouvez utiliser des groupes pour effectuer des opérations en bloc comme gérer les rôles et partager des ressources.

>[!NOTE]
>
>Les nouveaux utilisateurs qui n’ont pas accès à Brand Portal peuvent demander l’accès à partir de l’écran de connexion de Brand Portal. Pour plus d’informations, voir [Demande d’accès à Brand Portal](../using/brand-portal.md#request-access-to-brand-portal). Une fois que vous avez reçu les notifications de demande d’accès dans votre zone de notification, cliquez sur la notification adéquate, puis sur **[!UICONTROL Autoriser l’accès]**. Vous pouvez également cliquer sur le lien figurant dans l’e-mail de demande d’accès reçu. Ensuite, pour ajouter un utilisateur par le biais d’[Adobe [!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview), suivez les étapes 4 à 7 de la procédure ci-dessous.

>[!NOTE]
>
>Vous pouvez vous connecter à [Adobe [!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview) directement ou depuis Brand Portal. Si vous vous connectez directement, suivez les étapes 4 à 7 ci-dessous pour ajouter un utilisateur.

1. Dans la barre d’outils AEM supérieure, cliquez sur le logo Adobe pour accéder aux outils d’administration.

   ![Logo AEM](assets/aemlogo.png)

1. Dans le panneau des outils d’administration, cliquez sur **[!UICONTROL Utilisateurs]**.

   ![Panneau Outils d’administration](assets/admin-tools-panel-5.png)

1. Dans la page [!UICONTROL Rôles utilisateur], cliquez sur l’onglet **[!UICONTROL Gestion]**, puis sur **[!UICONTROL Lancer Admin Console]**.

   ![Rôles utilisateur pour lancer Admin Console](assets/launch_admin_console.png)

1. Dans Admin Console, effectuez l’une des opérations suivantes pour créer un utilisateur :

   * Dans la barre d’outils supérieure, cliquez sur **[!UICONTROL Aperçu]**. Sur la page [!UICONTROL Aperçu], cliquez sur **[!UICONTROL Affecter des utilisateurs]** depuis la carte du produit Brand Portal.

   ![Présentation d’Admin Console](assets/admin_console_overviewadduser.png)

   * Dans la barre d’outils supérieure, cliquez sur **[!UICONTROL Utilisateurs]**. Sur la page [!UICONTROL Utilisateurs], [!UICONTROL Utilisateurs] dans le rail de gauche sont sélectionnés par défaut. Cliquez sur **[!UICONTROL Ajouter un utilisateur]**.

   ![Ajout d’utilisateurs dans Admin Console](assets/admin_console_adduseruserpage.png)

1. Dans la boîte de dialogue Ajouter un utilisateur , saisissez l’ID d’e-mail de l’utilisateur que vous souhaitez ajouter ou sélectionnez-le dans la liste des suggestions qui s’affichent lorsque vous saisissez .

   ![Ajout d’un utilisateur à Brand Portal](assets/add_user_to_aem_bp.png)

1. Affectez l’utilisateur à au moins un profil de produit (auparavant appelé configurations de produit) afin qu’il puisse accéder à Brand Portal. Sélectionnez le profil de produit adéquat dans le champ **[!UICONTROL Sélectionnez un profil pour ce produit]**.
1. Cliquez sur **[!UICONTROL Enregistrer]**. Un e-mail de bienvenue est envoyé à l’utilisateur qui vient d’être ajouté. L’utilisateur invité peut cliquer sur le lien contenu dans l’e-mail de bienvenue pour accéder à Brand Portal. L’utilisateur peut se connecter à l’aide de l’ID d’e-mail (, [!UICONTROL Enterprise ID] ou [!UICONTROL Federated ID]) configuré dans Admin Console. Pour plus d’informations, voir [Première connexion](../using/brand-portal-onboarding.md).

   >[!NOTE]
   >
   >Si un utilisateur ne parvient pas à se connecter à Brand Portal, l’administrateur de l’organisation doit se rendre sur l’Admin Console Adobe . Vérifiez si l’utilisateur est présent et s’il a été ajouté à au moins un profil de produit.

   Pour plus d’informations sur l’octroi de privilèges d’administrateur, voir [Octroi de privilèges d’administrateur aux utilisateurs](../using/brand-portal-adding-users.md#provideadministratorprivilegestousers).

## Ajout d’un profil de produit {#add-a-product-profile}

Dans [!UICONTROL Admin Console], les profils de produit (auparavant appelés configurations de produit) servent à créer des groupes dans Brand Portal afin d’effectuer des opérations en bloc comme gérer les rôles et partager des ressources dans Brand Portal. **** est le profil de produit par défaut disponible ; vous pouvez créer d&#39;autres profils de produit et ajouter des utilisateurs aux nouveaux profils de produit.

>[!NOTE]
>
>Vous pouvez vous connecter à [](https://adminconsole.adobe.com/enterprise/overview) directement ou depuis Brand Portal. Si vous vous connectez directement à , suivez les étapes 4 à 7 de la procédure ci-dessous pour ajouter un profil de produit.

1. Dans la barre d’outils AEM supérieure, cliquez sur le logo Adobe pour accéder aux outils d’administration.

   ![Logo AEM](assets/aemlogo.png)

1. Dans le panneau des outils d’administration, cliquez sur **[!UICONTROL Utilisateurs]**.

   ![Panneau Outils d’administration](assets/admin-tools-panel-6.png)

1. Dans la page [!UICONTROL Rôles utilisateur], cliquez sur l’onglet **[!UICONTROL Gestion]**, puis sur **[!UICONTROL Lancer Admin Console]**.

   ![Lancement d’Admin Console](assets/launch_admin_console.png)

1. Dans la barre d’outils supérieure, cliquez sur **[!UICONTROL Produits]**.
1. Sur la page [!UICONTROL Produits], [!UICONTROL Profils de produit] sont sélectionnés par défaut. Cliquez sur **[!UICONTROL Nouveau profil]**.

   ![Ajout d’un nouveau profil de produit](assets/admin_console_addproductprofile.png)

1. Sur la page [!UICONTROL Créer un profil], indiquez le nom du profil, le nom d’affichage et la description du profil. Choisissez de notifier les utilisateurs par e-mail lorsqu’ils sont ajoutés ou supprimés du profil.

   ![Création d’un profil de produit](assets/admin_console_addaproductprofilecreatenewprofile.png)

1. Cliquez sur **[!UICONTROL Terminé]**. Groupe de configuration de produit. Par exemple, le **[!UICONTROL groupe Ventes]** est ajouté à Brand Portal.

   ![Profils de produits.](assets/admin_console_productprofileadded.png)

## Ajout d’utilisateurs à un profil de produit {#add-users-to-a-product-profile}

Pour ajouter des utilisateurs à un groupe Brand Portal, ajoutez-les au profil de produit correspondant (anciennement appelé configurations de produit) dans [!UICONTROL Admin Console]. Vous pouvez ajouter des utilisateurs individuellement ou en bloc.

>[!NOTE]
>
>Vous pouvez vous connecter à [](https://adminconsole.adobe.com/enterprise/overview) directement ou depuis Brand Portal. Si vous vous connectez directement à Admin Console, suivez les étapes 4 à 7 de la procédure ci-dessous pour ajouter des utilisateurs à un profil de produit.

1. Dans la barre d’outils supérieure, cliquez sur le logo Experience Manager pour accéder aux outils d’administration.

   ![Logo AEM](assets/aemlogo.png)

1. Dans le panneau des outils d’administration, cliquez sur **[!UICONTROL Utilisateurs]**.

   ![Panneau Outils d’administration](assets/admin-tools-panel-7.png)

1. Dans la page [!UICONTROL Rôles utilisateur], cliquez sur l’onglet **[!UICONTROL Gestion]**, puis sur **[!UICONTROL Lancer Admin Console]**.

   ![Lancement d’[!DNL Admin Console]](assets/launch_admin_console.png)

1. Dans la barre d’outils supérieure, cliquez sur **[!UICONTROL Produits]**.
1. Sur la page [!UICONTROL Produits], [!UICONTROL Profils de produit] sont sélectionnés par défaut. Ouvrez le profil de produit auquel vous souhaitez ajouter un utilisateur, par exemple [!UICONTROL Groupe des ventes].

   ![Profils de produit](assets/admin_console_productprofileadded.png)

1. Pour ajouter des utilisateurs individuels au profil de produit, procédez comme suit :

   * Cliquez sur **[!UICONTROL Ajouter un utilisateur]**.

   ![Associer le profil du produit dans Brand Portal](assets/admin_console_productprofilesalesgroup.png)

   * Dans la page [!UICONTROL Ajouter un utilisateur au groupe des ventes], saisissez l’e-mail de l’utilisateur que vous souhaitez ajouter ou sélectionnez-le dans la liste des suggestions qui apparaît lorsque vous commencez à taper.

   ![Ajout d’un utilisateur à un groupe](assets/admin_console_addusertosalesgroup.png)

   * Cliquez sur **[!UICONTROL Enregistrer]**.

1. Pour ajouter des utilisateurs en bloc au profil de produit, procédez comme suit :

   * Choisissez **[!UICONTROL points de suspension (...) > Ajouter des utilisateurs par fichier CSV]**.

   ![Ajout d’utilisateurs en bloc](assets/admin_console_addbulkusers.png)

   * Dans la page **[!UICONTROL Ajouter utilisateurs par CSV]**, téléchargez un modèle CSV ou glissez-déposez un fichier CSV.

   ![Ajout d’utilisateurs par csv](assets/admin_console_addbulkuserscsv.png)

   * Cliquez sur **[!UICONTROL Charger]**.

   Lorsque vous ajoutez des utilisateurs au profil de produit par défaut, Brand Portal, le système leur envoie un e-mail de bienvenue. Les utilisateurs invités peuvent ensuite accéder à Brand Portal en cliquant sur le lien contenu dans l’e-mail de bienvenue et en se connectant avec leur [!UICONTROL Adobe ID]. Voir [ Première connexion ](../using/brand-portal-onboarding.md).

   Les utilisateurs ajoutés à un profil de produit personnalisé ou nouveau ne reçoivent pas de notifications par e-mail.

## Octroi de privilèges d’administrateur aux utilisateurs {#provide-administrator-privileges-to-users}

Vous pouvez accorder à un utilisateur de Brand Portal des privilèges d’administrateur système ou d’administrateur de produit. Toutefois, évitez d’attribuer d’autres rôles administratifs disponibles dans . Par exemple, administrateur de profils de produit, administrateur de groupes d’utilisateurs et administrateur d’assistance. Voir [ Rôles administratifs ](https://helpx.adobe.com/fr/enterprise/using/admin-roles.html).

>[!NOTE]
>
>Vous pouvez vous connecter à [](https://adminconsole.adobe.com/enterprise/overview) directement ou depuis Brand Portal. Si vous vous connectez directement à , suivez les étapes 4 à 8 de la procédure ci-dessous pour ajouter un utilisateur à un profil de produit.

1. Dans la barre d’outils AEM supérieure, cliquez sur le logo Adobe pour accéder aux outils d’administration.

   ![Logo AEM](assets/aemlogo.png)

1. Dans le panneau des outils d’administration, cliquez sur **[!UICONTROL Utilisateurs]**.

   ![Panneau Outils d’administration](assets/admin-tools-panel-8.png)

1. Dans la page [!UICONTROL Rôles utilisateur], cliquez sur l’onglet **[!UICONTROL Gestion]**, puis sur **[!UICONTROL Lancer Admin Console]**.

   ![Lancement d’Admin Console](assets/launch_admin_console.png)

1. Dans la barre d’outils supérieure, cliquez sur **[!UICONTROL Utilisateurs]**.
1. Sur la page [!UICONTROL Utilisateurs], dans le rail de gauche, [!UICONTROL Utilisateurs] sont sélectionnés par défaut. Cliquez sur le nom de l’utilisateur à qui vous souhaitez accorder des privilèges d’administrateur.

   ![Ajout d’utilisateurs dans Admin Console](assets/admin_console_adduseruserpage.png)

1. Dans la page du profil utilisateur, recherchez la section **[!UICONTROL Droits d’administration]** en bas, puis choisissez **[!UICONTROL points de suspension (...) > Modifier les droits d’administration]**.
   ![Droits d’administrateur dans Admin Console](assets/admin_console_editadminrights.png)

1. Dans la page [!UICONTROL Modifier l’administrateur], sélectionnez Administrateur système ou Administrateur de produit.

   ![Modification des droits d’administrateur dans Admin Console](assets/admin_console_editadminrightsselection.png)

   >[!NOTE]
   >
   >Brand Portal ne prend en charge que les rôles Administrateur système et Administrateur de produit.
   >
   >Adobe recommande d’éviter l’utilisation du rôle Administrateur système, car il accorde des privilèges d’administrateur à l’échelle de l’entreprise pour tous les produits d’une entreprise. Par exemple, l’administrateur système d’une organisation qui comprend trois produits cloud pour le marketing dispose de l’ensemble des privilèges pour les trois produits. Seul un administrateur système peut configurer Experience Manager Assets pour que les ressources puissent être publiées d’Experience Manager Assets sur Brand Portal. Pour plus d’informations, voir [Configuration d’Experience Manager Assets avec Brand Portal](../using/configure-aem-assets-with-brand-portal.md).
   >
   >En revanche, le rôle Administrateur de produit accorde des privilèges d’administrateur uniquement pour un produit spécifique. Si vous souhaitez appliquer un contrôle d’accès plus précis dans Brand Portal, utilisez le rôle Administrateur de produit et sélectionnez le produit Brand Portal.

   >[!NOTE]
   >
   >Brand Portal ne prend pas en charge les privilèges d’administrateur de profils de produit (anciennement appelé administrateur de configuration). Évitez d’attribuer des droits d’administrateur de profil de produit à un utilisateur.

1. Vérifiez la sélection du type d’administrateur, puis cliquez sur **[!UICONTROL Enregistrer]**.

   >[!NOTE]
   >
   >Pour retirer les privilèges d’administrateur d’un utilisateur, apportez les modifications nécessaires sur la page **[!UICONTROL Modifier l’administrateur]**, puis cliquez sur **[!UICONTROL Enregistrer]**.


## Gestion des rôles utilisateur {#manage-user-roles}

Un administrateur peut modifier les rôles des utilisateurs dans Brand Portal.

Outre le rôle d’administrateur, Brand Portal prend en charge les rôles suivants :

* [!UICONTROL Observateur] : les utilisateurs disposant de ce rôle peuvent afficher les fichiers et dossiers qu’un administrateur partage avec eux. Les observateurs peuvent également rechercher et télécharger des ressources. Toutefois, ils ne peuvent pas partager de contenu (fichiers, dossiers et [!UICONTROL collections]) avec d’autres utilisateurs.
* [!UICONTROL Éditeur] : les utilisateurs et utilisatrices bénéficiant de ce rôle disposent de tous les privilèges d’une visionneuse. En complément, les éditeurs peuvent partager du contenu (dossiers, [!UICONTROL collections] et liens) avec d’autres utilisateurs.

1. Dans la barre d’outils AEM supérieure, cliquez sur le logo Adobe pour accéder aux outils d’administration.

   ![Logo AEM](assets/aemlogo.png)

1. Dans le panneau des outils d’administration, cliquez sur **[!UICONTROL Utilisateurs]**.

   ![Panneau Outils d’administration](assets/admin-tools-panel-9.png)

1. Dans la page [!UICONTROL Rôles utilisateur], l’onglet [!UICONTROL Utilisateurs] est sélectionné par défaut. Pour l’utilisateur dont vous souhaitez modifier le rôle, sélectionnez **[!UICONTROL Éditeur]** ou **[!UICONTROL Observateur]** dans la liste déroulante **[!UICONTROL Rôle]**.

   ![Modification des rôles d’utilisateurs](assets/modify_user_role.png)

   Pour modifier simultanément le rôle de plusieurs utilisateurs, sélectionnez les utilisateurs et le rôle adéquat dans la liste déroulante **[!UICONTROL Rôle]**.

   >[!NOTE]
   >
   >La liste [!UICONTROL Rôle] pour les utilisateurs administrateurs est désactivée. Vous ne pouvez pas sélectionner ces utilisateurs pour modifier leurs rôles.


   >[!NOTE]
   >
   >Le rôle d’utilisateur est également désactivé si l’utilisateur est membre du groupe Éditeur. Pour retirer les privilèges d’édition d’un utilisateur, supprimez l’utilisateur du groupe Éditeur ou modifiez le rôle du groupe entier en Observateur.


1. Cliquez sur **[!UICONTROL Enregistrer]**. Le rôle est modifié pour l’utilisateur en question. Si vous avez sélectionné plusieurs utilisateurs, les rôles de tous les utilisateurs sont modifiés simultanément.

   >[!NOTE]
   >
   >Les modifications apportées aux autorisations utilisateur apparaissent dans la page **[!UICONTROL Rôles utilisateur]** uniquement après la reconnexion des utilisateurs à Brand Portal.

## Gestion des rôles et des privilèges des groupes {#manage-group-roles-and-privileges}

Un administrateur peut associer des privilèges spécifiques à un [groupe](../using/brand-portal-adding-users.md#main-pars-title-278567577) d’utilisateurs sur Brand Portal. L’onglet **[!UICONTROL Groupes]** de la page **[!UICONTROL Rôles utilisateur]** permet aux administrateurs :

* d’attribuer des rôles aux groupes d’utilisateurs ;
* restreindre les groupes d’utilisateurs au téléchargement des rendus originaux des fichiers images (.jpeg, .tiff, .png, .bmp, .gif, .pjpeg, x-portable-anymap, x-portable-bitmap, x-portable-graymap, x-portable-pixmap, x-rgb, x-xbitmap, x-xpixmap, x-icon, image/photoshop, image/x-photoshop, .psd, image/vnd.adobe.photoshop) à partir de Brand Portal.

>[!NOTE]
>
>Pour les ressources partagées en tant que lien, l’autorisation d’accès aux rendus originaux des fichiers image s’applique en fonction des autorisations de l’utilisateur qui partage les ressources.

Pour modifier le rôle et le droit d’accès aux rendus originaux pour des membres de groupes spécifiques, procédez comme suit :

1. Sur la page **[!UICONTROL Rôles utilisateur]**, accédez à l’onglet **[!UICONTROL Groupes]**.
1. Sélectionnez les groupes dont vous souhaitez modifier les rôles.
1. Sélectionnez le rôle adéquat dans la liste déroulante **[!UICONTROL Rôle]**.

   Pour permettre aux membres du groupe d’accéder aux rendus originaux des fichiers image qu’ils téléchargent à partir du portail ou du lien partagé, conservez l’option **[!UICONTROL Accéder à l’original]** sélectionnée pour ce groupe. Cette approche inclut des types de fichiers tels que :

   * .jpeg
   * .tiff
   * .png
   * .bmp
   * .gif
   * .pjpeg
   * .psd
   * x-portable-anymap
   * x-portable-bitmap
   * x-portable-graymap
   * x-portable-pixmap
   * x-rgb
   * x-xbitmap
   * x-xpixmap
   * x-icon
   * image/photoshop
   * image/x-photoshop
   * image/vnd.adobe.photoshop

   Par défaut, l’option **[!UICONTROL Accès à l’original]** est sélectionnée pour tous les utilisateurs. Pour empêcher un groupe d’utilisateurs d’accéder aux rendus originaux, désélectionnez l’option correspondant à ce groupe.

   ![Rôles des groupes d’utilisateurs](assets/access-original-rend.png)

   >[!NOTE]
   >
   >Si un utilisateur est ajouté à plusieurs groupes, et si l’un de ces groupes présente des restrictions, les restrictions s’appliquent à cet utilisateur.
   >
   >En outre, les restrictions d’accès aux rendus originaux des fichiers image ne s’appliquent pas aux administrateurs, même s’ils sont membres de groupes restreints.


1. Cliquez sur **[!UICONTROL Enregistrer]**. Le rôle est modifié pour les groupes correspondants.

   >[!NOTE]
   >
   >L’association d’utilisateur à groupe, ou l’appartenance à un groupe d’un utilisateur, est synchronisée avec Brand Portal toutes les 8 heures. Les modifications apportées aux rôles des utilisateurs ou des groupes sont prises en compte après l’exécution de la prochaine tâche de synchronisation.
