---
title: Partage d’une collection
seo-title: Partage d’une collection
description: Les administrateurs d’AEM Assets Brand Portal peuvent partager et annuler le partage d’une collection, dynamique ou non, avec les utilisateurs autorisés. Les éditeurs peuvent uniquement visualiser et partager les collections créées par eux et partagées avec eux, ainsi que les collections publiques.
seo-description: Les administrateurs d’AEM Assets Brand Portal peuvent partager et annuler le partage d’une collection, dynamique ou non, avec les utilisateurs autorisés. Les éditeurs peuvent uniquement visualiser et partager les collections créées par eux et partagées avec eux, ainsi que les collections publiques.
uuid: 965 f 39 cd -1378-42 c 1-a 58 a -01 e 1 bf 825 aa 3
contentOwner: bdhar
content-type: référence
topic-tags: partage
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
discoiquuid: f 053013 e -5981-419 f -927 e-b 5 bb 1 d 47 eae 2
translation-type: tm+mt
source-git-commit: 0b70e82d034ce56fcfc5b49396e6d3a9da4b49d4

---


# Partage de collections sur le portail de marque {#share-collections-bp}

Les administrateurs d’AEM Assets Brand Portal peuvent partager et annuler le partage d’une collection, dynamique ou non, avec les utilisateurs autorisés. Les éditeurs peuvent uniquement visualiser et partager les collections créées par eux et partagées avec eux, ainsi que les collections publiques. Cependant, les éditeurs ne peuvent pas modifier une collection publique en collection non publique.

>[!NOTE]
>
>Editors cannot change a public collection to a non-public collection and, therefore, do not have **Public Collection** check box available in **Collection Settings** dialog.

## Partage d’une collection {#share-collection}

Pour partager une collection, procédez comme suit :

1. Cliquez sur l’icône de recouvrement située à gauche, puis sélectionnez **Navigation**.

   ![](assets/contenttree-1.png)

1. From the siderail on the left, click **Collections**.

   ![](assets/access_collections.png)

1. Dans la console **Collections**, effectuez l’une des opérations suivantes :

   * Placez le pointeur sur la collection que vous souhaitez partager. Dans les miniatures d’action rapide disponibles pour la collection, cliquez sur l’icône **Paramètres**.
   ![](assets/settings_thumbnail.png)

   * Sélectionnez la collection que vous souhaitez partager. From the toolbar at the top, click **Settings**.
   ![](assets/collection-sharing.png)

1. In the **Collection Settings** dialog box, select the users or groups with whom you want to share the collection and select the role for a user or a group to match their global role. Par exemple, affectez le rôle Éditeur à un éditeur global ou le rôle Visualisateur à un visualisateur global.

   Alternatively, to make the collection available to all users irrespective of their group membership and role, make it public by selecting the **Public Collection** check box.

   >[!NOTE]
   >
   >Les utilisateurs qui ne sont pas administrateurs peuvent toutefois ne pas être autorisés à créer des collections publiques, afin de limiter le nombre de collections publiques et gagner ainsi de l’espace sur le système. Organizations can disable the **Allow public collections creation** configuration from **General** settings available in admin tools panel.

   ![](assets/collection_sharingadduser.png)

   Editors cannot change a public collection to a non-public collection and, therefore, do not have **Public Collection** check box available in **Collection Settings** dialog.

   ![](assets/collection-setting-editor.png)

1. Click **Add**, and then **Save**. La collection est partagée avec les utilisateurs sélectionnés.

   >[!NOTE]
   >
   >Le rôle d’un utilisateur détermine l’accès aux ressources et aux dossiers d’une collection. Si un utilisateur n'a pas accès aux ressources, une collection vide est partagée avec l'utilisateur. Le rôle d’un utilisateur détermine aussi les actions disponibles pour les collections.

## Annulation du partage d’une collection {#unshare-a-collection}

Pour annuler le partage d’une collection précédemment partagée, procédez comme suit :

1. Dans la console **Collections**, sélectionnez la collection pour laquelle vous souhaitez annuler le partage.

   In the toolbar, click **Settings**.

   ![](assets/collection_settings.png)

1. On the **Collection Settings** dialog box, under **Members**, click the **x** symbol next to users or groups to remove them from the list of users you shared the collection with.

   ![](assets/unshare_collection.png)

1. Dans la boîte de message d’avertissement, cliquez sur **Confirmer** pour confirmer l’annulation du partage.

   Cliquez sur **Enregistrer**.

1. Connectez-vous à Brand Portal avec les informations d'identification de l'utilisateur que vous avez supprimé de la liste partagée. La collection est supprimée de la console **Collections**.
