# Registro della revisione della base

Ogni modifica ai file di `Base/` è annotata qui. Le versioni precedenti sono conservate in `Base/_versioni_precedenti/` con la data nel nome.

---

## 9 ottobre 2026 · Tema 1 · Evoluzione e rilevanza dell'AI

**File modificati:** `Tema1_Evoluzione_e_rilevanza_AI.pptx` (da 55 a 59 slide), `sorgenti_slide.zip` (aggiornato `build.js`).
**Versioni precedenti:** `_versioni_precedenti/2026-10-09_Tema1_Evoluzione_e_rilevanza_AI.pptx`, `_versioni_precedenti/2026-10-09_sorgenti_slide.zip`.
**Tema grafico:** neutro (confermato dall'utente; brand NetAi non applicato).

### Correzioni di fatti (verificate sulle fonti primarie)
| Slide | Prima | Dopo | Fonte |
|---|---|---|---|
| Effetti potenziali (ora 39) | +14% in media, +34% meno esperti; NBER WP 2023; "oltre 5.000" operatori | +15% in media, +36% meno qualificati, nessun aumento per i più qualificati; 5.172 operatori; QJE 2025. Nota: i valori 14% e 34% sono della prima versione 2023 | Brynjolfsson, Li, Raymond, QJE 140(2), 889-942, 2025; arXiv 2304.11771v2 |
| I benefici non sono uguali per tutti (ora 49) | qualità "+40% (oltre)"; HBS WP 2023 | qualità +32% in media; -19 punti percentuali confermati (84,5% nel gruppo senza AI); Organization Science 2026 | Dell'Acqua et al., Organization Science 37(2), 403-423, 2026 |
| Le origini (ora 7) e linea del tempo (8) | "1956: ... propone un seminario"; "nasce il termine AI" | proposta del 31 agosto 1955, seminario nell'estate 1956; "nasce la disciplina" | Proposta di Dartmouth, AI Magazine |

### Correzioni minori
- Cicli di entusiasmo e disillusione (ora 10): asse del tempo a intervalli regolari di cinque anni (1955-2025), etichette dei due inverni riallineate; nota aggiornata.
- Disponibilità di dati (ora 18): precisato che la competizione 2012 usava un sottoinsieme di circa 1,2 milioni di immagini (slide e note).
- Modelli di grandi dimensioni (ora 20): etichette del grafico in formato numerico generale (175 e 1,5 secondo la lingua del sistema); fonte resa esplicita (Radford 2019; Brown 2020).
- Hype cycle (ora 45): nelle note aggiunto che Gartner nel 2025 colloca l'AI generativa nella fase di disillusione, da ricontrollare a ogni edizione.
- Fonti e riferimenti: divisa in due slide (1 di 2, 2 di 2), ordinate per sottotema. Aggiunti Rosenblatt 1958, Shortliffe 1976 (MYCIN), Rumelhart, Hinton e Williams 1986, Deng et al. 2009, Krizhevsky et al. 2012, Radford et al. 2019, Brown et al. 2020, Kaplan et al. 2020, Ouyang et al. 2022, Gartner 2025. Aggiornate le citazioni di Brynjolfsson e Dell'Acqua alle versioni pubblicate.

### Data di validità (attività C)
- Slide del titolo: "Contenuti aggiornati a ottobre 2026"; nota per il relatore sui dati da ricontrollare.
- Fonti (2 di 2): "Dati verificati a ottobre 2026: ricontrollarli prima di ogni edizione."

### Slide aggiunte (allineamento alla struttura standard, attività A5)
- **Il filo conduttore** (4): tecnologia, contesto, scelte, con i sottotemi collegati; le tre domande del modulo (possibile, affidabile, conveniente).
- **Davanti a una novità sull'AI: una scheda pratica** (55): sei domande con il rimando ai sottotemi.
- **Che cosa evitare** (56): sei semplificazioni, una per sottotema.
Tutte con note del relatore complete.

### Secondo intervento, stesso giorno: rimandi ad altri temi (punto 10)
Decisione dell'utente: i moduli possono essere presentati anche da soli o in selezione. Nuova regola 11 nelle istruzioni e mappa dei collegamenti (sezione 10).
- Testo proiettato: tolto "Approfondimento nel Tema 3" (slide 47, Maturità delle capacità); "i casi d'uso per funzione sono trattati in moduli dedicati" sostituito con "Esempi indicativi, a scopo illustrativo" (slide 36).
- Note del relatore: i rimandi generici ("modulo dedicato", "altri moduli", "moduli successivi") sostituiti con il tema preciso (Temi 5 e 6, 8-11, 12, 14, 15, 16, 17 e 18; Temi 3 e 7). Aggiunti nelle note i rimandi agli altri temi dove tornano Brynjolfsson (T12), Dell'Acqua (T3, T12), hype cycle (T16), Shadow AI (T16, T17, T18).
- Slide 57 "Prossimo passo: il Tema 2": mantenuta, dichiarata facoltativa nelle note.
- Versione intermedia della mattina non conservata separatamente: le differenze sono tutte descritte qui.

### Decisioni prese
- Punto 9 (esercizi): per ora nessun intervento. Nel Tema 1 restano le "Domande di verifica" nelle note; nei Temi 6-18 restano gli "Esercizio suggerito" nelle note.
- Punto 10 (rimandi): applicato come sopra.

### Ancora aperto
- Punto 11: decidere dove trattare per esteso Brynjolfsson, Dell'Acqua (T1, T3, T12) e hype cycle (T1, T16). Per ora nel Tema 1 restano come esempi brevi, con rimando nelle note.

### Riferimenti bibliografici citati a memoria, da verificare
Dati bibliografici di Rosenblatt 1958, Shortliffe 1976, Rumelhart et al. 1986, Deng et al. 2009, Krizhevsky et al. 2012, Radford et al. 2019, Brown et al. 2020, Kaplan et al. 2020, Ouyang et al. 2022 (citazioni canoniche, rischio basso).

### Controlli eseguiti
validate.py: All validations PASSED · trattini medi e lunghi: 0 (slide, note e sorgente) · render di tutte le 59 slide controllato a vista; dopo il secondo intervento, ricontrollate le slide 36 e 47 e verificato che nel testo proiettato non restino rimandi ad altri temi (salvo la slide facoltativa 57) · note presenti su tutte le slide (circa 8.500 parole, circa 61 minuti di esposizione).

---

## 9 ottobre 2026 · Tema 2 · Fondamenti e funzionamento dell'AI

**File modificati:** `Tema2_Fondamenti_e_funzionamento_AI.pptx` (da 69 a 72 slide), `sorgenti_slide.zip` (aggiornati `body2.js` e `build2.js`, con `build2.js` = `common2.js` + `body2.js`).
**Versioni precedenti:** `_versioni_precedenti/2026-10-09_Tema2_Fondamenti_e_funzionamento_AI.pptx`, `_versioni_precedenti/2026-10-09_sorgenti_slide_dopo_T1.zip`.
**Tema grafico:** neutro.

### Verifica delle fonti
- AI Act, art. 3: definizione di sistema di AI **non modificata** dal Digital Omnibus (Reg. UE 2026/1744). Verifica su fonte secondaria (regulation-ai.eu), da confermare sul testo in GUUE insieme alle verifiche del Tema 18. Aggiunto nelle note della slide 7 e nelle fonti.
- Confermati: OCSE 2023 (con memorandum esplicativo 2024), Weizenbaum 1966 (CACM 9(1), 36-45), Vaswani 2017, Brown 2020, Ouyang 2022, Lewis 2020.
- Liu et al., "Lost in the Middle": citato come pubblicato nel 2024, Transactions of the ACL 12, 157-173 (prima "2023 / TACL 2024"), nelle fonti e nelle note della finestra di contesto. **Da uniformare nei Temi 8 e 14.**
- Note della RAG: Patrick Lewis indicato come primo autore (FAIR, UCL, NYU), non come "chi guidava il gruppo".

### Correzioni grafiche
- La finestra di contesto (ora 43): la didascalia "Ciò che non entra nella finestra, per il modello non esiste" era attraversata dal bordo tratteggiato; spostata all'interno del riquadro.
- Che cosa osserviamo e che cosa possiamo concludere (ora 11): righe leggermente compattate, didascalia arancione staccata dal piè di pagina.

### Rimandi ad altri temi (regola 11)
- Concetto chiave 2.7 (ora 64): tolto dal testo proiettato "approfondita nel Tema 3"; il rimando è nelle note. Il testo si discosta così di poco dal concetto chiave del documento di perimetro.
- Note: rimandi generici resi precisi (Temi 5 e 6; Tema 14; Temi 14 e 17; Tema 4; Tema 6; Temi 5-11). Il vecchio "AI Act eventualmente approfondito in un modulo dedicato" ora rimanda al Tema 18.
- Prossimo passo: il Tema 3 (ora 71): mantenuta, dichiarata facoltativa nelle note.

### Data di validità
Titolo: "Contenuti aggiornati a ottobre 2026", con nota sui dati che cambiano (finestre di contesto, memoria, modelli recenti). Fonti: "Dati verificati a ottobre 2026".

### Slide aggiunte (struttura standard)
- **Il filo conduttore** (4): modello, dati, contesto, modalità d'uso, con i sottotemi; tre distinzioni del modulo (addestramento e inferenza, modello e applicazione, variabilità e correttezza).
- **Da dove viene questa risposta? Una scheda pratica** (69): sei domande con rimando ai sottotemi.
- **Che cosa evitare** (70): sei semplificazioni (2.1, 2.2, 2.3, 2.4, 2.5, 2.7); gli equivoci sulle fonti restano nella slide "Tre equivoci frequenti" del 2.6.

### Controlli eseguiti
validate.py: All validations PASSED · trattini medi e lunghi: 0 (slide, note e sorgente) · slide nuove e modificate controllate a vista · nel testo proiettato nessun rimando ad altri temi, salvo la slide facoltativa 71 · note su tutte le 72 slide (circa 10.900 parole, circa 78 minuti di esposizione).

---

## 9 ottobre 2026 · Tema 3 · Capacità, limiti e affidabilità dell'AI

**File modificati:** `Tema3_Capacita_limiti_affidabilita_AI.pptx` (da 68 a 70 slide), `sorgenti_slide.zip` (aggiornati `body3.js` e `build3.js`, con `build3.js` = `common3.js` + `helpers.js` + `body3.js`). Nessuna copia di backup: le versioni precedenti sono su GitHub.
**Tema grafico:** neutro.

### Verifica delle fonti
- Confermati: Mata v. Avianca (S.D.N.Y., sanzione del 22 giugno 2023); Kalai et al. 2025 (arXiv 2509.04664); Dastin, Reuters 2018; Doshi e Hauser, Science Advances 10(28), 2024; esempio sull'AI Act (art. 3, in vigore dal 1° agosto 2024).
- Sharma et al.: citato nella versione pubblicata, ICLR 2024 (prima "2023, Anthropic").
- Dell'Acqua et al.: versione pubblicata, Organization Science 37(2), 2026; ora nominato anche nelle note di "Prestazioni diverse in base al compito", che prima rimandava solo al Tema 1.
- Aggiunto Parasuraman e Manzey (2010), Human Factors 52(3), come fonte dell'automation bias (note di "Supervisione umana e verifica proporzionata" e fonti).

### Correzioni grafiche
- Sette fattori (ora 52): i quattro fattori "sotto il nostro controllo" ora hanno un bordo colorato, come la legenda; prima il colore era quasi indistinguibile da quello degli altri.

### Rimandi ad altri temi (regola 11)
- Testo proiettato: nessun rimando, salvo la slide facoltativa "Prossimo passo: il Tema 4" (ora 69), dichiarata tale nelle note.
- Note: rimandi generici resi precisi (Temi 5 e 6; Tema 6; Temi 12 e 15; Tema 15; Temi 17 e 18; Tema 17; Tema 18).

### Data di validità
Titolo: "Contenuti aggiornati a ottobre 2026", con nota sui dati che cambiano (ragionamento, allucinazioni, funzioni). Fonti: "Dati verificati a ottobre 2026".

### Slide aggiunte (struttura standard)
- **Il filo conduttore** (5): che cosa sa fare, dove può sbagliare, quanto è affidabile, quando usarla, con i sottotemi; tre cose da tenere distinte (capacità dimostrate, affidabilità effettiva, adeguatezza al compito).
- **Che cosa evitare** (68): sei semplificazioni (3.2, 3.3, 3.4, 3.5, 3.6, 3.8), cinque verso la fiducia eccessiva e una verso la sfiducia totale.
- La scheda pratica esisteva già: "Prima di usare un risultato AI: una checklist" (67).

### Controlli eseguiti
validate.py: All validations PASSED · trattini medi e lunghi: 0 (slide, note e sorgente) · slide nuove e modificate controllate a vista · note su tutte le 70 slide (circa 10.500 parole, circa 75 minuti di esposizione).

---

## 9 ottobre 2026 · Tema 4 · Ecosistema AI: modelli, strumenti e piattaforme

**File modificati:** `Tema4_Ecosistema_AI.pptx` (da 68 a 70 slide), `sorgenti_slide.zip` (aggiornati `body4.js` e `build4.js`, con `build4.js` = `common4.js` + `helpers.js` + `helpers4.js` + `body4.js`). Nessuna copia di backup: le versioni precedenti sono su GitHub.
**Tema grafico:** neutro.

### Attualità a ottobre 2026 (note del relatore)
- Copilot (note degli assistenti generalisti): non più "in larga parte modelli di OpenAI", ma modelli di più fornitori (OpenAI, Anthropic, Microsoft) con scelta automatica. Esempio aggiunto anche in "Più modelli, modelli che cambiano" (scelta del modello, disattivazione da parte degli amministratori) e in "Disponibilità delle funzionalità" (modelli Anthropic disattivati per impostazione predefinita per le organizzazioni europee). **Fonti secondarie: da verificare prima di ogni sessione.**
- Modelli open-weight (note di "Quattro famiglie" e "Modelli proprietari e modelli con pesi accessibili"): esempi aggiornati a Gemma (Google), Mistral, gpt-oss (OpenAI, agosto 2025), Qwen e DeepSeek; Meta indicata con il cambio di strategia verso modelli prevalentemente chiusi nel 2026. **Fonti secondarie: da verificare prima di ogni sessione.**
- "Che cosa cambia" (4.8): aggiunti i due esempi recenti nelle note.
- Confermati: Open Source AI Definition 1.0 dell'OSI (2024); i quattro assistenti citati e i loro fornitori.

### Rimandi ad altri temi (regola 11)
- Testo proiettato: nessun rimando, salvo la slide facoltativa "Prossimo passo: il Tema 5" (ora 69), dichiarata tale nelle note.
- Note: formule generiche ("area dell'adozione aziendale", "tema dedicato", "area sicurezza e normativa", "prossimi temi") rese precise (Temi 5 e 6; 7; 8-11; 11; 12; 13; 15; 16; 17; 18).

### Data di validità
Titolo: "Contenuti aggiornati a ottobre 2026". Slide "Nota sull'aggiornamento dei contenuti" (ora 70): "ultima verifica: ottobre 2026".

### Slide aggiunte (struttura standard)
- **Il filo conduttore** (4): struttura e modelli, prodotti e approcci, autonomia e accesso, scelta ed evoluzione, con i sottotemi; messaggio "sapersi orientare, non conoscere a memoria tutti i prodotti".
- **Che cosa evitare** (68): sei semplificazioni (4.1, 4.2, 4.3, 4.5, 4.6, 4.7).
- La scheda pratica esisteva già: "Prima di scegliere uno strumento AI: una checklist" (67).

### Controlli eseguiti
validate.py: All validations PASSED · trattini medi e lunghi: 0 (slide, note e sorgente) · slide nuove e modificate controllate a vista · note su tutte le 70 slide (circa 10.300 parole, circa 74 minuti di esposizione). Due didascalie (slide 45 e 70) sono vicine al piè di pagina ma leggibili: lasciate invariate.

---

## 9 ottobre 2026 · Tema 5 · Il dialogo uomo-AI

**File modificati:** `Tema5_Dialogo_uomo_AI.pptx` (da 61 a 63 slide), `sorgenti_slide.zip` (aggiornati `body5.js` e `build5.js`, con `build5.js` = `common5.js` + `helpers.js` + `helpers4.js` + `extra5.js` + `body5.js`). Nessuna copia di backup: le versioni precedenti sono su GitHub.
**Tema grafico:** neutro.

### Fonti
- Lee, H.-P. et al. (2025), CHI 2025: confermati esistenza, autori (Microsoft Research e Carnegie Mellon) e campione (319 lavoratori della conoscenza). Citazione completata con gli atti della conferenza; nelle note della slide fonti: dati autodichiarati, da presentare come indicazione; DOI 10.1145/3706598.3713778 **da verificare**.
- Weizenbaum (1966): citazione completata (titolo intero, pagine 36-45), uniforme al Tema 2.
- Parasuraman e Manzey (2010): confermata (già verificata nel Tema 3).
- Nessun dato numerico o fatto datato da aggiornare.

### Grafica
- "Responsabilità e controllo ai diversi livelli" (ora 41): etichette "Livelli 3/4/5" corrette in "Livello 3/4/5".
- Concetto chiave del 5.6 (ora 50): etichetta del sottotema allineata al titolo "La qualità dipende anche dalla persona".

### Rimandi ad altri temi (regola 11)
- Testo proiettato: tolti i rimandi ai Temi 4 e 6 nelle slide "Assistenza, collaborazione, delega, automazione" (39), "Obiettivi chiari e comprensione del problema" (46) e "Domande, interpretazione e feedback" (48). Resta solo la slide facoltativa "Prossimo passo: il Tema 6" (62), dichiarata tale nelle note.
- Note: formule generiche ("tema dedicato", "area aziendale") rese precise (Tema 11; Temi 13 e 16; Temi 13, 16 e 18).

### Data di validità
Titolo: "Contenuti aggiornati a ottobre 2026", con nota per il relatore. Slide fonti (63): "Fonti verificate a ottobre 2026: ricontrollarle prima di ogni edizione."

### Slide aggiunte (struttura standard)
- **Il filo conduttore** (4): interfaccia naturale, dialogo e ruoli, collaborazione e delega, persona e rischi, con i sottotemi; messaggio "la tecnologia amplifica le capacità umane senza sostituire giudizio, competenze e responsabilità".
- **Che cosa evitare** (61): sei errori tipici (5.1, 5.2, 5.3, 5.5, 5.6, 5.7).
- La scheda pratica esisteva già: "Principi per un dialogo consapevole" (60).

### Controlli eseguiti
validate.py: All validations PASSED · trattini medi e lunghi: 0 (slide, note e sorgente) · slide nuove e modificate controllate a vista · note su tutte le 63 slide (circa 9.000 parole, circa 64 minuti di esposizione).

---

## 9 ottobre 2026 · Tema 6 · Prompting e tecniche di interazione con l'AI

**File modificati:** `Tema6_Prompting_tecniche_interazione.pptx` (da 72 a 74 slide), `sorgenti_slide.zip` (aggiornati `body6.js` e `build6.js`, con `build6.js` = `common6.js` + `helpers.js` + `helpers4.js` + `extra5.js` + `body6.js`). Nessuna copia di backup: le versioni precedenti sono su GitHub.
**Tema grafico:** neutro.

### Fonti e attualità
- "Nota sulle fonti e sugli esempi" (ora 74): le guide dei fornitori citate per nome (Anthropic, Prompt engineering overview; OpenAI, Prompt engineering e Reasoning best practices; Google, Prompt design strategies per la Gemini API), con indirizzi nelle note.
- Modelli che ragionano prima di rispondere: aggiunto nelle note di "Scegliere la tecnica in base al compito" (ora 38) che conviene partire senza esempi e non chiedere di "ragionare passo passo"; la scomposizione resta utile per il controllo della persona. **Verificato su fonti secondarie: da confermare sulla guida ufficiale OpenAI.**
- Le altre indicazioni (delimitazione, few-shot, iterazione, formati strutturati) sono principi stabili, coerenti con le guide.

### Grafica
- "Template di prompt" (ora 64): "1. Partecipanti" e "2. Decisioni" su righe separate.
- "Gestire i limiti della finestra di contesto" (ora 29): icona di "Ripetere le istruzioni" distinta da quella di "Ricominciare".

### Rimandi ad altri temi (regola 11)
- Testo proiettato: tolti i rimandi nelle slide 13, 45, 65 e 71. Resta solo la slide facoltativa "Prossimo passo: il Tema 7" (73), dichiarata tale nelle note.
- Note: formule generiche ("area dedicata", "tema dedicato", "area delle applicazioni", "tema su assistenti e agenti") rese precise (Temi 14, 17 e 18; Tema 11; Temi 8-11).
- Note allineate alle slide: "integrazione B" riformulata (37); voce "apertura" tolta dalla struttura dell'email (49); "verbale di riunione" al posto di "sintesi delle riunioni" (64).

### Data di validità
Titolo: "Contenuti aggiornati a ottobre 2026", con nota per il relatore. Slide fonti (74): "Fonti verificate a ottobre 2026: ricontrollarle prima di ogni edizione."

### Slide aggiunte (struttura standard)
- **Il filo conduttore** (4): definire, contesto e tecnica, iterare e dare forma, applicare e riutilizzare, con i sottotemi; messaggio "un buon prompt aumenta le probabilità di un risultato utile, ma non ne garantisce la correttezza".
- **Che cosa evitare** (72): sei errori tipici (6.1, 6.2, 6.3, 6.5, 6.6, 6.8).
- La scheda pratica esisteva già: "Uno schema per le richieste importanti" (71).

### Controlli eseguiti
validate.py: All validations PASSED · trattini medi e lunghi: 0 (slide, note e sorgente) · slide nuove e modificate controllate a vista · note su tutte le 74 slide (circa 10.300 parole, circa 74 minuti di esposizione).

---

## 9 ottobre 2026 · Tema 7 · Verifica degli output e pensiero critico nell'utilizzo dell'AI

**File modificati:** `Tema7_Verifica_output_pensiero_critico.pptx` (da 73 a 74 slide), `sorgenti_slide.zip` (aggiornati `body7.js` e `build7.js`, con `build7.js` = `common7.js` + `helpers.js` + `helpers4.js` + `extra5.js` + `extra7.js` + `body7.js`). Nessuna copia di backup: le versioni precedenti sono su GitHub.
**Tema grafico:** neutro.

### Fonti
- Reber e Schwarz (1999): citazione confermata (Consciousness and Cognition, 8(3)); aggiunte le pagine 338-342, **indicate a memoria: da verificare**.
- Parasuraman e Manzey (2010): titolo completato ("An Attentional Integration") e pagine 381-410, **da verificare**.
- Sharma et al.: uniformato al Tema 3 (2024, ICLR 2024, Anthropic). Mata v. Avianca: uniformato al Tema 3 (giugno 2023).
- Esempi numerici dichiarati illustrativi; nessun dato datato da aggiornare.

### Grafica
- "Incertezza e livello di fiducia" (19): colonna delle descrizioni allargata, "Non verificati" ora su due righe.
- Etichette dei concetti chiave del 7.4 (37) e del 7.8 (68) allineate ai titoli dei sottotemi.

### Rimandi ad altri temi (regola 11)
- Testo proiettato: tolte le diciture "(richiamato dal Tema 3)" dalla slide fonti (74), spostate nelle note. Resta solo la slide facoltativa "Che cosa viene dopo" (73), dichiarata tale nelle note.
- Note: "ROI e obblighi giuridici" con rimando preciso (Temi 12 e 18).

### Data di validità
Titolo: "Contenuti aggiornati a ottobre 2026", con nota per il relatore. Slide fonti (74): "Fonti verificate a ottobre 2026: ricontrollarle prima di ogni edizione."

### Slide aggiunte (struttura standard)
- Il filo conduttore (4) e la scheda pratica (71) esistevano già.
- **Che cosa evitare** (72): sei errori tipici (7.2, 7.3, 7.5, 7.6, 7.7, 7.8).

### Controlli eseguiti
validate.py: All validations PASSED · trattini medi e lunghi: 0 (slide, note e sorgente) · slide nuove e modificate controllate a vista · note su tutte le 74 slide (circa 10.700 parole, circa 77 minuti di esposizione).

---

## 9 ottobre 2026 · Tema 8 · AI per testi, documenti e conoscenza

**File modificati:** `Tema8_AI_testi_documenti_conoscenza.pptx` (da 81 a 82 slide), `sorgenti_slide.zip` (aggiornati `body8a.js`, `body8b.js`, `body8c.js` e `build8.js`, con `build8.js` = `common8.js` + `helpers.js` + `helpers4.js` + `extra5.js` + `extra8.js` + `body8a.js` + `body8b.js` + `body8c.js`). Nessuna copia di backup: le versioni precedenti sono su GitHub.
**Tema grafico:** neutro.

### Fonti
- Liu et al. (2024): uniformato al Tema 2 (Transactions of the ACL, 12, 157-173).
- Lewis et al. (2020): confermato; la nota "(architettura RAG, solo accennata)" spostata dalla slide alle note.
- Nessun dato datato da aggiornare: il tema descrive capacità e limiti generali, senza prodotti.

### Rimandi ad altri temi (regola 11)
- Testo proiettato: tolti i rimandi nelle slide 28 (Tema 3), 54 e 57 (Tema 7), 63 (Temi 11 e 14), 71 (Tema 10) e 75 (Tema 7), sostituiti da frasi autonome; i rimandi precisi erano già nelle note. Resta solo la slide facoltativa "Che cosa viene dopo" (81), dichiarata tale nelle note.
- Tolte dalle slide 61 e 74 le etichette "Integrazione D" e "Integrazione C" del documento di perimetro.

### Coerenza
- Etichette dei concetti chiave dell'8.1, 8.2, 8.6 e 8.8 allineate ai titoli dei sottotemi.

### Data di validità
Titolo: "Contenuti aggiornati a ottobre 2026", con nota per il relatore. Slide fonti (82): "Fonti verificate a ottobre 2026: ricontrollarle prima di ogni edizione."

### Slide aggiunte (struttura standard)
- Il filo conduttore (4) e la scheda pratica (79) esistevano già.
- **Che cosa evitare** (80): sei errori tipici (8.2, 8.3, 8.4, 8.5, 8.7, 8.8).

### Controlli eseguiti
validate.py: All validations PASSED · trattini medi e lunghi: 0 (slide, note e sorgente) · slide nuove e modificate controllate a vista · note su tutte le 82 slide (circa 12.900 parole, circa 92 minuti di esposizione).

---

## 9 ottobre 2026 · Tema 9 · AI per dati e analisi

**File modificati:** `Tema9_AI_dati_analisi.pptx` (da 84 a 85 slide), `sorgenti_slide.zip` (aggiornati `body9a.js`, `body9b.js`, `body9c.js` e `build9.js`, con `build9.js` = `common9.js` + `helpers.js` + `helpers4.js` + `extra5.js` + `extra8.js` + `body9a.js` + `body9b.js` + `body9c.js`). Nessuna copia di backup: le versioni precedenti sono su GitHub.
**Tema grafico:** neutro.

### Fonti e grafici
- Anscombe (1973): confermato (The American Statistician, 27(1)); aggiunte le pagine 17-21. Grafico del quartetto (30) coerente con i dati originali (medie 9 e 7,5, correlazione 0,82, quarto insieme con dieci punti su x = 8 e uno isolato).
- Vigen (2015), Spurious Correlations, Hachette Books: confermato.
- Esempi numerici fittizi controllati per coerenza interna (media e mediana, numero di confronti, formula GIORNI.LAVORATIVI.TOT).

### Rimandi ad altri temi (regola 11)
- Testo proiettato: tolti i rimandi nelle slide 9 (Tema 14), 17 (Tema 8), 56 (Tema 2), 70 (area responsabilità e normativa) e 78 (Tema 7). Resta solo la slide facoltativa "Che cosa viene dopo" (84), dichiarata tale nelle note.
- Note: "area della responsabilità e della normativa" reso preciso (Temi 17 e 18).

### Coerenza
- Tolte dalle slide 13, 32, 42 e 77 le etichette "Integrazione A/B/C/D" del documento di perimetro; "esempio dal perimetro" (68) diventa "esempio fittizio".
- Etichette dei concetti chiave del 9.4, 9.5, 9.7 e 9.8 allineate ai titoli dei sottotemi.

### Data di validità
Titolo: "Contenuti aggiornati a ottobre 2026", con nota per il relatore. Slide fonti (85): "Fonti verificate a ottobre 2026: ricontrollarle prima di ogni edizione."

### Slide aggiunte (struttura standard)
- Il filo conduttore (4) e la scheda pratica (82) esistevano già.
- **Che cosa evitare** (83): sei errori tipici (9.2, 9.3, 9.4, 9.5, 9.6, 9.7).

### Controlli eseguiti
validate.py: All validations PASSED · trattini medi e lunghi: 0 (slide, note e sorgente) · slide nuove e modificate controllate a vista · note su tutte le 85 slide (circa 13.500 parole, circa 97 minuti di esposizione).

---

## 9 ottobre 2026 · Tema 10 · AI multimodale e creazione di contenuti

**File modificati:** `Tema10_AI_multimodale_contenuti.pptx` (da 74 a 75 slide), `sorgenti_slide.zip` (aggiornati `body10a.js`, `body10b.js`, `body10c.js` e `build10.js`, con `build10.js` = `common10.js` + `helpers.js` + `helpers4.js` + `extra5.js` + `extra8.js` + `body10a.js` + `body10b.js` + `body10c.js`). Nessuna copia di backup: le versioni precedenti sono su GitHub.
**Tema grafico:** neutro.

### Fonti e attualità
- Caso 2019 (azienda energetica britannica, circa 220.000 euro, Wall Street Journal) e caso 2024 (Arup, Hong Kong, circa 25 milioni di dollari, CNN e Financial Times): confermati.
- C2PA: "non ancora adottate ovunque" ancora corretto.
- **Aggiunto l'art. 50 dell'AI Act:** dal 2 agosto 2026 obbligo di dichiarare i deepfake per chi usa sistemi AI e di marcatura leggibile dalle macchine per i fornitori; per i sistemi già sul mercato la marcatura è rinviata al 2 dicembre 2026 (Reg. 2026/1744); codice di condotta sulla trasparenza finalizzato a giugno 2026. Riga proiettata nel banner di "Comunicazione fuorviante" (66), dettaglio nelle note, riferimento nella slide fonti. **Rinvio della marcatura e codice di condotta da fonti secondarie: da confermare sul testo ufficiale.** Coerente con il Tema 18 ("art. 50, dal 2 ago 2026").

### Rimandi ad altri temi (regola 11)
- Testo proiettato: tolti i rimandi nelle slide 20, 28 e 67 ("area responsabilità e normativa"), 23 (Tema 6), 55 (Tema 8) e 68 (Tema 7), sostituiti da frasi autonome. Resta solo la slide facoltativa "Che cosa viene dopo" (74), dichiarata tale nelle note.
- Note: sei rimandi generici ("area della responsabilità") resi precisi (Temi 17 e 18).

### Coerenza
- Tolte dalle slide 37, 56, 57 e 61 le etichette "Integrazione B/C" del documento di perimetro.
- Etichette dei concetti chiave del 10.6, 10.7 e 10.8 allineate ai titoli dei sottotemi.

### Data di validità
Titolo: "Contenuti aggiornati a ottobre 2026", con nota per il relatore. Slide fonti (75): "Fonti verificate a ottobre 2026: ricontrollarle prima di ogni edizione."

### Slide aggiunte (struttura standard)
- Il filo conduttore (4) e la scheda pratica (72) esistevano già.
- **Che cosa evitare** (73): sei errori tipici (10.2, 10.3, 10.4, 10.5, 10.6, 10.8).

### Controlli eseguiti
validate.py: All validations PASSED · trattini medi e lunghi: 0 (slide, note e sorgente) · slide nuove e modificate controllate a vista · note su tutte le 75 slide (circa 11.900 parole, circa 85 minuti di esposizione).

---

## 9 ottobre 2026 · Tema 11 · Assistenti, agenti e automazioni con l'AI

**File modificati:** `Tema11_Assistenti_agenti_automazioni.pptx` (77 slide, invariato), `sorgenti_slide.zip` (aggiornati `body11a.js`, `body11b.js`, `body11c.js` e `build11.js`, con `build11.js` = `common11.js` + `helpers.js` + `helpers4.js` + `extra5.js` + `extra8.js` + `charts11.js` + `body11a.js` + `body11b.js` + `body11c.js`). Nessuna copia di backup: le versioni precedenti sono su GitHub.
**Tema grafico:** neutro.

### Fonti e attualità
- Parasuraman, Sheridan e Wickens (2000): confermato; completati sezione della rivista (Part A: Systems and Humans) e pagine 286-297.
- **OWASP aggiornato:** Top 10 for LLM Applications 2026 (OWASP GenAI Security Project, settembre 2026): prompt injection al primo posto, eccesso di autonomia (Excessive Agency) al terzo. Citazione aggiornata nella slide fonti (77) e riferimento nelle note di "Istruzioni nascoste nei contenuti" (65). Esiste anche una Top 10 per le applicazioni agentiche.
- Nota per il relatore su MCP (Model Context Protocol) nelle note di "Modello e sistema con strumenti" (15): **citata a memoria, da verificare.**
- Calcolo dell'accumulo degli errori (28) verificato (0,95^10 ≈ 60%, 0,95^20 ≈ 36%, 0,99^20 ≈ 82%).

### Rimandi ad altri temi (regola 11)
- Testo proiettato: tolti i rimandi nelle slide 12 (Tema 4), 38, 69 e 75 ("area successiva"), 47 e 66 (Tema 7), 53 (Tema 15) e 61 ("area utilizzo responsabile"). Resta solo la slide facoltativa "Che cosa viene dopo" (76), dichiarata tale nelle note.
- Note: rimandi generici ("area successiva", "area dedicata all'utilizzo responsabile") resi precisi (Temi 12 e 15; 13; 13 e 16; 17; 17 e 18; 18).

### Coerenza
- Tolta dalla slide 37 l'etichetta "Integrazione C".
- Etichette dei concetti chiave dell'11.1, 11.2, 11.4, 11.6 e 11.8 allineate ai titoli dei sottotemi.

### Data di validità
Titolo: "Contenuti aggiornati a ottobre 2026", con nota per il relatore. Slide fonti (77): "Fonti verificate a ottobre 2026: ricontrollarle prima di ogni edizione."

### Struttura
- Il filo conduttore (4) e la scheda pratica (74) esistevano già.
- **Che cosa evitare** (75): portata dal formato a quattro voci al formato standard a sei voci con il sottotema (11.1, 11.2, 11.5, 11.6, 11.7, 11.8); le quattro semplificazioni del documento di perimetro sono conservate.

### Controlli eseguiti
validate.py: All validations PASSED · trattini medi e lunghi: 0 (slide, note e sorgente) · slide modificate controllate a vista · note su tutte le 77 slide (circa 12.700 parole, circa 90 minuti di esposizione).

---

## 9 ottobre 2026 · Tema 12 · AI e creazione di valore per l'azienda

**File modificati:** `Tema12_AI_creazione_valore_azienda.pptx` (72 slide, invariato), `sorgenti_slide.zip` (aggiornati `body12a.js`, `body12b.js`, `body12c.js` e `build12.js`, con `build12.js` = `common12.js` + `helpers.js` + `helpers4.js` + `extra5.js` + `extra8.js` + `charts11.js` + `helpers12.js` + `body12a.js` + `body12b.js` + `body12c.js`). Nota tecnica: il `build12.js` precedente conteneva una versione più vecchia di `helpers12.js` (la funzione `rowsLabel` senza i parametri x e w); la versione attuale è compatibile e produce lo stesso risultato. Nessuna copia di backup: le versioni precedenti sono su GitHub.
**Tema grafico:** neutro.

### Fonti e attualità
- **Studi di produttività aggiornati alle versioni pubblicate**, come nel Tema 1: Brynjolfsson, Li e Raymond, The Quarterly Journal of Economics, 140(2), 889-942, 2025 (5.172 operatori, +15%, +36% per i meno esperti); Dell'Acqua et al., Organization Science, 37(2), 403-423, 2026 (758 consulenti, +12,2% compiti, +25,1% velocità, +32% qualità; -19 punti sul compito fuori frontiera). Aggiornati slide "Che cosa dicono alcuni studi" (28), note e fonti; nelle note la precisazione sui valori delle versioni 2023.
- Solow (1987): confermato; aggiunta la pagina 36, **citata a memoria: da verificare**. Goldratt e Cox (1984): aggiunto l'editore (North River Press).
- Calcoli degli esempi controllati: risparmio apparente ed effettivo (23), collo di bottiglia -67% e -25% (26), beneficio lordo e netto 100 e 35 (55).
- **Punto 11 (studi di produttività):** deciso; introdotti nel Tema 1, richiamati nel Tema 3, approfonditi nel Tema 12, con gli stessi dati. Hype cycle ancora aperto (Temi 1 e 16).

### Rimandi ad altri temi (regola 11)
- Testo proiettato: tolti i rimandi nelle slide 6 (Tema 15), 25 (Tema 13), 48 (Tema 15), 54 (Temi 13 e 14) e 63 (Tema 15). Resta solo la slide facoltativa "Che cosa viene dopo" (71), dichiarata tale nelle note. I rimandi nelle note erano già precisi.

### Coerenza
- Tolte dalle slide 24, 39 e 52 le etichette "Integrazione A/B/C"; nella slide 26 "numeri inventati, dal documento" diventa "esempio fittizio".
- Etichette dei concetti chiave del 12.2, 12.5, 12.6 e 12.7 allineate ai titoli dei sottotemi.

### Data di validità
Titolo: "Contenuti aggiornati a ottobre 2026", con nota per il relatore. Slide fonti (72): "Fonti verificate a ottobre 2026: ricontrollarle prima di ogni edizione."

### Struttura
- Il filo conduttore (5) e la scheda pratica "Domande sul valore" (69) esistevano già.
- **Che cosa evitare** (70): portata dal formato a quattro voci al formato standard a sei voci con il sottotema (12.1, 12.3, 12.3, 12.4, 12.6, 12.7); le quattro avvertenze del documento di perimetro sono conservate.

### Controlli eseguiti
validate.py: All validations PASSED · trattini medi e lunghi: 0 (slide, note e sorgente) · titoli delle slide invariati · slide modificate controllate a vista · note su tutte le 72 slide (circa 11.500 parole, circa 82 minuti di esposizione).

---

## 9 ottobre 2026 · Tema 13 · AI e trasformazione del lavoro e dei processi

**File modificati:** `Tema13_AI_trasformazione_lavoro_processi.pptx` (da 63 a 64 slide), `sorgenti_slide.zip` (aggiornati `body13a.js`, `body13b.js`, `body13c.js` e `build13.js`, con `build13.js` = `common13.js` + `helpers.js` + `helpers4.js` + `extra5.js` + `extra8.js` + `charts11.js` + `helpers12.js` + `body13a.js` + `body13b.js` + `body13c.js`). Come per il Tema 12, il `build13.js` precedente conteneva la versione più vecchia di `helpers12.js`; la versione attuale è compatibile. Nessuna copia di backup: le versioni precedenti sono su GitHub.
**Tema grafico:** neutro.

### Fonti
- Eloundou et al.: citato nella versione pubblicata su Science, 384(6702), 1306-1308, 2024, con il rimando all'analisi completa (arXiv:2303.10130, 2023), da cui vengono le stime dell'80% e del 19%. **Da verificare se la sintesi su Science riporta gli stessi valori.**
- Bessen (2015): confermato, cautele sull'esempio dei bancomat corrette. Autor, Levy e Murnane (2003): aggiunte le pagine 1279-1333.

### Rimandi ad altri temi (regola 11)
- Testo proiettato: tolti i rimandi nelle slide 10 (Tema 11), 18 (Tema 14), 19 (Tema 15), 44 e 54 (Tema 16), 57 (Temi 12 e 16). Slide "Le competenze per lavorare con l'AI" (48): i numeri dei temi sotto ogni competenza sostituiti da brevi descrizioni; la corrispondenza con i temi resta nelle note. Resta solo la slide facoltativa "Che cosa viene dopo" (63), dichiarata tale nelle note.

### Coerenza
- Slide 23: "Esempio dal documento di perimetro" diventa "Esempio fittizio"; slide 51: tolta l'etichetta "Integrazione C"; slide 56: tolto il rimando "(B)".
- Etichette dei concetti chiave del 13.2, 13.3, 13.4, 13.5, 13.7 e 13.8 allineate ai titoli dei sottotemi.

### Data di validità
Titolo: "Contenuti aggiornati a ottobre 2026", con nota per il relatore. Slide fonti (64): "Fonti verificate a ottobre 2026: ricontrollarle prima di ogni edizione."

### Slide aggiunte (struttura standard)
- Il filo conduttore (5) e la scheda pratica (61) esistevano già.
- **Che cosa evitare** (62): sei semplificazioni (13.1, 13.1, 13.3, 13.6, 13.7, 13.8).

### Controlli eseguiti
validate.py: All validations PASSED · trattini medi e lunghi: 0 (slide, note e sorgente) · slide nuove e modificate controllate a vista · note su tutte le 64 slide (circa 10.400 parole, circa 74 minuti di esposizione).

---

## 9 ottobre 2026 · Tema 14 · AI, dati e conoscenza aziendale

**File modificati:** `Tema14_AI_dati_conoscenza_aziendale.pptx` (78 slide, numero invariato), `sorgenti_slide.zip` (aggiornati `body14a.js`, `body14b.js`, `body14c.js` e `build14.js`, con `build14.js` = `common14.js` + `helpers.js` + `helpers4.js` + `extra5.js` + `extra8.js` + `charts11.js` + `helpers12.js` + `body14a.js` + `body14b.js` + `body14c.js`). Nessuna copia di backup: le versioni precedenti sono su GitHub.
**Tema grafico:** neutro.

### Fonti
- Liu et al. uniformato: Transactions of the ACL, 12, 157-173. La citazione è ora uguale in tutto il percorso.
- Lewis et al.: aggiunti volume e pagine, Advances in NeurIPS, 33, 9459-9474. Saltzer e Schroeder: aggiunte le pagine, 1278-1308.
- Polanyi: prima edizione Doubleday 1966, con la ristampa University of Chicago Press 2009. Nonaka e Takeuchi confermato.
- **Da verificare:** pagine di Lewis e di Saltzer e Schroeder, edizione di Polanyi (riferimenti citati a memoria).

### Rimandi ad altri temi (regola 11)
- Testo proiettato: tolti i rimandi nelle slide 9 (Tema 8), 31 (Tema 13), 34 (Tema 3), 35 (Tema 8), 45 (Tema 11), 50 (Temi 17 e 18), 64 e 65 (Tema 7). Le note contenevano già i riferimenti precisi. Resta solo la slide facoltativa "Che cosa viene dopo" (77), dichiarata tale nelle note.

### Coerenza
- Tolte le lettere (A), (B), (C), (D) dal testo proiettato delle slide 11, 14, 23, 28, 29, 40, 47, 52, 64 e 71; restano nelle note.
- Filo conduttore (5): "Quattro integrazioni trasversali" diventa "Quattro precisazioni trasversali", senza lettere, come nei Temi 12 e 13.
- Etichette dei concetti chiave (15, 24, 32, 41, 48, 57, 66, 72): tolti i suffissi "Integrazione" e allineati i nomi ai titoli dei divisori; allineati anche tre titoli della slide 6 (14.4, 14.6, 14.8).
- Slide 64: il grafico a torta con percentuali inventate è sostituito da un elenco senza numeri delle cause tipiche di risposte inadeguate, per evitare che venga citato come dato reale.

### Data di validità
Titolo: "Contenuti aggiornati a ottobre 2026", con nota per il relatore. Slide fonti (78): "Fonti verificate a ottobre 2026: ricontrollarle prima di ogni edizione."

### Struttura
- Il filo conduttore (5) e la scheda pratica "Domande su un assistente aziendale" (75) esistevano già.
- **Che cosa evitare** (76): portata dall'elenco semplice a sette righe al formato standard a sei voci con il sottotema (14.1, 14.4, 14.2, 14.6, 14.7, 14.8); la conoscenza tacita è ricordata nelle note.

### Controlli eseguiti
validate.py: All validations PASSED · trattini medi e lunghi: 0 (slide, note e sorgente) · titoli delle slide invariati · slide modificate controllate a vista · note su tutte le 78 slide (circa 12.200 parole, circa 87 minuti di esposizione).

---

## 9 ottobre 2026 · Tema 2 · correzione della slide 63

**File modificati:** `Tema2_Fondamenti_e_funzionamento_AI.pptx` (72 slide, numero invariato), `sorgenti_slide.zip` (aggiornati `body2.js` e `build2.js`, con `build2.js` = `common2.js` + `body2.js`).

- **Slide 63, "Variabilità non significa errore":** la nota citava i titoli della newsletter come se fossero sulla slide, mentre sono nella slide 58. Ogni quadrante ha ora un esempio fittizio in corsivo (tre titoli per la newsletter; la stessa categoria per lo stesso ticket; tre date diverse per la stessa scadenza; un prezzo superato ripetuto ogni volta). La nota descrive i quattro esempi e rimanda esplicitamente alla slide 58.
- **Slide 24:** il titolo "Individuare schemi e regolarità (es. Spam)", modificato a mano nel file, è stato riportato nel sorgente, così non si perde nelle prossime ricostruzioni.

### Controlli eseguiti
validate.py: All validations PASSED · trattini medi e lunghi: 0 · confronto con il file precedente: cambia solo la slide 63 · slide 63 controllata a vista.
