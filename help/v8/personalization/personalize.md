---
title: Personalizzare i contenuti in Campaign
description: Scopri come personalizzare i contenuti in Adobe Campaign Web
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
source-git-commit: f57e0f2de12780ff9f90c2c5f1933b0e9bffe493
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 66%

---


# Personalizzare i contenuti {#add-personalization}

Il Personalization di contenuti di consegna è una funzione chiave che consente di adattare i messaggi ai singoli destinatari, rendendo la comunicazione più rilevante e coinvolgente.

In Adobe Campaign, utilizzando [dati profilo](#data-personalization), come il nome del profilo, la posizione o le interazioni passate e [variabili specifiche della consegna](#variables-personalization), puoi personalizzare dinamicamente elementi come testo, immagini e offerte nella comunicazione.

La personalizzazione della consegna non solo migliora l’esperienza utente, ma migliora anche i tassi di coinvolgimento, portando a una conversione più elevata e alla soddisfazione dei clienti.

## Utilizzo dei dati del profilo per la personalizzazione {#data-personalization}

Puoi personalizzare qualsiasi consegna con i dati del profilo utilizzando l&#39;editor espressioni, accessibile nei campi con l&#39;icona **[!UICONTROL Apri finestra di dialogo per personalizzazione]**, ad esempio l&#39;oggetto, i collegamenti e-mail e i componenti di contenuto testo/pulsante. [Scopri come accedere all’editor di espressioni](gs-personalization.md/#access)

### Sintassi di personalizzazione {#syntax}

I tag di personalizzazione seguono una sintassi specifica: `<%= table.field %>`. Ad esempio, per inserire il cognome del destinatario dalla tabella dei destinatari, utilizza la sintassi `<%= recipient.lastName %>`.

Durante il processo di preparazione della consegna, Adobe Campaign interpreta automaticamente questi tag e li sostituisce con i valori dei campi corrispondenti per ogni destinatario. Puoi visualizzare la sostituzione effettiva simulando il contenuto.

Durante il caricamento dei contatti da un file esterno per una consegna e-mail autonoma, tutti i campi nel file di input sono disponibili per la personalizzazione. La sintassi è la seguente: `<%= dataSource.field %>`.

### Aggiungere tag di personalizzazione {#add}

Per aggiungere tag di personalizzazione a una consegna, segui i passaggi seguenti:

1. Apri l’editor di espressioni utilizzando l’icona **[!UICONTROL Apri finestra di personalizzazione]** che è accessibile dai campi di modifica di tipo testuale, tra cui l’oggetto o il corpo dell’SMS. [Scopri come accedere all’editor di espressioni](gs-personalization.md/#access)

   ![](assets/perso-access.png){zoomable="yes"}{width="800" align="center"}

1. Si apre l’editor di espressioni. I campi di personalizzazione disponibili nel database di Adobe Campaign sono organizzati in diversi menu sul lato sinistro dello schermo:

   ![](assets/perso-insert-field.png){zoomable="yes"}{width="800" align="center"}

   | Menu | Descrizione |
   |-----|------------|
   | ![](assets/do-not-localize/perso-subscribers-menu.png){zoomable="yes"} | Il menu **[!UICONTROL Applicazione per abbonati]** elenca i campi relativi agli abbonati a un’applicazione, ad esempio il terminale utilizzato o il sistema operativo. *Questo menu è disponibile solo per le notifiche push* |
   | ![](assets/do-not-localize/perso-recipients-menu.png){zoomable="yes"} | Il menu **[!UICONTROL Destinatario]** elenca i campi definiti nella tabella dei destinatari, ad esempio i nomi, le età o gli indirizzi dei destinatari. Durante il [caricamento dei contatti da un file esterno](../audience/file-audience.md) per una consegna e-mail autonoma, questo menu elenca tutti i campi disponibili nel file di input. |
   | ![](assets/do-not-localize/perso-message-menu.png){zoomable="yes"} | Il menu **[!UICONTROL Messaggio]** elenca i campi relativi ai registri di consegna, inclusi tutti i messaggi inviati a destinatari o dispositivi su tutti i canali, ad esempio la data dell’ultimo evento con un determinato destinatario |
   | ![](assets/do-not-localize/perso-delivery-menu.png){zoomable="yes"} | Il menu **[!UICONTROL Consegna]** elenca i campi relativi ai parametri necessari per eseguire le consegne, ad esempio il canale o l’etichetta di consegna. |

   >[!NOTE]
   >
   >Per impostazione predefinita, in ogni menu sono elencati tutti i campi della tabella selezionata (Destinatari/Messaggio/Consegna). Se desideri includere campi da tabelle collegate alla tabella selezionata, abilita l’opzione **[!UICONTROL Visualizza attributi avanzati]** che si trova sotto l’elenco.

1. Per aggiungere un campo di personalizzazione, posiziona il cursore nella posizione desiderata all’interno del contenuto e fai clic sul pulsante `+` per inserirlo.

1. Una volta che il contenuto è pronto, puoi salvarlo e testare il rendering della personalizzazione simulando il contenuto. L’esempio seguente mostra la personalizzazione di un messaggio SMS con i nomi dei destinatari.

   ![](assets/perso-preview1.png){zoomable="yes"}{width="800" align="center"}

   ![](assets/perso-preview2.png){zoomable="yes"}{width="800" align="center"}

## Utilizzo delle variabili per la personalizzazione {#variables-personalization}

Puoi inoltre utilizzare le variabili per personalizzare la consegna.
Ulteriori informazioni sull&#39;[aggiunta di variabili a una consegna](../advanced-settings/delivery-settings.md#variables-delivery).

Ad esempio, la variabile `deliveryType` è definita come segue.

![](assets/variables-deliveryType.png){zoomable="yes"}

Questa variabile può essere utilizzata nel contenuto della consegna, utilizzando l&#39;icona **[!UICONTROL Aggiungi Personalization]** e l&#39;espressione `<%= variables.deliveryType %>` per il nostro esempio.

![](assets/variables-perso.png){zoomable="yes"}

Puoi controllare l&#39;utilizzo della variabile con il pulsante **[!UICONTROL Simula contenuto]**.

![](assets/variables-simulate.png){zoomable="yes"}
