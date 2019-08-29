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
source-git-commit: 32c3cdb8e3fafd74cfb36e6bcfe0811e7152b2d0

---


# Utilisation des rapports {#work-with-reports}

The reporting capability is instrumental in assessing [!DNL Brand Portal] usage, and knowing how internal and external users interact with approved assets. Administrators can view [!DNL Brand Portal] Usage report, which is always available on Asset Reports page. Toutefois, les rapports des connexions d’utilisateurs et ressources téléchargées, expirées, publiées et partagées par des liens peuvent être générés et affichés à partir de la page Rapports de ressources. Ces rapports s'avèrent utiles pour analyser le déploiement des ressources, ce qui vous permet de dériver les mesures de réussite clés afin de mesurer l'adoption des ressources approuvées au sein et en dehors de votre organisation.

L’interface de gestion des rapports est intuitive et contient des options et commandes précises pour accéder aux rapports enregistrés. Vous pouvez consulter, télécharger ou supprimer des rapports à partir de la page Rapports de ressources, dans laquelle tous les rapports générés auparavant sont répertoriés.

## Affichage des rapports {#view-reports}

Pour afficher un rapport, procédez comme suit :

1. From the toolbar at the top, tap/click the [!DNL AEM] logo to access administrative tools.

   ![](assets/aemlogo.png)

2. From the administrative tools panel, click **Create/Manage Reports** to open **Asset Reports **page.

   ![](assets/access-asset-reports.png)

3. Access **Usage** report and other generated reports from Asset Reports page.

   >[!NOTE]
   >
   >Usage report is present by default in [!DNL Brand Portal]. Il ne peut pas être créé ni supprimé. Toutefois, vous pouvez créer, télécharger et supprimer les rapports Télécharger, Expiration, Publier, Partage de liens et Identifiants d'utilisateur.

   Pour afficher un rapport, appuyez/cliquez sur le lien du rapport. Vous pouvez également sélectionner le rapport, puis appuyer/cliquer sur l'icône Affichage dans la barre d'outils.

   Le rapport **Utilisation**[!DNL Brand Portal] affiche des informations sur le nombre d’utilisateurs de actuels, l’espace de stockage occupé par toutes les ressources et le nombre total des ressources dans [!DNL Brand Portal]. Il affiche également la capacité autorisée pour chacune de ces mesures.

   ![](assets/usage-report.png)

   Le rapport **Connexions des utilisateurs** fournit des informations concernant les utilisateurs qui se sont connectés à [!DNL Brand Portal]. The report shows display names, email IDs, personas (admin, viewer, editor, guest), groups, last login, activity status, and login count of each user from [!DNL Brand Portal] 6.4.2 deployment until the time of report generation.

   ![](assets/user-logins.png)

   Le rapport **Téléchargement** indique toutes les ressources téléchargées pendant une période et une plage horaire spécifiques.

   ![](assets/download-report.png)

   >[!NOTE]
   >
   >The assets** Download** report displays only the assets that were individually selected and downloaded from [!DNL Brand Portal]. Si un utilisateur a téléchargé un dossier contenant des ressources, le rapport n'affiche pas le dossier ou les actifs qu'il contient.

   Le rapport **Expiration** répertorie toutes les ressources qui sont arrivées à expiration pendant une période spécifique.

   ![](assets/expiration-report.png)

   **Publiez** les listes de rapports et fournit des informations sur toutes les ressources publiées depuis [!DNL AEM][!DNL Brand Portal] une période spécifiée.

   ![](assets/publish-report.png)

   >[!NOTE]
   >
   >Le rapport Publication n’affiche pas d’informations sur les fragments de contenu, car ils ne peuvent pas être publiés sur [!DNL Brand Portal].

   Le rapport **Partage de liens**[!DNL Brand Portal] répertorie toutes les ressources partagées à travers des liens à partir de l’interface de pendant une période spécifique. Le rapport indique également quand la ressource a été partagée par le biais du lien, par quel utilisateur, quand le lien expire et le nombre de liens partagés pour le client (et les utilisateurs avec lesquels le lien de la ressource a été partagé). Les colonnes du rapport Partage de liens ne sont pas personnalisables.

   ![](assets/link-share-report.png)

   >[!NOTE]
   >
   >Le rapport Partage de liens n’affiche pas les utilisateurs qui ont accès à une ressource partagée par le biais du lien ou qui ont téléchargé la ressource via le lien.
   >
   >
   >Pour effectuer le suivi des téléchargements réalisés par l’intermédiaire du lien partagé, vous devez générer le rapport de téléchargement après avoir sélectionné l’option **Uniquement les téléchargements via partage de lien** sur la page **Créer un rapport**. Cependant, l'utilisateur (téléchargé par) est anonyme dans ce cas.

## Génération de rapports {#generate-reports}

Administrators can generate and manage the following standard reports, once generated, they are saved to be [accessed](../using/brand-portal-reports.md#main-pars-header) later:

* Connexions des utilisateurs
* Télécharger
* Expiration
* Publication
* Partage de lien

Les colonnes des rapports Téléchargement, Expiration et Publication peuvent être personnalisées à des fins d’affichage. Pour générer un rapport, procédez comme suit :

1. From toolbar at the top, tap/click the [!DNL AEM] logo to access administrative tools.

   ![](assets/aemlogo.png)

2. From the administrative tools panel, tap/click **Create/Manage Reports** to open **Asset Reports **page.

   ![](assets/asset-reports.png)

3. Sur la page Rapports de ressources, appuyez/cliquez sur **Créer**.
4. From the **Create Report** page, select a report to create, and tap/click **Next**.

   ![](assets/crete-report.png)

5. Configurez les détails du rapport. Indiquez le titre, la description, la structure de dossiers (où le rapport doit s’exécuter et générer des statistiques) et la période pour les rapports **Téléchargement**, **Expiration** et **Publication**.

   ![](assets/create-report-page.png)

   Whereas, **Link Share Report** only needs the title, description, and date range parameters.

   ![](assets/create-link-share-report.png)

   >[!NOTE]
   >
   >Les caractères spéciaux # et % dans le titre du rapport sont remplacés par un tiret (-) sur la génération du rapport.

6. Tap/click **Next**, to configure the columns of Download, Expiration, and Publish reports.
7. Cochez ou décochez les cases adéquates selon vos besoins. For example, to view names of users (who downloaded assets) in **Download** report, select **Downloaded By**. L’image suivante montre comment sélectionner les colonnes par défaut dans le rapport Téléchargement.

   ![](assets/createdownloadreport.png)

   Vous pouvez également ajouter des colonnes personnalisées à ces rapports pour afficher davantage de données selon vos besoins.

   Pour ajouter des colonnes personnalisées au rapport Télécharger, Publier ou Expiration, procédez comme suit :

   1. To display a custom column, tap/click **Add** within **Custom Columns**.
   2. Specify name of the column in **Column Name** field.
   3. Sélectionnez la propriété à laquelle la colonne doit être associée à l’aide du sélecteur de propriété.

      ![](assets/property-picker.png)
Vous pouvez également saisir le chemin d’accès dans le champ de chemin d’accès à la propriété.

      ![](assets/property-path.png)

      Pour ajouter d’autres colonnes personnalisées, appuyez/cliquez sur **Ajouter** et répétez les étapes 2 et 3.

8. Cliquez/appuyez sur **Créer**. Un message indique que la génération du rapport a été lancée.

## Téléchargement de rapports {#download-reports}

Pour enregistrer et télécharger un rapport en tant que fichier .csv, effectuez l’une des opérations suivantes :

* Select a report on Asset Reports page, and tap/click **Download** from the toolbar at the top.

![](assets/download-asset-report.png)

* Dans la page Rapports de ressources, ouvrez un rapport. Select **Download** option from the top of the report page.

![](assets/download-report-fromwithin.png)

## Suppression de rapports {#delete-reports}

Pour supprimer un rapport existant, sélectionnez-le sur la page **Rapports de ressources** et appuyez/cliquez sur **Supprimer** dans la barre d’outils supérieure.

>[!NOTE]
>
>Le rapport **Utilisation** ne peut pas être supprimé.
