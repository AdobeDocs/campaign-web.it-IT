---
audience: end-user
title: Creare esperimenti di contenuto
description: Scopri come creare esperimenti di contenuti in Adobe Campaign Web
source-git-commit: f238fde4a79d3303f2b5c9a2d26b11ffad8ac54e
workflow-type: tm+mt
source-wordcount: '1121'
ht-degree: 2%

---

# Creare esperimenti di contenuto {#content-experiment}

## Informazioni sugli esperimenti di contenuto {#about-content-experiment}

Gli esperimenti sui contenuti in Adobe Campaign Web consentono di definire più varianti di consegna per test A/B al fine di misurare le prestazioni migliori per il pubblico di destinazione. Puoi variare il contenuto, l’oggetto o il mittente della consegna per testare versioni diverse e determinare quale variante produce i risultati migliori.

Puoi eseguire test A/B su vari elementi e-mail, ad esempio:

* **Oggetto**: verifica diverse righe dell&#39;oggetto dell&#39;e-mail per vedere quale genera il tasso di apertura più alto
* **Nome mittente**: prova con diverse combinazioni mittente
* **Contenuto del corpo dell&#39;e-mail**: crea più versioni di contenuto per identificare quale determina il tasso di click-through migliore

>[!NOTE]
>
>* Gli esperimenti sui contenuti sono attualmente disponibili solo per il canale e-mail.
>* Il test A/B non è supportato per i messaggi transazionali.
>* Massimo 3 trattamenti (varianti) per esperimento.

## Creare un esperimento sui contenuti {#create-content-experiment}

Per aggiungere un esperimento sui contenuti alla consegna e-mail, effettua le seguenti operazioni:

1. Crea una consegna e-mail o apri una bozza di consegna esistente. [Scopri come creare un&#39;e-mail](create-email.md)

1. Dalla pagina delle proprietà di consegna e-mail, fai clic sul pulsante **[!UICONTROL Crea esperimento]** nella sezione **[!UICONTROL Contenuto]**.

   ![Schermata che mostra il pulsante Crea esperimento nelle proprietà e-mail](assets/ab-testing-1.png){zoomable="yes"}

## Configurare le impostazioni dell’esperimento {#configure-experiment}

Configura l’esperimento utilizzando le sezioni seguenti:

![Schermata che mostra le impostazioni dell&#39;esperimento](assets/ab-testing-2.png){zoomable="yes"}

### Impostazioni pubblico {#audience-settings}

Definisci la percentuale della popolazione target che riceverà le varianti dell’esperimento.

Immetti un valore per impostare la dimensione del pubblico. Rappresenta la proporzione di destinatari che riceveranno una delle varianti dell’esperimento durante la fase di test.

* **Minimo**: 1%
* **Massimo**: 100%
* **Predefinito**: 10%

Il pubblico rimanente (90% per impostazione predefinita) riceverà la variante vincente una volta concluso l’esperimento e determinato un vincitore.

Ad esempio, con un pubblico di destinazione di 10.000 destinatari e una dimensione di pubblico del 10%, verranno selezionati in modo casuale 1.000 destinatari per partecipare all’esperimento. I restanti 9.000 destinatari riceveranno la variante vincente al termine dell’esperimento.

### Strategia vincente {#winning-strategy}

Seleziona la metrica da utilizzare per determinare la variante vincente:

* **[!UICONTROL Percentuale di apertura migliore]** (impostazione predefinita): vince la variante con la percentuale più elevata di aperture e-mail
* **[!UICONTROL Percentuale di click-through migliore]**: vince la variante con la percentuale di clic più elevata nell&#39;e-mail
* **[!UICONTROL Percentuale di annullamento abbonamento più debole]**: vince la variante con la percentuale più bassa di annullamenti abbonamenti

Il sistema tiene traccia automaticamente di queste metriche durante l’esperimento e calcola quale variante funziona meglio in base al criterio selezionato.

### Metodo di invio vincente {#sending-method}

Definisci per quanto tempo deve essere eseguito l’esperimento e seleziona il metodo di invio:

1. Immetti il valore della durata in ore. L’esperimento verrà eseguito per questo periodo prima di determinare la variante vincente.

   * **Minimo**: 3 ore
   * **Massimo**: 240 ore (10 giorni)
   * **Predefinito**: 24 ore

   >[!NOTE]
   >
   >Assicurati che la durata dell’esperimento sia sufficientemente lunga per raccogliere dati significativi. Una breve durata potrebbe non fornire una significatività statistica sufficiente, in particolare per metriche quali il tasso di click-through che potrebbe richiedere più tempo per accumularsi.

1. Scegli come inviare la variante vincente alla popolazione rimanente:

   * **[!UICONTROL Invio automatico]** attivato: al termine dell&#39;esperimento, il sistema invia automaticamente la variante vincente al pubblico rimanente.
   * **[!UICONTROL Invio automatico]** disattivato: fai clic manualmente sul pulsante **[!UICONTROL Invia]** per inviare la variante vincente dopo aver esaminato i risultati dell&#39;esperimento.

Se nessuna variante ottiene risultati significativamente migliori degli altri entro la fine dell&#39;esperimento, il sistema invia la prima variante alla popolazione rimanente. Consulta questa [sezione](#send-deliveries).

## Definire i trattamenti per i contenuti {#define-content}

Dopo aver salvato le impostazioni dell’esperimento, per impostazione predefinita viene creato un primo trattamento. Ora devi aggiungere gli altri trattamenti (fino a tre) e definirne il contenuto specifico.

1. Dalle proprietà di consegna, fai clic su **[!UICONTROL Modifica contenuto]**. I trattamenti sono visualizzati sul lato sinistro.

   ![Schermata che mostra il pannello esperimenti contenuti](assets/ab-testing-3.png){zoomable="yes"}

1. Fare clic sul pulsante **[!UICONTROL Aggiungi trattamento]** e definirne il nome. Ripetere questa operazione per tutti i trattamenti da aggiungere. È quindi possibile modificarne il nome, duplicarli e rimuoverli.

1. Fare clic su ogni trattamento e personalizzare i seguenti elementi:

   * **Nome mittente**: personalizza l&#39;indirizzo di posta elettronica
   * **Oggetto**: scrivere una riga dell&#39;oggetto univoca per ogni trattamento
   * **Corpo dell&#39;e-mail**: progetta diverse versioni di contenuto utilizzando E-mail Designer

   ![Schermata che mostra diversi trattamenti](assets/ab-testing-4.png){zoomable="yes"}

1. Visualizzare in anteprima ogni trattamento facendo clic sul trattamento e quindi su **[!UICONTROL Simula contenuto]**.

## Avvia l’esperimento e monitora i risultati {#validate-start}

Dopo aver definito tutti i trattamenti del contenuto, puoi convalidare e avviare l’esperimento.

1. Dalle proprietà di consegna, fai clic su **[!UICONTROL Rivedi e invia]**, quindi su **[!UICONTROL Prepara]**.

1. Quindi fai clic su **[!UICONTROL Avvia sperimentazione]** per iniziare il test A/B.

   ![Schermata che mostra il pulsante di avvio della sperimentazione](assets/ab-testing-5.png){zoomable="yes"}

1. Una volta eseguito l’esperimento, monitora le diverse metriche visualizzate nel dashboard di consegna.

Durante l&#39;esecuzione dell&#39;esperimento è possibile fare clic su **[!UICONTROL Interrompi invio]** per terminare l&#39;esperimento. Puoi anche decidere di inviare manualmente prima della fine dell&#39;esperimento facendo clic su **[!UICONTROL Seleziona e invia al vincitore]**.

>[!NOTE]
>
>I risultati vengono aggiornati quasi in tempo reale man mano che i destinatari interagiscono con l’e-mail. Tuttavia, i primi risultati potrebbero non avere rilevanza statistica; si consiglia di attendere il completamento della durata dell’esperimento prima di prendere decisioni finali.

## Inviare le consegne {#send-deliveries}

L&#39;invio può essere eseguito automaticamente o manualmente, in base a quanto scelto nelle impostazioni del **[!UICONTROL metodo di invio vincitore]**. Consulta questa [sezione](#sending-method).

### Invio automatico {#automatic-sending}

Per l’invio automatico, il sistema analizza i risultati in base alla strategia di vincita e determina il trattamento vincente. Il trattamento vincente viene inviato automaticamente al pubblico rimanente. Se non è emerso alcun vincitore chiaro, viene scelta la prima variante.

### Invio manuale {#manual-sending}

Se hai configurato l&#39;invio manuale, controlla i risultati al termine dell&#39;esperimento e fai clic su **[!UICONTROL Invia]** per inviare il trattamento vincente. Se non è emerso alcun vincitore chiaro, il primo trattamento viene selezionato per impostazione predefinita, ma puoi sceglierne uno diverso.

## Visualizza risultati finali {#final-results}

Al termine dell’esperimento e dopo che la consegna è stata completamente inviata, puoi accedere a rapporti completi:

1. Dal dashboard di consegna, fai clic su **[!UICONTROL Rapporti]**.

1. Passa alla scheda del rapporto **[!UICONTROL Esperimenti]** per visualizzare le metriche delle prestazioni chiave per ogni trattamento.

## Best practice {#best-practices}

Quando crei esperimenti di contenuto, prendi in considerazione i consigli seguenti:

* **Verifica un elemento alla volta**: per risultati più chiari, verifica le varianti di un singolo elemento (ad esempio, solo riga oggetto o solo contenuto) anziché più elementi contemporaneamente.

* **Scegli la durata appropriata**: attendi tempo sufficiente per la rilevanza statistica:
   * Per i test di velocità di apertura: di solito sono sufficienti 12-24 ore
   * Per i test della frequenza di click-through: possono essere necessarie 24-48 ore o più
   * Un pubblico più ampio può richiedere meno tempo, mentre un pubblico più piccolo potrebbe aver bisogno di più tempo

* **Ridimensiona il pubblico in modo appropriato**:
   * Assicurati che il pubblico dell’esperimento (la percentuale allocata al test) sia abbastanza ampio da produrre risultati significativi
   * Linea guida generale: almeno 1,000 pazienti per trattamento per risultati affidabili

* **Test regolari ma non eccessivi**: esegui esperimenti su campagne importanti, ma evita di testare ogni singolo invio per concentrare le risorse su decisioni di impatto.

* **Documenta i tuoi insegnamenti**: conserva i record dei risultati dell&#39;esperimento per informare le future strategie delle campagne.

## Argomenti correlati {#related-topics}

* [Creare il primo messaggio e-mail](create-email.md)
* [Configurare il contenuto dell’e-mail](edit-content.md)
* [Anteprima e invio di un’e-mail](../monitor/prepare-send.md)
* [Rapporti sulle consegne e-mail](../reporting/email-report.md)
