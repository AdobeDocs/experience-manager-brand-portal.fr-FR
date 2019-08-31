---
title: Utilisation des rapports
seo-title: Utilisation des rapports
description: Les administrateurs d’AEM Assets Brand Portal peuvent consulter des rapports sur l’utilisation de Brand Portal, de même que créer, gérer et afficher des rapports sur les ressources téléchargées, expirées, publiées, ainsi que sur les liens partagés via Brand Portal.
seo-description: Les administrateurs d’AEM Assets Brand Portal peuvent consulter des rapports sur l’utilisation de Brand Portal, de même que créer, gérer et afficher des rapports sur les ressources téléchargées, expirées, publiées, ainsi que sur les liens partagés via Brand Portal.
uuid: dc 4 e 5275-a 614-4 b 95-8 c 70-2 b 7 e 470 c 50 a 7
content-type: référence
topic-tags: administration
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
discoiquuid: 7683074 f-b 6 ea -42 e 0-a 411-3 b 13 eb 88 d 1 f 2
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Utilisation des rapports {#work-with-reports}

La fonctionnalité de création de rapports est essentielle pour évaluer l'utilisation du portail de marque et savoir comment les utilisateurs internes et externes interagissent avec les ressources approuvées. Les administrateurs peuvent afficher le rapport Utilisation de Brand Portal, qui est toujours disponible sur la page Rapports de ressources. Toutefois, les rapports des connexions d’utilisateurs et ressources téléchargées, expirées, publiées et partagées par des liens peuvent être générés et affichés à partir de la page Rapports de ressources. Ces rapports s'avèrent utiles pour analyser le déploiement des ressources, ce qui vous permet de dériver les mesures de réussite clés afin de mesurer l'adoption des ressources approuvées au sein et en dehors de votre organisation.

L’interface de gestion des rapports est intuitive et contient des options et commandes précises pour accéder aux rapports enregistrés. Vous pouvez consulter, télécharger ou supprimer des rapports à partir de la page Rapports de ressources, dans laquelle tous les rapports générés auparavant sont répertoriés.

## Affichage des rapports {#view-reports}

Pour afficher un rapport, procédez comme suit :

1. Dans la barre d’outils supérieure, appuyez/cliquez sur le logo AEM pour accéder aux outils d’administration.

   ![](assets/aemlogo.png)

2. From the administrative tools panel, click **[!UICONTROL Create/Manage Reports]** to open **[!UICONTROL Asset Reports]** page.

   ![](assets/access-asset-reports.png)

3. Access **[!UICONTROL Usage]** report and other generated reports from Asset Reports page.

   >[!NOTE]
   >
   >Le rapport Utilisation figure par défaut dans Brand Portal. Il ne peut pas être créé ni supprimé. Toutefois, vous pouvez créer, télécharger et supprimer les rapports Télécharger, Expiration, Publier, Partage de liens et Identifiants d'utilisateur.

   Pour afficher un rapport, appuyez/cliquez sur le lien du rapport. Vous pouvez également sélectionner le rapport, puis appuyer/cliquer sur l'icône Affichage dans la barre d'outils.

   Le rapport [!UICONTROL Utilisation] affiche des informations sur le nombre d’utilisateurs de Brand Portal actuels, l’espace de stockage occupé par toutes les ressources et le nombre total des ressources dans Brand Portal. Il affiche également la capacité autorisée pour chacune de ces mesures.

   ![](assets/usage-report.png)

   Le rapport [!UICONTROL Connexions des utilisateurs] fournit des informations concernant les utilisateurs qui se sont connectés à Brand Portal. Le rapport affiche les noms d'affichage, les ID de courriel, les personnes (admin, viewer, éditeur, invité), les groupes, la dernière connexion, l'état de l'activité et le nombre de connexions de chaque utilisateur du déploiement de Brand Portal 6.4.2 jusqu'au moment de la génération du rapport.

   ![](assets/user-logins.png)

   Le rapport [!UICONTROL Téléchargement] indique toutes les ressources téléchargées pendant une période et une plage horaire spécifiques.

   ![](assets/download-report.png)

   >[!NOTE]
   >
   >[!UICONTROL Le] rapport Télécharger les ressources affiche uniquement les actifs qui ont été sélectionnés individuellement et téléchargés à partir de Brand Portal. Si un utilisateur a téléchargé un dossier contenant des ressources, le rapport n'affiche pas le dossier ou les actifs qu'il contient.

   Le rapport [!UICONTROL Expiration] répertorie toutes les ressources qui sont arrivées à expiration pendant une période spécifique.

   ![](assets/expiration-report.png)

   Le rapport [!UICONTROL Publication] répertorie et donne des informations sur toutes les ressources qui sont publiées d’AEM sur Brand Portal dans une période spécifiée.

   ![](assets/publish-report.png)

   >[!NOTE]
   >
   >Le rapport Publication n’affiche pas d’informations sur les fragments de contenu, car ils ne peuvent pas être publiés sur Brand Portal.

   Le rapport [!UICONTROL Partage de liens] répertorie toutes les ressources partagées à travers des liens à partir de l’interface de Brand Portal pendant une période spécifique. Le rapport indique également quand la ressource a été partagée par le biais du lien, par quel utilisateur, quand le lien expire et le nombre de liens partagés pour le client (et les utilisateurs avec lesquels le lien de la ressource a été partagé). Les colonnes du rapport Partage de liens ne sont pas personnalisables.

   ![](assets/link-share-report.png)

   >[!NOTE]
   >
   >Le rapport Partage de liens n’affiche pas les utilisateurs qui ont accès à une ressource partagée par le biais du lien ou qui ont téléchargé la ressource via le lien.
   >
   >
   >Pour effectuer le suivi des téléchargements réalisés par l’intermédiaire du lien partagé, vous devez générer le rapport de téléchargement après avoir sélectionné l’option **[!UICONTROL Uniquement les téléchargements via partage de lien]** sur la page **Créer un rapport[!UICONTROL .]** Cependant, l'utilisateur (téléchargé par) est anonyme dans ce cas.

## Génération de rapports {#generate-reports}

Administrators can generate and manage the following standard reports, once generated, they are saved to be [accessed](../using/brand-portal-reports.md#main-pars-header) later:

* Connexions des utilisateurs
* Télécharger
* Expiration
* Publication
* Partage de lien

Les colonnes des rapports Téléchargement, Expiration et Publication peuvent être personnalisées à des fins d’affichage. Pour générer un rapport, procédez comme suit :

1. Dans la barre d’outils supérieure, appuyez/cliquez sur le logo AEM pour accéder aux outils d’administration.

   ![](assets/aemlogo.png)

2. From the administrative tools panel, tap/click **[!UICONTROL Create/Manage Reports]** to open **Asset Reports **page.

   ![](assets/asset-reports.png)

3. Sur la page Rapports de ressources, appuyez/cliquez sur **[!UICONTROL Créer]**.
4. From the **[!UICONTROL Create Report]** page, select a report to create, and tap/click **[!UICONTROL Next]**.

   ![](assets/crete-report.png)

5. Configurez les détails du rapport. Indiquez le titre, la description, la structure de dossiers (où le rapport doit s’exécuter et générer des statistiques) et la période pour les rapports [!UICONTROL Téléchargement], [!UICONTROL Expiration] et [!UICONTROL Publication].

   ![](assets/create-report-page.png)

   Whereas, [!UICONTROL Link Share Report] only needs the title, description, and date range parameters.

   ![](assets/create-link-share-report.png)

   >[!NOTE]
   >
   >Les caractères spéciaux # et % dans le titre du rapport sont remplacés par un tiret (-) sur la génération du rapport.

6. Tap/click **[!UICONTROL Next]**, to configure the columns of Download, Expiration, and Publish reports.
7. Cochez ou décochez les cases adéquates selon vos besoins. For example, to view names of users (who downloaded assets) in [!UICONTROL Download] report, select **[!UICONTROL Downloaded By]**. L’image suivante montre comment sélectionner les colonnes par défaut dans le rapport Téléchargement.

   ![](assets/createdownloadreport.png)

   Vous pouvez également ajouter des colonnes personnalisées à ces rapports pour afficher davantage de données selon vos besoins.

   Pour ajouter des colonnes personnalisées au rapport Télécharger, Publier ou Expiration, procédez comme suit :

   1. To display a custom column, tap/click **[!UICONTROL Add]** within [!UICONTROL Custom Columns].
   2. Specify name of the column in **[!UICONTROL Column Name]** field.
   3. Sélectionnez la propriété à laquelle la colonne doit être associée à l’aide du sélecteur de propriété.

      ![](assets/property-picker.png)
Vous pouvez également saisir le chemin d’accès dans le champ de chemin d’accès à la propriété.

      ![](assets/property-path.png)

      Pour ajouter d’autres colonnes personnalisées, appuyez/cliquez sur **Ajouter** et répétez les étapes 2 et 3.

8. Cliquez/appuyez sur **[!UICONTROL Créer]**. Un message indique que la génération du rapport a été lancée.

## Téléchargement de rapports {#download-reports}

Pour enregistrer et télécharger un rapport en tant que fichier .csv, effectuez l’une des opérations suivantes :

* Select a report on Asset Reports page, and tap/click **[!UICONTROL Download]** from the toolbar at the top.

![](assets/download-asset-report.png)

* Dans la page Rapports de ressources, ouvrez un rapport. Select **[!UICONTROL Download]** option from the top of the report page.

![](assets/download-report-fromwithin.png)

## Suppression de rapports {#delete-reports}

Pour supprimer un rapport existant, sélectionnez-le sur la page **[!UICONTROL Rapports de ressources]** et appuyez/cliquez sur **Supprimer[!UICONTROL dans la barre d’outils supérieure.]**

>[!NOTE]
>
>Le rapport [!UICONTROL Utilisation] ne peut pas être supprimé.
