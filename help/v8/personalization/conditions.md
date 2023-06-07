---
title: Creare contenuto condizionale
description: Scopri come definire le condizioni per personalizzare i contenuti nell’interfaccia web di Adobe Campaign
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
badge: label="Alpha" type="Positive"
exl-id: b650a859-e27d-4a36-a725-a1f5bb31e014
source-git-commit: 218f433eb72a0ed928732c96ebee64294daee852
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 8%

---

# Creare contenuti condizionali{#add-conditions}

>[!CONTEXTUALHELP]
>id="acw_homepage_card3"
>title="Creare contenuto condizionale"
>abstract="Crea contenuti condizionali per definire la personalizzazione dinamica in base al profilo del destinatario, sostituendo automaticamente blocchi di testo e immagini quando vengono soddisfatte determinate condizioni. Questa funzione può elevare le tue campagne e offrire esperienze altamente mirate e personalizzate al tuo pubblico."

Il contenuto condizionale è una funzione potente che consente di creare una personalizzazione dinamica in base al profilo del destinatario, sostituendo automaticamente blocchi di testo e immagini quando vengono soddisfatte determinate condizioni. Questa funzione può elevare le tue campagne e offrire esperienze altamente mirate e personalizzate al tuo pubblico.

Configurando i campi di contenuto condizionale, puoi creare ad esempio una personalizzazione dinamica avanzata in base al profilo del destinatario. I blocchi di testo, i collegamenti, l’oggetto e/o le immagini vengono sostituiti nel contenuto del messaggio quando viene soddisfatta una particolare condizione. Ad esempio, puoi visualizzare &quot;Sig.&quot; o &quot;Sig.ra&quot; in base al valore del campo Genere nel database di Adobe Campaign, oppure includere un collegamento diverso in base alla lingua preferita del destinatario.

## Sintassi di personalizzazione{#perso-syntax}

## Utilizzare le condizioni nell’editor di personalizzazione{#condition-perso-editor}

Per definire un contenuto condizionale per una consegna:

1. Apri una consegna e modifica il contenuto.
1. Fai clic su **[!UICONTROL Apri finestra di dialogo per personalizzazione]** , ad esempio SMS, a destra del campo Messaggio.

   ![](assets/open-perso-editor-sms.png)

1. Nell’editor di personalizzazione, passa a **[!UICONTROL Funzioni di supporto]**.
1. Fai clic sull’icona &quot;+&quot; accanto al simbolo **Se** funzione. La seguente riga è aggiunta alla schermata centrale:
   `<% if (<FIELD>==<VALUE>) { %>Insert content here<% } %>`
1. Sostituisci `<FIELD>` da un campo di personalizzazione. Ad esempio, l’azienda del destinatario: `recipient.company`.
1. Sostituisci `<VALUE>` da un valore da soddisfare. Ad esempio, `ADOBE`.

## Esempio: riga dell’oggetto SMS condizionale{#condition-subject-line}

Per creare un oggetto condizionale per un messaggio SMS, effettua le seguenti operazioni:

1. Apri una consegna e modifica il contenuto.
1. Fai clic sull’icona Apri finestra di dialogo per personalizzazione, a destra dell’oggetto.
1. Nell’editor di personalizzazione, passa a


```sql
<% if 
(recipient.email == 'recipient@domain.com' ) 
{ % >
<table>
    <tr>
        <td>variant A</td>
    </tr>
</table>
< % } 
else 
{ % >
<table>
    <tr>
        <td>variant B< td>
    </tr>
</table>
< % } 
%>
```
