---
audience: end-user
title: Migliore esperienza di authoring delle e-mail
description: Scopri come semplificare la creazione di e-mail con temi e moduli riutilizzabili, garantendo coerenza ed efficienza nella progettazione delle campagne.
badge: label="Disponibilità limitata" type="Informative"
feature: Email Design
topic: Content Management
role: User
level: Beginner, Intermediate
keywords: Temi e-mail, moduli, riutilizzabilità, coerenza marchio, progettazione e-mail, CSS personalizzato, ottimizzazione mobile
exl-id: c9e02bca-032d-4771-ad53-5bbebabc4c5d
source-git-commit: 9b51dc84a5b6954c973e1560aad877ef770eb8f9
workflow-type: tm+mt
source-wordcount: '2060'
ht-degree: 2%

---

# Applicare temi al contenuto dell’e-mail {#apply-email-themes}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn2"
>title="Temi nel Designer e-mail (LA)"
>abstract="Applica stili di tema e variabili riutilizzabili per mantenere il contenuto delle e-mail coerente con il tuo marchio. Questa funzionalità è disponibile solo per un set di organizzazioni (disponibilità limitata)"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=it" text="Consulta le note sulla versione"

>[!CONTEXTUALHELP]
>id="acw_email_apply_theme"
>title="Applicare un tema all’e-mail"
>abstract="Seleziona un tema per l’e-mail per applicare rapidamente uno stile specifico che sia adatto al brand e alla progettazione."

>[!AVAILABILITY]
>
>Questa funzionalità è a disponibilità limitata. Per ottenere l’accesso, contatta il rappresentante Adobe.

Con i temi, gli utenti non tecnici hanno la possibilità di creare contenuti riutilizzabili che si adattano a un marchio e a un linguaggio di progettazione specifici aggiungendo stili personalizzati sopra i modelli standard<!-- to achieve brand specific results-->.

Questa funzione consente agli addetti al marketing di sfruttare le e-mail visivamente accattivanti e coerenti con il brand in modo più rapido e con meno sforzo, fornendo al contempo opzioni di personalizzazione avanzate per esigenze di progettazione univoche.

## Guardrail e limitazioni {#themes-guardrails}

* Quando crei un’e-mail da zero, puoi scegliere di iniziare a creare i contenuti utilizzando un tema per applicare rapidamente uno stile specifico che si adatta al tuo marchio e design.

  Se scegli la modalità Stile manuale, non potrai applicare alcun tema a meno che non reimposti l’e-mail.

* [I frammenti](../content/fragments.md) non sono compatibili tra le modalità Usa temi e Stile manuale.

   * I frammenti con tema non sono disponibili nei contenuti e-mail creati senza l’utilizzo di temi.

   * Per sfruttare un [frammento](../content/fragments.md) in un contenuto a tema, questo frammento deve essere stato creato utilizzando i temi. [Ulteriori informazioni](#leverage-themes-fragment)

   * Quando utilizzi un frammento nel contenuto dell’e-mail, accertati di applicare un tema definito per questo frammento. In caso contrario, potrebbero verificarsi problemi di visualizzazione, in particolare in Outlook 2021 e nelle versioni precedenti. [Ulteriori informazioni](#leverage-themes-fragment)

* Se utilizzi un contenuto creato in HTML, sarai in [modalità di compatibilità](existing-content.md) e non puoi applicare temi direttamente a questo contenuto.

   * Per applicare i temi, è innanzitutto necessario salvare il contenuto importato [come nuovo modello](../content/create-email-templates.md#save-as-template), quindi convertire il modello in un contenuto compatibile con i temi. Puoi quindi utilizzare questo modello per creare il contenuto delle e-mail. Scopri come convertire un modello creato con lo stile manuale in [questa sezione](#theme-convertor).

   * Puoi anche convertire i contenuti HTML importati. [Ulteriori informazioni](existing-content.md)

  <!--To fully leverage all the capabilities of the Email Designer, including themes, you must either create a new content in Use Themes mode, or convert your imported HTML content. [Learn more](existing-content.md)-->

* Quando si utilizzano font Web personalizzati (inclusi font Google) nei temi, tenere presente che molti client di posta elettronica non li supportano. Definisci sempre i font di fallback appropriati nel tema per garantire la leggibilità in tutti i client e-mail.

   * Gmail e Yahoo! non caricare font web esterni e torneranno ai font di sistema, indipendentemente dalla famiglia di font specificata in HTML/CSS.
   * Gli unici font Google supportati da Gmail sono Roboto e Google Sans.
   * I client di posta elettronica che *do* supportano i caratteri Web includono Apple Mail, iOS Mail, Android Mail, Thunderbird e Outlook per macOS.

<!--If you apply a theme to a content using a [fragment](../content/fragments.md) created with Manual Styling mode, the rendering may not be optimal.-->

## Crea un tema {#create-and-edit-themes}

Per definire un tema che puoi sfruttare nei contenuti delle e-mail future, segui i passaggi indicati di seguito.

1. Per iniziare, crea un nuovo [modello di contenuto](../content/create-email-templates.md).

1. Selezionare l&#39;opzione **[!UICONTROL Crea o modifica temi]**.

   ![Editor modelli di contenuto con l&#39;opzione Crea o modifica temi](assets/theme-create.png)

1. Seleziona un tema Adobe. In questo esempio, seleziona il **[!UICONTROL tema predefinito]** e fai clic su **[!UICONTROL Crea]**.

   ![Selettore tema con tema predefinito selezionato e pulsante Crea](assets/theme-select.png)

1. Puoi anche selezionare un modello personalizzato dalla scheda **[!UICONTROL I miei temi]** e fare clic su **[!UICONTROL Modifica]** per aggiornarlo.

   ![Scheda Temi personali in cui sono elencati i temi personalizzati con Modifica evidenziata](assets/theme-edit.png)

1. Nella scheda **[!UICONTROL Impostazioni generali]**, inizia a definire il tema assegnandogli un nome specifico adatto al tuo marchio. È possibile modificare la larghezza predefinita del riquadro di visualizzazione per le e-mail<!--and also export the current theme for reuse-->.

   <!--![General settings tab for theme name, viewport width, and export](assets/theme-general-settings.png)-->

1. Utilizza la barra a destra per spostarti tra le diverse schede e aggiornare le impostazioni di progettazione.

   ![Barra a destra dell&#39;editor temi con schede per colori, testo, spaziatura e altre impostazioni di progettazione](assets/theme-right-pane.png)

1. Dalla scheda **[!UICONTROL Colori]**:

   * Utilizza il pulsante **[!UICONTROL Modifica]** per impostare una **[!UICONTROL palette di colori]** con i colori predefiniti per il tuo marchio. Seleziona un **[!UICONTROL predefinito]** per creare rapidamente una combinazione di colori o regolare singolarmente ogni colore del tema. Puoi anche utilizzare una combinazione di entrambi.

     ![Animazione di modifica della tavolozza colori tema con predefiniti e colori personalizzati](assets/theme-colors.gif)

   * Fai clic su **[!UICONTROL Aggiungi variante]** per creare più varianti di colore, ad esempio la modalità chiara e scura, in cui ogni variante del tema ha la propria palette di colori e controlli sfumatura.

     ![Varianti di colore nell&#39;editor temi con Aggiungi variante per tavolozze aggiuntive](assets/theme-colors-variant.png)

   * Per ogni variante, fai clic sull&#39;icona **[!UICONTROL Modifica]** per modificare un singolo elemento. Puoi utilizzare la palette predefinita creata oppure qualsiasi colore personalizzato.

     ![Animazione di modifica di singoli colori all&#39;interno di una variante di colore tema](assets/theme-colors-edit-variant.gif)

1. Nelle **[!UICONTROL Impostazioni testo]** è possibile impostare il tipo di carattere globale che si desidera utilizzare per l&#39;intero tema. Per un controllo più granulare, è inoltre possibile modificare ogni intestazione e tipo di paragrafo per regolare il carattere, le dimensioni, lo stile e così via.

   ![Scheda Impostazioni testo per gli stili globali di carattere e intestazione o paragrafo in un tema](assets/theme-text.png)

   >[!NOTE]
   >
   >Quando selezioni i font web personalizzati, tieni presente che molti client e-mail come Gmail e Yahoo! non supportano i font per web esterni e torneranno ai font di sistema. Prendi in considerazione l’inclusione di font di fallback per garantire che il contenuto venga visualizzato correttamente in tutti i client e-mail. [Ulteriori informazioni](#themes-guardrails)

1. Nella scheda **[!UICONTROL Spaziatura]** selezionare un singolo elemento dall&#39;elenco per disporlo correttamente tra i diversi componenti.

   <!--![Spacing tab listing structure elements to adjust spacing between components](assets/theme-spacing.png)-->

1. Utilizzando le altre schede a destra, è possibile gestire separatamente ogni elemento pulsante, divisore, formattazione immagine aggiuntiva e spaziatura layout griglia per questo tema.

   ![Controlli per lo stile dei pulsanti nella barra a destra dell&#39;editor temi](assets/theme-buttons.png)

1. Fai clic su **[!UICONTROL Salva]** per memorizzare questo tema per utilizzi futuri. Ora è visualizzato nella scheda **[!UICONTROL I miei temi]**.

<!--A little strange upon hitting Save, because once the theme is created, you need to hit Close to go back to Design your template screen, then click Cancel if you don't want to proceed with template creation.-->

## Applicare temi a un contenuto e-mail {#apply-themes-email}

Per applicare temi di stile predefiniti o personalizzati a un modello di contenuto o a un messaggio e-mail, effettua le seguenti operazioni.

1. In [!DNL Adobe Campaign], [crea una consegna e-mail](create-email.md) o lavori da una consegna esistente, oppure crea un [modello di contenuto](../content/create-email-templates.md#create-template-from-scratch) e [modifica il contenuto dell&#39;e-mail](get-started-email-designer.md#start-authoring).

1. Puoi selezionare una delle seguenti azioni:

   * Seleziona un [modello e-mail](../content/use-email-templates.md) predefinito per aprire E-mail Designer. A ogni modello viene automaticamente applicato un tema predefinito.

   * Progetta un [nuovo contenuto da zero](create-email-content.md) e seleziona **[!UICONTROL Usa temi]** per iniziare con un tema di stile predefinito.

     ![Schermata iniziale di E-mail Designer con le opzioni Usa temi e Stile manuale](assets/theme-from-scratch.png)

     >[!CAUTION]
     >
     >Se si sceglie la modalità Stile manuale, non sarà possibile applicare alcun tema a meno che la progettazione non venga reimpostata.
     >
     >Per sfruttare un [frammento](../content/fragments.md) in un contenuto a tema, questo frammento deve essere stato creato utilizzando i temi. [Ulteriori informazioni](#leverage-themes-fragment)

1. Una volta nel Designer e-mail, fai clic sul pulsante **[!UICONTROL Temi]** nella barra a destra. Viene visualizzato il tema predefinito o il tema del modello. Per questo tema è possibile alternare tra le due varianti di colore.

   ![Area di lavoro Designer e-mail con il pannello Temi aperto che mostra il tema attivo e le varianti di colore](assets/theme-default-hero.png)

1. Fare clic sulla freccia accanto al tema attualmente utilizzato. Viene visualizzato l’elenco dei temi personalizzati e Adobe disponibili.

   ![Menu a discesa Tema espanso per mostrare i temi Adobe e I miei temi](assets/theme-hero-change.png)

1. Fai clic su **[!UICONTROL I miei temi]** e seleziona un tema creato.

   ![Elenco dei temi personali con un tema creato dall&#39;utente selezionato nel selettore temi](assets/theme-select-custom.png)

1. Fai clic all’esterno dell’elenco a discesa. Il tema personalizzato appena selezionato applica automaticamente i relativi stili a tutti i componenti e-mail. Puoi cambiare le varianti di colore, se presenti.

1. Quando un tema è selezionato in un modello di contenuto, è possibile fare clic sul pulsante **[!UICONTROL Modifica tema]** per aggiornarlo. [Ulteriori informazioni](#create-and-edit-themes)

   ![Modello di contenuto in E-mail Designer con pulsante Modifica tema nel pannello Temi](assets/theme-edit-in-template.png){width="40%"}

   >[!NOTE]
   >
   >Questa opzione non è disponibile quando si utilizzano i temi nei contenuti delle e-mail.

1. Se sfrutti un tema utilizzando diverse varianti di colore, puoi scegliere una variante specifica per un dato componente struttura. Ciò ti consente di definire una variante di colore per l’intero contenuto e di utilizzare una variante diversa per una sola struttura specifica.

   >[!NOTE]
   >
   >Non è possibile eseguire questa azione sui componenti di contenuto.

   A questo scopo, seleziona un componente struttura, fai clic sull&#39;opzione **[!UICONTROL Usa variante tema specifica]** nella scheda **[!UICONTROL Stili]** a destra e applica la variante desiderata a tale struttura.

   ![Struttura selezionata con l&#39;opzione Usa variante del tema specifico nella scheda Stili](assets/theme-structure-variant.png)

   In questo esempio, la prima variante di colore del tema corrente viene applicata all’intero contenuto dell’e-mail, ma la terza variante di colore viene applicata alla struttura selezionata. Puoi vedere che i colori di sfondo del corpo e del riquadro di visualizzazione per quella specifica struttura sono diversi dal resto del contenuto.

È possibile cambiare tema in qualsiasi momento. Il contenuto dell’e-mail rimane invariato, ma gli stili vengono aggiornati per riflettere il nuovo tema.

### Sblocco degli stili {#unlocking-styles}

Quando un componente è selezionato, puoi sbloccarne lo stile utilizzando l&#39;icona dedicata nella scheda **[!UICONTROL Stili]**.

![Scheda Stili in un componente selezionato con l&#39;icona Sblocca stile](assets/theme-unlock-style.png){width="90%"}

Il tema selezionato viene ancora applicato a quel componente, ma è possibile ignorarne gli elementi di stile. Se si modificano i temi, il nuovo tema viene applicato solo agli elementi di stile che non sono stati ignorati.<!--can you revert this action?-->

Se ad esempio si sblocca un componente di testo, è possibile modificare <!--the font size from 11 to 14 and --> il colore del carattere da nero a rosso:

![Componente testo sbloccato con colore del testo rosso personalizzato su sfondo bianco](assets/theme-unlock-style-ex-white.png){width="80%" align="center" zoomable="yes"}

Se si modificano i temi, <!--the font size is still 14 and -->il colore del carattere rimane rosso per quel componente, ma il colore di sfondo per questo componente cambierà con il nuovo tema:

![Lo stesso testo sbloccato con colore rosso mantenuto e sfondo aggiornato da un nuovo tema](assets/theme-unlock-style-ex-colored.png){width="80%"}

## Sfruttare i temi in un frammento {#leverage-themes-fragment}

Per sfruttare un frammento in un modello o in un messaggio e-mail con [temi applicati](#apply-themes-email), è necessario che il frammento sia stato creato utilizzando i temi. In caso contrario, non potrai utilizzare questo frammento nel contenuto a tema.

Per creare un frammento compatibile con i temi, effettua le seguenti operazioni.

1. In [!DNL Adobe Campaign], crea un frammento visivo e fai clic su **[!UICONTROL Crea]** per progettare il contenuto del frammento. [Scopri come](../content/create-fragment.md#create-from-scratch)

1. Seleziona **[!UICONTROL Usa temi]** per iniziare con un tema di stile predefinito.

   ![Opzioni di avvio di Designer e-mail frammento con l&#39;opzione Usa temi selezionata](assets/fragment-use-themes.png){width="100%"}

   >[!CAUTION]
   >
   >Se scegli la modalità Stile manuale, non potrai applicare alcun tema a meno che non reimposti la progettazione del frammento.

1. Una volta in E-mail Designer, puoi iniziare a creare il frammento.

1. Fai clic sul pulsante **[!UICONTROL Temi]** nella barra a destra. Viene visualizzato il tema predefinito. Puoi cambiare le diverse varianti di colore per questo tema.

   ![Contenuto del frammento in E-mail Designer con barra Temi che mostra il tema predefinito](assets/fragment-default-theme.png){width="100%" align="center" zoomable="yes"}

1. Puoi selezionare altri temi per visualizzare in anteprima il contenuto del frammento. A tale scopo, selezionare la freccia accanto al tema predefinito e fare clic su **[!UICONTROL Seleziona temi]**.

   ![Intestazione tema con freccia e controllo Seleziona temi per anteprima frammento](assets/fragment-select-themes.png){width="40%"}

1. Puoi spostarti tra le **[!UICONTROL schede Temi di Adobe]** e **[!UICONTROL Temi personali]** e selezionare fino a cinque temi compatibili (da entrambe le schede) per il frammento.

   ![Finestra di dialogo Seleziona temi compatibili con le schede Temi di Adobe e Temi personali](assets/fragment-select-compatible-themes.png){width=70%}

   >[!CAUTION]
   >
   >Quando utilizzi il frammento in un contenuto e-mail, assicurati di [applicare un tema](#apply-themes-email) definito per questo frammento. In caso contrario, potrebbero verificarsi problemi di visualizzazione, in particolare in Outlook 2021 e nelle versioni precedenti.

1. Fai clic su **[!UICONTROL Chiudi]**.

1. Selezionare nuovamente la freccia accanto al **[!UICONTROL tema predefinito]**. Ora puoi passare dai diversi temi appena selezionati all’anteprima di ogni rendering di stile.

   ![Area di lavoro frammenti con più temi selezionati per l&#39;anteprima nel pannello Temi](assets/fragment-selected-themes.png){width=90%}

1. Fai di nuovo clic su **[!UICONTROL Seleziona temi]** per aggiungere altri temi o modificare la selezione.

## Rendere un modello compatibile con i temi {#theme-convertor}

[!DNL Adobe Campaign] consente di convertire un modello creato con lo stile manuale in un contenuto compatibile con il tema. Ciò può essere particolarmente utile se sono stati creati modelli di contenuto prima dell&#39;introduzione dei temi in [!DNL Adobe Campaign] o se si sta importando contenuto esterno.

>[!NOTE]
>
> Solo i **modelli e-mail** possono essere convertiti per essere compatibili con i temi. Le singole e-mail non possono essere convertite; devi prima salvare il contenuto come modello.

1. Apri un [modello di contenuto](../content/create-email-templates.md) per e-mail e modificane il contenuto tramite E-mail Designer.

1. Seleziona l&#39;icona **[!UICONTROL Temi]** nella barra a destra e fai clic sul pulsante **[!UICONTROL Genera tema da contenuto]**.

   ![Pannello Temi con pulsante Genera tema da contenuto evidenziato](assets/generate-theme.png){width=100%}

1. Viene visualizzata la finestra **[!UICONTROL Crea tema]**. [!DNL Adobe Campaign] rileva automaticamente gli elementi di stile e li consolida in un nuovo tema.

   ![Crea una finestra di dialogo del tema che riepiloga gli stili rilevati dal contenuto del modello](assets/generate-theme-create-window.png){width=90%}

1. Immetti un nome per il tema.

1. Effettuate le regolazioni necessarie, esattamente come fate quando create un tema da zero, ad esempio aggiungendo una variante di colore, modificando i font e così via. [Scopri come](#create-and-edit-themes)

   ![Tema generato nell&#39;editor che mostra la tavolozza dei colori e i controlli delle varianti](assets/generate-theme-colors.png){width=90%}

1. Fai clic su **[!UICONTROL Salva]** per memorizzare questo nuovo tema da riutilizzare. Ora puoi applicare questo tema ai contenuti, come qualsiasi altro tema. [Scopri come](#apply-themes-email)
