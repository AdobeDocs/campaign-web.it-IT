---
audience: end-user
title: Gestire i modelli di campagna con Adobe Campaign Web
description: Scopri come gestire i modelli di campagna con Adobe Campaign Web
badge: label="Beta"
source-git-commit: d9273f383e2301ea761ac67eeb47f6d9fd769d44
workflow-type: tm+mt
source-wordcount: '971'
ht-degree: 3%

---


# Gestire i modelli di campagna{#manage-campaign-templates}

Tutte le campagne di marketing si basano su un modello, che memorizza le caratteristiche e le funzionalità principali. Campaign viene fornito con un set di modelli incorporati per aiutarti a iniziare. Puoi creare e configurare i modelli della campagna e quindi creare campagne a partire da questi modelli.

## Creare un modello di campagna

Per creare un modello di campagna, effettua le seguenti operazioni:

Apri Campaign Explorer e passa a Risorse > Modelli > Modelli campagna.
Fai clic su Nuovo nella barra degli strumenti sopra l’elenco dei modelli.


Puoi anche duplicare il modello incorporato per riutilizzarlo e adattarne la configurazione. A questo scopo, fai clic con il pulsante destro del mouse sul modello e seleziona Duplica.

Immetti l’etichetta del nuovo modello di campagna.

Fai clic su Salva e riapri il modello.

Nella scheda Modifica, definisci le proprietà del modello.

Seleziona il collegamento Parametri avanzati campagna... per aggiungere un flusso di lavoro al modello della campagna.



Modifica il valore di Targeting e dei flussi di lavoro in Sì e conferma. Scopri come aggiungere funzionalità in questa sezione.

Al modello viene aggiunta la scheda Targeting e flussi di lavoro. Fare clic su Aggiungi flusso di lavoro..., immettere un promemoria e fare clic su OK.

Crea il flusso di lavoro in base alle tue esigenze.



Fai clic su Salva. Il modello è ora pronto per essere utilizzato per creare una nuova campagna.

Le varie schede e schede secondarie del modello della campagna consentono di accedere alle relative impostazioni, come descritto in Configurazione generale.

Seleziona moduli Il collegamento Parametri avanzati della campagna... ti consente di abilitare e disabilitare i processi per le campagne basate su questo modello. Seleziona le funzionalità che desideri abilitare nelle campagne create in base a questo modello.



Se non è selezionata una funzionalità, gli elementi relativi al processo (menu, icone, opzioni, schede, schede secondarie, ecc.) non vengono visualizzati nell’interfaccia del modello o nelle campagne basate su questo modello. Le schede a sinistra dei dettagli della campagna e le schede disponibili coincidono con le funzionalità selezionate nel modello. Ad esempio, la funzionalità Spese e obiettivi non è abilitata, la scheda Budget corrispondente non viene visualizzata nelle campagne basate su questo modello.

Inoltre, al dashboard della campagna vengono aggiunte scelte rapide per le finestre di configurazione. Quando una funzionalità è abilitata, un collegamento diretto consente di accedervi dal dashboard della campagna.

Esempi di configurazione Ad esempio, con le seguenti impostazioni:



Il dashboard della campagna mostra:



Manca la scheda Targeting e flussi di lavoro.

Sono disponibili le seguenti funzionalità:



Manca la scheda Budget.

Anche le impostazioni avanzate della campagna riflettono questa configurazione.



La scheda Approvazioni non è disponibile.

Con questa configurazione:


Il dashboard della campagna mostra:



È disponibile la scheda Targeting e flussi di lavoro, ma manca il collegamento Aggiungi un documento.

Sono disponibili le seguenti funzionalità:



È disponibile la scheda Budget.

Anche le impostazioni avanzate della campagna riflettono questa configurazione.



La scheda Approvazioni è disponibile, ma le schede Popolazione controllo e Indirizzi seed non sono abilitate.

Tipologia dei moduli Gruppo di controllo

Quando questo modulo è selezionato, viene aggiunta una scheda aggiuntiva alle impostazioni avanzate del modello e delle campagne basate su questo modello. La configurazione può essere definita tramite il modello o singolarmente per ogni campagna. Per ulteriori informazioni sui gruppi di controllo, consulta questa sezione.



Indirizzi di seed

Quando questo modulo è selezionato, viene aggiunta una scheda aggiuntiva alle impostazioni avanzate del modello e delle campagne basate su questo modello. La configurazione può essere definita tramite il modello o singolarmente per ogni campagna.



Documenti

Quando questo modulo è selezionato, viene aggiunta una scheda aggiuntiva alla scheda Modifica del modello e alle campagne basate su questo modello. I documenti allegati possono essere aggiunti dal modello o singolarmente per ciascuna campagna. Per ulteriori informazioni sui documenti, consulta questa sezione.



Profilo di consegna

Quando questo modulo è selezionato, alla scheda Documenti viene aggiunta una scheda secondaria Strutture di consegna per definire le strutture di consegna per la campagna. Ulteriori informazioni sui profili di consegna sono disponibili in questa sezione.



Targeting e flussi di lavoro

Quando selezioni il modulo Targeting e flussi di lavoro, viene aggiunta una scheda che consente di creare uno o più flussi di lavoro per le campagne basate su questo modello. Puoi anche configurare singolarmente i flussi di lavoro per ogni campagna in base a questo modello.Ulteriori informazioni sui flussi di lavoro delle campagne in questa sezione.



Quando questo modulo è abilitato, alle impostazioni avanzate della campagna viene aggiunta una scheda Processi per definire la sequenza di esecuzione del processo.

Approvazioni

Se abiliti le approvazioni, puoi selezionare i processi da approvare e gli operatori responsabili delle approvazioni. Per ulteriori informazioni sulle approvazioni, consulta questa sezione.



Puoi scegliere se abilitare o meno l’approvazione del processo tramite la scheda Approvazioni della sezione impostazioni avanzate dei modelli.

Spese e obiettivi

Quando questo modulo è selezionato, viene aggiunta una scheda Budget ai dettagli del modello e delle campagne basate su questo modello, in modo da poter selezionare il budget associato.



Proprietà modello


Quando crei un modello di campagna, devi immettere le seguenti informazioni:

Inserisci l’etichetta del modello: l’etichetta è obbligatoria ed è l’etichetta predefinita per tutte le campagne basate su questo modello.
Seleziona la natura della campagna dall’elenco a discesa. I valori disponibili in questo elenco sono quelli salvati nell&#39;enumerazione natureOp.
Per scoprire come accedere e configurare le enumerazioni, consulta questa pagina.

Seleziona il tipo di campagna: univoca, ricorrente o periodica. Per impostazione predefinita, i modelli di campagna si applicano a campagne univoche. Le campagne ricorrenti e periodiche sono descritte in questa sezione.

Specifica la durata della campagna, ovvero il numero di giorni durante i quali la campagna avrà luogo. Quando crei una campagna basata su questo modello, le date di inizio e di fine della campagna verranno compilate automaticamente.

Se la campagna è ricorrente, devi specificare le date di inizio e di fine della campagna direttamente nel modello.

Specifica il programma correlato del modello: le campagne basate su questo modello sono collegate al programma selezionato.

