# Mappa degli sprechi informativi · Laser Srl · Sessione 1

Ultimo aggiornamento: 16 ottobre 2026 · Fonte: board AFFiNE della sessione 1 (`Laser Srl Sessione 1.md`), trascrizione del formatore

**A che cosa serve:** riordina i post-it della sessione 1 per reparto e per tipo di spreco, li raggruppa in temi trasversali e li collega ai casi d'uso del portfolio. Si proietta in apertura della sessione 2 e diventa la materia prima della shortlist (sessione 2) e della matrice (sessione 3).

**Avvertenze**
- La frequenza è indicata solo per un post-it (Amministrazione). Le altre stime vanno chieste in aula (vedi "Da chiedere in apertura").
- Le colonne Commerciale e Acquisti della board sono rimaste vuote; Qualità e HR non compaiono. Alcuni temi commerciali e di acquisto sono stati portati dalla Direzione.
- È comparso un reparto non previsto nell'agenda: **Elettrico**.
- Le colonne "Caso d'uso" e "Rischio" sono proposte del formatore, da validare con Laser.

## 1. Gli sprechi, reparto per reparto

Categorie: le sette della slide "Sette sprechi informativi" (cercare, ricopiare, aspettare, rifare, correggere, chiedere a voce, tradurre). Codici caso d'uso: `portfolio_casi_uso.md`.

| # | Reparto | Spreco (come scritto in aula, ripulito) | Categoria | Caso d'uso vicino | Rischio di errore AI |
|---|---|---|---|---|---|
| D1 | Direzione | Cercare informazioni | Cercare | C01 | Medio |
| D2 | Direzione | Correggere: lavoro sulle fatture, tanti modelli diversi (nota incompleta) | Correggere, ricopiare | Estrazione dati da fatture (nuovo) | Medio: numeri e importi |
| D3 | Direzione | Gestione fornitori: controllo dei documenti forniti | Correggere | Confronto documenti (nuovo) | Medio |
| D4 | Direzione | Confronto su fatture | Correggere | Confronto documenti (nuovo) | Medio: importi |
| D5 | Direzione | Traduzioni, si lavora molto con l'estero; serve un controllo di supporto | Tradurre | C11 | Basso o medio: dati tecnici e numeri |
| D6 | Direzione | Supporto per le offerte | Rifare | C10 | Medio: prezzi e condizioni |
| D7 | Direzione | Controllo dei disegni per capire le modifiche rispetto allo standard e definire con precisione i costi | Cercare, correggere | C01 + confronto | **Alto:** costi e dettagli tecnici |
| D8 | Direzione | Preventivi ripetuti: doppio controllo su varie informazioni per essere certi | Rifare, correggere | C10 | **Alto:** l'AI non è un secondo controllo indipendente |
| A1 | Amministrazione | Recuperare informazioni divise tra i reparti; tempo perso a cercare e ad aspettare risposte. **Frequenza: 4-5 volte al mese** | Cercare, aspettare | C01 (ricerca interna) | Medio |
| A2 | Amministrazione | Riconciliazione dei dati: banca, clienti, estratti conto | Correggere, ricopiare | C12 | Medio: calcoli da eseguire con strumenti, non generati come testo |
| U1 | Ufficio Tecnico | Tavole 3D: disegni ripetitivi | Rifare | Nessuno (vedi nota 1) | n.a. |
| U2 | Ufficio Tecnico | Ricerca tra moltissime tavole dei disegni passati che servono oggi | Cercare | C01 | Medio |
| U3 | Ufficio Tecnico | Normative di settore diverse da stato a stato; conoscenza molto verticale | Cercare, tradurre | Assistente su fonti normative (nuovo) | **Alto:** argomento di nicchia e locale |
| U4 | Ufficio Tecnico | Gestione montatori: controllo incrociato delle informazioni (disegno, presenza del pezzo, gestionale) | Correggere, ricopiare | C03 | Medio |
| U5 | Ufficio Tecnico | Assistenza ai colleghi: domande su procedure tecniche | Chiedere a voce | C01, C13 | Medio |
| P1 | Produzione | Gestione pezzi (da chiarire) | Da chiarire | Da definire | Da definire |
| P2 | Produzione | Riprogrammazione e logistica | Aspettare, rifare | Da definire (vedi nota 2) | Da definire |
| S1 | Service | Accesso alle informazioni necessarie per rispondere al cliente | Cercare | C07 | Medio |
| S2 | Service | Chatbot per l'assistenza (è un'idea di soluzione: va nel parcheggio) | Parcheggio | C07, poi per i clienti | Medio |
| E1 | Elettrico | Inserimento degli ordini | Ricopiare | Estrazione da email (nuovo) | Medio |
| E2 | Elettrico | Database delle informazioni tecniche dei singoli clienti (per esempio i pezzi usati in passato) | Cercare | C01, C09 | Medio |
| E3 | Elettrico | Richieste commerciali sui pezzi: arrivano via email e con foto e vanno ricercate a sistema | Cercare, ricopiare | C09 | Medio: pezzo sbagliato, costi e fermi |

**Nota 1 (U1).** I disegni ripetitivi si affrontano di solito con strumenti CAD parametrici, configuratori e librerie di componenti, prima che con l'AI generativa. È il caso tipico di "prima il problema, poi lo strumento".

**Nota 2 (P1, P2).** Post-it troppo sintetici per capire lo spreco. La pianificazione della produzione usa in genere strumenti di schedulazione e dati del gestionale; l'AI può avere un ruolo (previsioni, ottimizzazione) solo dopo aver chiarito il problema.

**Trascrizione da correggere nella board:** "Sto arrivando!vano via mail" va letto "arrivano via mail" (E3); la nota D2 si interrompe ("tanti modelli difficoltà a..."): chiedere alla Direzione come finisce.

## 2. Sei temi trasversali

| Tema | Post-it | Reparti | Che cosa accomuna | Possibile risposta | Demo collegata |
|---|---|---|---|---|---|
| **A · Informazioni disperse** | D1, A1, U2, U5, S1, E2, E3 | 5 su 6 | Le informazioni esistono, ma sono sparse tra reparti, archivi e persone | Ordine delle fonti + assistente che cerca e **cita i documenti** | Demo 1 (manuale) |
| **B · Controlli incrociati e confronti** | D2, D3, D4, D7, D8, U4, A2 | 3 | Confrontare documenti, fatture, disegni, gestionale per trovare differenze | Estrazione e confronto assistiti, con verifica umana | Demo 2 (contraddizioni) |
| **C · Offerte e preventivi** | D6, D8, E3 | 2 | Richieste diverse, requisiti da estrarre, preventivi simili rifatti | Scheda requisiti + bozza assistita (C10) | Demo 2 |
| **D · Estero: lingue e normative** | D5, U3 | 2 | Traduzioni e regole diverse per paese | Traduzione con glossario (C11); normative solo da fonti ufficiali fornite | Gara di prompt |
| **E · Lavoro ripetitivo sui disegni** | U1 | 1 | Disegni simili rifatti | Soprattutto strumenti non AI (CAD parametrico) | Nessuna |
| **F · Pianificazione della produzione** | P1, P2 | 1 | Da chiarire | Da approfondire | Nessuna |

**Lettura per la sessione 2.** Il tema A è il più diffuso: tocca quasi tutti i reparti e corrisponde alla demo 1. Il tema B è quello in cui il recupero del Tema 3 serve di più: chi usa l'AI per un "doppio controllo" deve sapere che l'AI non è un controllo indipendente (autoverifica, tendenza ad assecondare).

## 3. Dove allucinazioni e bias contano di più

Collegamento diretto con il recupero del Tema 3 in apertura della sessione 2.

| Spreco | Rischio principale | Perché | Contromisura |
|---|---|---|---|
| U3 Normative per paese | Allucinazione | Argomento di nicchia, locale, che cambia nel tempo: è il terreno più favorevole alle invenzioni (slide "Attività che richiedono livelli diversi di verifica") | Solo testi ufficiali forniti allo strumento; risposta con articolo e fonte; verifica di un esperto |
| D7, D8 Disegni, costi, preventivi | Allucinazione su numeri; autoverifica | Numeri, importi, dettagli tecnici; il "doppio controllo" fatto dall'AI non è indipendente | Calcoli con strumenti; confronto con il documento originale; il controllo finale resta della persona |
| D3, D4 Fornitori e fatture | Bias della domanda | "Questa fattura è corretta, vero?" spinge l'AI a confermare | Domanda neutra: "elenca tutte le differenze tra ordine e fattura" |
| A2 Riconciliazioni | Numeri generati | Un LLM che "calcola" scrivendo può sbagliare | Foglio di calcolo o esecuzione di codice; controllo dei totali |
| E3 Pezzi da foto | Allucinazione e conferma | L'AI può riconoscere un pezzo plausibile ma sbagliato e confermarlo se glielo suggeriamo | Proporre più candidati con il codice; confronto con il catalogo |
| D5 Traduzioni | Rischio più basso | Trasformare un testo fornito è il compito in cui l'AI sbaglia meno | Rilettura di numeri, unità, termini tecnici; glossario |
| A1, U2, S1 Ricerca | Risposta oltre i documenti | Se il documento non c'è, l'AI può ricostruire una risposta | Chiedere sempre la fonte; "se non è nei documenti, dillo" |

## 4. Da chiedere in apertura della sessione 2

1. **Frequenza e tempo:** per ogni tema, quante volte al mese e quanto tempo ogni volta? Si raccoglie con i bollini (3 a testa sui post-it che pesano di più).
2. **Direzione, D2:** come finisce la nota sulle fatture? Si tratta di fatture di fornitori in formati diversi?
3. **Produzione, P1 e P2:** che cosa si intende con "gestione pezzi"? Che cosa provoca le riprogrammazioni?
4. **Commerciale e Acquisti:** colonne vuote. Nessuno presente, o sprechi già portati dalla Direzione?
5. **Elettrico:** ordini ed email con foto: in quale sistema si cercano i pezzi? Esiste un catalogo con codici e immagini?
6. **Dati delle macchine** (domanda d'indagine della sessione 1, slide "Tre luoghi dell'AI"): risposta raccolta? Serve per la slide sui dati abilitanti.

## 5. Che cosa portare nella board AFFiNE

- Cornice 2 (sprechi): ricolorare i post-it per reparto, aggiungere il colore per **Elettrico** (da scegliere in legenda) e la stella sui temi A e B.
- Cornice 1 (parcheggio): spostare S2 "Chatbot per assistenza" nella colonna Service.
- Striscia ponte sotto la cornice 2: i sei temi della sezione 2, con le frecce verso la cornice 4 (shortlist).
