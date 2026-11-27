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

## Copyright

Copyright (c) 2026 Pignolo Gimmy, con la collaborazione di Gemini e Claude. Tutti i diritti riservati. Vedi [LICENSE](LICENSE).
