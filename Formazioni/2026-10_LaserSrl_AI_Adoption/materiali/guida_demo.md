# Guida alle demo e ai materiali fittizi · Laser Srl · AI Adoption

Ultimo aggiornamento: 10 ottobre 2026

Tutti i materiali sono **fittizi**: azienda "Forni Demo S.r.l.", forno "TF-900 Demo", clienti con nomi di fantasia, dati inventati. Ogni documento lo dichiara in fondo alla pagina. Si possono caricare in Copilot senza rischi di riservatezza.

## I materiali

| File | Serve per | Slide |
|---|---|---|
| `Manuale_TF-900_Demo_fittizio.docx` | Demo 1 (knowledge assistant) | N16 |
| `Richiesta_offerta_Galletas_Ejemplo_fittizia.docx` | Demo 2 (bozza strutturata dalla richiesta del cliente) | N17, B7 |
| `Ticket_assistenza_fittizi.xlsx` | Demo 3 (sintesi operativa dei ticket) | N18 |
| `Report_intervento_RI-2026-118_fittizio.docx` | Demo 3, seconda parte (report dalle note dettate) | N18 |
| `Documento_1_scheda_prodotto_fittizia.docx` · `Documento_2_procedura_interna_fittizia.docx` · `Documento_3_offerta_riservata_fittizia.docx` | Caso "posso caricarlo?" (sessione 3, uso sicuro) | T17·16 |

I materiali sono collegati tra loro: i ticket citano gli allarmi e i ricambi del manuale, il report d'intervento corrisponde ai ticket TK-2026-0412 e TK-2026-0415, la procedura interna (Documento 2) fissa i tempi di presa in carico dei ticket di sicurezza.

## Prima di registrare o di andare in aula

1. Usare **l'account Copilot con cui si farà la demo** e verificare che sia la versione con protezione dei dati aziendali (icona o dicitura di protezione).
2. Provare ogni prompt **almeno tre volte**: le risposte cambiano (variabilità, T2·58). Annotare che cosa cambia: è materiale per l'aula.
3. Per i video: registrare lo schermo, tagliare le attese, durata 2-3 minuti; tenere una voce fuori campo o commentare dal vivo in aula.
4. Salvare screenshot dei passaggi chiave per le slide N16, N17, N18 (riserva se Copilot o la rete non rispondono).

---

## Demo 1 · Dal manuale al knowledge assistant (dal vivo)

**Messaggio:** l'AI trova e riassume quello che c'è nel documento, ma bisogna chiedere la fonte e controllare. Collegamenti: T8·27 (tracciabilità), T14·36 e T14·39 (recupero), T8·69 (caricare non significa elaborare).

**Preparazione:** allegare il manuale a Copilot.

| # | Prompt | Che cosa dovrebbe rispondere | Che cosa far notare |
|---|---|---|---|
| 1 | "Compare l'allarme A01 sul bruciatore 2 della zona 2. Che cosa devo fare? Indica i capitoli del manuale da cui prendi le informazioni." | Riarmare una volta; se si ripete controllare l'elettrodo (cap. 6 e 8); usare l'elettrodo RD-1021B (cap. 10 e 11) | Risposta con fonte: si può verificare in pochi secondi |
| 2 | "Ogni quanto va pulito il filtro aria dei bruciatori?" | **Trappola:** il capitolo 8 dice ogni 3 mesi, la tabella del capitolo 9 dice ogni settimana | Se Copilot dà una sola risposta, chiedere: "Ci sono indicazioni diverse nel manuale su questo punto?" La contraddizione esiste solo se si cerca |
| 3 | "Qual è la coppia di serraggio dei bulloni del bruciatore?" | **Trappola:** il manuale non lo dice. Risposta corretta: "non presente" | Se inventa un valore: è un'allucinazione su un dato che sembra plausibile (T3·20) |
| 4 | "Qual è la capacità produttiva del forno in kg all'ora?" | Il manuale dice che non esiste un valore unico (cap. 2) | Verificare se Copilot "stima" comunque un numero |
| 5 | "La ricetta R01 è compatibile con le caratteristiche della macchina?" | **Trappola:** R01 prevede 6,0 m/min, ma la velocità massima del nastro è 5 m/min (cap. 2 e 5) | Errore nel documento stesso: l'AI lo nota solo se la domanda la porta a confrontare |
| 6 | "Un cliente chiede se può escludere il microinterruttore della porta che si apre da sola. Che cosa rispondo?" | No: mai escludere (cap. 1 e 6); sostituire il microinterruttore RD-4410 | Tema di sicurezza: qui la risposta dell'AI va sempre confrontata con il manuale approvato |

## Demo 2 · Dalla richiesta del cliente alla bozza strutturata (video)

**Messaggio:** l'AI organizza in pochi secondi una richiesta in inglese e trova le lacune; prezzi, tempi e referenze restano al commerciale. Collegamenti: T8·37 (dal non strutturato al dato), T8·47 (contraddizioni e lacune), T6·71 (schema delle richieste importanti), scheda progetto C10 del portfolio.

**Preparazione:** allegare `Richiesta_offerta_Galletas_Ejemplo_fittizia.docx`.

**Prompt (da mostrare anche in slide B7):**
> Sei un tecnico commerciale di un costruttore di linee per biscotti. Analizza la richiesta allegata.
> 1. Estrai i requisiti in una tabella in italiano (requisito, valore richiesto, fonte: email o allegato).
> 2. Segnala le contraddizioni tra email e allegato.
> 3. Elenca le informazioni mancanti che servono per dimensionare la linea e preparare l'offerta.
> 4. Prepara una bozza di risposta in inglese che ringrazia, conferma la ricezione e chiede i chiarimenti.
> Non inserire prezzi, tempi di consegna, referenze o impegni: li aggiungerà il commerciale.

**Che cosa dovrebbe trovare:**
- **Contraddizione:** capacità 800 kg/h nell'email, 1.000 kg/h nell'allegato.
- **Informazioni mancanti** (almeno alcune): peso e spessore dei pezzi; caratteristiche dell'impasto; alimentazione elettrica (tensione e frequenza dello stabilimento: in Messico la rete elettrica è diversa da quella europea, da verificare); pressione e tipo di gas; altezza del capannone; norme o certificazioni richieste nel paese; dettagli sull'assistenza da remoto (connessione, sicurezza informatica); dimensionamento dell'impastatrice.

**Trappole da far notare:**
- Il cliente chiede **referenze in America Latina**: se Copilot le inventa, è il caso perfetto per parlare di allucinazioni.
- Se la bozza promette tempi ("la linea sarà pronta entro settembre 2027"), ha superato il limite indicato nel prompt: va corretta.

## Demo 3 · Dai ticket alla sintesi operativa (video)

**Messaggio:** l'AI vede schemi ricorrenti in tanti ticket, ma i dati sporchi e i casi di sicurezza richiedono il controllo di una persona. Collegamenti: T9·38 (anomalie), T9·40 (correlazione e causalità), T14·19 (obsolescenza delle fonti), C07 e C15 del portfolio.

**Preparazione:** allegare `Ticket_assistenza_fittizi.xlsx` (e il manuale, se lo strumento lo consente).

**Prompt:**
> Sei il responsabile del servizio assistenza. Analizza i ticket allegati e prepara una sintesi operativa di una pagina:
> 1. problemi ricorrenti, per codice di allarme e per matricola, con il numero di ticket;
> 2. per ogni problema ricorrente, un'ipotesi di causa comune, indicando che è un'ipotesi;
> 3. ticket che riguardano la sicurezza e che vanno segnalati subito;
> 4. ticket aperti in ordine di priorità;
> 5. problemi di qualità dei dati (duplicati, campi vuoti o sbagliati).

**Che cosa dovrebbe trovare:**
- **A01 sui forni del 2024** (matricole TF9-2024-029, -031, -033, tre clienti diversi): ipotesi elettrodo vecchio tipo RD-1021; possibile campagna preventiva con RD-1021B.
- **A09 dopo il lavaggio del nastro** (clienti A ed E): i clienti usano la procedura vecchia (Rev. 01); mandare la Rev. 03.
- **Sicurezza:** TK-2026-0413 e TK-2026-0423 (il cliente G vuole escludere il sensore della porta, ticket ancora aperti e non segnalati); TK-2026-0415 (microinterruttore bloccato con una fascetta). Secondo la procedura interna (Documento 2) andavano presi in carico entro 2 ore.
- **Cliente D:** cottura non uniforme sul lato destro, compatibile con filtri aria sporchi (manuale, cap. 11); in attesa del cliente da settembre.
- **Dati:** TK-2026-0420 duplica TK-2026-0419, con il campo "Macchina" sbagliato ("Email"); quattro ticket senza codice di allarme (TK-2026-0403, 0416, 0417, 0421; per le richieste di ricambi è normale).

**Trappole da far notare:**
- **Correlazione e causalità:** "elettrodo vecchio" è un'ipotesi plausibile, non una causa dimostrata.
- Se la sintesi **non mette in evidenza i ticket di sicurezza**, è il punto più importante della demo: l'AI ha riassunto bene, ma ha perso ciò che conta di più.

**Seconda parte (facoltativa, 1 minuto):** allegare `Report_intervento_RI-2026-118_fittizio.docx` e chiedere: "Trasforma le note del tecnico in un report strutturato (problema, verifiche, interventi, esito, azioni da fare) ed elenca le azioni con un responsabile." Verificare che **la nota sul microinterruttore bloccato** non sparisca nella versione "pulita".

---

## Caso "posso caricarlo?" (sessione 3, uso sicuro)

Mostrare i tre documenti e chiedere (o dire, nel percorso B): "posso caricarlo in Copilot?"

| Documento | Risposta | Perché |
|---|---|---|
| 1 · Scheda prodotto | Sì | Già pubblico |
| 2 · Procedura interna | Sì, ma solo nello strumento aziendale autorizzato | Uso interno, nessun dato personale né di clienti |
| 3 · Offerta riservata | No, o solo se la policy lo consente, nello strumento autorizzato, dopo aver tolto prezzi, sconto, nome e cellulare | Prezzi e margini riservati, dato personale, nota interna "non comunicare" |

Collegamenti: T17·16 (quali informazioni), T17·19 (minimizzare), T17·20 (anonimo, pseudonimo, oscurato).
