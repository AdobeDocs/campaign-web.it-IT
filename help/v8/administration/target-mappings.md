---
title: Gestire le mappature target
description: Scopri come gestire destinazione mappature.
exl-id: 144d5650-9632-4af3-b64e-f6e81503a621
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 14%

---

# Gestire le mappature target {#target-mappings}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn2"
>title="Mappature target"
>abstract="È ora possibile creare mappature target nell’interfaccia utente di Campaign Web. Le mappature target definiscono il modo in cui i diversi canali di consegna (e-mail, SMS, notifiche push) si collegano ai campi dati di uno schema."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=it" text="Consulta le note sulla versione"

>[!CONTEXTUALHELP]
>id="acw_targetmapping_list"
>title="Mappature target "
>abstract="Mappature target"

## Informazioni sulle mappature destinazione {#about}

Ogni canale di comunicazione utilizza una mappatura destinazione predefinita per destinazione i propri destinatari. Ad esempio, per impostazione predefinita, i modelli per il recapito di e-mail e SMS destinazione **[!UICONTROL Destinatari.]** La mappatura destinazione utilizza quindi i **campi della tabella nms:recipient** . Per le notifiche push, il mapping destinazione predefinito è **Applicazioni sottoscrittore (nms:appSubscriptionRcp),** collegato alla tabella dei destinatari.

Target mappature sono accessibili dal **[!UICONTROL menu Mappature]** di Target > **[!UICONTROL Amministrazione]**. Da questa schermata è possibile accesso dettagli su ogni mappatura di destinazione o creare nuove mappature di destinazione in base alle proprie esigenze.

![Target schermata dell&#39;elenco delle mappature che mostra le mappature disponibili](assets/target-mappings-list.png)

Per ulteriori informazioni sui mapping di destinazione incorporati forniti con Adobe Campaign, fare riferimento alla documentazione[&#128279;](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html?lang=it){target="_blank"} della console client Campaign v8.

## Creare una mappatura target {#create-mapping}

>[!CONTEXTUALHELP]
>id="acw_targetmapping_properties"
>title="Proprietà mappatura target"
>abstract="La sezione **[!UICONTROL Proprietà]** ti consente di definire impostazioni generiche per mappatura e popolazione target."

>[!CONTEXTUALHELP]
>id="acw_targetmapping_mapping"
>title="Mappatura target"
>abstract="La sezione **[!UICONTROL Mappatura]** ti consente di identificare gli attributi dallo schema della mappatura target da utilizzare per i vari campi dell’indirizzo di consegna."

>[!CONTEXTUALHELP]
>id="acw_targetmapping_denylist"
>title="Elenco Bloccati mappatura target"
>abstract="Elenco Bloccati mappatura target"

>[!CONTEXTUALHELP]
>id="acw_targetmapping_storage"
>title="Archiviazione mappatura target"
>abstract="La sezione **[!UICONTROL Archiviazione]** ti consente di identificare dove devono essere archiviati i registri."

Per creare una nuova mappatura di destinazione, accesso l&#39;**[!UICONTROL >**&#x200B;[!UICONTROL &#x200B; Amministrazione &#x200B;]&#x200B;**Target menu mappature]**. Fai clic sull&#39;pulsante **[!UICONTROL di mappatura]** dei Crea, quindi seguire i passaggi descritti nelle sezioni seguenti.

1. **[!UICONTROL Nella sezione Proprietà]** immettere un **[!UICONTROL Etichetta]** per la mappatura destinazione.

1. Espandere la **[!UICONTROL sezione Opzioni aggiuntive]** per definire impostazioni avanzate, ad esempio il nome interno, la cartella di archiviazione e la descrizione della mappatura destinazione.

1. Seleziona la popolazione destinazione. Puoi:

   * **[!UICONTROL Utilizzare direttamente]** la dimensione targeting: selezionare la dimensione da destinazione direttamente dall&#39;elenco delle dimensioni disponibili.
   * **[!UICONTROL Usa dati]** collegati: Inizia da una dimensione targeting (ad esempio le sottoscrizioni) e quindi passa alla dimensione targeting che desideri destinazione (ad esempio destinatari).

   ![Proprietà mappature Target schermata con le opzioni di popolamento](assets/target-mappings-properties.png)

1. Se la dimensione selezionata non è già utilizzata da una mappatura destinazione esistente, è necessario creare gli schemi per store i log. Opzioni aggiuntive sono disponibili nella **[!UICONTROL sezione Archiviazione]** . Espandi la sezione seguente per ulteriori dettagli.

   +++Opzioni di archiviazione per nuove dimensioni targeting

   1. **&#x200B;**&#x200B;Spazio dei nomi: identifica lo spazio dei nomi che verrà utilizzato per creare i registri.
   1. **[!UICONTROL Suffisso dello schema]** di estensione: fornisci un suffisso per il nuovo schema.

      Nell&#39;esempio seguente, il nome broadlog sarà &quot;cusbroadlogSupplier&quot;.

      ![Esempio di opzioni di archiviazione per nuove dimensioni targeting](assets/target-mappings-new.png)

   1. **[!UICONTROL Registri di]** consegna: attiva le opzioni in questa sezione per arricchire i registri di invio con un campo di codice segmento o un campo contenente l&#39;indirizzo IP di consegna. Ad esempio, salvare un codice di segmento calcolato durante la workflow nei registri di invio per perfezionare il destinazione in un secondo momento. In questo modo è possibile targeting profili con questo specifico codice segmento.

   1. **[!UICONTROL Esclusioni]**: specifica come store i log delle esclusioni.

   1. **[!UICONTROL Registri di]** tracciamento: attivare l&#39;opzione Genera uno schema per il **[!UICONTROL rilevamento per]** generare uno schema di archiviazione per i registri di rilevamento.

   +++

1. Utilizzare la **[!UICONTROL sezione Mapping]** per identificare gli attributi dello schema del mapping di destinazione da utilizzare per ogni campo dell&#39;indirizzo di consegna. Per ogni campo, selezionare l&#39;attributo desiderato da mappare. È inoltre possibile versione un&#39;espressione per identificare il campo. Ad esempio, applicare una funzione inferiore all&#39;attributo address.

   ![Sezione di mappatura che mostra la selezione degli attributi per i campi dell&#39;indirizzo di consegna](assets/target-mappings-mapping.png)

1. Quando la mappatura destinazione è pronta, fare clic sull&#39;pulsante **[!UICONTROL Crea]** . Il sistema crea automaticamente la mappatura dei destinazione e tutti i relativi schemi per i log.

Una volta creata la mappatura destinazione, sullo schermo vengono visualizzate due sezioni aggiuntive:

* **[!UICONTROL Denylisting]**: questa sezione consente di identificare gli attributi dallo schema di mappatura del destinazione da utilizzare per i denilisti.

  ![Denylisting sezione che mostra la selezione di attributi](assets/target-mappings-denylisting.png)

* **[!UICONTROL Archiviazione]**: questa sezione consente di identificare le tabelle da utilizzare per store registri.

  ![Sezione Archiviazione che mostra le opzioni della tabella per i registri](assets/target-mappings-storage.png)

   * **[!UICONTROL Invia messaggio schema]**: identifica lo schema da utilizzare per store i registri di invio.
   * **[!UICONTROL Messaggi esclusi]**: specifica come gestire l&#39;archiviazione dei registri di recapito e di esclusione.

      * **[!UICONTROL Archiviare esclusioni e messaggi nella stessa tabella]**
      * **[!UICONTROL Archivia solo]** messaggi: non store esclusioni.
      * **[!UICONTROL Archiviare le esclusioni e i messaggi in tabelle]** separate: selezionare lo schema da utilizzare per store i registri di esclusione nel **[!UICONTROL campo Schema]** di rifiuto.

   * **[!UICONTROL Registri di]** tracciamento: scegli dove store i registri di tracciamento e l&#39;origine traffico predefinita.
   * **[!UICONTROL Campi]** aggiuntivi: specifica un elenco di campi aggiuntivi da store nei registri di consegna. Questi campi possono store in modo permanente informazioni sui singoli membri del destinazione (ad esempio, `recipient/@firstName`) o store dati aggiuntivi calcolati durante il workflow (ad esempio, `[targetData/@offeCode]`).

     A tale scopo, selezionare **[!UICONTROL Aggiungi campo]**. Identificare le informazioni da salvare nel **[!UICONTROL campo Origine]** e l&#39;attributo da utilizzare nei registri di invio per salvare queste informazioni nel **[!UICONTROL campo Destinazione]** .

     ![Sezione di campi aggiuntivi che mostra le opzioni per la memorizzazione di dati aggiuntivi](assets/target-mappings-additional.png){width="50%" zoomable="yes"}