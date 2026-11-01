# Guida di stile — Italiano (it)

Scritta da un simracer italiano che gioca ad AMS2 da anni, per fissare come deve suonare
Zero to Apex nella sua lingua. Vale per tutte e 2.064 le stringhe del corpus.

## 1. Trattamento

**Uso il "tu".** Mai il "Lei".

In italiano il "Lei" è la lingua del software gestionale, della banca, del modulo di
iscrizione. Nessun gioco di corse italiano lo usa mai per rivolgersi al giocatore —
i simulatori, i giochi ufficiali di F1, i forum e i Discord di
simracing italiani parlano tutti in seconda persona diretta. Zero to Apex ha una manager
che ti scrive in prima persona e un motore che ti parla come un ingegnere alla radio: con
il "Lei" quella voce suonerebbe come l'ufficio contratti, non come il box.

## 2. Vocabolario dell'automobilismo

La community italiana di oggi (TV, box, forum) non è quella dei manuali di meccanica
degli anni '80: decenni di F1 in diretta hanno naturalizzato più anglicismi di quanti i
libri ne accettino ancora. Divido per quello che si dice davvero oggi, non per quello che
"si dovrebbe" dire.

| Termine EN | Scelta IT | Perché |
|---|---|---|
| pit stop | **pit stop** (invariato) | Si dice così in ogni box, in ogni telecronaca. "Sosta ai box" esiste ma è la glossa del libro, non il parlato. |
| paddock | **paddock** (invariato) | Non esiste un equivalente italiano usato davvero. Stesso trattamento dello spagnolo nel glossario del mod. |
| safety car | **safety car** (invariato) | "Auto di sicurezza" è morto insieme ai manuali degli anni '90. In pista e in telecronaca è sempre "safety car" o "SC". |
| setup | **setup** (invariato) | Nel box e sui forum di simracing oggi si dice "il setup". "Assetto" resta nei manuali tecnici, ma il pubblico di questo mod, che gioca in un'interfaccia inglese, dice "setup". |
| stint | **stint** (invariato) | Naturalizzato dalla telecronaca F1/MotoGP moderna ("il primo stint", "cambio di stint"). Non ha un traducente che si usi davvero. |
| pole | **pole** / **pole position** (invariato) | Mai tradotto, in nessun contesto italiano dell'automobilismo, da sempre. |
| grid | **griglia** (tradotto) | "Griglia di partenza" è italiano da decenni, non suona come un prestito. Qui è la regola, non l'eccezione. |
| qualifying | **qualifiche** (tradotto) | Mai sentito dire "qualifying" in italiano. Sempre "le qualifiche". |
| rookie | **rookie** (invariato) | La stampa e la TV di oggi dicono "rookie" molto più spesso di "esordiente"/"debuttante", che ormai suonano da libro di scuola. |
| teammate | **compagno di squadra** (tradotto) | Sempre tradotto, senza eccezioni, in ogni contesto motoristico italiano. |

Il filo conduttore: dove l'italiano ha una parola propria consolidata da decenni (griglia,
qualifiche, compagno di squadra) la uso; dove il box e la TV di oggi dicono l'inglese
(pit stop, paddock, safety car, setup, stint, pole, rookie) lo lascio, anche quando un
manuale offrirebbe un traducente.

## 3. Concetti propri del mod

Parola esatta da usare in tutto il corpus:

| Concetto EN | Parola IT | Perché |
|---|---|---|
| Rating | **Rating** (invariato) | Come "rating Elo" negli scacchi, è un prestito già naturalizzato nello sport italiano. Inventare "Valutazione" accanto a un ELO che resta ELO (keep-en) creerebbe due parole diverse per la stessa idea. |
| Memories | **Ricordi** (tradotto) | Non c'è ragione di lasciarlo in inglese: è un album personale di epoche passate, e "ricordi" è la parola naturale, non tecnica. |
| Sponsorship shop | **Negozio sponsor** (tradotto) | Il negozio delle sponsor card che si apre dopo una gara. **Mai "Negozio carte"**: quel nome traduceva "Card Shop", che è come si chiamava questa schermata quando ho scritto la guida. In inglese le tre chiavi (`tour.shop.intro.t`, `cards.shopTitle`, `cards.results.shopCta`) dicevano tre cose diverse — "Card shop", "Sponsor shop", "Sponsorship shop" — e proprio questa localizzazione ha fatto correggere l'originale: oggi dicono tutte "Sponsorship shop", e gli altri sette idiomi traducono "negozio degli sponsor". "Negozio sponsor" ricalca la chiave gemella della stessa schermata, `cards.walletSub` ("Sponsorship wallet" → "Portafoglio sponsor"), e non inventa niente: `negozio` è già come lo chiama tutto il testo intorno (`cards.shopPending`, `tour.shop.intro.b`) e `sponsor` è già invariabile in tutto il corpus. |
| Seat | **Sedile** (tradotto) | È la parola che usa davvero la stampa di paddock italiana per un posto in squadra ("cercare un sedile", "perdere il sedile"), non un tecnicismo inventato. |
| Contract | **Contratto** (tradotto) | Ovvio, nessuna ambiguità. |
| Silly Season | **Silly Season** (invariato) | Unico caso di frase intera lasciata in inglese: è così che la stampa sportiva italiana (Gazzetta, Sky Sport) la scrive, anche nei titoli. Tradurla ("stagione delle follie") non l'ho mai letta usare sul serio. |
| Paddock | **Paddock** (invariato) | Nessun equivalente italiano in uso reale — stesso trattamento dello spagnolo del mod. |

## 4. Tono

La voce del mod è secca: un ingegnere alla radio, non un ufficio marketing. In italiano
questo si ottiene per sottrazione:

- Frasi corte, dirette, senza subordinate di cortesia ("vorremmo informarti che...").
- Niente punti esclamativi, niente aggettivi da depliant ("un'esperienza unica",
  "un'occasione imperdibile", "il tuo viaggio verso il successo").
- Niente forme impersonali per ammorbidire un ordine o un rifiuto ("si consiglia di",
  "è possibile che tu debba"). Se il motore rifiuta un'azione, lo dice in faccia.
- Attenzione ai calchi dall'inglese che sembrano italiano ma non lo sono: "realizzare"
  per "capire", "supportare" per "sostenere/reggere", "il team" quando il testo dice
  "the team" ma intende "la squadra" nel senso sportivo — vanno adattati, non ricalcati.
- Il gergo tecnico (budget, ritmo, trattativa) resta quello vero di un box, non un
  sinonimo più elegante da traduttore.

## 5. Lunghezza

L'italiano tende ad allungarsi rispetto all'inglese, di solito il 10-20% in più
(articoli, preposizioni articolate, desinenze verbali). Quando il testo tradotto non
entra nel `max_len`, l'ordine di sacrificio è:

1. **L'articolo**, se il contesto visivo (un'etichetta, un chip) lo rende superfluo.
2. **L'aggettivo o l'avverbio ridondante** con quello che lo schermo già mostra
   (es. "ATTUALE" quando la posizione nello schermo lo dice già).
3. **La perifrasi**, sostituita da un sinonimo più corto e altrettanto naturale
   ("trattativa" invece di "processo di negoziazione").
4. **L'abbreviazione convenzionale**, solo dentro un chip numerico dove lo spazio è
   davvero fisso (es. "sett." per "settimana"), e mai se genera ambiguità.
5. **Mai**: numeri, simboli di valuta, `{placeholder}` o `{{placeholder}}`. Si tagliano
   per ultimi, solo su testo di puro andamento (`chrome`), mai su un'etichetta che il
   giocatore deve capire al volo.

## 6. Dieci esempi dal corpus

1. **`access_title`** — EN `ACCESS · 2 WAYS IN` (max_len 28)
   IT: **`ACCESSO · 2 VIE`**
   La versione letterale ("ACCESSO · 2 VIE D'INGRESSO") sfora il limite. Taglio "d'ingresso"
   come ha fatto lo spagnolo tagliando "in": "vie" da solo regge il senso nel contesto.

2. **`pd_ahead_of_mate`** — EN `you lead, P{{pos}}`
   IT: **`comandi, P{{pos}}`**
   "Comandare" è il verbo che la telecronaca italiana usa per "essere in testa alla gara".
   Più corto e più da box del letterale "sei in testa a".

3. **`pd_break_fee`** — EN `Walking out costs ₡ {{n}}`
   IT: **`Andartene costa ₡ {{n}}`**
   Il bottone poco sopra dice "Rescindi" (formale); questa riga di conferma è colloquiale
   di proposito, come in inglese passa da "Terminate" a "Walking out". "Andartene"
   mantiene quel salto di registro; "recedere dal contratto" lo avrebbe annullato.

4. **`off_no_negotiation`** — EN `No room to negotiate — sign as-is`
   IT: **`Zero margine di trattativa — si firma così com'è`**
   "As-is" reso con l'idioma italiano "così com'è", non con un calco tipo "come è".
   "Trattativa" è la parola che usa davvero la stampa di mercato, non "negoziazione".

5. **`buyConfirm.title`** — EN `Buy this car?`
   IT: **`Comprare questa auto?`**
   Niente punto interrogativo rovesciato (l'italiano non lo usa). "Auto" invece di "vettura":
   è quello che diresti indicando l'auto sullo schermo, non una scheda tecnica. In prosa
   narrativa "macchina" va benissimo (`ctype_pitch_*` dice "ti vogliamo in macchina"), ma le
   ETICHETTE dell'interfaccia dicono tutte "auto" -- 32 stringhe contro 14 -- e un'etichetta
   che si scosta dalle altre si nota.

6. **`ob_intro` / `ob_intro_v0`** — EN `{player}, I'm Atenea Montero. As of today, I run
   your career.\n\nI don't hand out seats; I open doors, and results keep them open.
   Everything that matters lands here: offers, milestones, the decisions only you can
   make.\n\nI don't write to fill your screen, so read what I send. Atenea`
   IT: **`{player}, sono Atenea Montero. Da oggi la tua carriera la gestisco io.\n\nNon
   distribuisco sedili; apro porte, e i risultati le tengono aperte. Tutto quello che
   conta arriva qui: offerte, traguardi, le decisioni che puoi prendere solo tu.\n\nNon
   scrivo per riempirti lo schermo, quindi leggi quello che ti mando. Atenea`**
   Frasi corte come l'inglese, niente "Gentile pilota" da email aziendale. "Seats" diventa
   "sedili" — la parola vera di paddock — non il burocratico "posti".

7. **`calib_epic_body`** — EN `Listen. A {{class}} series is touring {{country}} this
   week... Don't waste it.`
   IT: **`Ascolta. Questa settimana una serie {{class}} fa tappa in {{country}}, e hanno
   aperto la griglia a piloti tutti da scoprire. Occasioni così non si ripetono: uno
   schieramento pieno di professionisti, un weekend per dimostrare di che pasta sei
   fatto. Corri questa e nella tua carriera ci sarà un prima e un dopo. Non sprecarla.`**
   "Grid" tradotto in "griglia" (regola §2). "Di che pasta sei fatto" è l'idioma vero, non
   il calco "cosa sei fatto". Tengo la stessa carica drammatica dell'inglese senza
   scivolare nel depliant ("un'opportunità imperdibile" non compare mai).

8. **`nego_ultimatum_v1`** — EN `{player}, we want you in the car, but this is the
   line.\n\nOriginal terms. Yes or no.`
   IT: **`{player}, ti vogliamo in macchina, ma il limite è questo.\n\nTermini
   originali. Sì o no.`**
   Resto tagliente come l'originale: niente attenuanti ("però dobbiamo dirti che...") che
   l'italiano da trattativa tenderebbe ad aggiungere. "Sì o no." resta un punto secco.

9. **`ops_damage_irked`** — EN `Another {cost} on repairs at {track}, {player}. This is
   becoming a habit.\n\nThe budget isn't bottomless, and the mechanics would like a quiet
   weekend for once. Tidy it up.\n\n{team}`
   IT: **`Altri {cost} di riparazioni a {track}, {player}. Sta diventando
   un'abitudine.\n\nIl budget non è infinito, e ai meccanici farebbe comodo un weekend
   tranquillo per una volta. Datti una regolata.\n\n{team}`**
   I quattro placeholder restano al loro posto. "Datti una regolata" sostituisce il
   letterale "sistemalo": è il tono di un team manager infastidito ma non furioso, non
   quello di una lettera di richiamo aziendale.

10. **`pd_ask_youth`** — EN `Being young` (max_len 24)
    IT: **`Essere giovani`**
    Resto sulla forma nominale nuda invece di "La giovane età" da opuscolo: l'etichetta
    vive accanto ad altre quattro dello stesso taglio ("Ritmo puro", "Correre pulito"...)
    e deve avere la stessa forma secca, non suonare più curata delle vicine.
