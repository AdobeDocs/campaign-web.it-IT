---
audience: end-user
title: Utilizzare un gruppo trappola
description: Scopri come utilizzare un gruppo di trappole per la consegna nell’interfaccia utente web di Campaign
exl-id: 48c34581-8825-4798-b24e-c462303f7645
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 4%

---

# Utilizzare un gruppo trappola {#trap-group}

Un **[!UICONTROL gruppo trap]** (noto anche come **[!UICONTROL elenco seed]**) viene utilizzato per includere indirizzi specifici nelle consegne per monitorare e verificare il processo di distribuzione eseguendo il targeting di profili che non corrispondono ai criteri di destinazione definiti. In questo modo, i destinatari che non rientrano nell’ambito di consegna possono ricevere la consegna, come qualsiasi altro destinatario.

Un **[!UICONTROL gruppo trap]** è un gruppo di **[!UICONTROL indirizzi seed]**, denominato **[!UICONTROL Profilo di test]** nell&#39;interfaccia utente Web di Campaign.

## Perché utilizzare un gruppo di trappole {#why-trap-group}

È possibile utilizzare un **[!UICONTROL gruppo trap]**:

1. **Come prova**: ogni membro del **[!UICONTROL gruppo trap]** riceve la consegna come se facesse parte del pubblico.

1. **Per proteggere la tua mailing list**: ricevendo ciò che il pubblico riceverà, ogni **[!UICONTROL profilo di test]** del **[!UICONTROL gruppo di trap]** verrà notato se la mailing list viene utilizzata da una terza parte.

>[!NOTE]
>
>Oltre a [inviare bozze durante la creazione della consegna](../email/create-email.md#preview-test) e dal [gruppo di controllo](control-group.md), l&#39;aggiunta di un gruppo di trap è un buon modo per testare il pubblico.

## Informazioni sui gruppi di trap {#about-trap-group}

I profili di test vengono automaticamente esclusi dai rapporti sulle seguenti statistiche di consegna: **Clic**, **Aperture**, **Annullamenti abbonamenti**. I rapporti si concentrano solo sul pubblico reale.

Per una consegna e-mail, è necessario solo l&#39;indirizzo e-mail per il **[!UICONTROL gruppo di trap]**. La personalizzazione di altri campi viene compilata in modo casuale da Campaign.

## Aggiungere un gruppo di trappole in una consegna {#trap-group-in-delivery}

Per impostare un **[!UICONTROL gruppo di trap]**, vai alle impostazioni **[!UICONTROL Pubblico]** della consegna. Sono disponibili due opzioni:

* [Selezionare i profili di test](#select-test-profiles)
* [Creare una condizione](#create-condition)

[Schermata interfaccia impostazioni gruppo trap](assets/trap-group.png){zoomable="yes"}

### Selezionare i profili di test {#select-test-profiles}

Quando scegli **Seleziona profili di test**, utilizza il pulsante **Aggiungi profili di test** come illustrato di seguito:

[Schermata del pulsante Aggiungi profilo di test](assets/trap-no-test-profile.png){zoomable="yes"}

Quando fai clic sul pulsante, puoi accedere ai profili di test da aggiungere al **[!UICONTROL gruppo di trap]**. Seleziona quelli che desideri utilizzare.

Puoi anche creare nuovi profili di test. [Ulteriori informazioni](#create-seed)

[Seleziona schermata interfaccia profili di test](assets/trap-select-test-profiles.png){zoomable="yes"}

Dopo aver confermato i profili di test, verifica che il numero corretto sia visualizzato in **[!UICONTROL Gruppo di trap]**.

[Schermata di conferma del gruppo di trap](assets/trap-check.png){zoomable="yes"}

### Creare una condizione {#create-condition}

Con l&#39;opzione **[!UICONTROL Crea condizione]**, crea una query per definire i profili di test che desideri utilizzare:

[Crea schermata dell&#39;interfaccia della condizione](assets/trap-create-condition.png){zoomable="yes"}

La query viene visualizzata in **[!UICONTROL Gruppo di trap]**.

[Schermata di visualizzazione della query del gruppo di trap](assets/trap-custom.png){zoomable="yes"}

## Creare un nuovo profilo di test {#create-seed}

Puoi creare un nuovo **[!UICONTROL profilo di test]** dalla cartella **[!UICONTROL Explorer]** > **[!UICONTROL Risorse]** > **[!UICONTROL Gestione campagne]** > **[!UICONTROL Membri seed]**.

[Crea schermata di navigazione del profilo di test](assets/trap-create.png){zoomable="yes"}

Configura tutte le impostazioni per il **[!UICONTROL profilo di test]** come faresti per qualsiasi profilo:

[Schermata di configurazione del profilo di test](assets/trap-create-contact.png){zoomable="yes"}