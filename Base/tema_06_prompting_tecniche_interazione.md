# Tema 6 — Prompting e tecniche di interazione con l'AI

**Area:** Interagire con l'AI  
**Stato:** Consolidato e approvato  
**Finalità del documento:** definire il perimetro tematico; non costituisce ancora una scaletta di lezioni.

## Obiettivo formativo

Sviluppare nei partecipanti la capacità di formulare richieste efficaci ai sistemi AI, selezionare e organizzare le informazioni di contesto, utilizzare differenti tecniche di interazione e migliorare progressivamente i risultati ottenuti.

## Consapevolezza da sviluppare

Il prompting non consiste nell'uso di formule rigide: richiede di definire correttamente il problema, comunicare obiettivi e vincoli, offrire informazioni pertinenti e guidare il sistema attraverso eventuali iterazioni. Un prompt ben formulato aumenta le possibilità di ottenere un risultato utile, ma non ne garantisce la correttezza. L'efficacia dipende anche dal modello, dal compito e dalla capacità dell'utilizzatore di valutare gli output.

## Sottotemi approvati

### 6.1 — Fondamenti del prompting

- Definizione e funzione del prompt.
- Prompt come domanda, istruzione o richiesta di esecuzione.
- Differenza tra richieste generiche e contestualizzate.
- Chiarezza, specificità e pertinenza.
- Ambiguità e informazioni mancanti.
- Relazione tra qualità dell'input e utilità dell'output.
- Differenza tra prompting e programmazione tradizionale.
- Limiti delle istruzioni e assenza di garanzia sul risultato.

**Integrazione C — Prompting e limiti delle istruzioni:** un prompt ben costruito non conferisce al sistema capacità che non possiede e non elimina automaticamente errori o allucinazioni.

**Concetto chiave:** il prompt comunica obiettivi e aspettative, ma non è un comando che assicura un risultato deterministico e corretto.

### 6.2 — Gli elementi di una richiesta efficace

- Definizione del problema da affrontare.
- Chiarimento dell'obiettivo.
- Descrizione del compito.
- Informazioni sul contesto e sul destinatario.
- Vincoli, requisiti e condizioni.
- Formato e livello di dettaglio dell'output.
- Criteri per riconoscere un risultato soddisfacente.
- Ruoli e prospettive assegnati al modello.

**Integrazione A — Il prompting come definizione del problema:** prima di scrivere la richiesta occorre capire quale problema risolvere, a quale scopo e con quali criteri di successo.

**Concetto chiave:** un prompt efficace rende espliciti i requisiti rilevanti; non deve necessariamente essere lungo o contenere tutti gli elementi in ogni situazione.

### 6.3 — Il ruolo del contesto nel prompting

- Informazioni preliminari e conoscenze di riferimento.
- Contesto aziendale e professionale.
- Utilizzo di documenti e materiali pertinenti.
- Distinzione tra informazioni, istruzioni ed esempi.
- Qualità, pertinenza e completezza del contesto.
- Identificazione delle informazioni mancanti.
- Richiesta di chiarimenti e dichiarazione delle ipotesi.
- Gestione di informazioni contraddittorie.
- Limiti e gestione della finestra di contesto.

**Integrazione B — Chiedere all'AI di esplicitare le informazioni mancanti:** il sistema può essere istruito a formulare domande di chiarimento e distinguere i dati disponibili dalle ipotesi prima di produrre il risultato.

**Concetto chiave:** fornire più informazioni non produce automaticamente risultati migliori; è preferibile un contesto pertinente, sufficientemente completo e comprensibile.

### 6.4 — Tecniche fondamentali di prompting

- Zero-shot prompting.
- Few-shot prompting e utilizzo di esempi.
- Istruzioni strutturate.
- Delimitazione e organizzazione dei contenuti.
- Scomposizione dei compiti complessi.
- Richiesta di alternative.
- Confronto tra opzioni attraverso criteri definiti.
- Richiesta di chiarimenti prima dell'esecuzione.
- Selezione delle tecniche in funzione del compito.

**Integrazione B — Chiedere all'AI di esplicitare le informazioni mancanti:** una tecnica utile è richiedere domande mirate quando l'input non consente di procedere in modo affidabile, invece di lasciare implicite le supposizioni.

**Concetto chiave:** la complessità della tecnica deve essere proporzionata al compito; non esiste una strategia unica migliore in ogni situazione.

### 6.5 — Prompting iterativo e miglioramento progressivo

- Prima formulazione della richiesta.
- Analisi delle carenze del risultato.
- Feedback e richieste di correzione.
- Raffinamento progressivo delle istruzioni.
- Approfondimento e riformulazione.
- Gestione delle conversazioni articolate.
- Quando modificare la richiesta e quando ricominciare.
- Limiti del miglioramento attraverso successive iterazioni.

**Integrazione C — Prompting e limiti delle istruzioni:** un output più aderente a tono e formato richiesti non è necessariamente più accurato; ripetere una richiesta non garantisce la rimozione degli errori.

**Concetto chiave:** l'iterazione consente di migliorare l'aderenza al compito, ma la verifica indipendente della correttezza appartiene a una fase distinta.

### 6.6 — Guidare il formato e la struttura degli output

- Definizione del formato desiderato.
- Testi strutturati, elenchi, tabelle e schemi.
- Report, documenti e comunicazioni professionali.
- Livello di dettaglio e sintesi.
- Tono, stile e adattamento al destinatario.
- Introduzione agli output strutturati, come JSON e CSV.
- Vincoli di presentazione.
- Requisiti e criteri di qualità verificabili.

**Concetto chiave:** la forma dell'output ne condiziona l'utilità nelle attività successive, ma la buona formattazione non dimostra la correttezza del contenuto.

### 6.7 — Prompting per attività professionali

- Scrittura e revisione di contenuti.
- Analisi e sintesi documentale.
- Elaborazione e organizzazione di informazioni.
- Ricerca e confronto di alternative.
- Analisi e interpretazione di dati.
- Brainstorming e problem solving.
- Preparazione di report e comunicazioni.
- Adattamento del prompting al tipo di attività.
- Differenze tra attività creative, analitiche e operative.

**Concetto chiave:** il metodo deve adattarsi allo scopo e al contesto lavorativo; il tema insegna ad applicare i principi, non a memorizzare prompt universali.

### 6.8 — Istruzioni riutilizzabili e standardizzazione del prompting

- Differenza tra prompt occasionale e ricorrente.
- Template di prompt.
- Librerie condivise di istruzioni.
- Istruzioni personalizzate e preferenze persistenti.
- Introduzione agli assistenti configurati per attività specifiche.
- Standardizzazione di formati e criteri di qualità.
- Gestione delle versioni delle istruzioni.
- Aggiornamento, manutenzione e verifica nel tempo.
- Limiti della standardizzazione.

**Concetto chiave:** istruzioni riutilizzabili possono favorire coerenza e produttività, ma devono essere manutenute e non sostituiscono il controllo dei risultati.

## Domande guida per i partecipanti

1. Che cos'è un prompt e a che cosa serve?
2. Come identificare correttamente il problema prima di formulare una richiesta?
3. Quali elementi rendono una richiesta sufficientemente chiara e specifica?
4. Quali informazioni di contesto sono davvero pertinenti?
5. Come chiedere chiarimenti su dati mancanti o ipotesi non dichiarate?
6. Quando utilizzare esempi, scomposizione del compito o istruzioni strutturate?
7. Come migliorare un output attraverso feedback e iterazione?
8. Come richiedere un risultato nel formato più utile per il proprio lavoro?
9. Quando conviene trasformare un prompt in un template riutilizzabile?
10. Perché un buon prompt non garantisce un risultato corretto?

## Priorità e profondità di trattazione

| Sottotema | Priorità | Profondità suggerita |
| --- | --- | --- |
| 6.1 — Fondamenti del prompting | Alta | Comprendere bene |
| 6.2 — Elementi di una richiesta efficace | Alta | Comprendere e applicare |
| 6.3 — Ruolo del contesto | Alta | Comprendere e applicare |
| 6.4 — Tecniche fondamentali | Alta | Conoscere e sperimentare |
| 6.5 — Prompting iterativo | Alta | Comprendere e applicare |
| 6.6 — Formati e strutture degli output | Alta | Applicare |
| 6.7 — Prompting per attività professionali | Alta | Applicare in contesti diversi |
| 6.8 — Istruzioni riutilizzabili | Media | Comprendere e conoscere |

**Comprendere e applicare:** definizione del problema, struttura della richiesta, gestione del contesto, istruzioni chiare, iterazione e feedback.

**Conoscere e sperimentare:** zero-shot, few-shot, scomposizione dei compiti, confronto di alternative, output strutturati e template riutilizzabili.

**Solo accennare:** prompt engineering specialistico, ottimizzazione sistematica su benchmark, programmazione di sistemi di prompting e tecniche avanzate legate a specifiche architetture.

## Gestione delle sovrapposizioni interne

| Sottotemi | Distinzione da mantenere |
| --- | --- |
| 6.1 e 6.2 | Il 6.1 spiega il concetto e la funzione del prompt; il 6.2 descrive gli elementi operativi di una richiesta. |
| 6.2 e 6.3 | Il 6.2 introduce il quadro completo; il 6.3 approfondisce la scelta e l'uso delle informazioni di contesto. |
| 6.3 e 6.4 | Il 6.3 riguarda la gestione delle lacune informative; il 6.4 la tecnica per ottenere chiarimenti. |
| 6.4 e 6.5 | Il 6.4 illustra strategie specifiche; il 6.5 il processo di revisione progressiva. |
| 6.4 e 6.6 | Il 6.4 riguarda le modalità di guidare il sistema; il 6.6 la forma e la struttura del risultato richiesto. |
| 6.7 e 6.8 | Il 6.7 applica il metodo ai compiti professionali; il 6.8 riguarda riuso e standardizzazione nel tempo. |

**Decisione:** mantenere separati tutti gli otto sottotemi. Trattare 6.2, 6.3 e 6.4 in modo complementare, evitando duplicazioni di obiettivo, contesto e istruzioni.

## Confini con gli altri temi

- **Tema 2 — Fondamenti e funzionamento:** non ripetere le spiegazioni tecniche su token, inferenza e finestra di contesto.
- **Tema 3 — Capacità, limiti e affidabilità:** non ripetere l'analisi delle allucinazioni e dei bias; richiamare i limiti solo per contestualizzare le tecniche.
- **Tema 5 — Il dialogo uomo-AI:** non ripetere la teoria della collaborazione; sviluppare qui il metodo operativo.
- **Tema 7 — Verifica degli output e pensiero critico:** non entrare nelle metodologie di fact-checking e controllo indipendente; distinguere l'aderenza alla richiesta dalla correttezza.
- **Area delle applicazioni AI:** utilizzare esempi professionali per illustrare le tecniche, senza trasformare 6.7 in un catalogo completo di casi d'uso.
- **Tema su assistenti e agenti:** introdurre template e istruzioni persistenti senza affrontare la configurazione tecnica di sistemi complessi.
- **Area sicurezza e normativa:** non approfondire privacy, protezione dei dati, riservatezza e prompt injection. L'integrazione D proposta non è stata selezionata; resta comunque necessario evitare negli esempi l'inserimento di dati riservati in strumenti non autorizzati.

## Risultati di apprendimento attesi

Al termine del tema, il partecipante dovrebbe essere in grado di:

1. Spiegare cosa sia un prompt e quali funzioni svolga.
2. Definire il problema prima di formulare una richiesta.
3. Esplicitare obiettivi, requisiti e criteri di qualità.
4. Selezionare e fornire informazioni di contesto adeguate.
5. Riconoscere lacune informative e chiedere chiarimenti.
6. Utilizzare tecniche di prompting proporzionate al compito.
7. Migliorare progressivamente le risposte attraverso feedback e iterazioni.
8. Specificare strutture e formati di output utilizzabili.
9. Adattare le tecniche alle principali attività professionali.
10. Costruire e riutilizzare template di istruzioni.
11. Riconoscere i limiti del prompting e la necessità di verificare i risultati.

## Criterio di approfondimento

Il tema non è un repertorio di formule o prompt preconfezionati e non richiede conoscenze specialistiche di sviluppo dei modelli. Si concentra sui principi trasferibili tra strumenti, con esempi riferiti a compiti professionali. Una richiesta semplice può essere appropriata quanto una strutturata: la complessità dipende dal compito. Il prompting è parte dell'utilizzo efficace dell'AI, ma non sostituisce la qualità delle informazioni, la competenza professionale e la verifica degli output.

**Messaggio centrale:** il prompting efficace nasce dalla capacità di definire il problema, comunicarlo con chiarezza, fornire informazioni pertinenti e guidare progressivamente il sistema verso un risultato adeguato allo scopo, senza confondere aderenza alla richiesta e correttezza.
