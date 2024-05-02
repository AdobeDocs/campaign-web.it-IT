---
audience: end-user
title: Utilizzare l’attività del flusso di lavoro Estrai file
description: Scopri come utilizzare l’attività del flusso di lavoro Extract file
source-git-commit: 575219c7bcef303e211f504d13227183933924cc
workflow-type: tm+mt
source-wordcount: '860'
ht-degree: 7%

---

# Estrai file {#extract-file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile"
>title="Estrai file"
>abstract="Il **Extract file** attività ti consente di esportare dati da Adobe Campaign sotto forma di un file esterno. I dati possono quindi essere esportati in una posizione server come SFTP, archiviazione Cloud o il server della campagna utilizzando un’attività Transfer file."

Il **Extract file** l&#39;attività è un **Gestione dei dati** attività. Utilizza questa attività per esportare dati da Adobe Campaign sotto forma di un file esterno. I dati possono quindi essere esportati in una posizione server come SFTP, archiviazione Cloud o il server della campagna utilizzando un’attività Transfer file.

Per configurare **Extract file** attività, aggiungi un **Extract file** nel flusso di lavoro, quindi segui i passaggi indicati di seguito.

## Configura il file da estrarre {#extract-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_file"
>title="File da estrarre"
>abstract="Seleziona il file da estrarre."

Il **[!UICONTROL File da estrarre]** consente di configurare le proprietà del file e i dati da includere.

![](../assets/extract-file-file.png)

1. In **[!UICONTROL Nome file]** , immettere il nome desiderato per il file da estrarre.

   Puoi personalizzare il nome del file utilizzando variabili evento, condizioni e funzioni data/ora. A questo scopo, fai clic su **[!UICONTROL Apri finestra di dialogo per personalizzazione]** per aprire l’editor di espressioni. [Scopri come utilizzare le variabili evento e l’editor di espressioni](../event-variables.md)

1. Specificare le colonne da presentare nel file estratto. Per farlo, segui questi passaggi:

   1. Fai clic su **[!UICONTROL Aggiungi colonna di output]**.
   1. Scegli l’attributo da visualizzare nella colonna, quindi conferma. Gli attributi disponibili dipendono dalla dimensione di targeting del flusso di lavoro.
   1. Una volta aggiunta la colonna, puoi modificarne la **[!UICONTROL Etichetta]** e modificare il **[!UICONTROL Attributo]**.
   1. Per applicare una trasformazione ai valori della colonna, selezionarla dall&#39;elenco a discesa. Ad esempio, è possibile convertire tutti i valori nella colonna selezionata in maiuscolo.

1. Ripeti questi passaggi per aggiungere tutte le colonne necessarie nel file di estrazione. Per modificare la posizione di una colonna, utilizzare le frecce su e giù.

1. Per rimuovere tutte le righe duplicate dal file estratto, attivare **[!UICONTROL Rimuovi righe duplicate(Elenco)]** opzione.

1. Per ordinare il file estratto in base a un attributo, attivare **[!UICONTROL Abilita ordinamento]** quindi scegliere l&#39;attributo in base al quale si desidera ordinare il file, insieme al metodo di ordinamento desiderato (crescente o decrescente). Puoi ordinare in base a qualsiasi attributo della dimensione di targeting corrente, indipendentemente dal fatto che sia stato aggiunto o meno alle colonne del file.

## Configurare il formato del file estratto {#file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_destinationformat"
>title="Formato di destinazione"
>abstract="Seleziona il formato."

Il **[!UICONTROL Destinazione]** sezione di formato consente di configurare la formattazione del file estratto.

1. Scegli la **[!UICONTROL Formato di output]** per il file estratto: **Testo**, **Testo con colonne fisse**, **CSV (Excel)** o **XML**.

1. Fai clic su **[!UICONTROL Formato di estrazione]** per accedere alle opzioni specifiche relative al formato selezionato. Per ulteriori informazioni, espandi la sezione seguente.

+++ Opzioni di formato di estrazione disponibili

   * **[!UICONTROL Usa prima riga come intestazione di colonna]** (Formato Testo/CSV (Excel)): attiva questa opzione per utilizzare la prima colonna come intestazione.
   * **[!UICONTROL Separatore colonne]** (formato testo): specifica il carattere da utilizzare come separatore di colonna nel file di output.
   * **[!UICONTROL Delimitatore stringa]** (Formato testo): specifica come delimitare le stringhe nel file di output.
   * **[!UICONTROL Fine riga]** (formato testo): specifica come delimitare la fine delle righe nel file di output.
   * **[!UICONTROL Codifica]**: scegli la codifica del file di output.
   * **[!UICONTROL Formato data e separatori]**: specifica come formattare le date nel file di output.
   * **[!UICONTROL Formato numero]**: specifica come formattare i numeri nel file di output.
   * **[!UICONTROL Esporta etichette anziché valori interni delle enumerazioni]**: attiva questa opzione se esporti valori di enumerazione e desideri recuperare le etichette delle colonne, che sono più facili da comprendere, anziché gli ID interni.

+++

   ![](../assets/extract-file-format.png)

## Aggiungi una fase di post-elaborazione {#script}

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_postprocessing"
>title="Post-elaborazione"
>abstract="Definisci un passaggio di post-elaborazione"

Il **[!UICONTROL Esporta script di modifica]** consente di applicare una fase di elaborazione da eseguire durante l’estrazione dei dati, ad esempio la compressione o la crittografia. A questo scopo, fai clic su **[!UICONTROL Modifica script]** pulsante.

Viene aperto l’editor espressioni, che consente di immettere il comando da applicare al file. Il riquadro a sinistra fornisce sintassi predefinite che è possibile utilizzare per creare lo script. [Scopri come utilizzare le variabili evento e l’editor di espressioni](../event-variables.md)

![](../assets/extract-file-script.png)

## Opzioni aggiuntive {#additiona-options}

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_outbound"
>title="Transizione in uscita"
>abstract="Attiva/disattiva l’opzione **Genera una transizione in uscita** per aggiungere una transizione in uscita dopo l’attività corrente."

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_error"
>title="Errori del processo"
>abstract="Attiva/disattiva l’opzione **Errori di processo** per aggiungere una transizione in uscita contenente errori."

Una volta configurata l’estrazione del file di output, sono disponibili opzioni aggiuntive relative alle transizioni e alla gestione degli errori:

* **[!UICONTROL Genera transizione in uscita]**: attiva questa opzione per aggiungere una transizione in uscita e configurarne l’etichetta.
* **[!UICONTROL Non generare un file se la transizione in entrata è vuota]**: attiva questa opzione per saltare l’estrazione del file se la transizione in entrata non contiene dati.
* **[!UICONTROL Errore di processo]**: attiva questa opzione per aggiungere una transizione in uscita se si verifica un errore durante l’estrazione del file.

## Esempio {#example}

Nell’esempio seguente viene utilizzato un **Creare un pubblico** attività seguita da **Extract file** per estrarre tutti i profili target in un file CSV.

![](../assets/extract-file-example.png)

* Il **[!UICONTROL Nome file]** è configurato per includere la data dell’estrazione.

  ![](../assets/extract-file-example-name.png)

* Vengono aggiunte colonne per visualizzare nel database il nome e il cognome dei profili, gli ID cliente e le date di creazione.

  ![](../assets/extract-file-example-columns.png)
