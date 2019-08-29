---
title: Gestion des utilisateurs, des groupes et des rôles utilisateur
seo-title: Gestion des utilisateurs, des groupes et des rôles utilisateur
description: Les administrateurs peuvent utiliser Adobe Admin Console pour créer des utilisateurs et des profils de produit AEM Assets Brand Portal et gérer leurs rôles à l’aide de l’interface utilisateur de Brand Portal. Ce privilège n’est pas disponible pour les visualisateurs et les éditeurs.
seo-description: Les administrateurs peuvent utiliser Adobe Admin Console pour créer des utilisateurs et des profils de produit AEM Assets Brand Portal et gérer leurs rôles à l’aide de l’interface utilisateur de Brand Portal. Ce privilège n’est pas disponible pour les visualisateurs et les éditeurs.
uuid: 0 dc 1867 c -6 d 1 b -4 d 0 d-a 25 e -0 df 207 c 269 b 8
content-type: référence
topic-tags: administration
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
discoiquuid: ba 468 e 80-d 077-4 af 6-b 782-238 fc 557 e 22 b
translation-type: tm+mt
source-git-commit: 32c3cdb8e3fafd74cfb36e6bcfe0811e7152b2d0

---


# Manage Users, Groups, and User Roles {#manage-users-groups-and-user-roles}

Administrators can use [!DNL Adobe Admin Console] to create [!DNL AEM Assets Brand Portal] users and product profiles, and manage their roles using the Brand Portal user interface. Ce privilège n’est pas disponible pour les visualisateurs et les éditeurs.

In [Admin Console](http://adminconsole.adobe.com/enterprise/overview), you can view all the products associated with your organization. Un produit peut être n'importe quelle [!DNL Experience Cloud] solution, telle [!DNL Adobe Analytics]que, [!DNL Adobe Target]ou [!DNL AEM Brand Portal]. Vous devez choisir le produit AEM Brand Portal et créer des profils de produit.

<!--
Comment Type: draft

<note type="note">
<p>Product Profiles (formerly known as product configurations*). </p>
<p>* The nomenclature has changed from product configurations to product profiles in the new Adobe Admin Console.</p>
</note>
-->
![](assets/create-user-group.png)

These product profiles are synced with the [!DNL Brand Portal] user interface every 8 hours and visible as groups in [!DNL Brand Portal]. Once you add users and create product profiles, and add users to those product profiles, you can assign roles to users and groups in [!DNL Brand Portal].

>[!NOTE]
>
>To create groups in [!DNL Brand Portal], from [!DNL Adobe Admin Console], use **Products** page &gt; **Product Profiles**, instead of **User** page &gt; **User Groups**. Product profiles in [!DNL Adobe Admin Console] are used to create groups in [!DNL Brand Portal].

## Ajout d’un utilisateur {#add-a-user}

If you are a product administrator, use [[!DNL Adobe Admin Console]](http://adminconsole.adobe.com/enterprise/overview) to create users and assign them to product profiles (*formerly known as product configurations*), which show as groups in [!DNL Brand Portal]. Vous pouvez utiliser des groupes pour effectuer des opérations en bloc comme gérer les rôles et partager des ressources.

>[!NOTE]
New users who do not have access to [!DNL Brand Portal] can request access from the login screen of [!DNL Brand Portal]. For more information, refer to [Request access to [!DNL Brand Portal]](../using/brand-portal.md#request-access-to-brand-portal). After you receive access request notifications in your notification area, click the relevant notification and then click **Grant Access**. Vous pouvez également suivre le lien figurant dans le courrier électronique de demande d'accès reçu. Next, to add a user through [[!DNL Adobe Admin Console]](http://adminconsole.adobe.com/enterprise/overview), follow Steps 4-7 in the procedure below.

>[!NOTE]
You can login to [[!DNL Adobe Admin Console]](http://adminconsole.adobe.com/enterprise/overview) directly or from [!DNL Brand Portal]. Si vous vous connectez directement, suivez les étapes 4-7 de la procédure ci-dessous pour ajouter un utilisateur.

1. From the [!DNL AEM] toolbar at the top, click the Adobe logo to access administrative tools.

   ![Logo AEM](assets/aemlogo.png)

2. Dans le panneau des outils d’administration, cliquez sur **Utilisateurs**.

   ![Panneau Outils d'administration](assets/admin-tools-panel-5.png)

3. In the **User Roles** page, click the **Management** tab, then click **Launch Admin Console**.

   ![Rôles utilisateur pour lancer la console d'administration](assets/launch_admin_console.png)

4. Dans Admin Console, effectuez l’une des opérations suivantes pour créer un utilisateur :

   * Dans la barre d’outils supérieure, cliquez sur **Présentation**. In the **Overview** page, click **Assign Users** from the **[!DNL AEM Brand Portal]** product card.
   ![Présentation de la console d'administration](assets/admin_console_overviewadduser.png)

   * Dans la barre d’outils supérieure, cliquez sur **Utilisateurs**. In the **Users** page, **Users** in the left rail is selected by default. Click **Add User**.
   ![Console d'administration Ajout d'utilisateurs](assets/admin_console_adduseruserpage.png)

5. Dans la boîte de dialogue Ajouter un utilisateur, saisissez l’e-mail de l’utilisateur que vous souhaitez ajouter ou sélectionnez l’utilisateur dans la liste des suggestions qui apparaît dès que vous commencez à taper.

   ![Ajout d'un utilisateur à Brand Portal](assets/add_user_to_aem_bp.png)

6. Affectez l’utilisateur à au moins un profil de produit (auparavant appelé configurations de produit) afin qu’il puisse accéder à Brand Portal. Sélectionnez le profil de produit adéquat dans le champ **Sélectionnez un profil pour ce produit**.
7. Cliquez sur **Enregistrer**. Un e-mail de bienvenue est envoyé à l’utilisateur que vous avez ajouté. The invited user can access [!DNL Brand Portal] by clicking the link in the welcome email and signing in using an [!UICONTROL Adobe ID]. Pour plus d’informations, voir [Première connexion](../using/brand-portal-onboarding.md).

   >[!NOTE]
   If a user is unable to log on to [!DNL Brand Portal], the Administrator of the organization should visit Adobe [!UICONTROL Admin Console] and check whether the user is present and has been added to at least one product profile.

   Pour plus d’informations sur l’octroi de privilèges administratifs, voir [Octroi de privilèges d’administrateur aux utilisateurs](../using/brand-portal-adding-users.md#provideadministratorprivilegestousers).

## Ajout d’un profil de produit {#add-a-product-profile}

Product profiles (formerly known as product configurations) in [!UICONTROL Admin Console] are used to create groups in [!DNL Brand Portal] so that you can perform bulk operations such as role management and asset sharing in [!DNL Brand Portal]. **[!DNL Brand Portal]** est le profil de produit disponible par défaut. Vous pouvez créer d’autres profils de produit et ajouter des utilisateurs à ces derniers.

>[!NOTE]
You can login to [[!UICONTROL Admin Console]](http://adminconsole.adobe.com/enterprise/overview) directly or from [!DNL Brand Portal]. If you login to [!UICONTROL Admin Console] directly, follow Steps 4-7 in the procedure below to add a product profile.

1. From the [!DNL AEM] toolbar at the top, click the Adobe logo to access administrative tools.

   ![[!DNL AEM] Logo](assets/aemlogo.png)

2. Dans le panneau des outils d’administration, cliquez sur **Utilisateurs**.

   ![Panneau Outils d'administration](assets/admin-tools-panel-6.png)

3. In the **User Roles** page, click the **Management** tab, then click **Launch Admin Console**.

   ![Lancement de la console d'administration](assets/launch_admin_console.png)

4. Dans la barre d’outils supérieure, cliquez sur **Produits**.
5. In the **Products** page, **Product Profiles** is selected by default. Cliquez sur **Nouveau profil**.

   ![Ajouter un nouveau profil de produit](assets/admin_console_addproductprofile.png)

6. Dans la page **Créer un nouveau profil**, indiquez le nom du profil, le nom d’affichage, la description du profil, puis choisissez si vous souhaitez informer les utilisateurs par e-mail lorsqu’ils sont ajoutés ou supprimés du profil.

   ![Créer un profil de produit](assets/admin_console_addaproductprofilecreatenewprofile.png)

7. Cliquez sur **Terminé**. The product configuration group, for example **Sales group**, is added to Brand Portal.

   ![Profils de produit](assets/admin_console_productprofileadded.png)

## Ajout d’utilisateurs à un profil de produit {#add-users-to-a-product-profile}

To add users to a [!DNL Brand Portal] group, add them to the corresponding product profile (formerly known as product configurations) in [!UICONTROL Admin Console]. Vous pouvez ajouter des utilisateurs individuellement ou en bloc.

>[!NOTE]
You can login to [[!DNL Admin Console]](http://adminconsole.adobe.com/enterprise/overview) directly or from [!DNL Brand Portal]. Si vous vous connectez directement à la console d'administration, suivez les étapes 4-7 de la procédure ci-dessous pour ajouter des utilisateurs à un profil de produit.

1. From the [!DNL AEM] toolbar at the top, click the Adobe logo to access administrative tools.

   ![[!DNL AEM] Logo](assets/aemlogo.png)

2. Dans le panneau des outils d’administration, cliquez sur **Utilisateurs**.

   ![Panneau Outils d'administration](assets/admin-tools-panel-7.png)

3. In the **User Roles** page, click the **Management** tab, then click **Launch Admin Console**.

   ![Lancement [!DNL Admin Console]](assets/launch_admin_console.png)

4. Dans la barre d’outils supérieure, cliquez sur **Produits**.
5. In the **Products** page, **Product Profiles** is selected by default. Open the product profile to which you want to add a user, for example, **Sales group**.

   ![Profils de produit](assets/admin_console_productprofileadded.png)

6. Pour ajouter des utilisateurs individuels au profil de produit, procédez comme suit :

   * Click **Add User**.
   ![Associer le profil du produit dans [!DNL Brand Portal]](assets/admin_console_productprofilesalesgroup.png)

   * In the **Add User to Sales group** page, type the email ID of the user you want to add or select the user from the list of suggestions that appear as you type.
   ![Ajout d'un utilisateur à un groupe](assets/admin_console_addusertosalesgroup.png)

   * Cliquez sur **Enregistrer**.



7. Pour ajouter des utilisateurs en bloc au profil de produit, procédez comme suit :

   * Choose ellipsis (**...**) &gt; **Add users by CSV**.
   ![Ajout d'utilisateurs en bloc](assets/admin_console_addbulkusers.png)

   * In the **Add Users by CSV** page, download a CSV template or drag-and-drop a CSV file.
   ![Ajout d'utilisateurs par csv](assets/admin_console_addbulkuserscsv.png)

   * Cliquez sur **Charger**.
   If you added users to the default product profile, that is, [!DNL Brand Portal], a welcome email is sent to the email ID of the users you added. The invited users can access [!DNL Brand Portal] by clicking the link in the welcome email and signing in using an [!UICONTROL Adobe ID]. Pour plus d’informations, voir [Première connexion](../using/brand-portal-onboarding.md).

   Les utilisateurs ajoutés à un nouveau profil de produit ou à un profil de produit personnalisé ne reçoivent pas de notifications par e-mail.

## Octroi de privilèges d’administrateur aux utilisateurs {#provide-administrator-privileges-to-users}

You can provide the system administrator or the product administrator privilege to a [!DNL Brand Portal] user. Do not provide other administrative rights available in [!UICONTROL Admin Console], such as product profile administrator, user group administrator, and support administrator. Pour en savoir plus sur ces rôles, voir [Rôles administratifs](https://helpx.adobe.com/enterprise/using/admin-roles.html).

>[!NOTE]
You can login to [[!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview) directly or from [!DNL Brand Portal]. If you login to [!UICONTROL Admin Console] directly, follow Steps 4-8 in the procedure below to add a user to a product profile.

1. From the [!DNL AEM] toolbar at the top, click the Adobe logo to access administrative tools.

   ![Aemlogo](assets/aemlogo.png)

2. Dans le panneau des outils d’administration, cliquez sur **Utilisateurs**.

   ![Panneau Outils d'administration](assets/admin-tools-panel-8.png)

3. In the **User Roles** page, click the **Management** tab, then click **Launch Admin Console**.

   ![Lancement de la console d'administration](assets/launch_admin_console.png)

4. Dans la barre d’outils supérieure, cliquez sur **Utilisateurs**.
5. In the **Users** page, **Users** in the left rail is selected by default. Cliquez sur le nom de l’utilisateur à qui vous souhaitez accorder des privilèges d’administrateur.

   ![Ajout d'utilisateurs dans la console d'administration](assets/admin_console_adduseruserpage.png)

6. In the user profile page, locate the **Administrative Rights** section at the bottom, and choose ellipsis (**...**) &gt; **Edit admin rights**.
   ![Droits d'administrateur dans la console d'administration](assets/admin_console_editadminrights.png)

7. Dans la page **Modifier l’administrateur**, sélectionnez Administrateur système ou Administrateur de produit.

   ![Modification des droits d'administrateur dans la console d'administration](assets/admin_console_editadminrightsselection.png)

   >[!NOTE]
   [!DNL Brand Portal] ne prend en charge que les rôles Administrateur système et Administrateur du produit.
   [!DNL Adobe] recommande d’éviter l’utilisation du rôle Administrateur système, car il accorde des privilèges d’administrateur à l’échelle de l’entreprise pour tous les produits d’une entreprise. Par exemple, un administrateur système d'une organisation qui comprend trois produits Marketing Cloud dispose de l'ensemble des privilèges pour les trois produits. Only a System Administrator can configure [!DNL AEM] Assets so that assets can be published from [!DNL AEM] Assets to [!DNL Brand Portal]. For more information, see [Configure AEM Assets integration with [!DNL Brand Portal]](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html).
   En revanche, le rôle Administrateur de produit accorde des privilèges d’administrateur pour un produit spécifique uniquement. If you want to enforce a more granular access control within [!DNL Brand Portal], use the Product Administrator role and select the product as **[!DNL AEM Brand Portal]**.

   >[!NOTE]
   [!DNL Brand Portal] ne prend pas en charge les privilèges d’administrateur de profil de produit (auparavant appelé administrateur de configuration). Évitez d’attribuer des droits d’administrateur de profil de produit à un utilisateur.

8. Examinez la sélection du type d’administrateur, puis cliquez sur **Enregistrer**.

   >[!NOTE]
   Pour retirer les privilèges d’administrateur d’un utilisateur, apportez les modifications nécessaires dans la page **Modifier l’administrateur**, puis cliquez sur **Enregistrer**.

## Gestion des rôles utilisateur {#manage-user-roles}

Un administrateur peut modifier les rôles des utilisateurs dans [!DNL Brand Portal].

In addition to the Administrator role, [!DNL Brand Portal] supports the following roles:

* **Observateur** : les utilisateurs disposant de ce rôle peuvent afficher les fichiers et dossiers qu’un administrateur partage avec eux. Les utilisateurs peuvent également rechercher des fichiers et les télécharger. However, Viewers cannot share content (files, folders, [!UICONTROL collections]) with other users.
* **Éditeur** : les utilisateurs disposant de ce rôle possèdent tous les privilèges d’un visualisateur. In addition, Editors can share content (folders, [!UICONTROL collections], links) with other users.

1. From the [!DNL AEM] toolbar at the top, click the Adobe logo to access administrative tools.

   ![Aemlogo](assets/aemlogo.png)

2. Dans le panneau des outils d’administration, cliquez sur **Utilisateurs**.

   ![Panneau Outils d'administration](assets/admin-tools-panel-9.png)

3. In the **User Roles** page, the **Users** tab is selected by default. For the user whose role you want to change, select **Editor** or **Viewer** from the **Role** drop-down.

   ![Modification des rôles d'utilisateurs](assets/modify_user_role.png)

   Pour modifier simultanément le rôle de plusieurs utilisateurs, sélectionnez les utilisateurs et le rôle adéquat dans la liste déroulante **Rôle**.

   >[!NOTE]
   La liste **Rôle** des utilisateurs Administrateur est désactivée. Vous ne pouvez pas sélectionner ces utilisateurs pour modifier leur rôle.

   >[!NOTE]
   Le rôle utilisateur est également désactivé si l’utilisateur est membre du groupe Éditeur. Pour retirer les privilèges d’édition d’un utilisateur, supprimez l’utilisateur du groupe Éditeur ou modifiez le rôle du groupe entier en Visualisateur.

4. Cliquez sur **Enregistrer**. Le rôle est modifié pour l’utilisateur correspondant. Si vous avez sélectionné plusieurs utilisateurs, les rôles de tous les utilisateurs sont modifiés simultanément.

   >[!NOTE]
   Changes in user permissions are reflected in the **User Roles** page only after the users re-login to Brand Portal.

## Gestion des rôles et des privilèges des groupes {#manage-group-roles-and-privileges}

An Administrator can associate specific privileges with a [group](../using/brand-portal-adding-users.md#main-pars-title-278567577) of users on Brand Portal. The **Groups** tab on the **User Roles** page allows administrators to:

* d’attribuer des rôles aux groupes d’utilisateurs ;
* Restreignez les groupes d’utilisateurs au téléchargement des rendus originaux des fichiers images (.jpeg, .tiff, .png, .bmp, .gif, .pjpeg, x-portable-anymap, x-portable-bitmap, x-portable-graymap, x-portable-pixmap, x-rgb, x-xbitmap, x-xpixmap, x-icon, image/photoshop, image/x-photoshop, .psd, image/vnd.adobe.photoshop) à partir de Brand Portal.

>[!NOTE]
Pour les ressources partagées sous forme de liens, l’autorisation d’accès aux rendus originaux des fichiers images s’applique selon les autorisations de l’utilisateur qui partage les ressources.

Pour modifier le rôle et le droit d'accès aux rendus initiaux pour des membres de groupe spécifiques, procédez comme suit :

1. On the **User Roles** page, navigate to the **Groups** tab.
2. Sélectionnez les groupes dont vous souhaitez modifier les rôles.
3. Sélectionnez le rôle adéquat dans la liste déroulante **Rôle**.

   To allow the members of a group to have access to original renditions of image files (.jpeg, .tiff, .png, .bmp, .gif, .pjpeg, x-portable-anymap, x-portable-bitmap, x-portable-graymap, x-portable-pixmap, x-rgb, x-xbitmap, x-xpixmap, x-icon, image/photoshop, image/x-photoshop, .psd, image/vnd.adobe.photoshop) which they download from the portal or shared link, keep the **Access to  Original** option selected for that group. By default, **Access to Original** option is selected for all the users. Pour empêcher un groupe d’utilisateurs d’accéder aux rendus originaux, désélectionnez l’option correspondant à ce groupe.

   ![Rôles des groupes d'utilisateurs](assets/access-original-rend.png)

   >[!NOTE]
   Si un utilisateur est ajouté à plusieurs groupes et si l'un de ces groupes possède des restrictions, les restrictions s'appliquent à cet utilisateur.
   En outre, les restrictions pour accéder aux rendus originaux des fichiers images ne s’appliquent pas aux administrateurs, même s’ils sont des membres de groupes restreints.

4. Cliquez sur **Enregistrer**. Le rôle est modifié pour les groupes correspondants.

   >[!NOTE]
   The user-to-group association, or the group membership of a user, is synced to  [!DNL Brand Portal] every 8 hours. Les modifications apportées aux rôles des utilisateurs ou des groupes sont prises en compte après l’exécution de la prochaine tâche de synchronisation.
