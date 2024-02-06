---
audience: end-user
title: Invio graduale
description: Ulteriori informazioni sulle impostazioni di consegna in Campaign Web
badge: label="Disponibilità limitata"
source-git-commit: 6676aa00e3ed7ea54f1ecd9b3e87d317e5208712
workflow-type: tm+mt
source-wordcount: '784'
ht-degree: 5%

---


# Invia in ondate {#send-using-waves}

>[!CONTEXTUALHELP]
>id="acw_deliveries_waves_definition"
>title="Dividere le consegne in più batch"
>abstract="Invece di inviare grandi volumi di messaggi contemporaneamente, definisci le ondate per suddividere le consegne in più batch. Puoi configurare più scaglioni della stessa dimensione o impostare un calendario per le diverse scaglioni da inviare."

>[!CONTEXTUALHELP]
>id="acw_deliveries_waves_size"
>title="Definire la dimensione di ogni scaglione"
>abstract="Immettete una dimensione per tutte le ondate che state aggiungendo. Immetti un valore numerico (numero di messaggi per ogni ondata) o una percentuale (0-100%)."

Per bilanciare il carico, puoi dividere le consegne in più batch. Configura il numero di batch e la loro proporzione rispetto all’intera consegna, nonché l’intervallo tra due ondate.

>[!NOTE]
>
>Puoi definire solo la dimensione e il ritardo tra due scaglioni consecutivi. Non è possibile regolare i criteri di selezione dei destinatari per ogni ondata.

Per inviare le consegne scaglionate, segui la procedura riportata di seguito.

1. Apri [impostazioni di consegna](delivery-settings.md#retries).

1. Accedi a **[!UICONTROL Consegna]** sezione.

1. Seleziona la **[!UICONTROL Invia in più ondate]** opzione.

1. Per configurare le ondate, puoi effettuare le seguenti operazioni:

   * [Pianifica più scaglioni della stessa dimensione.](#waves-same-size)
   * [Pianifica scaglioni in base a un calendario](#waves-calendar)

1. Prepara e invia la consegna come di consueto. [Ulteriori informazioni](../msg/gs-deliveries.md)

   >[!CAUTION]
   >
   >Assicurati che gli ultimi scaglioni non superino la scadenza di consegna, definita nella sezione **[!UICONTROL Validità]** scheda. In caso contrario, alcuni messaggi potrebbero non essere inviati. [Ulteriori informazioni](delivery-settings.md#validity)
   >
   >È inoltre necessario concedere tempo sufficiente per i nuovi tentativi durante la configurazione degli ultimi scaglioni. [Ulteriori informazioni](delivery-settings.md#retries)

1. Per monitorare gli invii, vai al [registri di consegna](../monitor/delivery-logs.md).

   Puoi visualizzare le consegne già inviate negli scaglioni elaborati (**[!UICONTROL Inviato]** stato) e le consegne da inviare negli scaglioni rimanenti (**[!UICONTROL In sospeso]** stato).

Una regola di controllo specifica per la tipologia, **[!UICONTROL Controllo programmazione ondata]**, assicura che l’ultimo scaglione sia pianificato prima del limite di validità della consegna. Le tipologie di campagne e le relative regole sono configurate in **[!UICONTROL Tipologia]** delle impostazioni di consegna. Ulteriori informazioni sulle regole di controllo in [Documentazione di Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/control-rules.html).

## Pianifica più scaglioni della stessa dimensione. {#waves-same-size}

Se selezionate questa opzione, tutte le onde hanno la stessa dimensione (tranne l&#39;ultima) e il ritardo tra ogni onda è sempre lo stesso.

![](assets/waves-same-size.png)

* Specifica la dimensione di tutte le ondate in cui si sta suddividendo la consegna. È possibile immettere una percentuale o un valore numerico. Solo l&#39;ultima ondata può variare in dimensioni in quanto deve includere il numero rimanente di messaggi.

  Ad esempio, se si immette **[!UICONTROL 30%]** nel campo corrispondente, le prime tre ondate rappresentano il 30% di tutti i messaggi inclusi nella consegna, mentre la quarta rappresenta il restante 10%.

* In **[!UICONTROL Interval]** , specificare il ritardo tra l&#39;inizio di due scaglioni consecutivi. Ad esempio, se si immette **[!UICONTROL 2 giorni]**, la prima ondata inizia immediatamente, la seconda inizierà tra due giorni, la terza ondata tra quattro giorni, e così via.

Un caso d’uso comune per l’utilizzo di più scaglioni della stessa dimensione riguarda un call center. Quando gestisci una campagna fedeltà telefonica, la tua organizzazione ha una capacità limitata di elaborare il numero di chiamate per contattare gli abbonati.

Utilizzando le ondate, è possibile limitare il numero di messaggi a 20 al giorno, che rappresenta la capacità di elaborazione giornaliera di un call center.

A questo scopo, seleziona la **[!UICONTROL Pianificazione di più scaglioni della stessa dimensione]** opzione. Invio **[!UICONTROL 20]** come dimensione delle onde e **[!UICONTROL 1 giorno]** nel **[!UICONTROL Interval]** campo.

![](assets/waves-call-center.png)

## Pianifica scaglioni in base a un calendario {#waves-calendar}

Se selezioni questa opzione, devi definire il giorno/ora di inizio per ogni scaglione che stai inviando, nonché la dimensione di ogni scaglione.

* In **[!UICONTROL Inizio]** , specificare il ritardo tra l&#39;inizio di due ondate consecutive.

* In **[!UICONTROL Dimensione]** , immettere un numero fisso o una percentuale.

Aggiungi tutte le ondate necessarie.

Nell’esempio seguente, la prima ondata rappresenta il 25% del numero totale di messaggi inclusi nella consegna e inizia immediatamente. Le due fasi successive completano la consegna e sono impostate per iniziare a intervalli di sei ore.

![](assets/waves-calendar.png)

Un caso d’uso comune per l’utilizzo di più scaglioni secondo un calendario è durante il processo di incremento.

Quando le e-mail vengono inviate utilizzando una nuova piattaforma, i provider di servizi Internet (ISP) sospettano che gli indirizzi IP non siano riconosciuti. Se grandi quantità di e-mail vengono inviate improvvisamente, gli ISP spesso le contrassegnano come spam.

Per evitare di essere contrassegnati come spam, puoi aumentare progressivamente il volume inviato scaglionando. Ciò dovrebbe garantire un regolare sviluppo della fase di avvio e consentirti di ridurre il tasso complessivo di indirizzi non validi.

A tale scopo, utilizza **[!UICONTROL Pianifica ondate in base a un calendario]** opzione. Ad esempio, imposta la prima ondata su 10%, la seconda su 15%, la terza su 20% e così via.

![](assets/waves-ramp-up.png)



