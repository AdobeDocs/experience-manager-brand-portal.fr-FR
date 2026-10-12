---
title: Administrer l’accès des utilisateurs et utilisatrices sur Brand Portal
description: Configurez l’accès des invités et des nouveaux utilisateurs et utilisatrices sur Brand Portal.
contentOwner: mgulati
topic-tags: administration
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
role: Admin
exl-id: 27a9cd26-9bb3-473b-b1ac-37f77975c912
TQID: 'https://experienceleague.adobe.com/SGJ5f5BOFd4Yiu2OiR9wyRU3wk-YlnGrX5Zm5JmPHuY'
product_v2:
  - id: d09181b5-a36a-43de-ba01-36641440bc43
    internal-label: Experience Manager Assets
  - id: fd1f54a9-f50c-467d-8956-cebbaf4f3eb8
    internal-label: Experience Manager
feature_v2:
  - id: cda65036-5305-4f01-89da-9b3506ae8c50
    internal-label: Administration
  - id: da0dfbce-df02-4f8b-b32d-a4e3b1d05085
    internal-label: Configuration
  - id: a45b1e7f-e65f-4cd3-be86-5cec5d9449ef
    internal-label: Content management
subfeature_v2:
  - id: e00c7c12-7035-41fe-ad76-1ec82c8c3f01
    internal-label: Brand Portal
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4cfa580ba79b189ec4bcef8003c66734aa465ba3
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 32%
---
# Administrer l’accès des utilisateurs et utilisatrices sur Brand Portal {#administer-user-access-on-brand-portal}

À compter de la version 6.4.2, Adobe Experience Manager Assets Brand Portal autorise les administrateurs à configurer l’accès des invités et permet aux utilisateurs de demander l’accès sur le Brand Portal de leur entreprise. Ces configurations sont proposées sous forme de configurations de **[!UICONTROL Paramètres d’accès]** dans le panneau d’administration. Les deux paramètres sont désactivés par défaut.

![](assets/access-configs.png)

**A** - Configuration pour permettre aux invités d’accéder à Brand Portal à l’aide du lien **[!UICONTROL `Guest Access?`]** sur l’écran d’accueil de Brand Portal. (désactivée par défaut).

**B** - Configuration pour permettre aux utilisateurs de demander l’accès à Brand Portal à l’aide du lien **[!UICONTROL `Need access?`]** sur l’écran d’accueil de Brand Portal. (désactivée par défaut).

## Autoriser l’accès des invités {#allow-guest-access}

En autorisant l’accès des invités, les utilisateurs peuvent accéder aux ressources publiques sans avoir à se connecter à Brand Portal.
Pour autoriser l’accès des visiteurs et visiteuses anonymes, l’administrateur ou l’administratrice doit procéder comme suit :

1. Sélectionnez le logo AEM pour accéder aux outils d’administration dans la barre d’outils supérieure.
1. Dans le panneau Outils d’administration, sélectionnez **[!UICONTROL Accès]** pour ouvrir la page **[!UICONTROL Paramètres d’accès]**.
1. Activez la configuration **[!UICONTROL Autoriser l’accès des invités]**.
1. **[!UICONTROL Enregistrez]** les modifications.
1. Déconnectez-vous pour que les modifications soient prises en compte.

![](assets/bp-welcome-screen.png)

## Autoriser les utilisateurs à demander l’accès {#allow-users-to-request-access}

Les administrateurs peuvent autoriser les utilisateurs de l’entreprise à demander l’accès à Brand Portal à partir de l’écran de bienvenue. Toutefois, les administrateurs doivent activer la configuration **[!UICONTROL Autoriser les utilisateurs à demander l’accès]** afin que le lien de demande d’accès s’affiche sur l’écran de bienvenue.

Pour permettre aux utilisateurs de l’organisation de demander l’accès sur Brand Portal, les administrateurs doivent :

1. Sélectionnez le logo AEM pour accéder aux outils d’administration dans la barre d’outils supérieure.
1. Dans le panneau Outils d’administration, sélectionnez **[!UICONTROL Accès]** pour ouvrir la page **[!UICONTROL Paramètres d’accès]**.
1. Activez la configuration **[!UICONTROL Autoriser les utilisateurs à demander l’accès]**.
1. **[!UICONTROL Enregistrez]** les modifications.
1. Déconnectez-vous pour que les modifications soient prises en compte.
