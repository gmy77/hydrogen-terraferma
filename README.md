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

- **Calendario lungo.** Ogni giorno simulato vale 15 giorni del calendario: un anno dura circa 39 minuti a velocità 1×,
  e con **Velocità 30× o 100×** («Secoli») passano decenni in pochi minuti.
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
