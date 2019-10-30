---
title: Chargement de la liste des utilisateurs de Brand Portal
seo-title: Chargement de la liste des utilisateurs de Brand Portal
description: 'Découvrez comment charger la liste des utilisateurs de Brand Portal dans AEM Assets. '
seo-description: Découvrez comment charger la liste des utilisateurs de Brand Portal dans AEM Assets.
uuid: null
content-type: reference
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: ht
source-git-commit: f7f8c507d7f9866025987317af23f25c0b51c332

---


# Chargement de la liste des utilisateurs de Brand Portal {#upload-bp-user-list}

Les administrateurs d’AEM peuvent charger le fichier de configuration des utilisateurs de Brand Portal (.csv) contenant la liste des utilisateurs Brand Portal actifs dans AEM Assets. Un dossier de contribution peut uniquement être partagé avec les utilisateurs actifs de Brand Portal définis dans la liste des utilisateurs. L’administrateur peut également ajouter de nouveaux utilisateurs dans le fichier de configuration et charger la liste modifiée des utilisateurs.

Il peut ajouter de nouveaux utilisateurs dans AEM Admin Console. Pour plus d’informations, voir [Gestion des utilisateurs](brand-portal-adding-users.md). Une fois des utilisateurs ajoutés dans Admin Console, ceux-ci peuvent être ajoutés au fichier de configuration des utilisateurs de Brand Portal, puis se voir attribuer l’autorisation d’accéder au dossier de contribution.

**Pour charger la liste des utilisateurs de Brand Portal, procédez comme suit :**
1. Connectez-vous à votre instance d’auteur AEM
URL par défaut : http:// localhost:4502/aem/start.html
1. Dans le panneau **Outils** ![](assets/tools.png), accédez à **[!UICONTROL Ressources &gt; Utilisateurs Brand Portal]**.
   ![](assets/upload-user-list1.png)
1. La fenêtre de chargement des contributeurs de Brand Portal s’affiche.
Recherchez sur votre ordinateur local le **fichier de configuration (.csv)** contenant la liste des utilisateurs actifs de Brand Portal, puis chargez-le.
1. Cliquez sur **[!UICONTROL Enregistrer]**.
   ![](assets/upload-user-list2.png)


Les administrateurs peuvent donner un accès à des utilisateurs/groupes spécifiques à partir de cette liste d’utilisateurs lors de la configuration du dossier de contribution.

Pour plus d’informations, voir [Configuration du dossier de contribution](brand-portal-contribution-folder.md).
