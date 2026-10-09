# Tema 2 — Fondamenti e funzionamento dell'Intelligenza Artificiale

**Area:** Comprendere l'AI  
**Stato:** Consolidato e approvato  
**Finalità del documento:** definire il perimetro tematico; non costituisce ancora una scaletta di lezioni.

## Obiettivo formativo

Fornire ai partecipanti una comprensione concettuale dei principali sistemi di Intelligenza Artificiale, dei meccanismi attraverso cui apprendono dai dati e generano risultati, delle modalità di interazione e delle differenti fonti informative utilizzabili.

## Consapevolezza da sviluppare

L'AI non è una forma di intelligenza umana digitale né un semplice archivio di informazioni. È un insieme di sistemi con meccanismi differenti, il cui comportamento dipende dal modello, dai dati, dal contesto e dalle modalità di utilizzo.

## Sottotemi approvati

### 2.1 — Che cos'è l'Intelligenza Artificiale

- Definizione e caratteristiche dell'AI.
- Differenza tra AI e intelligenza umana.
- Sistemi specializzati e concetto di intelligenza artificiale generale (AGI).
- **Integrazione A — Comprensione apparente e antropomorfizzazione:** distinguere capacità osservabili, ragionamento e caratteristiche mentali che le persone possono attribuire impropriamente ai sistemi AI.

**Concetto chiave:** l'AI non è un'unica tecnologia e le prestazioni osservabili non autorizzano automaticamente ad attribuirle caratteristiche umane.

### 2.2 — Le principali categorie di AI

- AI simbolica e basata su regole.
- Machine Learning.
- Deep Learning e reti neurali.
- AI predittiva, discriminativa e generativa.
- AI multimodale.

**Concetto chiave:** esistono approcci e capacità differenti, adatti a problemi differenti. Le categorie elencate rispondono a criteri di classificazione diversi e non sono tutte mutuamente esclusive.

### 2.3 — Come un sistema AI apprende dai dati

- Concetto di apprendimento automatico.
- Dati di addestramento ed esempi.
- Individuazione di schemi e regolarità.
- Parametri del modello.
- Generalizzazione verso nuovi input.
- Differenza tra addestramento e inferenza.

**Concetto chiave:** nei sistemi di Machine Learning l'addestramento modifica i parametri del modello, mentre l'inferenza utilizza il modello per elaborare nuovi input. Non tutti i sistemi AI apprendono dai dati.

### 2.4 — Che cosa sono i Large Language Models (LLM)

- Definizione di modello linguistico di grandi dimensioni.
- Token e rappresentazione del linguaggio.
- Architettura Transformer e attenzione, a livello concettuale.
- Generazione delle risposte.
- Capacità linguistiche, di analisi e di ragionamento.
- Perché un modello può affrontare compiti diversi.

**Concetto chiave:** gli LLM generano output usando regolarità apprese e il contesto disponibile; la spiegazione non va ridotta alla sola metafora del completamento automatico.

### 2.5 — Come funziona un'interazione con l'AI

- Input, prompt e output.
- Tokenizzazione.
- Finestra di contesto.
- Inferenza e generazione.
- Cronologia conversazionale.
- Contesto temporaneo e memoria persistente.
- Distinzione tra il modello e l'applicazione che lo integra, che può includere strumenti, ricerca e altri componenti software.

**Concetto chiave:** il risultato dipende anche dalle informazioni rese disponibili durante l'interazione; il funzionamento del modello e quello del prodotto che lo utilizza non coincidono sempre.

### 2.6 — Conoscenza e fonti informative

- Informazioni apprese durante l'addestramento.
- Informazioni fornite durante l'interazione.
- Accesso a fonti e strumenti esterni.
- Conoscenza incorporata e recupero di informazioni.
- Aggiornamento dei dati e limiti temporali.
- Grounding e introduzione alla Retrieval-Augmented Generation (RAG).
- **Integrazione B — Modalità di adattamento a un contesto specifico:** differenza fra istruzioni, documenti nel contesto, recupero da basi informative e fine-tuning.

**Concetto chiave:** fornire un documento o collegare una fonte a un sistema AI non significa necessariamente riaddestrare il modello.

### 2.7 — Variabilità dei risultati

- Natura probabilistica della generazione.
- Perché lo stesso input può produrre output differenti.
- Influenza di istruzioni, contesto e parametri di generazione.
- Differenza tra comportamento deterministico e probabilistico.
- Riproducibilità dei risultati.

**Concetto chiave:** una stessa richiesta può produrre risposte differenti; la variabilità è distinta dalla questione della correttezza e dell'affidabilità, approfondita nel Tema 3.

## Domande guida

1. Che cosa intendiamo per Intelligenza Artificiale?
2. Come si distinguono AI, Machine Learning, Deep Learning e AI generativa?
3. Che cos'è un modello AI e come viene addestrato?
4. Che cos'è un Large Language Model?
5. Che cosa accade, in termini generali, quando inviamo un prompt?
6. Da dove provengono le informazioni utilizzate per produrre una risposta?
7. Qual è la differenza tra addestramento, contesto, memoria, recupero documentale e fine-tuning?
8. Perché le risposte possono variare a parità di richiesta?

## Profondità di trattazione

| Livello | Concetti |
|---|---|
| **Comprendere bene** | Differenza tra AI e software tradizionale; addestramento e inferenza; funzionamento generale degli LLM; contesto; fonti informative; variabilità delle risposte. |
| **Conoscere** | Machine Learning; Deep Learning; token; Transformer; parametri; fine-tuning; grounding; RAG. |
| **Solo accennare** | Matematica delle reti neurali; ottimizzazione; dettagli delle architetture; procedure avanzate di addestramento e configurazione. |

Tutti i sette sottotemi sono confermati. La diversa profondità non implica l'eliminazione di contenuti.

## Gestione delle sovrapposizioni interne

| Sottotemi | Distinzione |
|---|---|
| 2.1 e 2.2 | Definizione generale vs classificazione degli approcci. |
| 2.3 e 2.4 | Apprendimento automatico in generale vs funzionamento degli LLM. |
| 2.4 e 2.5 | Meccanismo del modello vs processo dell'interazione con l'utente. |
| 2.5 e 2.6 | Interazione vs provenienza e disponibilità delle informazioni. |
| 2.4 e 2.7 | Generazione degli output vs variabilità della generazione. |

## Confini con gli altri temi

- **Tema 1:** non ripetere storia, accelerazione e rilevanza generale.
- **Tema 3:** rimandare l'analisi approfondita di allucinazioni, bias, accuratezza, errori e valutazione dell'affidabilità.
- **Tema 4:** rimandare confronti tra modelli commerciali, prodotti, piattaforme e strumenti.
- **Temi dedicati all'interazione:** rimandare le tecniche operative di prompting.
- **Tema sui dati aziendali:** rimandare l'implementazione pratica di basi documentali, integrazioni e sistemi informativi.

Nel 2.6 è sufficiente introdurre concettualmente la RAG; non serve insegnare a costruire una soluzione RAG.

## Risultati attesi

Il partecipante dovrebbe essere in grado di:

1. Distinguere le principali famiglie e capacità dei sistemi AI.
2. Descrivere a grandi linee come avvengono addestramento e inferenza.
3. Spiegare il funzionamento generale di un LLM e di una conversazione con esso.
4. Distinguere ciò che un modello ha appreso dalle informazioni fornite o recuperate durante l'uso.
5. Comprendere che il comportamento dipende dal modello, dall'applicazione e dal contesto.
6. Interpretare la variabilità degli output senza confonderla automaticamente con un errore.

## Criterio di approfondimento

Usare spiegazioni intuitive e rigorose, evitando sia la tecnicizzazione eccessiva sia semplificazioni fuorvianti. L'obiettivo è capire i meccanismi per poter utilizzare e valutare l'AI, non imparare a sviluppare modelli.
