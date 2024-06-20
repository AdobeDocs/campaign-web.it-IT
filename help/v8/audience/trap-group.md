---
audience: end-user
title: Utilizzare un gruppo di trappole
hide: true
hidefromtoc: true
description: Scopri come utilizzare un gruppo di trappole per la consegna nell’interfaccia utente web di Campaign
source-git-commit: 15d8ea478a234136dc654683798957d6c7026327
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 3%

---

# Utilizza un **[!UICONTROL gruppo trap]** {#trap-group}

A **[!UICONTROL gruppo trap]** viene utilizzato per eseguire il targeting di destinatari che non corrispondono ai criteri di target definiti. In questo modo, i destinatari che non rientrano nell’ambito di consegna possono ricevere la consegna, come farebbe qualsiasi altro destinatario.
A **[!UICONTROL gruppo trap]** è un gruppo di **[!UICONTROL indirizzi seed]**.

## Perché utilizzare **[!UICONTROL gruppo trap]**

È possibile utilizzare **[!UICONTROL gruppo trap]** :

1. **Come prova** : ogni membro del **[!UICONTROL Gruppo di trappole]** riceverà la consegna come se facesse parte del pubblico.


1. **Per proteggere la mailing list** : ricevendo ciò che il pubblico riceverà, ogni **[!UICONTROL indirizzo seed]** del **[!UICONTROL Gruppo di trappole]** sarà notato se la mailing list viene utilizzata da una terza parte.

## Informazioni su **[!UICONTROL Gruppo di trappole]**

Gli indirizzi di seed vengono automaticamente esclusi dai rapporti sulle seguenti statistiche di consegna: **Clic**, **Aperture**, **Annullamenti iscrizione**. I rapporti riguardano solo il pubblico reale.

Per una consegna e-mail, è necessario solo l’indirizzo e-mail per il **[!UICONTROL Gruppo di trappole]**, la personalizzazione di altri campi verrà compilata in modo casuale da Campaign.

## Come impostare un **[!UICONTROL Gruppo di trappole]** nella consegna

Per impostare un **[!UICONTROL Gruppo di trappole]**, passare alla **[!UICONTROL Pubblico]** impostazioni della consegna. Sono disponibili 2 opzioni:
- [Selezionare i profili di test](#select-test-profile)
- [Creare una condizione](#create-condition)

![](assets/trap-group.png){zoomable="yes"}

### Selezionare i profili di test {#select-test-profiles}

Quando scegli &quot;Seleziona profili di test&quot;, avrai la finestra seguente in cui sei invitato **[!UICONTROL Aggiungi profili di test]** :

![](assets/trap-no-test-profile.png){zoomable="yes"}

Quando fai clic sul pulsante, potrai accedere agli indirizzi seed a cui aggiungere i tuoi **[!UICONTROL gruppo trap]**. Seleziona quelli che desideri utilizzare.
Puoi creare nuovi indirizzi di seed. [Ulteriori informazioni](#create-seed)

![](assets/trap-select-test-profiles.png){zoomable="yes"}

Quando confermate gli indirizzi trap, verificate di avere il numero corretto in **[!UICONTROL Gruppo di trappole]**.

![](assets/trap-check.png){zoomable="yes"}

### Creare una condizione {#create-condition}

Con il **[!UICONTROL Crea condizione]** , si apre una nuova finestra in cui è possibile personalizzare una query per definire gli indirizzi di seed che si desidera utilizzare:

![](assets/trap-create-condition.png){zoomable="yes"}

La query verrà visualizzata in **[!UICONTROL Gruppo di trappole]**.

![](assets/trap-custom.png){zoomable="yes"}

## Come creare un nuovo **[!UICONTROL indirizzo seed]** {#create-seed}

È possibile creare un nuovo **[!UICONTROL indirizzo seed]** in **[!UICONTROL Esplora]** > **[!UICONTROL Risorse]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Membri seed]**

![](assets/trap-create.png){zoomable="yes"}

Puoi completare tutti i dettagli sul membro seed come se si trattasse di un profilo di pubblico:

![](assets/trap-create-contact.png){zoomable="yes"}