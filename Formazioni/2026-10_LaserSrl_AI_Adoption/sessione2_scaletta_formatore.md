# Scaletta del formatore · Sessione 2 · Laser Srl · AI Adoption

Ultimo aggiornamento: 16 ottobre 2026 · Sostituisce, per la sessione 2, la tabella di `agenda.md` (percorso A) · Deck: `slide/Sessione2_Laser.pptx`

## Che cosa cambia rispetto all'agenda

Nella sessione 1 non c'è stato tempo per il **Tema 3** (capacità, limiti, affidabilità): restano da fare in particolare **allucinazioni e bias**, che l'agenda considera da "comprendere bene". Il recupero va **in apertura**, per due motivi:
1. prepara lo sguardo critico sulle tre demo (le trappole delle demo sono allucinazioni, omissioni e correlazioni scambiate per cause);
2. tocca direttamente gli sprechi della sessione 1: normative per paese, costi dai disegni, "doppio controllo" sui preventivi (vedi `mappa_sprechi_sessione1.md`, sezione 3).

Per far posto a 40 minuti di recupero, gli altri blocchi si accorciano di 35 minuti in tutto. Slide tolte rispetto all'agenda: T4·22, T4·48, T11·24, T10·18, T9·56, T15·43, N20 e N23 (contenuti assorbiti in N19 e N21). Margine finale: 15 minuti.

**Notazione.** Il numero è la slide del deck della sessione 2. Tra parentesi l'origine: **S1·n** = slide n del deck della sessione 1 (blocco Tema 3 già adattato, non presentato); **T3·23** = Tema 3, slide 23 della base; **Nuova** = slide creata per questa sessione. Le note del relatore delle slide riprese dalla base e dalla S1 sono quelle originali. **Tema 6:** le origini usano la numerazione della versione del 16 ottobre 2026 (57 slide); il deck della sessione 2 contiene le slide nella versione precedente, con contenuti equivalenti salvo la slide 35: il ciclo del miglioramento progressivo nella nuova base è sostituito da "Il prompting come conversazione" (T6·30).

## Sintesi dei tempi

| Ora | Blocco | Durata | Slide |
|---|---|---|---|
| 0:00 | Apertura e ripresa | 15' | 1-4 |
| 0:15 | **Recupero Tema 3: allucinazioni e bias** | 40' | 5-25 |
| 0:55 | Strumenti: che cosa c'è in Laser | 15' | 26-30 |
| 1:10 | Prompting essenziale e gara di prompt | 30' | 31-37 |
| 1:40 | *Pausa* | 15' | |
| 1:55 | Assistenti per documenti e tre demo | 40' | 38-46 |
| 2:35 | Agenti AI | 10' | 47-49 |
| 2:45 | Dagli sprechi ai casi d'uso: processi, service, macchina | 30' | 50-59 |
| 3:15 | Esercizio: shortlist dei casi d'uso | 25' | 60-62 |
| 3:40 | Chiusura | 5' | 63 |
| 3:45 | *Margine* | 15' | |

---

## 0:00 · Apertura e ripresa (15')

| # | Slide | Origine | Che cosa fare |
|---|---|---|---|
| 1 | Titolo sessione 2 | S1·1 adattata | Benvenuto; obiettivo del giorno: dagli sprechi agli strumenti |
| 2 | Il percorso in tre sessioni | S1·2 | Dire apertamente che si riprende il Tema 3 non concluso |
| 3 | Che cosa avete provato | Nuova (N13) | Giro rapido sui compiti per casa: richiesta, risultato, errori, tempo. Annotare 2-3 casi: torneranno nel recupero (errori) e nella shortlist (idee) |
| 4 | Gli sprechi che avete indicato | Nuova | Proiettare anche la board AFFiNE (cornice 2). **Bollini:** 3 a testa sugli sprechi che pesano di più. Fare le domande della sezione 4 di `mappa_sprechi_sessione1.md` (frequenza, D2, P1-P2, Commerciale e Acquisti) |

**Percorso B:** nessun bollino; il formatore legge i sei temi e chiede per alzata di mano quale pesa di più.

## 0:15 · Recupero Tema 3: allucinazioni e bias (40')

Messaggio del blocco: **calibrare la fiducia**. Né fidarsi sempre, né scartare l'AI perché "sbaglia".

| # | Slide | Origine | Min | Che cosa fare |
|---|---|---|---|---|
| 5 | Capacità, limiti e affidabilità (titolo) | S1·61 adattata | | "Lo avevamo lasciato in sospeso" |
| 6 | Calibrare la fiducia | S1·62 | 2 | La scala: fiducia eccessiva, calibrata, sfiducia totale |
| 7 | 3.3 Allucinazioni e informazioni false | S1·67 | | |
| 8 | Che cos'è un'allucinazione | S1·68 | 2 | Tre forme: inventate, inesatte, prive di fondamento |
| 9 | Citazioni e fonti inesistenti | S1·69 | 2 | Caso Mata contro Avianca, in breve |
| 10 | Perché si verificano | S1·70 | 2 | Senza tecnicismi: genera il plausibile, non verifica |
| 11 | Plausibilità e veridicità: quale delle due è vera? | T3·23 | 3 | **Mini-attività:** alzata di mano A o B. Risposta: A (art. 3; in vigore il 1° agosto 2024) |
| 12 | L'autorevolezza apparente | S1·71 | 2 | Segnali di forma e di sostanza |
| 13 | Attività con livelli diversi di verifica | S1·72 | 2 | **Collegare alla mappa:** normative per paese (U3) e costi dai disegni (D7) stanno nella colonna di sinistra |
| 14 | Caccia all'allucinazione | S1·91 | 7 | **Esercizio 1, dal vivo con Copilot** (scheda in `sessione2_esercitazioni.md`) |
| 15 | 3.4 Bias e distorsioni | S1·73 | | "Un'allucinazione è un errore; un bias è una tendenza" |
| 16 | Che cosa sono bias e distorsioni | S1·74 | 2 | La bilancia starata |
| 17 | Da dove nascono | S1·75 | 1 | Solo il caso Amazon, in una frase |
| 18 | L'influenza del contesto e delle istruzioni | S1·76 | 2 | Il fornitore A: domanda orientata e domanda neutra |
| 19 | Bias di conferma e tendenza ad assecondare | S1·77 | 2 | "Sei sicuro?": l'AI può cambiare una risposta giusta |
| 20 | Neutralità apparente e oggettività effettiva | T3·33 | 1 | **Facoltativa:** saltare se si è in ritardo |
| 21 | Esercizio: domanda orientata o neutra? | Nuova | 6 | **Esercizio 2** sui casi di Laser (fornitori, disegni, fatture, ticket) |
| 22 | I limiti dell'autoverifica | T3·48 | 2 | **Collegare a D8:** il "doppio controllo" fatto dall'AI non è indipendente |
| 23 | Supervisione umana e verifica proporzionata | S1·83 | 1 | Tre livelli di verifica |
| 24 | Attività a basso e alto impatto | S1·87 | 1 | La matrice impatto e verificabilità: tornerà nella shortlist |
| 25 | Prima di usare un risultato AI: una checklist | T3·67 | 1 | Sei domande da portare a casa; si useranno dopo ogni demo |

**Se il tempo stringe:** saltare 17 e 20; ridurre l'esercizio 2 a un solo caso fatto insieme.
**Percorso B:** l'esercizio 1 si mostra con screenshot già preparati; l'esercizio 2 diventa un esempio guidato (il formatore legge la domanda orientata e mostra la versione neutra).

## 0:55 · Strumenti: che cosa c'è in Laser (15')

| # | Slide | Origine | Che cosa fare |
|---|---|---|---|
| 26 | Strumenti e richieste efficaci (titolo) | S1·61 adattata | |
| 27 | Modello, sistema, applicazione, piattaforma | T4·7 | Il motore e l'auto (richiamo del Tema 2) |
| 28 | Capacità del modello e funzionalità dell'applicazione | T4·25 | Perché lo stesso modello si comporta diversamente in prodotti diversi |
| 29 | L'AI nei software di produttività | T4·31 | Copilot dentro Outlook, Word, Excel, Teams |
| 30 | Copilot in Laser: che cosa c'è e che cosa no | Nuova (N14) | **Da completare con Laser prima della sessione:** quale Copilot, quali licenze, impostazioni sui dati |

**Contenuto sensibile al tempo:** ricontrollare T4 prima dell'edizione.

## 1:10 · Prompting essenziale (30')

| # | Slide | Origine | Che cosa fare |
|---|---|---|---|
| 31 | Prima il problema, poi il prompt | T6·12 | Si aggancia a "prima il problema, poi lo strumento" della sessione 1 |
| 32 | Otto elementi possibili | T6·13 | |
| 33 | Anatomia di una richiesta | T6·14 | |
| 34 | Zero-shot e few-shot | T6·25 | Esempio: dare due traduzioni già approvate come modello (spreco D5) |
| 35 | Il ciclo del miglioramento progressivo | T6·30 | |
| 36 | Uno schema per le richieste importanti | T6·55 | |
| 37 | Gara di prompt | Nuova (N15) | **Esercizio 3** (12-15'): stesso compito per tutti, prompt a coppie, il formatore ne prova 2-3 su Copilot |

**Percorso B:** il formatore mostra un prompt debole e la versione migliorata, poi lancia la versione migliorata dal vivo.

## 1:40 · Pausa (15')

Trascrivere nella board i bollini dell'apertura e gli esiti della caccia all'allucinazione.

## 1:55 · Assistenti per documenti e tre demo (40')

Prima delle demo, un richiamo verbale: solo materiali fittizi o non riservati, solo strumenti autorizzati. Dopo ogni demo: **"che cosa verifichereste prima di usarlo?"**, con la checklist della slide 25.

| # | Slide | Origine | Che cosa fare |
|---|---|---|---|
| 38 | Tre dimostrazioni (titolo) | S1·61 adattata | |
| 39 | Il filo conduttore: quattro modalità | T8·4 | Produrre, trasformare, analizzare, recuperare |
| 40 | Demo 1: dal manuale al knowledge assistant | Nuova (N16) | **Dal vivo.** Tema A degli sprechi (informazioni disperse). Trappola della coppia di serraggio: richiama la caccia all'allucinazione. Il contrasto sul filtro aria (prompt 2) è già emerso nella gara di prompt: usarlo come richiamo o saltarlo |
| 41 | Il recupero, in sintesi | T14·36 | |
| 42 | Tracciabilità: risalire alle fonti | T8·27 | |
| 43 | Demo 2: dalla richiesta del cliente alla bozza | Nuova (N17) | **Video.** Temi B e C (confronti, offerte). Trappola delle referenze inventate |
| 44 | Dal non strutturato al dato utilizzabile | T8·37 | Collegare a E1 ed E3 (ordini ed email con foto) |
| 45 | Demo 3: dai ticket alla sintesi operativa | Nuova (N18) | **Video.** Service (S1). Correlazione e causalità; ticket di sicurezza persi nella sintesi |
| 46 | Caricare non significa elaborare | T8·69 | |

Prompt, risposte attese e trappole: `materiali/guida_demo.md`. Esiti delle prove: `materiali/Registro_prove_demo.xlsx`.

## 2:35 · Agenti AI (10')

| # | Slide | Origine | Che cosa fare |
|---|---|---|---|
| 47 | Chatbot, assistenti, agenti, automazioni | T11·5 | |
| 48 | L'accumulo degli errori | T11·28 | Lega allucinazioni e agenti: un errore in un passaggio si propaga |
| 49 | Reversibili e irreversibili | T11·46 | |

## 2:45 · Dagli sprechi ai casi d'uso: processi, service, macchina (30')

| # | Slide | Origine | Che cosa fare |
|---|---|---|---|
| 50 | Dagli sprechi ai casi d'uso (titolo) | S1·61 adattata | |
| 51 | Compito e processo | T13·22 | |
| 52 | Un processo trasformato | T13·23 | |
| 53 | Colli di bottiglia | T12·26 | Velocizzare un'attività non serve se il collo di bottiglia è altrove (esempio: A1, l'attesa delle risposte dagli altri reparti) |
| 54 | Dai vostri sprechi ai casi d'uso | Nuova (N19) | I sei temi della mappa con i casi d'uso vicini e il luogo (ufficio, clienti, macchina) |
| 55 | AI nel service e nella macchina | Nuova (N21) | Troubleshooting, ricambi da foto, qualità visiva, anomalie, manutenzione predittiva |
| 56 | Anomalie e scostamenti | T9·38 | |
| 57 | Quattro condizioni distinte | T14·3 | Disponibilità, accessibilità, utilizzabilità, affidabilità |
| 58 | Dati abilitanti in Laser | Nuova (N22) | **Adattare** alla risposta sulla domanda d'indagine della sessione 1 (le macchine raccolgono dati?) |
| 59 | Dimostrazione, pilota, estensione | T16·43 | |

**Percorso B:** invariato (è già frontale).

## 3:15 · Esercizio: shortlist dei casi d'uso (25')

| # | Slide | Origine | Che cosa fare |
|---|---|---|---|
| 60 | Che cos'è un caso d'uso | T15·17 | |
| 61 | Gli elementi della descrizione | T15·18 | |
| 62 | Esercizio: dalla mappa alla shortlist | Nuova (N24) | **Esercizio 4** a gruppi misti: si parte dai temi con più bollini |

**Percorso B:** il formatore presenta 3 casi del portfolio collegati ai temi A, B e C (C10, C07, C11) e chiede all'aula di correggerli.

## 3:40 · Chiusura (5')

| # | Slide | Origine | Che cosa fare |
|---|---|---|---|
| 63 | Che cosa portiamo alla sessione 3 | Nuova (N25) | La shortlist va nella board (cornice 4); compito: stimare frequenza e tempo dei casi scelti |

---

## Prima della sessione

1. Chiedere a Laser quale Copilot è in uso e completare la slide 30.
2. Provare su Copilot l'esercizio 1 (caccia all'allucinazione) e la prova "Sei sicuro?" dell'esercizio 2; salvare gli screenshot per il percorso B.
3. Completare le prove delle demo nel registro; registrare i video delle demo 2 e 3.
4. Aggiornare la board AFFiNE come indicato nella sezione 5 della mappa sprechi.
5. Stampare: schede dell'esercizio 2 (una per coppia), griglia della shortlist (una per gruppo), bollini colorati.
6. Adattare la slide 58 se in sessione 1 è arrivata la risposta sui dati delle macchine.

## Materiali

- `mappa_sprechi_sessione1.md`: sprechi riordinati, temi trasversali, domande da fare.
- `sessione2_esercitazioni.md`: schede dei quattro esercizi e delle due mini-attività.
- `materiali/guida_demo.md` e materiali fittizi delle demo.
