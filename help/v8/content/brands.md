---
audience: end-user
title: Gestisci marchio
description: Scopri come creare e gestire le linee guida per il brand
exl-id: d4d2c6bb-7fd0-49a0-9d73-356f4a24f021
source-git-commit: f238fde4a79d3303f2b5c9a2d26b11ffad8ac54e
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 3%

---

# Creare e gestire i brand personali {#brands}

Le linee guida per il brand sono un set completo di regole e standard che definiscono l’identità visiva e verbale di un brand. Servono come riferimento per garantire una rappresentazione coerente del marchio in tutti i canali di marketing e comunicazione.

In [!DNL Adobe Campaign Web], gli utenti possono immettere e organizzare manualmente informazioni sul brand o caricare documenti di linee guida per il brand per l&#39;estrazione automatica dei dati.

## Accedere ai brand {#generative-access}

Per accedere al menu **[!UICONTROL Marchi]** in [!DNL Adobe Campaign Web], è necessario assegnare agli utenti i profili di prodotto **[!UICONTROL Amministratore (amministratore)]** e **[!UICONTROL Brand kit]** per creare e gestire i marchi. Per l&#39;accesso in sola lettura, gli utenti hanno bisogno del profilo di prodotto [!UICONTROL Assistente IA]. [Ulteriori informazioni](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/manage-permissions)

+++ Scopri come assegnare le autorizzazioni relative al brand

1. Nella home page di [Admin Console](https://adminconsole.adobe.com/enterprise), accedi al tuo prodotto Campaign.

   ![Pagina principale di Admin Console che mostra l&#39;accesso al prodotto Campaign](assets/brands_admin_1.png)

1. Selezionare **[!DNL Product profile]** in base al livello di autorizzazioni che si desidera concedere all&#39;utente.

   ![Selezione profilo prodotto in Admin Console](assets/brands_admin_2.png)

1. Fare clic su **[!DNL Add users]** per assegnare il profilo di prodotto selezionato.

   ![Opzione Aggiungi utenti in Admin Console](assets/brands_admin_3.png)

1. Digita il nome dell’utente, il gruppo di utenti o l’indirizzo e-mail.

1. Fai clic su **Salva** per applicare le modifiche.

Gli utenti già assegnati a questo ruolo dispongono di autorizzazioni aggiornate automaticamente.

+++

## Creare il brand {#create-brand-kit}

Per creare e gestire le linee guida per il tuo marchio, segui i passaggi indicati di seguito.

Gli utenti possono immettere i dettagli manualmente o caricare un documento sulle linee guida del brand per estrarre automaticamente le informazioni:

1. Nel menu **[!UICONTROL Marchi]**, fai clic su **[!UICONTROL Crea marchio]**.

   ![Menu Marchi con opzione Crea marchio](assets/brands-1.png)

1. Immetti un **[!UICONTROL Nome]** per il tuo marchio.

1. Trascina e rilascia o seleziona il file per caricare le linee guida per il brand ed estrarre automaticamente le informazioni rilevanti per il brand. Fai clic su **[!UICONTROL Crea marchio]**.

   Il processo di estrazione delle informazioni ora inizia. Il completamento potrebbe richiedere alcuni minuti.

   ![Caricamento di file per l&#39;estrazione delle linee guida per il brand](assets/brands-2.png)

1. I contenuti e gli standard di creazione visiva vengono ora compilati automaticamente. Sfoglia le diverse schede per adattare le informazioni in base alle esigenze. [Ulteriori informazioni](#personalize)

1. Dal menu avanzato di ogni sezione o categoria, puoi aggiungere riferimenti per estrarre automaticamente le informazioni rilevanti sul brand.

   Per rimuovere il contenuto esistente, utilizzare le opzioni **[!UICONTROL Cancella sezione]** o **[!UICONTROL Cancella categoria]**.

   ![](assets/brands-15.png)

1. Una volta configurata, fai clic su **[!UICONTROL Salva]**, quindi su **[!UICONTROL Pubblica]** per rendere disponibili le linee guida per il brand in AI Assistant.

1. Per apportare modifiche al tuo marchio pubblicato, fai clic su **[!UICONTROL Modifica marchio]**.

   >[!NOTE]
   >
   >In questo modo viene creata una copia temporanea in modalità di modifica, che sostituisce la versione live pubblicata.

   ![Modifica opzione marchio nel menu Marchi](assets/brands-8.png)

1. Dal dashboard **[!UICONTROL Brands]**, apri il menu avanzato facendo clic sull&#39;icona ![](assets/do-not-localize/Smock_More_18_N.svg) per:

   * Visualizza marchio
   * Modifica
   * Contrassegna come marchio predefinito
   * Duplica
   * Pubblicazione
   * Annulla pubblicazione
   * Elimina

   ![Opzioni di menu avanzate nel dashboard Marchi](assets/brands-6.png)

Le linee guida del brand sono ora accessibili dal menu a discesa **[!UICONTROL Brand]** nell&#39;Assistente di intelligenza artificiale. In questo modo l’Assistente AI può generare contenuti e risorse in linea con le specifiche dell’utente. [Ulteriori informazioni sull&#39;Assistente IA](../content/generative-gs.md)

Puoi anche utilizzare le linee guida del tuo marchio per valutare la qualità dei contenuti e l’allineamento del brand. [Ulteriori informazioni sulla convalida della qualità dei contenuti](brands-score.md#validate-quality)

![Menu dell&#39;assistente AI con elenco a discesa del marchio](assets/brands_6.png)

### Imposta un marchio predefinito {#default-brand}

Puoi designare un marchio predefinito da applicare automaticamente durante la generazione del contenuto e il calcolo dei punteggi di allineamento durante la creazione della campagna.

Per impostare un marchio predefinito, vai alla dashboard **[!UICONTROL Marchi]**. Apri il menu avanzato facendo clic sull&#39;icona ![](assets/do-not-localize/Smock_More_18_N.svg) e seleziona **[!UICONTROL Contrassegna come marchio predefinito]**.

![Opzioni di menu avanzate nel dashboard Marchi](assets/brands-6.png)

