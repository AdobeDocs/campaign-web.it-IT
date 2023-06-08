---
title: Personalizzare i contenuti in Campaign
description: Scopri come personalizzare i contenuti nell’interfaccia web di Adobe Campaign
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
badge: label="Alpha" type="Positive"
source-git-commit: b8b1cb62c11b66eaade5937fa798d58a9c376127
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 36%

---


# Personalizzare i contenuti{#add-personalization}

La personalizzazione può essere aggiunta a qualsiasi consegna utilizzando l’editor di espressioni.

Un tag di personalizzazione utilizza sempre la seguente sintassi: `<%=table.field%>`.Ad esempio, per inserire il nome del destinatario, memorizzato nella tabella dei destinatari, il tag di personalizzazione utilizza la sintassi &lt;%= recipient.lastName %>.

Quando viene preparata una consegna, questi tag vengono automaticamente interpretati da Adobe Campaign e sostituiti dal valore del campo per un determinato destinatario. La sostituzione fisica può quindi essere visualizzata durante la simulazione del contenuto.

Per aggiungere tag di personalizzazione a una consegna, fai clic sull’icona Apri finestra di dialogo per personalizzazione accessibile dai campi di modifica di tipo testo, ad esempio l’oggetto o il corpo dell’SMS.

![](assets/perso-access.png)

Viene visualizzato l’editor espressioni. I campi di personalizzazione sono organizzati in tre menu, situati a sinistra dello schermo. Questi menu consentono di accedere a tutti i campi disponibili nel database di Adobe Campaign.

| Menu | Descrizione |
|-----|------------|
| ![](assets/do-not-localize/perso-recipients-menu.png) | Il **[!UICONTROL Destinatario]** Il menu elenca tutti i campi definiti nella tabella dei destinatari, ad esempio il nome, l&#39;età o l&#39;indirizzo del destinatario. |
| ![](assets/do-not-localize/perso-message-menu.png) | Il **[!UICONTROL Messaggio]** Il menu elenca tutti i campi relativi ai registri di consegna, ovvero tutti i messaggi inviati a destinatari o dispositivi su tutti i canali, ad esempio la data dell’ultimo evento con un determinato destinatario |
| ![](assets/do-not-localize/perso-delivery-menu.png) | Il **[!UICONTROL Consegna]** Il menu elenca tutti i campi relativi ai parametri necessari per eseguire le consegne, ad esempio il canale di consegna, l’etichetta e così via. |

>[!NOTE]
>
>Per impostazione predefinita, l’elenco mostra tutti i campi all’interno della tabella selezionata (Destinatari, / Messaggio / Consegna). Se si desidera includere campi da tabelle collegate alla tabella selezionata, abilitare **[!UICONTROL Visualizzare attributi avanzati]** sotto l’elenco.

Per aggiungere un campo di personalizzazione, posiziona il cursore nella posizione desiderata all’interno del contenuto e fai clic sul pulsante + per inserirlo.

![](assets/perso-insert-field.png)

## Personalizzare il contenuto delle e-mail {#personalize-emails}

Per personalizzare il contenuto dell’e-mail, apri il messaggio in E-mail Designer ed esegui le seguenti operazioni:

1. Fai clic all’interno di un blocco di testo.
1. Nella barra degli strumenti contestuale, seleziona **[!UICONTROL Aggiungi personalizzazione]**.

   ![](assets/perso-add-to-content.png)

1. Inserisci il nome del destinatario nell’editor di personalizzazione e conferma.

   ![](assets/perso-add-name.png)

   L’attributo di personalizzazione viene aggiunto al contenuto dell’e-mail.

   Puoi simulare il contenuto per controllarne il rendering. [Ulteriori informazioni](../preview-test/preview-content.md)

   ![](assets/perso-rendering.png)

1. Per aggiungere un blocco di contenuto all’e-mail, segui questi stessi passaggi e seleziona un blocco di contenuto dall’ultima icona:

   ![](assets/perso-insert-block.png)

1. Una volta inserito, il blocco di contenuto viene aggiunto al contenuto dell’e-mail e viene adattato automaticamente al profilo del destinatario quando viene generata la personalizzazione, nella fase di preparazione della consegna.

   ![](assets/perso-content-block-in-email.png)


## Personalizzare le offerte {#personalize-offers}

Puoi anche accedere all’editor di personalizzazione quando aggiungi contenuti testuali alle rappresentazioni delle offerte. Per ulteriori informazioni, consulta [questa sezione](../content/offers.md).

