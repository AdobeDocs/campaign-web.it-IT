---
title: Creare un profilo
description: Scopri come creare un profilo in Campaign Web.
exl-id: 0680b726-8f2f-45bf-8aa0-c1d4aa1c2990
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 46%

---

# Creare un profilo {#profiles}

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_details"
>title="Dettagli di base"
>abstract="Questa sezione offre informazioni approfondite sui dettagli di base del profilo. Per modificare qualsiasi informazione, apporta le modifiche direttamente nel rispettivo campo e fai clic sul pulsante **Salva** nell’angolo superiore a destra dello schermo."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_contactinformation"
>title="Informazioni di contatto"
>abstract="Questa sezione offre informazioni approfondite sulle informazioni di contatto del profilo. Per modificare qualsiasi informazione, apporta le modifiche direttamente nel rispettivo campo e fai clic sul pulsante **Salva** nell’angolo superiore a destra dello schermo."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_address"
>title="Indirizzo"
>abstract="Questa sezione offre informazioni approfondite sull’indirizzo postale del profilo e sulla qualità dell’indirizzo. Per modificare qualsiasi informazione, apporta le modifiche direttamente nel rispettivo campo e fai clic sul pulsante **Salva** nell’angolo superiore a destra dello schermo."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_account"
>title="Dettagli dell’account"
>abstract="Questa sezione offre informazioni approfondite sui dettagli dell’account del profilo. Per modificare qualsiasi informazione, apporta le modifiche direttamente nel rispettivo campo e fai clic sul pulsante **Salva** nell’angolo superiore a destra dello schermo."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_nolongercontact"
>title="Da non contattare più"
>abstract="Questa sezione offre informazioni approfondite sulle preferenze di contatto del profilo. Per modificare qualsiasi informazione, apporta le modifiche direttamente nel rispettivo campo e fai clic sul pulsante **Salva** nell’angolo superiore a destra dello schermo."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_customfields"
>title="Campi personalizzati"
>abstract="I campi personalizzati sono attributi specifici personalizzati in base alle tue esigenze e configurati per la tua istanza. Per modificare qualsiasi informazione, apporta le modifiche direttamente nel rispettivo campo e fai clic sul pulsante **Salva** nell’angolo superiore a destra dello schermo."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_othersfields"
>title="Altri"
>abstract="Questa sezione fornisce attributi incorporati aggiuntivi. Per modificare qualsiasi informazione, apporta le modifiche direttamente nel rispettivo campo e fai clic sul pulsante **Salva** nell’angolo superiore a destra dello schermo."

Per creare un profilo, effettua le seguenti operazioni:

1. Passa a **[!UICONTROL Gestione clienti]** > **[!UICONTROL Profili]** e fai clic sul pulsante **[!UICONTROL Crea profilo]** nell&#39;angolo superiore destro della schermata.

1. Viene visualizzato l’elenco degli attributi disponibili per il profilo, organizzati in diverse sezioni descritte nella tabella seguente.

   ![Schermata con l&#39;elenco degli attributi disponibili per il profilo, suddivisa in sezioni](assets/create-profile.png){zoomable="yes"}

   | Sezione Attributi | Descrizione |
   |  ---  |  ---  |
   | **Dettagli di base** | Informazioni di base sul profilo, ad esempio nome o data di nascita.<br/>Per impostazione predefinita, i profili sono archiviati nella cartella **[!UICONTROL Destinatari]**. Puoi modificarlo navigando nella posizione desiderata. [Scopri come utilizzare le cartelle](../get-started/permissions.md#folders) |
   | **Informazioni di contatto** | Le informazioni di contatto del profilo, ad esempio l’indirizzo e-mail o il numero di telefono. |
   | **Indirizzo** | Indirizzo postale del profilo. In questa sezione viene inoltre fornita una valutazione della qualità dell&#39;indirizzo. L’indirizzo di un profilo è considerato valido se sono specificati i campi &quot;Cognome,&quot; &quot;Città&quot; e &quot;CAP&quot;. |
   | **Dettagli account** | Informazioni sull’account del profilo, ad esempio lo stato o il numero di account. |
   | **Non contattare più** | Preferenze di contatto del profilo. Quando una di queste opzioni è selezionata, il profilo si trova sul inserisco nell&#39;elenco Bloccati di.<br/>Ad esempio, se il destinatario ha fatto clic su un collegamento di annullamento dell&#39;abbonamento in una newsletter, queste informazioni vengono aggiunte ai dati di contatto. Questo destinatario non è più indirizzato ai canali selezionati. Ulteriori informazioni sulla gestione della quarantena nella [documentazione di Adobe Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/quarantines.html){target="_blank"} |
   | **Campi personalizzati** | Se i campi personalizzati sono stati configurati, vengono visualizzati in questa sezione. I campi personalizzati sono attributi aggiuntivi aggiunti allo schema **[!UICONTROL Profili]** tramite la console Adobe Campaign. Ulteriori informazioni sono disponibili nella [documentazione di Adobe Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/shemas-forms/extend-schema.html){target="_blank"} |
   | **Altri** | Attributi incorporati aggiuntivi. |

1. Dopo aver configurato il profilo, fai clic su **[!UICONTROL Crea]** per salvarlo nel database.

   Dopo il salvataggio, puoi modificare il profilo in qualsiasi momento aprendolo dall’elenco dei profili. [Scopri come esplorare i dettagli dei profili](profile-view.md).