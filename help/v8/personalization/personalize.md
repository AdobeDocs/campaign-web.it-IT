---
title: Personalizzare i contenuti in Campaign
description: Scopri come personalizzare i contenuti nell’interfaccia web di Adobe Campaign
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
badge: label="Beta"
source-git-commit: 9fb4a5057ec05877ffbadc85d1198ab24faf8972
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 100%

---


# Personalizzare i contenuti {#add-personalization}

Puoi personalizzare qualsiasi consegna utilizzando l’editor di espressioni, accessibile nei campi tramite l’icona **[!UICONTROL Apri finestra di personalizzazione]**, come l’oggetto, i collegamenti e-mail e i componenti di contenuto testo/pulsante. [Scopri come accedere all’editor di espressioni](gs-personalization.md/#access)

## Sintassi di personalizzazione {#syntax}

I tag di personalizzazione seguono una sintassi specifica: `<%= table.field %>`. Ad esempio, per inserire il cognome del destinatario dalla tabella dei destinatari, utilizza la sintassi `<%= recipient.lastName %>`.

Durante il processo di preparazione della consegna, Adobe Campaign interpreta automaticamente questi tag e li sostituisce con i valori dei campi corrispondenti per ogni destinatario. Puoi visualizzare la sostituzione effettiva simulando il contenuto.

Durante il caricamento dei contatti da un file esterno per una consegna e-mail autonoma, tutti i campi nel file di input sono disponibili per la personalizzazione. La sintassi è la seguente: `<%= dataSource.field %>`.

## Aggiungere tag di personalizzazione {#add}

Per aggiungere tag di personalizzazione a una consegna, segui i passaggi seguenti:

1. Apri l’editor di espressioni utilizzando l’icona **[!UICONTROL Apri finestra di personalizzazione]** che è accessibile dai campi di modifica di tipo testuale, tra cui l’oggetto o il corpo dell’SMS. [Scopri come accedere all’editor di espressioni](gs-personalization.md/#access)

   ![](assets/perso-access.png){width="800" align="center"}

1. Si apre l’editor di espressioni. I campi di personalizzazione disponibili nel database di Adobe Campaign sono organizzati in diversi menu sul lato sinistro dello schermo:

   ![](assets/perso-insert-field.png){width="800" align="center"}

   | Menu | Descrizione |
   |-----|------------|
   | ![](assets/do-not-localize/perso-subscribers-menu.png) | Il menu **[!UICONTROL Applicazione per abbonati]** elenca i campi relativi agli abbonati a un’applicazione, ad esempio il terminale utilizzato o il sistema operativo. *Questo menu è disponibile solo per le notifiche push* |
   | ![](assets/do-not-localize/perso-recipients-menu.png) | Il menu **[!UICONTROL Destinatario]** elenca i campi definiti nella tabella dei destinatari, ad esempio i nomi, le età o gli indirizzi dei destinatari. Durante il [caricamento dei contatti da un file esterno](../audience/file-audience.md) per una consegna e-mail autonoma, questo menu elenca tutti i campi disponibili nel file di input. |
   | ![](assets/do-not-localize/perso-message-menu.png) | Il menu **[!UICONTROL Messaggio]** elenca i campi relativi ai registri di consegna, inclusi tutti i messaggi inviati a destinatari o dispositivi su tutti i canali, ad esempio la data dell’ultimo evento con un determinato destinatario |
   | ![](assets/do-not-localize/perso-delivery-menu.png) | Il menu **[!UICONTROL Consegna]** elenca i campi relativi ai parametri necessari per eseguire le consegne, ad esempio il canale o l’etichetta di consegna. |

   >[!NOTE]
   >
   >Per impostazione predefinita, in ogni menu sono elencati tutti i campi della tabella selezionata (Destinatari/Messaggio/Consegna). Se desideri includere campi da tabelle collegate alla tabella selezionata, abilita l’opzione **[!UICONTROL Visualizza attributi avanzati]** che si trova sotto l’elenco.

1. Per aggiungere un campo di personalizzazione, posiziona il cursore nella posizione desiderata all’interno del contenuto e fai clic sul pulsante `+` per inserirlo.

1. Una volta che il contenuto è pronto, puoi salvarlo e testare il rendering della personalizzazione simulando il contenuto. L’esempio seguente mostra la personalizzazione di un messaggio SMS con i nomi dei destinatari.

   ![](assets/perso-preview1.png){width="800" align="center"}

   ![](assets/perso-preview2.png){width="800" align="center"}
