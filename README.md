# HYDROGEN · Terraferma 1532

Simulazione di un borgo murato vicentino del Cinquecento, in un solo file HTML (WebGL2, nessuna dipendenza).

I paesani vivono la giornata, sbagliano, **imparano dai propri errori** e **si insegnano le cose** tra loro.
Quando un bisogno del borgo diventa pressante si riunisce la **vicinia** in piazza: chi conosce un rimedio lo propone,
il parroco propone la sua devozione, tutti votano con le ballotte e poi si apre il **cantiere**.

## Come si avvia

**Gioca online:** https://gmy77.github.io/hydrogen-terraferma/

Oppure scarica il repo e apri `index.html` con un browser recente (Chrome, Edge o Firefox).
Il borgo si salva da solo nel browser: riaprendo la pagina la cronaca riprende da dove era rimasta.
Per ricominciare usa il pulsante **Nuovo borgo** oppure apri `index.html?nuovo`.
(HYDROGEN 3 usa un salvataggio nuovo: i borghi salvati con la versione 2 ripartono da capo.)

## Il ciclo bisogno → idea → vicinia → cantiere → verifica

| Bisogno | Opere pratiche (servono il sapere giusto) | Devozione (proposta dal parroco) |
|---|---|---|
| Acqua | Pozzo-cisterna alla veneziana, Roggia dal torrente | Capitello votivo della Madonna |
| Riparo | Portico coperto della Contrada Bassa | — |
| Sicurezza | Lanterne di ferro, Barchessa fuori le mura | Croce votiva |
| Cibo | Granaio pubblico (fontego), Filare di gelsi con abbeveratoio, Mulino ad acqua (dopo la roggia) | — |
| Salute | Orto dei Semplici, Filtro di sabbia della cisterna | Edicola di San Rocco |

- **Il sapere si conquista.** Il fabbro sa forgiare lanterne, il mugnaio conosce i mulini, la fornaia i granai,
  l'erborista le erbe, muratori e tagliapietre sanno murare. Il resto si impara sbagliando
  (il pozzo che si secca, le viti bruciate, il grano marcito, i buoi chiusi fuori dalle mura)
  o ascoltando chi l'ha imparato.
- **Fede contro pratica.** Un'opera di devozione conforta ma non risolve: se il bisogno non cala, chi l'ha votata
  impara la lezione e perde un po' di fede. Se invece il tempo cambia per caso, i devoti gridano al miracolo.
- **Anche le opere possono sbagliare.** La prima cisterna nasce senza filtro di sabbia: l'acqua è torbida,
  arrivano le febbri, lo speziale capisce perché e la vicinia vota il rifacimento.
- **I cantieri sono vivi.** Ponteggi, gru a ruota, paesani che portano pietre e travi, polvere, martelli;
  all'inaugurazione suonano le campane e parte la girandola di fuochi.
- **Cronaca del Borgo.** Ogni fatto importante viene annotato con la data («Adì 7 maggio 1532 …»).

## Stagioni e generazioni (HYDROGEN 3)

- **Calendario lungo.** Ogni giorno simulato vale 15 giorni del calendario. Dal menu **Velocità** si sceglie quanto corre il tempo:
  a **Normale** un giorno del borgo dura poco più di 3 minuti (un anno circa 78 minuti), c'è anche **Lenta** per guardare con calma,
  e salendo fino ad **Anni (60×)** e **Secoli (200×)** passano decenni in pochi minuti. La velocità scelta resta memorizzata.
- **Quattro stagioni.** L'erba ingiallisce d'estate e si arrossa d'autunno; d'inverno nevica e la neve si posa su tetti e campi.
  Il meteo segue la stagione (estati secche, autunni piovosi), d'inverno non si ara, il freddo pesa sulla salute e la fame sul granaio.
- **Famiglie vere.** Ogni paesano ha nome, cognome, età e sesso. Ci si sposa, nascono figli, si invecchia (capelli bianchi, bastone) e si muore,
  con una mortalità simile a quella delle campagne del Cinquecento, che cresce con febbri, fame e inverni duri.
- **Il sapere passa di generazione in generazione.** A 14 anni i figli prendono il mestiere del genitore e ne ereditano parte del sapere.
  I segreti di mestiere (murare, mulino, lanterne, erbe…) si passano solo in famiglia, tra colleghi o lavorando insieme al cantiere.
  Ciò che si è solo sentito dire si può dimenticare; ciò che si è imparato sbagliando resta.
  Se muore l'ultimo che sapeva una cosa, quel sapere si perde: la cronaca lo annota.
- **I ruoli passano di mano.** Quando muore il bifolco, la lavandaia, lo speziale o il parroco, il posto va a un figlio o a un altro paesano;
  se non c'è nessuno arriva qualcuno da Vicenza. Quando il borgo si svuota, arriva gente dalla campagna dei colli Berici.

## Osservatorio del Borgo

Il pulsante **📊 Osservatorio** (o `index.html#osservatorio`) apre una pagina di grafici:

- **Borgo:** popolazione e bambini, piramide delle età, nascite e morti, età media, fede media, regole apprese,
  regole conosciute, i cinque bisogni e le opere costruite, giorno per giorno.
- **Persone:** l'elenco di tutti, vivi e defunti, ordinabile e con ricerca. Per ognuno: gli aspetti di oggi (energia, sete, fede, prudenza,
  regole sapute, errori, regole dimenticate), la famiglia (genitori, coniuge, figli), la sua storia in grafico e una
  **simulazione di 1000 vite possibili** da oggi, con probabilità di essere vivo a ogni età, età attesa alla morte,
  rischio di morire entro un anno e probabilità di sposarsi o avere un figlio.
- **Sapere:** come si diffonde ogni regola nel tempo, chi l'ha scoperta per primo e quanti la sanno oggi.

- **Registro** (anche dal pulsante **🧮 Registro**): ogni cosa che accade riceve un numero progressivo, con data, ora,
  giorno simulato e i valori del borgo in quell'istante (abitanti, i cinque bisogni, regole conosciute).
  Grafici: la **linea del tempo** con ogni evento come un punto sulla riga della sua categoria, il ritmo degli eventi,
  il totale progressivo, il conteggio per categoria (quota e frequenza per anno) e l'andamento di ogni categoria nel tempo.
  Sotto c'è la tabella completa, con filtri, ricerca ed **esportazione CSV**.

Dalla scheda di un paesano nel borgo, il pulsante **📊 Scheda completa** apre direttamente la sua pagina.

## Il borgo che cresce: case, mura, licenze, tasse e legna

- **Il paese**: il borgo è fondato ai piedi del **monte a nord**, con il Bosco del Comune sulle pendici.
  A sud ci sono la porta e i campi; più giù la **strada bianca** scende fino alla **città nuova sul grande mare**,
  con moli, navi, un campanile altissimo e la chiesa con la cupola.
- **Spazio per le famiglie**: ogni casa ha posto per una famiglia. Quando gli abitanti superano i posti comodi
  nasce il bisogno **Case** e le nascite rallentano. La vicinia costruisce prima negli **ultimi lotti dentro le mura**,
  poi vota l'**allargamento delle mura** verso ovest: il **Borgo Nuovo**, con la Porta Nuova e tre file di case.
- **Licenza e tassa**: per allargare le mura la comunità manda una **supplica al Podestà di Vicenza**, che risponde dopo un mese.
  La licenza costa una tassa: se in cassa non ci sono i soldi, la supplica è respinta e si riprova più avanti.
- **Cassa della comunità** (ducati): entrano il lavoro dei paesani, la vendemmia, il mulino e il granaio;
  escono la **taglia alla Serenissima**, pagata a **San Martino** per ogni focolare, le licenze, i mastri dei cantieri e la legna comprata.
- **Legna**: serve ai cantieri e per scaldarsi d'inverno (senza legna le case gelano e arrivano le febbri).
  Si **taglia nel Bosco del Comune**, dove i boscaioli lavorano con l'ascia e gli alberi ricrescono dalle ceppaie in qualche anno,
  oppure si **compra dal mercante della città sul mare**. Chi taglia quasi tutto il bosco impara a farlo a turno (il «ceduo»).
- **Nozze con chi viene da fuori**: se in paese non c'è nessuno libero, ci si sposa con qualcuno dei paesi vicini,
  che viene a vivere nel borgo.

## Generazioni, pelle e pregiudizio

- **Camposanto** accanto alla chiesa: le ultime sepolture con la croce, le ossa più vecchie nell'**ossario**, come si faceva davvero.
  Cliccandolo si vedono gli ultimi sepolti e l'età media alla morte degli adulti (con le regole attuali, intorno ai 50-60 anni).
- **Colore della pelle ereditato**: ogni persona ha la sua tonalità e i figli nascono con una via di mezzo tra quella dei genitori.
  Dalla città sul mare arriva gente di ogni colore, e ci si sposa anche con chi viene da fuori.
- **Il pregiudizio è una credenza falsa.** All'inizio, come è verosimile nel 1532, qualcuno diffida di chi ha la pelle diversa:
  a volte non lo ascolta, gli dà meno voti in vicinia, e i bambini lo prendono in giro.
  Ma vivere vicini, lavorare insieme al cantiere, imparare da quella persona e vedere riuscire le sue proposte lo smentiscono,
  finché si impara la regola: «Il colore della pelle non dice niente di una persona: contano ciò che sa e ciò che fa».
- **Regola della simulazione**: il colore della pelle **non cambia nulla** di ciò che una persona è o sa fare
  (salute, mestiere, sapere, forza, figli, durata della vita). Cambia solo l'aspetto e i pregiudizi degli altri.
  Nell'Osservatorio i grafici «Pregiudizio medio» e «Abitanti per colore della pelle» mostrano come va a finire.

## Chiesa, messa e preghiere

- Ogni mattina le campane chiamano alla **messa**: quasi tutto il paese entra in chiesa, e sopra la facciata si legge quanti fedeli ci sono.
- Chi arriva dalla città sul mare può essere cristiano di **rito greco** (la comunità greca di Venezia era numerosa): stesso Dio, altro rito, prega in casa.
- Quando il borgo è in difficoltà (sete, febbri, fame, paura) i più devoti **pregano** perché il bisogno passi. Pregare dà **conforto** (un po' di energia).
- **Ricevono risposta?** Un mese dopo si controlla se quel bisogno è calato e, per confronto, quanto spesso calano i bisogni negli stessi periodi.
  Chi si sente esaudito si rafforza nella fede, chi no a volte dubita; la predica, le feste e la comunità riportano piano la fede verso la media del tempo.
- La scheda della **chiesa** mostra chi officia, battesimi, nozze e funerali, i fedeli alla messa, i più devoti e il confronto delle preghiere;
  nell'Osservatorio ci sono i grafici «Fedeli alla messa» e «Preghiere e risposte».
- Nella simulazione **non c'è un intervento divino programmato**: ciò che accade dipende dal tempo, dal lavoro e dal caso.
  Se ci sia una risposta, come nella vita, resta una questione di fede.

## Eventi storici: la città sul mare, la peste, la carestia, le piene, il mais

- **La città sul mare** è viva: di giorno i **carri** salgono e scendono la strada bianca, le **navi** entrano ed escono dal porto.
- **La peste** arriva prima in città, con le navi del grano piene di **ratti** (si vedono sui moli), poi può salire al borgo coi carri.
  C'è anche la grande peste del **1576**. Nel borgo il contagio passa in casa e tra i vicini; chi si ammala guarisce (e resta immune) o muore.
- **Come nella vita vera**: dal pulpito la peste è il **castigo di Dio** per i peccati, si fanno processioni (che però radunano la gente e
  **aumentano il contagio**) e si cerca un **capro espiatorio** nei forestieri venuti dal porto: il pregiudizio cresce.
  Quando la peste finisce, i fatti lo smentiscono: sono morti borghigiani e forestieri, devoti e no, e la colpa non era di nessuno.
- **Ciò che si impara**: isolare i malati (il **lazzaretto**, come quello di Venezia del 1423) e **chiudere la porta** a chi viene da luoghi appestati
  (le «fedi di sanità»): durante le epidemie in città i carri restano fermi lungo la strada.
- La simulazione segue il **meccanismo vero** (le pulci dei ratti, scoperto nel 1898), mentre i paesani credono all'«aria cattiva».
- **Dopo la peste**, come accadde davvero, arriva gente dalla campagna a riempire case e mestieri e ci si sposa di più: il borgo si riprende in pochi anni.
  Nel 1577 arriva la notizia del voto del Doge per la chiesa del **Redentore** di Palladio.
- **Carestia** (anche quella grande del **1590**): chi ha il granaio resiste. **Piene del torrente**: campi allagati e legna perduta,
  finché non si alzano gli **argini**. **Il mais** («sorgo turco») arriva dalla città verso metà secolo: il primo raccolto può fallire,
  poi rende più del frumento e accanto alla strada del mare cresce un campo che cambia colore con le stagioni.

## Case e luoghi

Ogni casa ha la sua famiglia: le spose vanno a vivere dal marito, i figli restano coi genitori, chi arriva trova una casa libera.
Cliccando una casa si vede chi ci abita, la contrada, se le finestre sono accese e gli ultimi fatti della famiglia;
cliccando un nome si passa a quella persona. Hanno una scheda con nota storica anche la chiesa, il campanile, il lavatoio,
il pozzo, i banchi del mercato, le due porte, le mura, i campi e le vigne.

## Grafica

Ombre del sole e della luna, bagliore di torce e finestre, acqua con riflessi, nebbia del mattino,
stelle e lucciole di notte, effetto plastico (tilt-shift). Con **Grafica: Leggera** si spengono ombre e post-produzione
per i computer meno potenti.

## Comandi

- Trascina o W/A/S/D: muovi la vista · Rotella o Q/E: zoom
- Clic su un paesano: pensieri, memoria e lezioni apprese · Clic su un edificio: nota storica ed effetto
- **Regia automatica**: la camera vola sulla vicinia, sui cantieri e sulle inaugurazioni
- **Audio**: campane, tuoni, pioggia e martelli (sintetizzati, nessun file esterno)

`originale-v1.html` è la prima versione dell'esperimento, conservata per confronto.
I prossimi passi sono in [TODO.md](TODO.md).

## Copyright

Copyright (c) 2026 Pignolo Gimmy, con la collaborazione di Gemini e Claude. Tutti i diritti riservati. Vedi [LICENSE](LICENSE).
