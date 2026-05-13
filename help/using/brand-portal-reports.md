---
title: Utilisation des rapports
description: Les administrateurs et administratrices de Experience Manager Assets Brand Portal peuvent afficher des rapports sur l’utilisation de Brand Portal, ainsi que créer, gérer et afficher des rapports sur les ressources téléchargées, expirées, publiées, et les liens partagés via Brand Portal.
content-type: reference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
role: Admin
exl-id: 03d0292c-23c2-4ea0-9781-eb27768e6c33
TQID: https://experienceleague.adobe.com/4p-phv75ZqbWNLAxXeZ-QEpZxSTgv-oV8AEIbue9Zvw
product_v2:
  - id: d09181b5-a36a-43de-ba01-36641440bc43
  - id: fd1f54a9-f50c-467d-8956-cebbaf4f3eb8
feature_v2:
  - id: cda65036-5305-4f01-89da-9b3506ae8c50
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e48edcb1ed5d76686794f7a7ed6389c7f4ab1ed3
workflow-type: tm+mt
source-wordcount: 1010
ht-degree: 35%

---

# Utilisation des rapports {#work-with-reports}

La fonctionnalité de création de rapports de Brand Portal permet d’évaluer l’utilisation de Brand Portal et la façon dont les utilisateurs internes et externes interagissent avec les ressources approuvées. Les administrateurs peuvent afficher le rapport Utilisation de Brand Portal, qui est toujours disponible sur la page Rapports de ressources. Cependant, les rapports sur les connexions des utilisateurs et les ressources téléchargées, expirées, publiées et partagées par le biais de liens peuvent être générés et affichés à partir de la page Rapports de ressources . Ces rapports s’avèrent utiles pour analyser le déploiement des ressources et permettent d’obtenir des indicateurs clés de réussite pour mesurer l’adoption des ressources approuvées au sein et en dehors de l’organisation.

L’interface de gestion des rapports est intuitive et contient des options et commandes précises pour accéder aux rapports enregistrés. Vous pouvez consulter, télécharger ou supprimer des rapports à partir de la page Rapports de ressources, dans laquelle tous les rapports générés auparavant sont répertoriés.

## Affichage des rapports {#view-reports}

Pour afficher un rapport, procédez comme suit :

1. Dans la barre d’outils supérieure, cliquez sur le logo Experience Manager pour accéder aux outils d’administration.

   ![](assets/aemlogo.png)

1. Dans le panneau des outils d’administration, cliquez sur **[!UICONTROL Créer/gérer des rapports]** pour ouvrir la page **[!UICONTROL Rapports de ressources]**.

   ![](assets/access-asset-reports.png)

1. Accédez au rapport **[!UICONTROL Utilisation]** et aux autres rapports générés à partir de la page Rapports de ressources.

   >[!NOTE]
   >
   >Le rapport d’utilisation est un rapport par défaut généré dans Brand Portal. Elle ne peut pas être créée ou supprimée. Cependant, vous pouvez créer, télécharger et supprimer les rapports Téléchargement, Expiration, Publication, `Link Share` et Connexions des utilisateurs.

   Pour afficher un rapport, cliquez sur son lien. Vous pouvez également sélectionner le rapport, puis cliquer sur l’icône Affichage dans la barre d’outils.

   Le **[!UICONTROL Rapport d’utilisation]** affiche des informations sur le nombre d’utilisateurs Brand Portal actifs, l’espace de stockage occupé par toutes les ressources et le nombre total de ressources dans Brand Portal. Les utilisateurs de Brand Portal qui ne sont affectés à aucun profil de produits dans Admin Console sont considérés comme des utilisateurs inactifs et ne sont pas reflétés dans le **[!UICONTROL rapport d’utilisation]**.
Il affiche également la capacité autorisée pour chacune de ces mesures.

   ![](assets/usage-report.png)

   Le rapport **[!UICONTROL Connexions utilisateur]** donne des informations sur les utilisateurs qui se sont connectés à Brand Portal. Le rapport affiche les noms d’affichage, les ID d’e-mail, les rôles (administrateur, observateur, éditeur, invité), les groupes, la dernière connexion, le statut d’activité et le nombre de connexions de chaque utilisateur depuis le déploiement de Brand Portal 6.4.2 jusqu’à la génération du rapport.

   ![](assets/user-logins.png)

   Le rapport **[!UICONTROL Télécharger]** détaille toutes les ressources téléchargées pendant une période et une plage horaire spécifiques.

   ![](assets/download-report.png)

   >[!NOTE]
   >
   >Le rapport **[!UICONTROL Télécharger]** de ressources affiche uniquement les ressources qui ont été sélectionnées et téléchargées individuellement à partir de Brand Portal. Si un utilisateur a téléchargé un dossier contenant des ressources, le rapport n’affiche pas le dossier ou les ressources qu’il contient.

   Le rapport **[!UICONTROL Expiration]** répertorie et détaille toutes les ressources qui ont expiré au cours d’une période spécifique.

   ![](assets/expiration-report.png)

   Le rapport **[!UICONTROL Publication]** répertorie et donne des informations sur toutes les ressources qui sont publiées d’Experience Manager Assets sur Brand Portal dans une période spécifiée.

   ![](assets/publish-report.png)

   >[!NOTE]
   >
   >Le rapport Publication n’affiche pas d’informations sur les fragments de contenu, car ils ne peuvent pas être publiés sur Brand Portal.

   Le rapport **[!UICONTROL Partage de liens]** répertorie toutes les ressources partagées par le biais de liens à partir de l’interface de Brand Portal au cours d’une période spécifique. Le rapport détaille la date de partage de la ressource par le biais d’un lien, l’utilisateur ou l’utilisatrice qui l’a partagée et la date d’expiration du lien. Il indique également le nombre de liens partagés pour le client et les utilisateurs et utilisatrices. Les colonnes du rapport Partage de liens ne sont pas personnalisables.

   ![](assets/link-share-report.png)

   >[!NOTE]
   >
   >Le rapport Partage de liens n’affiche pas les utilisateurs et utilisatrices qui ont accès à la ressource partagée au moyen du lien ou qui ont téléchargé la ressource via le lien.
   >
   >Pour effectuer le suivi des téléchargements via le lien partagé, vous devez générer un rapport de téléchargement après avoir sélectionné l’option **[!UICONTROL Uniquement les téléchargements avec partage de lien]** sur la page **[!UICONTROL Créer un rapport]**. Cependant, l’utilisateur (téléchargé par) est anonyme dans ce cas.

## Génération de rapports {#generate-reports}

Les administrateurs et administratrices peuvent générer et gérer les rapports standard suivants. Une fois générés, les rapports sont enregistrés pour [accès ultérieur](../using/brand-portal-reports.md#main-pars-header).

* Connexions des utilisateurs
* Téléchargement
* Expiration
* Publication
* Partage de liens

L’affichage des colonnes des rapports Téléchargement, Expiration et Publication peut être personnalisé. Pour générer un rapport, procédez comme suit :

1. Dans la barre d’outils supérieure, cliquez sur le logo Experience Manager pour accéder aux outils d’administration.

1. Dans le panneau des outils d’administration, cliquez sur **[!UICONTROL Créer/gérer des rapports]** pour ouvrir la page **[!UICONTROL Rapports de ressources]**.

   ![](assets/asset-reports.png)

1. Dans la page Rapports de ressources, cliquez sur **[!UICONTROL Créer]**.
1. Sur la page **[!UICONTROL Créer un rapport]**, sélectionnez un rapport à créer, puis cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/crete-report.png)

1. Configurez les détails du rapport. Indiquez le titre, la description, la structure des dossiers (où le rapport doit s’exécuter et générer des statistiques) et la période des rapports **[!UICONTROL Téléchargement]**, **[!UICONTROL Expiration]** et **[!UICONTROL Publication]**.

   ![](assets/create-report-page.png)

   Le rapport **[!UICONTROL Partage de liens]** n’a besoin que des paramètres de titre, de description et de période.

   ![](assets/create-link-share-report.png)

   >[!NOTE]
   >
   >La génération du rapport remplace les caractères spéciaux `#` et `%` dans le titre par un trait d’union (-).

1. Cliquez sur **[!UICONTROL Suivant]** pour configurer les colonnes des rapports Téléchargement, Expiration et Publication.
1. Cochez ou décochez les cases pertinentes selon vos besoins. Par exemple, pour afficher les noms des utilisateurs (qui ont téléchargé des ressources) dans le rapport **[!UICONTROL Télécharger]**, sélectionnez **[!UICONTROL Téléchargé par]**. L’image suivante illustre la sélection des colonnes par défaut dans le rapport Télécharger .

   ![](assets/createdownloadreport.png)

   Vous pouvez également ajouter des colonnes personnalisées à ces rapports pour afficher davantage de données en fonction de vos besoins.

   Pour ajouter des colonnes personnalisées au rapport de téléchargement, de publication ou d’expiration, procédez comme suit :

   1. Pour afficher une colonne personnalisée, cliquez sur **[!UICONTROL Ajouter]** dans [!UICONTROL Colonnes personnalisées].
   1. Indiquez le nom de la colonne dans le champ **[!UICONTROL Nom de la colonne]**.
   1. Sélectionnez la propriété à laquelle la colonne doit mapper à l’aide d’un sélecteur de propriétés.

      ![](assets/property-picker.png)
Vous pouvez également saisir le chemin d’accès dans le champ de chemin d’accès à la propriété.

      ![](assets/property-path.png)

      Pour ajouter d’autres colonnes personnalisées, cliquez sur **Ajouter** et répétez les étapes 2 et 3.

1. Cliquez sur **[!UICONTROL Créer]**. Un message indique que la génération du rapport a été lancée.

## Téléchargement de rapports {#download-reports}

Pour enregistrer et télécharger un rapport en tant que fichier .csv, effectuez l’une des opérations suivantes :

* Sélectionnez un rapport sur la page Rapports de ressources, puis cliquez sur **[!UICONTROL Télécharger]** dans la barre d’outils supérieure.

![](assets/download-asset-report.png)

* Dans la page Rapports de ressources, ouvrez un rapport. Sélectionnez l’option **[!UICONTROL Télécharger]** en haut de la page du rapport.

![](assets/download-report-fromwithin.png)

## Suppression de rapports {#delete-reports}

Pour supprimer un rapport existant, sélectionnez-le dans la page **[!UICONTROL Rapports de ressources]** et cliquez sur **[!UICONTROL Supprimer]** dans la barre d’outils supérieure.

>[!NOTE]
>
>Le rapport **[!UICONTROL Utilisation]** ne peut pas être supprimé.
