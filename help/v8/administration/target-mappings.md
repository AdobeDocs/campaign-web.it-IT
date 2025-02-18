---
title: Gestire le mappature target
description: Scopri come gestire le mappature di destinazione.
source-git-commit: c0a40e8c68b009b6803d8f24e6572c4ea359ba9f
workflow-type: tm+mt
source-wordcount: '751'
ht-degree: 2%

---

# Gestire le mappature target {#target-mappings}

>[!CONTEXTUALHELP]
>id="acw_targetmapping_list"
>title="Mappature target "
>abstract="Mappature target"

## Informazioni sulle mappature di destinazione {#about}

Ogni canale di comunicazione utilizza una mappatura target predefinita per eseguire il targeting dei propri destinatari. Ad esempio, per impostazione predefinita, i modelli di consegna e-mail e SMS sono destinati a **[!UICONTROL Destinatari]**. La mappatura di destinazione utilizza pertanto i campi della tabella **nms:recipient**. Per le notifiche push, il mapping di destinazione predefinito è **Applicazioni in abbonamento (nms:appSubscriptionRcp)**, che è collegato alla tabella dei destinatari.

I mapping di destinazione sono accessibili dal menu **[!UICONTROL Amministrazione]** > **[!UICONTROL Mapping di destinazione]**. Da questa schermata, puoi accedere ai dettagli su ogni mappatura di destinazione, oppure creare nuove mappature di destinazione in base alle tue esigenze.

![](assets/target-mappings-list.png)

Per ulteriori informazioni sui mapping di destinazione incorporati forniti con Adobe Campaign, consulta la [documentazione della console client di Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html?lang=it){target="_blank"}.

## Creare una mappatura di destinazione {#create-mapping}

>[!CONTEXTUALHELP]
>id="acw_targetmapping_properties"
>title="Proprietà mappatura target"
>abstract="La sezione **[!UICONTROL Proprietà]** consente di definire impostazioni generiche per la mappatura di destinazione e la popolazione di destinazione."

>[!CONTEXTUALHELP]
>id="acw_targetmapping_mapping"
>title="Mappatura target"
>abstract="La sezione **[!UICONTROL Mapping]** ti consente di identificare gli attributi dallo schema della mappatura di destinazione da utilizzare per i vari campi dell&#39;indirizzo di consegna."

>[!CONTEXTUALHELP]
>id="acw_targetmapping_denylist"
>title="Elenco Bloccati mappatura target"
>abstract="Elenco Bloccati mappatura target"

>[!CONTEXTUALHELP]
>id="acw_targetmapping_storage"
>title="Archiviazione mappatura target"
>abstract="La sezione **[!UICONTROL Archiviazione]** ti consente di identificare dove devono essere archiviati i registri."

Per creare una nuova mappatura di destinazione, accedere al menu **[!UICONTROL Amministrazione]** > **[!UICONTROL Mappature di destinazione]**. Fai clic sul pulsante **[!UICONTROL Crea mappatura]**, quindi segui i passaggi descritti nelle sezioni seguenti.

1. Nella sezione **[!UICONTROL Proprietà]** immettere un **[!UICONTROL Etichetta]** per la mappatura di destinazione.

1. Espandi la sezione **[!UICONTROL Opzioni aggiuntive]** per definire impostazioni avanzate, ad esempio il nome interno della mappatura di destinazione, la cartella di archiviazione e la descrizione.

1. Seleziona la popolazione target. Puoi effettuare le seguenti operazioni:

   * **[!UICONTROL Utilizza direttamente la dimensione di targeting]**: seleziona la dimensione di destinazione direttamente dall&#39;elenco delle dimensioni disponibili.
   * **[!UICONTROL Usa dati collegati]**: questa opzione consente di iniziare da una dimensione di targeting (ad esempio le sottoscrizioni) e quindi di passare alla dimensione di targeting di cui si desidera eseguire il targeting (ad esempio i destinatari).

   ![](assets/target-mappings-properties.png)

1. Se la dimensione selezionata non è già utilizzata da una mappatura di destinazione esistente, è necessario creare gli schemi per memorizzare i registri. A tale scopo, sono disponibili opzioni aggiuntive nella sezione **[!UICONTROL Archiviazione]**. Espandi la sezione seguente per ulteriori dettagli.

   +++Opzioni di archiviazione per nuove dimensioni di targeting

   1. **[!UICONTROL Spazio dei nomi]**: identifica lo spazio dei nomi che verrà utilizzato per creare i registri.
   1. **[!UICONTROL Suffisso dello schema dell&#39;estensione]**: specificare un suffisso per il nuovo schema.

      Nell’esempio seguente, il nome del registro di trasmissione sarà &quot;cusbroadlogSupplier&quot;.

      ![](assets/target-mappings-new.png)

   1. **[!UICONTROL Registri di consegna]**: attiva le opzioni in questa sezione per arricchire i registri di invio con un campo del codice segmento o con un campo contenente l&#39;indirizzo IP di consegna. Ad esempio, puoi salvare un codice di segmento calcolato durante il flusso di lavoro nei registri di invio per perfezionare il target in un secondo momento. Questo ti consente di eseguire il targeting dei profili che hanno questo codice di segmento specifico.

   1. **[!UICONTROL Esclusioni]**: specifica come memorizzare i registri di esclusioni.

   1. **[!UICONTROL Registri di tracciamento]**: attiva **[!UICONTROL Genera uno schema per il tracciamento]** per generare uno schema di archiviazione per i registri di tracciamento

+++

1. Utilizza la sezione **[!UICONTROL Mapping]** per identificare gli attributi dallo schema della mappatura di destinazione da utilizzare per ogni campo degli indirizzi di consegna. Per ogni campo, seleziona l’attributo desiderato da mappare. Puoi anche creare un’espressione per identificare il campo. Ad esempio, è possibile applicare una funzione inferiore all&#39;attributo address.

   ![](assets/target-mappings-mapping.png)

1. Quando la mappatura di destinazione è pronta, fai clic sul pulsante **[!UICONTROL Crea]**. I sistemi creano automaticamente la mappatura di destinazione e tutti gli schemi correlati per i registri.

Una volta creata la mappatura di destinazione, nella schermata vengono visualizzate due sezioni aggiuntive:

* **[!UICONTROL Inserire nell&#39;elenco Bloccati di]**: questa sezione ti consente di identificare gli attributi dallo schema della mappatura di destinazione da utilizzare per i inserisce nell&#39;elenco Bloccati di.

  ![](assets/target-mappings-denylisting.png)

* **[!UICONTROL Archiviazione]**: questa sezione ti consente di identificare le tabelle da utilizzare per archiviare i registri.

  ![](assets/target-mappings-storage.png)

   * **[!UICONTROL Schema messaggio]**: identifica lo schema da utilizzare per memorizzare i registri di invio.
   * **[!UICONTROL Messaggi esclusi]**: questa sezione specifica come gestire l&#39;archiviazione dei registri di consegna ed esclusione.

      * **[!UICONTROL Memorizza esclusioni e messaggi nella stessa tabella]**
      * **[!UICONTROL Archivia solo i messaggi]**: non archiviare le esclusioni.
      * **[!UICONTROL Memorizzare esclusioni e messaggi in tabelle separate]**: selezionare lo schema da utilizzare per memorizzare i registri di esclusione nel campo **[!UICONTROL Schema di rifiuto]**.

   * **[!UICONTROL Registri di tracciamento]**: scegli dove memorizzare i registri di tracciamento e l&#39;origine del traffico predefinita.
   * **[!UICONTROL Campi aggiuntivi]**: questa sezione ti consente di specificare un elenco di campi aggiuntivi da archiviare nei registri di consegna. Questi campi possono memorizzare in modo permanente le informazioni sui singoli membri del target (ad es. `recipient/@firstName`) o memorizzare dati aggiuntivi calcolati durante il flusso di lavoro (esempio: `[targetData/@offeCode]`)

     A tale scopo, selezionare **[!UICONTROL Aggiungi campo]**. Identifica le informazioni da salvare nel campo **[!UICONTROL Source]** e l&#39;attributo da utilizzare nei registri di invio per salvare tali informazioni nel campo **[!UICONTROL Destination]**.

     ![](assets/target-mappings-additional.png){width="50%" zoomable="yes"}
