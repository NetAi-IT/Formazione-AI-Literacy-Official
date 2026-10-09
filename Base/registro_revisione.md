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
