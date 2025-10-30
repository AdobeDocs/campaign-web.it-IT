---
audience: end-user
title: Modificare il contenuto dell’e-mail
description: Scopri come iniziare a creare i contenuti utilizzando E-mail designer nell’interfaccia utente di Campaign Web
exl-id: a5b966bb-09da-4a50-98d4-010fdfbb75cf
source-git-commit: 16fe04858870c58b2f0244f33f691f1606050e61
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 100%

---


# Guida introduttiva a E-mail Designer {#get-started-email-designer}

Dopo aver creato un’e-mail in Adobe Campaign, è necessario definirne il contenuto.

E-mail Designer consente di creare e-mail accattivanti e personalizzate tramite un’interfaccia intuitiva con funzionalità di trascinamento della selezione. Partendo da zero, importando contenuti esistenti o sfruttando i modelli esistenti, puoi progettare e perfezionare tutti i contenuti per ogni e-mail, sia promozionale o transazionale.

<!--Built to deliver HTML optimized for responsive design, the Email Designer allows you to easily define and apply visibility conditions and dynamic content to an email, template, or content fragment directly through the user interface. You can seamlessly switch between the drag and drop interface and HTML code at the click of a button.

The Email Designer allows you to create email content and email content templates. It is compatible with simple emails, transactional emails, A/B test emails, multilingual emails, and recurring emails.-->

* Utilizza le funzionalità di progettazione delle e-mail di [!DNL Campaign] per creare e-mail dinamiche. [Ulteriori informazioni](create-email-content.md)

* Migliora l’esperienza cliente creando e-mail personalizzate in base agli attributi del profilo. [Ulteriori informazioni](../personalization/personalize.md)

* Configura i campi per contenuti condizionali per creare una personalizzazione dinamica in base al profilo del destinatario. [Ulteriori informazioni](../personalization/conditions.md)

## Best practice per la progettazione delle e-mail {#best-practices}

Quando si inviano le e-mail, tieni presente che i destinatari possono inoltrarle e, a volte, questo può causare problemi con il rendering. Ciò è particolarmente vero quando si utilizzano classi CSS che potrebbero non essere supportate dal provider e-mail utilizzato per l’inoltro. Ad esempio, se utilizzi la classe CSS “is-desktop-hidden” per nascondere un’immagine su dispositivi mobili, il rendering potrebbe non essere corretto.

Per ridurre al minimo questi problemi di rendering, ti consigliamo di mantenere la struttura della tua e-mail il più semplice possibile. Prova a utilizzare un’unica progettazione che funzioni bene sia per i dispositivi desktop che mobili ed evita di utilizzare classi CSS complesse o altri elementi di progettazione che potrebbero non essere completamente supportati da tutti i client e-mail. Quando utilizzi le immagini nelle e-mail, evita quelle di dimensioni superiori a 2 MB o utilizza collegamenti immagine codificati.

Seguendo queste best practice, puoi contribuire a garantire che le e-mail vengano visualizzate correttamente in modo coerente, indipendentemente da come vengono visualizzate o inoltrate dai destinatari.

## Iniziare a creare i contenuti {#start-authoring}

Dalla dashboard di consegna e-mail, passa alla schermata [Modifica contenuto](edit-content.md) per aprire la pagina Home di E-mail designer. Da qui, scegli come progettare l’e-mail tra le seguenti opzioni:

* **Creare un messaggio e-mail da zero** tramite l’interfaccia di E-mail designer. Scopri come progettare il contenuto delle e-mail in [questa sezione](create-email-content.md).

* **Immetti o incolla il codice HTML non elaborato** direttamente in E-mail designer. Scopri come codificare i contenuti in [questa sezione](code-content.md).

* **Importa contenuto HTML esistente** da un file o da una cartella .zip. Scopri come importare un contenuto e-mail in [questa sezione](existing-content.md).

* **Seleziona un contenuto esistente** da un elenco di modelli incorporati o personalizzati. Scopri come utilizzare i modelli e-mail in [questa sezione](../content/create-email-templates.md).

  ![Opzioni disponibili nell’interfaccia di E-mail designer per la creazione di contenuti e-mail](assets/email_designer_create_options.png){zoomable="yes"}
