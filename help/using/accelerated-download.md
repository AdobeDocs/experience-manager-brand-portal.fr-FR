---
title: Accélérer les téléchargements de Brand Portal
seo-title: Accélérer les téléchargements de Brand Portal
description: Améliorez les performances de téléchargement à partir de Brand Portal et des liens partagés.
seo-description: Améliorez les performances de téléchargement à partir de Brand Portal et des liens partagés.
uuid: 2871137e-6471-49a7-872a-841bd92543d1
contentOwner: mgulati
topic-tags: download-install
content-type: référence
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 301f7a0b-5527-4aac-b731-bfc145fed0c0
translation-type: tm+mt
source-git-commit: fb8243ea896d39b324a69ea534271ee3015c076f

---


# Accélérer les téléchargements de Brand Portal {#guide-to-accelerate-downloads-from-brand-portal}

Le portail de marque permet d'améliorer les performances de téléchargement des fichiers volumineux en s'intégrant à IBM Aspera Connect, une application d'installation à la demande. L'application utilise la technologie propriétaire pour supprimer les surcharges TCP et contribue à améliorer la vitesse de transfert des fichiers. Cette intégration garantit une expérience de téléchargement améliorée.

>[!NOTE]
>
>La vitesse de téléchargement varie selon les utilisateurs, car elle dépend de facteurs tels que la bande passante du réseau, la latence du serveur et l'emplacement géographique des clients.

Si cette option est activée, les utilisateurs de Brand Portal peuvent réduire considérablement le temps nécessaire pour télécharger les fichiers de ressources souhaités à partir de Brand Portal ou de liens partagés en installant le client Aspera Connect.

![](assets/enable-fast-file-download.png)

## Conditions préalables pour accélérer le téléchargement de fichiers  {#prerequisites-to-accelerate-file-download}

Pour télécharger les fichiers plus rapidement, vérifiez les éléments suivants :

* **[!UICONTROL Activez l'option Accélération]** de téléchargement (désactivée par défaut) à partir [!UICONTROL des paramètres] généraux du panneau Outils d'administration.
* Le port 33001 (TCP et UDP) est ouvert sur le pare-feu. Pour plus d'informations sur les conditions préalables, consultez [la documentation](https://downloads.asperasoft.com/en/documentation/8)du client Aspera Connect.
* Installez Aspera Connect à l'aide des privilèges d'administrateur.
* For platform support of Aspera transfer client, see [Aspera Connect platform support matrix](https://www.asperasoft.com/company/support/transfer-clients/).

## Téléchargement de domaines {#download-domains}

Vous trouverez ci-après les domaines de téléchargement pour différentes zones géographiques :

| Code région | Domaine |
|---|---|
| NA OR1 | downloads-na1.brand-portal.adobe.com |
| NA VA5 | downloads-na2.brand-portal.adobe.com |
| EMEA LON5 | downloads-emea1.brand-portal.adobe.com |
| APAC SIN2 | downloads-apac1.brand-portal.adobe.com |

## Sample download performance using file accelerator {#expected-download-performance-using-file-accelerator}

Le tableau suivant montre les performances de téléchargement de 2 Go à l'aide de l'accélérateur de téléchargement de fichiers Aspera Connect :

**Les résultats observés varient en raison de facteurs tels que la bande passante du réseau, la latence du serveur et l'emplacement du client. Le serveur de portail de marque se trouve à Oregon (États-Unis).*

| Emplacement du client | Latence entre le client et le serveur (millisecondes) | Vitesse avec Aspera Connect File Transfer Accelerator (mbps) | Temps nécessaire pour télécharger un fichier 2 Go avec l'accélérateur de transfert de fichier Aspera (secondes) |
|---------------------------|-----------------------------------|---------------------------------------------|-------------------------------------------------------------------------|
| Ouest des États-Unis (Californie du Nord) | 18 | 36 | 57 |
| Ouest des États-Unis (Oregon) | 42 | 36 | 57 |
| Est des États-Unis (Virginie du Nord) | 85 | 35 | 58 |
| Asie-Pacifique (Tokyo) | 124 | 36 | 57 |
| Noida (Inde) | 275 | 13.36 | 153 |
| Sydney | 175 | 29 | 70 |
| Londres | 179 | 35 | 58 |
| Singapour | 196 | 34 | 60 |

## Workflow de téléchargement avec l’accélérateur de fichiers {#download-workflow-using-file-accelerator}

Pour télécharger des ressources plus rapidement à partir de Brand Portal :

1. Connectez-vous au portail de marque à l'aide d'un navigateur pris en charge.
2. Recherchez et sélectionnez le fichier de ressource, le dossier ou la collection que vous souhaitez télécharger. Appuyez/cliquez sur l’option de téléchargement.
La boîte de dialogue de téléchargement s’affiche avec l’option [Activer l’accélération des téléchargements] sélectionnée.
   ![](assets/download-assetsbp.png)

   >[!NOTE]
   >
   >La fonctionnalité d’envoi d'e-mail de notification contenant le lien pour télécharger les ressources n’est actuellement pas prise en charge lorsque les téléchargements plus rapides sont activés.

   ![](assets/fast-download-emailchk.png)

3. Tap/click the **[!UICONTROL Download]** option.
Pour accélérer les téléchargements sur votre compte de client Brand Portal, l’application cliente Aspera Connect doit être installée sur votre système.

4. **Téléchargement du client Aspera Connect**

Si le client Aspera Connect n’est pas installé sur le système ou si le client installé est obsolète, une invite s’affiche sur la page du navigateur pour vous permettre de télécharger le client Aspera Connect spécifique au système en sélectionnant **[!UICONTROL Télécharger la dernière version]**.

   ![](assets/aspera-not-launched.png)

   To download the latest version of Aspera Connect from [https://downloads.asperasoft.com/connect2/](https://downloads.asperasoft.com/connect2/), select **[!UICONTROL Download Now]** and follow the instructions.

5. **Installation du client Aspera Connect** 
Pour installer la configuration du client IBM Aspera Connect, exécutez la configuration à partir du fichier. msi de l'application cliente IBM Aspera Connect et suivez l'assistant d'installation.

6. Une fois le client installé, actualisez la page du navigateur et recommencez la procédure de téléchargement ou sélectionnez **[!UICONTROL Redémarrer]** dans la boîte de dialogue **Téléchargement]de la ressource (étape 2).[!UICONTROL **
When using Aspera Connect for the first time, the browser prompts to open the link using **[!UICONTROL IBM Aspera Connect]**. Pour ignorer cette boîte de dialogue à l’avenir, activez **[!UICONTROL Mémoriser mon choix pour les liens FASP]**.

   >[!NOTE]
   >
   >Ce message varie en fonction du navigateur.

7. Une boîte de dialogue vous permet de confirmer si vous voulez poursuivre le transfert. Sélectionnez **[!UICONTROL Autoriser]pour commencer.**
To skip this dialog in future, enable **[!UICONTROL Use my choice for all connections with this host]**.
Le téléchargement démarre. Une boîte de dialogue affiche la progression du téléchargement. Use the dialog box to **[!UICONTROL pause]**, **[!UICONTROL resume]**, or **[!UICONTROL cancel]** the download.
L’application Aspera Connect fournit un workflow d’activité sur le système où l’utilisateur peut visualiser et gérer toutes les sessions de transfert. Pour plus d’informations, consultez la [documentation du client Aspera Connect](https://downloads.asperasoft.com/en/documentation/8).

![](assets/aspera-activity-window.png)

À la fin du téléchargement, la boîte de dialogue affiche l’emplacement où les ressources sont téléchargées sur le système de l’utilisateur. En cas d’échec, une erreur s’affiche.

>[!NOTE]
>
>There is a known limitation in Aspera Connect client application that no prompt to select download location appears if **[!UICONTROL Always ask me where to save downloaded files]** is enabled under the tab [!UICONTROL Transfers] within [!UICONTROL Preferences]. Avant tout téléchargement, fournissez donc l’emplacement dans la zone de texte **[!UICONTROL Enregistrer les fichiers téléchargés dans]**.

## Utilisation de l’accélérateur de fichiers sur le navigateur Microsoft Edge {#using-file-accelerator-on-microsoft-edge-browser}

Microsoft Edge s’exécute en mode protégé amélioré (EPM) qui empêche la communication avec le serveur Aspera Connect sur le même réseau privé ou avec un site de confiance. Par conséquent, une fenêtre s’affiche chaque fois qu’une connexion au serveur est établie.

![](assets/switchapps-msedge.png)

Pour utiliser la fonctionnalité de téléchargement accéléré sur Microsoft Edge, supprimez le site Brand Portal de la liste des sites de confiance.

1. Ouvrez le Panneau de configuration (appuyez sur la **[!UICONTROL touche Windows + X]**, puis sélectionnez **[!UICONTROL Panneau de configuration]**).
2. Accédez à **[!UICONTROL Réseau et Internet &gt; Options Internet]**. Cliquez sur l’onglet **[!UICONTROL Sécurité].**
3. Cliquez sur **[!UICONTROL Zone Sites de confiance**[!UICONTROL **, puis sur]Sites]**.
4. Supprimez le site Brand Portal de la liste.

## Préférences du client Aspera Connect  {#aspera-connect-client-preferences}

Certaines préférences utiles peuvent être définies dans les préférences du client IBM Aspera Connect en cliquant avec le bouton droit sur l’icône et en sélectionnant **[!UICONTROL Préférences]**.

![](assets/download_assets_frombrandportalimg19.png)

Vous pouvez définir l’emplacement de téléchargement par défaut.

![](assets/aspera-preferences.png)

En outre, le client Aspera Connect peut être marqué pour se lancer automatiquement au démarrage du système de manière à ce que le client de connexion soit exécuté et disponible pour que le téléchargement démarre plus rapidement.

![](assets/aspera-automaticallylaunch.png)

## Résolution des problèmes relatifs à l’accélération des téléchargements  {#troubleshoot-issues-with-download-acceleration}

Si l’accélération des téléchargements ne fonctionne pas, suivez ces étapes de dépannage :

1. Check that ports are not blocked, by visiting [https://test-connect.asperasoft.com](https://test-connect.asperasoft.com/) from your machine.

   Si les ports ne sont pas ouverts, demandez à votre équipe réseau de veiller à ce que les ports 33001 (à la fois TCP et UDP) ne soient pas bloqués dans le pare-feu.

2. Si les ports sont ouverts, vérifiez que votre réseau n’est pas trop lent en mesurant la bande passante disponible à l’aide de [/](https://www.speedtest.net/)https://www.speedtest.net/.

   Si la bande passante est faible (1 à 10 Mbit/s) ou en Kbit/s, utilisez les Préférences Aspera et essayez de limiter la bande passante en fonction de celle disponible.

3. Pour confirmer que les téléchargements à partir du serveur de démonstration d’Aspera fonctionnent, utilisez [](https://demo.asperasoft.com/aspera/user)https://demo.asperasoft.com/aspera/user\
   (nom d'utilisateur : asperaweb, mot de passe : demoaspera).

4. Si aucune des étapes de dépannage ci-dessus ne fonctionne, désélectionnez l’option Activer l’accélération des téléchargements et utilisez le téléchargement normal.
