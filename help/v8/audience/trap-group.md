---
audience: end-user
title: Utilizzare un gruppo di trappole
hide: true
hidefromtoc: true
description: Scopri come utilizzare un gruppo di trappole per la consegna nell’interfaccia utente web di Campaign
source-git-commit: 2feea0c5a1b021786e58bf6a69a2018ec37ea4b1
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 2%

---

# Utilizza un **[!UICONTROL gruppo di trap]** {#trap-group}

Un **[!UICONTROL gruppo trap]** (noto anche come **[!UICONTROL elenco seed]**) viene utilizzato per includere indirizzi specifici nelle consegne per monitorare e verificare il processo di distribuzione eseguendo il targeting di profili che non corrispondono ai criteri di destinazione definiti. In questo modo, i destinatari che non rientrano nell’ambito di consegna possono ricevere la consegna, come farebbe qualsiasi altro destinatario.
Un **[!UICONTROL gruppo trap]** è un gruppo di **[!UICONTROL indirizzi seed]**, denominato **[!UICONTROL Profilo di test]** nell&#39;interfaccia utente Web di AC.

## Perché utilizzare **[!UICONTROL Trap group]**

È possibile utilizzare **[!UICONTROL gruppo trap]**:

1. **Come prova**: ogni membro del **[!UICONTROL gruppo di trap]** riceverà la consegna come se facesse parte del pubblico.


1. **Per proteggere la tua mailing list** : ricevendo ciò che il pubblico riceverà, ogni **[!UICONTROL profilo di test]** del **[!UICONTROL gruppo di trap]** verrà notato se la mailing list viene utilizzata da una terza parte.

>[!NOTE]
>
>Il gruppo di trap è diverso da [invio di bozze durante la creazione della consegna](../email/create-email.md#preview-test) e da [gruppo di controllo](control-group.md).


## Informazioni su **[!UICONTROL Trap group]**

I profili di test vengono automaticamente esclusi dai rapporti sulle seguenti statistiche di consegna: **Clic**, **Aperture**, **Annullamenti abbonamenti**. I rapporti riguardano solo il pubblico reale.

Per una consegna e-mail, è necessario solo l&#39;indirizzo e-mail per il **[!UICONTROL gruppo di trap]**; la personalizzazione degli altri campi verrà compilata in modo casuale da Campaign.

## Come impostare un **[!UICONTROL gruppo di trap]** nella consegna

Per impostare un **[!UICONTROL gruppo di trap]**, vai alle impostazioni **[!UICONTROL Pubblico]** della consegna. Sono disponibili 2 opzioni:
- [Selezionare i profili di test](#select-test-profile)
- [Creare una condizione](#create-condition)

![](assets/trap-group.png){zoomable="yes"}

### Selezionare i profili di test {#select-test-profiles}

Quando scegli &quot;Seleziona profili di test&quot;, avrai la finestra seguente in cui sei invitato a **[!UICONTROL Aggiungi profili di test]**:

![](assets/trap-no-test-profile.png){zoomable="yes"}

Quando fai clic sul pulsante, potrai accedere ai profili di test e aggiungere il **[!UICONTROL gruppo di trap]**. Seleziona quelli che desideri utilizzare.
Puoi creare nuovi profili di test. [Ulteriori informazioni](#create-seed)

![](assets/trap-select-test-profiles.png){zoomable="yes"}

Quando confermi i profili di test, verifica di disporre del numero corretto in **[!UICONTROL Gruppo di trap]**.

![](assets/trap-check.png){zoomable="yes"}

### Creare una condizione {#create-condition}

Con l&#39;opzione **[!UICONTROL Crea condizione]**, verrà visualizzata una nuova finestra in cui è possibile personalizzare una query per definire i profili di test che si desidera utilizzare:

![](assets/trap-create-condition.png){zoomable="yes"}

La query verrà visualizzata in **[!UICONTROL Gruppo di trap]**.

![](assets/trap-custom.png){zoomable="yes"}

## Come creare un nuovo **[!UICONTROL Profilo di test]** {#create-seed}

Puoi creare un nuovo **[!UICONTROL profilo di test]** in **[!UICONTROL Explorer]** > **[!UICONTROL Risorse]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Membri seed]**

![](assets/trap-create.png){zoomable="yes"}

Puoi completare tutti i dettagli sul tuo **[!UICONTROL profilo di test]** come se fosse un profilo di pubblico:

![](assets/trap-create-contact.png){zoomable="yes"}