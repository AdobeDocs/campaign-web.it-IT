---
audience: end-user
title: Creare e-mail multilingue con Adobe Experience Manager
description: Scopri come creare consegne e-mail multilingue utilizzando copie in lingua Adobe Experience Manager in Campaign Web.
feature: Email
topic: Content Management
role: User
level: Intermediate
exl-id: 6fc6ff43-ac7f-46c7-aa1a-9489ffc45423
source-git-commit: 3a5121a4dca59532e1aada49c26de6ece1a58e4b
workflow-type: tm+mt
source-wordcount: '546'
ht-degree: 2%

---

# Creare e-mail multilingue con Adobe Experience Manager {#aem-multilingual}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn3"
>title="Experience Manager Live e copie per lingua"
>abstract="Ora puoi accedere alla lingua e alle Live Copy di Adobe Experience Manager direttamente in Campaign. L&#39;aggiornamento dei contenuti in tempo reale elimina la sincronizzazione manuale per flussi di lavoro multilingue semplificati."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=it" text="Consulta le note sulla versione"

L’integrazione di Adobe Experience Manager consente di creare consegne e-mail multilingue utilizzando copie in lingua Adobe Experience Manager. Questo consente di gestire varianti di contenuto in lingue diverse e di inviare e-mail personalizzate in base alle preferenze della lingua del destinatario.

## Prerequisiti {#prerequisites}

Prima di creare una consegna e-mail multilingue, assicurati di disporre di:

* Accesso a un’istanza di Adobe Experience Manager configurata per l’integrazione dell’interfaccia web di Adobe Campaign.
* Contenuto Adobe Experience Manager con copie per lingua già creato e approvato. Ulteriori informazioni sulla Creazione guidata copia in lingua nella [documentazione di Adobe Experience Manager](https://experienceleague.adobe.com/it/docs/experience-manager-cloud-service/content/sites/administering/reusing-content/translation/wizard)
* Modello di consegna e-mail configurato per ricevere contenuti Adobe Experience Manager. Consulta i passaggi descritti nella sezione [Abilitare la modalità multilingue](#enable-multilingual).

## Creare una consegna multilingue

Per creare una consegna e-mail multilingue, devi innanzitutto abilitare l’opzione multilingue nelle impostazioni di consegna. Il sistema rileva automaticamente le copie per lingua disponibili e consente di scegliere quali aggiungere.

### Abilita modalità multilingue {#enable-multilingual}

Crea una nuova consegna e abilita l’opzione multilingue nelle impostazioni avanzate.

1. Dal menu **[!UICONTROL Consegne]**, fai clic su **[!UICONTROL Crea consegna]**.

   ![](assets/lg-copy-1.png)

1. Seleziona il modello **[!UICONTROL Email delivery con contenuto AEM]** e fai clic su **[!UICONTROL Create delivery]**.

   ![](assets/lg-copy-2.png)

1. Immetti un’etichetta per la consegna e configura il pubblico. [Ulteriori informazioni](../email/create-email.md)

1. Accedi alle **[!UICONTROL Impostazioni]** della consegna, quindi passa alla sezione **[!UICONTROL Avanzate]**.

1. Abilita l&#39;opzione **[!UICONTROL Abilita AEM multilingue]**.

   ![](assets/lg-copy-3.png)

1. Assicurati che:

   * **[!UICONTROL Modalità di modifica contenuto]** è impostata su **[!UICONTROL AEM]**.
   * È selezionato l&#39;account Adobe Experience Manager **[!UICONTROL esterno]** corretto.

1. Fai clic su **[!UICONTROL Salva e chiudi]**.

### Crea varianti di contenuto {#create-variants}

Seleziona il contenuto Adobe Experience Manager e scegli le varianti di lingua da includere nella consegna.

1. Fare clic su **[!UICONTROL Modifica contenuto]**.

1. Seleziona **[!UICONTROL Crea variante di contenuto]**.

   ![](assets/lg-copy-4.png)

1. Seleziona il contenuto Adobe Experience Manager dall’elenco.

   ![](assets/lg-copy-5.png)

1. Il sistema rileva tutte le copie in lingua associate al contenuto selezionato (relazione padre-figlio). Ad esempio, se il contenuto Adobe Experience Manager presenta varianti in francese, tedesco e italiano, tutte le varianti sono disponibili per la selezione.

   Seleziona le varianti di lingua da includere nella consegna.

   ![](assets/lg-copy-6.png)

1. Fai clic su **[!UICONTROL Salva]**.

1. Esamina le varianti di lingua nell’editor dei contenuti. Ora puoi [gestire ogni variante singolarmente](#manage-variants) o procedere con [l&#39;invio della consegna](../monitor/prepare-send.md).

   ![](assets/lg-copy-7.png)

## Gestione varianti di lingua {#manage-variants}

Dopo aver creato le varianti di contenuto, puoi gestirle direttamente nella consegna:

1. Per impostare una lingua predefinita, accedere al menu avanzato per la variante scelta e selezionare **[!UICONTROL Imposta come predefinita]**. La lingua predefinita viene utilizzata quando le preferenze della lingua di un profilo non sono impostate o non corrispondono a nessuna variante disponibile.

   Fai clic su **[!UICONTROL Elimina]** per rimuovere qualsiasi variante dalla consegna.

   ![](assets/lg-copy-8.png)

1. Dal menu avanzato delle varianti di contenuto, fai clic su **[!UICONTROL Gestisci impostazioni internazionali]** per aggiungere altre impostazioni internazionali alla consegna.

   ![](assets/lg-copy-9.png)

1. Seleziona copie in altre lingue per includere altre varianti e fai clic su **[!UICONTROL Salva]**.

   ![](assets/lg-copy-11.png)

1. Se il contenuto viene aggiornato in Adobe Experience Manager, fare clic su **[!UICONTROL Aggiorna contenuto AEM]** per sincronizzare tutte le varianti con la versione più recente.

   ![](assets/lg-copy-10.png)

1. Fai clic su **[!UICONTROL Scollega contenuto AEM]** se desideri modificare il contenuto direttamente in Campaign o interrompere il collegamento con Adobe Experience Manager.

   >[!CAUTION]
   >
   >Dopo lo scollegamento, non è possibile aggiornare il contenuto da Adobe Experience Manager o creare nuove varianti. Il contenuto diventa indipendente da Adobe Experience Manager.
