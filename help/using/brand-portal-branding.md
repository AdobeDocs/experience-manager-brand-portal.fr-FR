---
title: Personnalisation du papier peint, de l’en-tête et des e-mails
seo-title: Personnalisation du papier peint, de l’en-tête et des e-mails
description: Les administrateurs de Brand Portal peuvent personnaliser de façon limitée l’interface s’affichant sur l’écran des utilisateurs. Vous pouvez choisir une image d’arrière-plan spécifique (papier peint) pour la page de connexion de Brand Portal. Vous pouvez également ajouter une image d’en-tête et personnaliser les e-mails de partage des ressources pour correspondre à la marque du client.
seo-description: Les administrateurs de Brand Portal peuvent personnaliser de façon limitée l’interface s’affichant sur l’écran des utilisateurs. Vous pouvez choisir une image d’arrière-plan spécifique (papier peint) pour la page de connexion de Brand Portal. Vous pouvez également ajouter une image d’en-tête et personnaliser les e-mails de partage des ressources pour correspondre à la marque du client.
uuid: e 078 d 0 b 9-18 b 5-467 a-ae 90-7 f 0 b 9 fd 0 d 414
content-type: référence
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
topic-tags: administration
discoiquuid: 7 b 573 a 4 f -2 d 4 e -48 d 6-b 259-436 d 0 cfbdce 9
translation-type: tm+mt
source-git-commit: 32c3cdb8e3fafd74cfb36e6bcfe0811e7152b2d0

---


# Personnalisation du papier peint, de l’en-tête et des e-mails {#customize-wallpaper-header-and-email-message}

[!DNL Brand Portal]Les administrateurs de peuvent personnaliser de façon limitée l’interface s’affichant sur l’écran des utilisateurs. You can choose a specific background image (wallpaper) for the [!DNL Brand Portal] login page. Vous pouvez également ajouter une image d’en-tête et personnaliser les e-mails de partage des ressources pour correspondre à la marque du client.

## Personnalisation du papier peint de l’écran de connexion {#customize-the-login-screen-wallpaper}

En l’absence d’image de papier peint de marque personnalisée, un papier peint par défaut est affiché sur la page de connexion.

1. From the [!DNL AEM] toolbar at the top, click the Adobe logo to access administrative tools.

   ![](assets/aemlogo.png)

2. From the administrative tools panel, click **Branding**.

   ![](assets/admin-tools-panel-10.png)

3. On the left rail of the **Configure Branding** page, **Wallpaper** is selected by default. L’image d’arrière-plan par défaut qui apparaît sur la page de connexion s’affiche.

   ![](assets/default_wallpaper.png)

4. To add a new background image, click the **Choose Image** icon from the toolbar at the top.

   ![](assets/choose_wallpaperimage.png)

   Utilisez l’une des méthodes suivantes :

   * To upload an image from your computer, click **Upload**. Accédez à l’image requise et téléchargez-la.
   * To use an existing Brand Portal image, click **Select from existing**. Sélectionnez une image à l’aide du sélecteur de ressource.
   ![](assets/asset-picker.png)

5. Spécifiez un texte et une description d’en-tête pour l’image d’arrière-plan. To save the changes, click **Save** from the toolbar at the top.

6. From the toolbar at the top, click the **Preview** icon to generate a preview of the Brand Portal interface with the image.

   ![](assets/chlimage_1.png)

   ![](assets/custom-wallpaper-preview.png)

7. To activate or deactivate the default wallpaper, do the following in the **Configure Branding** &gt; **Wallpaper** page:

   * To display the default wallpaper image on the Brand Portal login page, click **Deactivate Wallpaper** from the toolbar at the top. Un message confirme la désactivation de l’image personnalisée.
   ![](assets/chlimage_1-1.png)

   * Pour restaurer l’image par défaut sur la page de connexion de Brand Portal, cliquez sur **Activer le papier peint** dans la barre d’outils. Un message confirme la restauration de l’image.
   ![](assets/chlimage_1-2.png)

   * Cliquez sur **Enregistrer** pour enregistrer les modifications.



## Personnalisation de l’en-tête {#customize-the-header}

L'en-tête apparaît sur diverses pages du portail de marque une fois que vous vous êtes connecté à Brand Portal.

1. Dans la barre d'outils AEM en haut, cliquez sur le logo Adobe pour accéder aux outils d'administration.

   ![](assets/aemlogo.png)

2. From the administrative tools panel, click **Branding**.

   ![](assets/admin-tools-panel-11.png)

3. To customize the page header for the Brand Portal interface, on the **Configure Branding** page, select **Header Image** from the left rail. L’image d’en-tête par défaut s’affiche.

   ![](assets/default-header.png)

4. To upload a header image, click the **Choose Image** icon and choose **Upload**.

   To use an existing  [!DNL Brand Portal] image, choose **Select from existing**.

   ![](assets/choose_wallpaperimage-1.png)

   Sélectionnez une image à l’aide du sélecteur de ressource.

   ![](assets/asset-picker-header.png)

5. Pour inclure une URL dans l’image d’en-tête, spécifiez-la dans la zone **URL d’image**. Vous pouvez spécifier des URL externes ou internes. Les liens internes peuvent également être des liens relatifs, par exemple
   `/mediaportal.html/content/dam/mac/tenant_id/tags`.
Ce lien redirige les utilisateurs vers le dossier des balises.
To save the changes, click **Save** from the toolbar at the top.

   ![](assets/configure_brandingheaderimageurl.png)

6. Dans la barre d’outils supérieure, cliquez sur l’icône **Aperçu** pour générer un aperçu de l’interface de avec l’image d’en-tête.[!DNL Brand Portal]

   ![](assets/chlimage_1-3.png)
   ![](assets/custom_header_preview.png)

7. To activate or deactivate the header image, do the following in the **Configure Branding** &gt; **Header Image** page:

   * To prevent a header image from appearing on  [!DNL Brand Portal] pages, click **Deactivate Header** from the toolbar at the top. Un message confirme la désactivation de l’image.
   ![](assets/chlimage_1-4.png)

   * To make the header image reappear on  [!DNL Brand Portal] pages, click **Activate Header** from the toolbar at the top. Un message confirme l’activation de l’image.
   ![](assets/chlimage_1-5.png)

   * Cliquez sur **Enregistrer** pour enregistrer les modifications.



## Personnalisation des e-mails {#customize-the-email-messaging}

Lorsque des ressources sont partagées en tant que lien, l’utilisateur reçoit un e-mail contenant le lien. Les administrateurs peuvent personnaliser le logo, la description et le pied de page de ces e-mails.

1. From the  [!DNL AEM] toolbar at the top, click the Adobe logo to access administrative tools.

   ![](assets/aemlogo.png)

2. From the administrative tools panel, click **Branding**.

   ![](assets/admin-tools-panel-12.png)

3. When assets are shared as links or downloaded through emails, and when  [!UICONTROL collections] are shared, email notifications are sent to users. To customize the email message, on the **Configure Branding** page, select **Email Message** from the left rail.

   ![](assets/configure-branding-page-email.png)

4. Pour ajouter un logo aux e-mails sortants, cliquez sur **Télécharger** dans la barre d’outils supérieure.

5. Dans la section **Description**, indiquez le texte de l’en-tête et du pied de page de l’e-mail. To save the changes, click **Save** from the toolbar at the top.

   >[!NOTE]
   >
   >Si vous n'utilisez pas la taille recommandée pour le logo ou si le texte d'en-tête et de pied de page dépasse le nombre de mots recommandé, le contenu du message électronique peut s'afficher.
