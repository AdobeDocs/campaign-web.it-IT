---
title: Personalizzare i contenuti in Campaign
description: Scopri come personalizzare i contenuti nell’interfaccia web di Adobe Campaign
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
badge: label="Alpha" type="Positive"
source-git-commit: d12c3019fb47164864259ecc40225fcb04de0e6c
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 8%

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
