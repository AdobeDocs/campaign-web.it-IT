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

# Utilizza un **[!UICONTROL gruppo di trap]** {#trap-group}

Un **[!UICONTROL gruppo di trap]** viene utilizzato per eseguire il targeting di destinatari che non corrispondono ai criteri di destinazione definiti. In questo modo, i destinatari che non rientrano nell’ambito di consegna possono ricevere la consegna, come farebbe qualsiasi altro destinatario.
Un **[!UICONTROL gruppo trap]** è un gruppo di **[!UICONTROL indirizzi seed]**.

## Perché utilizzare **[!UICONTROL gruppo trap]**

È possibile utilizzare **[!UICONTROL gruppo trap]**:

1. **Come prova**: ogni membro del **[!UICONTROL gruppo di trap]** riceverà la consegna come se facesse parte del pubblico.


1. **Per proteggere la tua mailing list** : ricevendo ciò che il pubblico riceverà, ogni **[!UICONTROL indirizzo seed]** del **[!UICONTROL gruppo di trap]** verrà notato se la mailing list viene utilizzata da una terza parte.

## Informazioni su **[!UICONTROL Trap group]**

Gli indirizzi di seed vengono automaticamente esclusi dai report sulle seguenti statistiche di consegna: **Clic**, **Aperture**, **Annullamenti abbonamenti**. I rapporti riguardano solo il pubblico reale.

Per una consegna e-mail, è necessario solo l&#39;indirizzo e-mail per il **[!UICONTROL gruppo di trap]**; la personalizzazione degli altri campi verrà compilata in modo casuale da Campaign.

## Come impostare un **[!UICONTROL gruppo di trap]** nella consegna

Per impostare un **[!UICONTROL gruppo di trap]**, vai alle impostazioni **[!UICONTROL Pubblico]** della consegna. Sono disponibili 2 opzioni:
- [Selezionare i profili di test](#select-test-profile)
- [Creare una condizione](#create-condition)

![](assets/trap-group.png){zoomable="yes"}

### Selezionare i profili di test {#select-test-profiles}

Quando scegli &quot;Seleziona profili di test&quot;, avrai la finestra seguente in cui sei invitato a **[!UICONTROL Aggiungi profili di test]**:

![](assets/trap-no-test-profile.png){zoomable="yes"}

Quando fai clic sul pulsante, potrai accedere agli indirizzi seed a cui aggiungere il **[!UICONTROL gruppo trap]**. Seleziona quelli che desideri utilizzare.
Puoi creare nuovi indirizzi di seed. [Ulteriori informazioni](#create-seed)

![](assets/trap-select-test-profiles.png){zoomable="yes"}

Quando confermi gli indirizzi trap, verifica di avere il numero corretto in **[!UICONTROL Gruppo trap]**.

![](assets/trap-check.png){zoomable="yes"}

### Creare una condizione {#create-condition}

Con l&#39;opzione **[!UICONTROL Crea condizione]**, verrà visualizzata una nuova finestra in cui è possibile personalizzare una query per definire gli indirizzi di seed che si desidera utilizzare:

![](assets/trap-create-condition.png){zoomable="yes"}

La query verrà visualizzata in **[!UICONTROL Gruppo di trap]**.

![](assets/trap-custom.png){zoomable="yes"}

## Come creare un nuovo **[!UICONTROL indirizzo seed]** {#create-seed}

Puoi creare un nuovo **[!UICONTROL indirizzo seed]** in **[!UICONTROL Explorer]** > **[!UICONTROL Risorse]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Membri seed]**

![](assets/trap-create.png){zoomable="yes"}

Puoi completare tutti i dettagli sul membro seed come se si trattasse di un profilo di pubblico:

![](assets/trap-create-contact.png){zoomable="yes"}