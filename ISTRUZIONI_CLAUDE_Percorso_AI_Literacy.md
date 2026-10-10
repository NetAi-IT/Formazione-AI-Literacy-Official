# Istruzioni per Claude · Percorso di formazione AI Literacy

> **Leggi questo file per intero prima di lavorare sul percorso.** Riassume il lavoro fatto nella conversazione di produzione delle slide (8 e 9 ottobre 2026), le regole da rispettare, le attività che restano per la revisione dell'intero percorso e, nella sezione 9, l'indice completo degli argomenti delle slide; nella sezione 10, la mappa dei collegamenti tra temi.

Ultimo aggiornamento: 9 ottobre 2026 (revisione dei Temi 1-4, area "Comprendere l'AI", completata; revisione dei Temi 5-7, area "Interagire con l'AI", completata; revisione dei Temi 8-11, area "Esplorare le possibilità dell'AI", completata; revisione dei Temi 12-16, area "Comprendere il valore per l'azienda", completata; revisione dei Temi 17 e 18, area "Utilizzare l'AI responsabilmente", completata: revisione dei 18 temi conclusa; regola sui rimandi e mappa dei collegamenti, sezione 10; indice degli argomenti; base indipendente da singole formazioni; nuova struttura con le cartelle `Base/` e `Formazioni/`; cartella di lavoro spostata in `Formazione AI Literacy Official`; correzione della slide 28 del Tema 18 sulle macchine dopo il Digital Omnibus; cartella `Normative/` con i testi ufficiali; prima formazione derivata: Laser Srl).

---

## 1. Contesto

- **Utente:** formazione@netai.it. Progetto Claude: "Formazione AI Literacy".
- **Obiettivo:** una **base di contenuti completa** sull'AI Literacy, livello AI Awareness, per personale e management con diversi livelli di familiarità con l'AI.
  - Non è una singola formazione: è la libreria da cui derivare **future formazioni**, di durata, pubblico e formato diversi.
  - Ogni formazione specifica si costruisce selezionando e adattando questi contenuti (vedi attività D e l'indice nella sezione 9).
- **Cartella di lavoro:** `/Users/michelebarchi/Claude/Projects/Formazione AI Literacy Official` (attenzione a maiuscole e spazi nel nome).
  - Nelle sessioni collegate al computer è montata come `$HOME/mnt/Formazione AI Literacy Official`. Se non compare tra le cartelle collegate, chiederne l'accesso con `device_request_folder_access`.
  - **La vecchia cartella `/Users/michelebarchi/Claude/Projects/Formazione Ai literacy` è obsoleta:** non leggere né scrivere lì. Contiene ancora una copia dei file, che l'utente può eliminare.
  - **La cartella è un repository git locale:** contiene `.git` e `.gitattributes`, un commit iniziale e nessun remote configurato. Al 9 ottobre 2026 `Base/` e questo file non erano ancora sotto versione.
    - Non eseguire commit, push o altre operazioni git senza richiesta esplicita dell'utente.
    - **Le versioni precedenti le gestisce l'utente su GitHub, manualmente** (decisione del 9 ottobre 2026). Non creare copie di backup dei file e non usare cartelle come `_versioni_precedenti/`.
    - Nella shell sul computer dell'utente la cancellazione di file è disattivata finché l'utente non la autorizza. Per questo alcune operazioni git (commit, checkout, merge) possono lasciare file `.lock` o fallire. In quel caso chiedere il permesso di cancellazione per questa cartella.
  - **Nel progetto Claude** "Formazione AI Literacy" esiste una copia dei file sotto `Formazione AI Literacy Official/...`. La fonte di riferimento per lavorare resta la cartella sul computer; la copia del progetto serve alla consultazione da altre conversazioni.
- **Struttura della cartella** (riorganizzata il 9 ottobre 2026):
  ```
  Formazione AI Literacy Official/
  ├── ISTRUZIONI_CLAUDE_Percorso_AI_Literacy.md   (questo file)
  ├── Base/                                       (la base di contenuti)
  │   ├── tema_01_...md … tema_18_...md           18 documenti di perimetro
  │   ├── Tema1_...pptx … Tema18_...pptx          18 presentazioni complete
  │   └── sorgenti_slide.zip                      sorgenti per rigenerare i deck
  ├── Normative/                                  testi normativi ufficiali (PDF)
  │   └── AIAct/                                  Reg. (UE) 2024/1689 e Reg. (UE) 2026/1744, testo italiano GUUE
  └── Formazioni/                                 una sottocartella per ciascuna formazione
      └── 2026-10_LaserSrl_AI_Adoption/           Laser Srl, 3 sessioni da 4 ore (in progettazione)
  ```
  - La cartella `Normative/` contiene i testi ufficiali aggiunti dall'utente: usarli come fonte primaria per le verifiche normative (estrazione con `pdftotext -layout`). Non si modifica.
  - I **18 documenti di perimetro** sono la fonte primaria dei contenuti, già "consolidati" dall'utente.
  - Le **18 presentazioni** sono una per tema, prodotte nella conversazione di produzione.
  - `sorgenti_slide.zip` contiene i sorgenti JavaScript (vedi sezione 6).
- **Regole di organizzazione dei file:**
  1. **La cartella `Base/` non si modifica**, salvo una revisione della base richiesta esplicitamente dall'utente (attività A, B, C, E, F della sezione 5).
     - In quel caso si sovrascrive direttamente il file: le versioni precedenti sono su GitHub, gestite dall'utente.
     - Annotare ogni modifica in `Base/registro_revisione.md`.
  2. **Ogni nuova formazione ha una sottocartella propria** in `Formazioni/`, con un nome breve e la data, per esempio `Formazioni/2026-11_Management_AI_Awareness/`. Contiene:
     - `scheda_formazione.md`: committente, pubblico, obiettivi, durata, formato, date, brand;
     - `agenda.md`: blocchi, tempi, slide e temi usati, esercizi;
     - i deck e i materiali prodotti per quella formazione (dispense, esercizi, checklist);
     - `note_scelte.md`: che cosa è stato preso dalla base, che cosa adattato e perché.
  3. I file delle formazioni si creano come **nuovi file**: si copiano o si selezionano contenuti dalla base, senza spostare né rinominare i file di `Base/`.
  4. Questo file di istruzioni resta nella cartella principale. Va aggiornato quando cambia la struttura o la base. Dopo ogni modifica, aggiornare anche la copia nei documenti del progetto Claude: `Formazione AI Literacy Official/ISTRUZIONI_CLAUDE_Percorso_AI_Literacy.md`.
- **Stato:** tutte le 18 presentazioni sono state prodotte e consegnate. **Revisione tema per tema in corso:** Temi 1-4 (area "Comprendere l'AI") revisionati il 9 ottobre 2026 (fatti verificati, fonti complete, data di validità, aggiunte le slide filo conduttore, scheda pratica e Che cosa evitare; tema neutro confermato). Dettagli e punti rimasti aperti in `Base/registro_revisione.md`. **Il passo successivo, indicato dai documenti di perimetro, è la revisione trasversale dei 18 temi.** Dopo la revisione, la base potrà essere usata per progettare formazioni specifiche.

---

## 2. Preferenze e regole vincolanti

1. **Mai usare il trattino medio (carattere Unicode U+2013, "en dash") nei testi generati. Evitare anche il trattino lungo (U+2014, "em dash").** Il trattino normale "-" è ammesso.
   - Vale per slide, note, documenti e risposte in chat.
   - Al loro posto usare due punti, virgole, punti, "·" o parentesi.
   - Dopo ogni generazione, controllare il testo estratto con `python3 -c "import sys;t=open(sys.argv[1]).read();print(t.count('\\u2013')+t.count('\\u2014'))" t.md`: il risultato deve essere 0.
2. **Brand NetAi:** se non è indicato esplicitamente, chiedere sempre se applicarlo ai documenti.
   - Per i 18 deck l'utente ha scelto un **tema neutro, non NetAi**.
   - Va ancora deciso se applicare il brand alla versione finale (vedi attività F).
3. **Lingua:** italiano, per le slide, le note e le risposte all'utente.
4. **Contenuti completi, senza vincoli di tempo:** ogni deck copre il documento di perimetro per intero.
   - Questo vale per la fase di produzione.
   - La riduzione per l'aula è un'attività separata (vedi attività D).
5. **Note del relatore complete su ogni slide**, in forma di testo parlato e continuo.
6. **Esercizi rimandati** (decisione del 9 ottobre 2026: per ora nessun intervento, né aggiunte né rimozioni; nelle slide proiettate non vanno esercizi): nelle note compare solo un suggerimento "Esercizio suggerito: ..." nella slide chiave di ogni sottotema. Gli esercizi veri vanno sviluppati in seguito (vedi attività E).
7. **Esempi aziendali sempre fittizi e dichiarati come tali.** Nessun dato riservato. I casi reali citati, come Mata v. Avianca, Arup o Amazon, sono indicati con la loro fonte.
8. **Riferimenti citati a memoria:** vanno segnalati all'utente come "da verificare".
9. **Temi normativi:** precisare sempre che non si tratta di un parere legale. Verificare le date sulle fonti ufficiali e non presentare mai una data unica come scadenza universale.
11. **Rimandi ad altri temi** (decisione del 9 ottobre 2026; i moduli possono essere presentati anche da soli o in selezione):
    - **mai nel testo proiettato** delle slide (niente "Approfondimento nel Tema N", "trattato in moduli dedicati");
    - **precisi nelle note del relatore**: indicare il tema, ed eventualmente il sottotema, invece di formule generiche come "modulo dedicato";
    - la slide finale "Prossimo passo" o "Che cosa viene dopo" resta, dichiarata nelle note come **facoltativa**;
    - i collegamenti tra temi sono registrati nella **mappa della sezione 10**, che l'agente usa per i controlli di prerequisiti, ripetizioni e passaggi e per costruire le formazioni derivate.
10. **Struttura delle risposte all'utente dopo ogni consegna:**
    - una riga su che cosa è stato consegnato;
    - la struttura in breve e i punti notevoli;
    - le fonti da verificare;
    - la proposta del passo successivo.

---

## 3. Inventario del percorso

### 3.1 Aree e temi

Le aree vanno tenute con questi nomi in tutti i deck.

| # | Area | Tema | File PPTX | Slide |
|---|---|---|---|---|
| 1 | Comprendere l'AI | Evoluzione e rilevanza dell'AI | Tema1_Evoluzione_e_rilevanza_AI.pptx | 59 |
| 2 | Comprendere l'AI | Fondamenti e funzionamento | Tema2_Fondamenti_e_funzionamento_AI.pptx | 72 |
| 3 | Comprendere l'AI | Capacità, limiti, affidabilità | Tema3_Capacita_limiti_affidabilita_AI.pptx | 70 |
| 4 | Comprendere l'AI | Ecosistema AI | Tema4_Ecosistema_AI.pptx | 70 |
| 5 | Interagire con l'AI | Dialogo uomo e AI | Tema5_Dialogo_uomo_AI.pptx | 63 |
| 6 | Interagire con l'AI | Prompting e tecniche di interazione | Tema6_Prompting_tecniche_interazione.pptx | 74 |
| 7 | Interagire con l'AI | Verifica degli output e pensiero critico | Tema7_Verifica_output_pensiero_critico.pptx | 74 |
| 8 | Esplorare le possibilità | Testi, documenti, conoscenza | Tema8_AI_testi_documenti_conoscenza.pptx | 82 |
| 9 | Esplorare le possibilità | Dati e analisi | Tema9_AI_dati_analisi.pptx | 85 |
| 10 | Esplorare le possibilità | AI multimodale e contenuti | Tema10_AI_multimodale_contenuti.pptx | 75 |
| 11 | Esplorare le possibilità | Assistenti, agenti, automazioni | Tema11_Assistenti_agenti_automazioni.pptx | 77 |
| 12 | Valore per l'azienda | Creazione di valore | Tema12_AI_creazione_valore_azienda.pptx | 72 |
| 13 | Valore per l'azienda | Trasformazione del lavoro e dei processi | Tema13_AI_trasformazione_lavoro_processi.pptx | 64 |
| 14 | Valore per l'azienda | Dati e conoscenza aziendale | Tema14_AI_dati_conoscenza_aziendale.pptx | 78 |
| 15 | Valore per l'azienda | Opportunità e valutazione | Tema15_Opportunita_valutazione_AI.pptx | 76 |
| 16 | Valore per l'azienda | Adozione e cambiamento organizzativo | Tema16_Adozione_AI_cambiamento_organizzativo.pptx | 76 |
| 17 | Uso responsabile | Rischi, sicurezza, tutela delle informazioni | Tema17_Utilizzo_responsabile_rischi_sicurezza.pptx | 75 |
| 18 | Uso responsabile | Normativa, regole e governance | Tema18_Normativa_regole_governance_AI.pptx | 77 |

**Totale: circa 1.300 slide.** L'indice dettagliato di tutti gli argomenti è nella sezione 9.

Nomi completi delle aree: "Comprendere l'AI" (1-4), "Interagire con l'AI" (5-7), "Esplorare le possibilità dell'AI" (8-11), "Comprendere il valore per l'azienda" (12-16), "Utilizzare l'AI responsabilmente" (17-18).

### 3.2 Struttura standard di un deck

I Temi 1-7 sono un po' più semplici; la struttura si è stabilizzata dal Tema 8.

**Introduzione**
- Titolo: master TITOLO, con kicker "PERCORSO AI LITERACY · TEMA N", titolo e area.
- Obiettivo del modulo: due card, "Che cosa vogliamo sviluppare" e "Quale consapevolezza".
- Eventuale slide di inquadramento propria del documento (per esempio le quattro condizioni nel T14, i tre piani nel T18).
- Domande guida.
- Il filo conduttore: dimensioni e integrazioni.
- Il percorso del modulo, con le priorità.
- Eventuale scenario guida del documento.

**Per ogni sottotema**
- Sezione e slide divisore (numero, titolo, sottotitolo).
- Da 5 a 9 slide di contenuto.
- Slide chiave (master CHIAVE) con il concetto chiave e l'"Esercizio suggerito" nelle note.
- Dal Tema 8 in poi, un indicatore a pillole in alto a destra mostra la dimensione corrente. I nomi variano per tema:
  - T8 `modeTag`, T9 `phaseTag`, T10 `opTag`, T11 `areaTag`, T12 `valTag`, T13 `workTag`;
  - T14 `infoTag` (5 pillole), T15 `stepTag`, T16 `adTag`;
  - T17 `riskTag` (6 pillole), T18 `govTag` (6 pillole).

**Conclusioni**
- Le domande guida con le nostre risposte.
- Che cosa portiamo a casa: i risultati attesi.
- Una scheda pratica.
- Eventuale slide "Che cosa evitare".
- Che cosa viene dopo: due pannelli, PERCORSO e PROSSIMO TEMA.
- Fonti e riferimenti.

---

## 4. Contenuti e decisioni notevoli per tema

Servono per non perdere il filo nella revisione.

**Temi 1-6**

| Tema | Elementi notevoli |
|---|---|
| T1 | Storia (Turing, Dartmouth), transformer, crescita del calcolo (Epoch AI), studi di produttività (Brynjolfsson QJE 2025: +15%, +36%; Dell'Acqua Organization Science 2026: +12,2%, +25,1%, +32%, -19 punti), hype cycle (Gartner 2025: GenAI in disillusione). **Revisionato il 9 ottobre 2026** |
| T2 | **Revisionato il 9 ottobre 2026.** Definizione AI Act (art. 3, non modificato dal Digital Omnibus) e OCSE, ELIZA, transformer, RLHF (Ouyang 2022), RAG (Lewis 2020), "Lost in the Middle" (Liu 2024, TACL 12) |
| T3 | **Revisionato il 9 ottobre 2026.** Allucinazioni (Mata v. Avianca, Kalai 2025), piaggeria (Sharma, ICLR 2024), bias (caso Amazon), frontiera irregolare. Esempio didattico di frase vera e falsa sull'AI Act |
| T4 | Ecosistema di prodotti e fornitori. **Contenuto molto sensibile al tempo.** **Revisionato il 9 ottobre 2026:** Copilot multi-modello (OpenAI, Anthropic, Microsoft); esempi open-weight aggiornati (Gemma, Mistral, gpt-oss, Qwen, DeepSeek; Meta verso modelli chiusi) |
| T5 | ELIZA, automation bias (Parasuraman e Manzey 2010), Lee et al. 2025 sul pensiero critico. **Revisionato il 9 ottobre 2026:** nessun dato da aggiornare; tolti i rimandi proiettati ai Temi 4 e 6; aggiunte "Il filo conduttore" e "Che cosa evitare" |
| T6 | Tecniche di prompting. **Revisionato il 9 ottobre 2026:** nota sui modelli che ragionano prima di rispondere (note di "Scegliere la tecnica in base al compito"); guide dei fornitori citate per nome nella slide finale; tolti i rimandi proiettati al Tema 7; aggiunte "Il filo conduttore" e "Che cosa evitare" |

**Temi 7-12**

| Tema | Elementi notevoli |
|---|---|
| T7 | Fluidità e verità (Reber e Schwarz 1999), proporzionalità della verifica. "Che cosa viene dopo" aggiornato al Tema 8. **Revisionato il 9 ottobre 2026:** fonti uniformate al Tema 3 (Sharma ICLR 2024, Avianca giugno 2023); tolti i rimandi proiettati al Tema 3; aggiunta "Che cosa evitare" |
| T8 | Uso dell'AI su documenti, RAG solo accennato. **Revisionato il 9 ottobre 2026:** Liu uniformato al Tema 2; tolti sei rimandi proiettati ad altri temi e le etichette "Integrazione C/D"; aggiunta "Che cosa evitare" |
| T9 | Quartetto di Anscombe, correlazioni spurie (Vigen). **Revisionato il 9 ottobre 2026:** fonti e grafico di Anscombe verificati; tolti cinque rimandi proiettati e le etichette "Integrazione A/B/C/D"; aggiunta "Che cosa evitare" |
| T10 | Deepfake (casi WSJ 2019 e Arup 2024), C2PA. **Revisionato il 9 ottobre 2026:** aggiunto l'art. 50 dell'AI Act (dichiarazione dei deepfake dal 2 agosto 2026; marcatura rinviata al 2 dicembre 2026 per i sistemi già sul mercato) in slide 66, note e fonti; tolti i rimandi proiettati e le etichette "Integrazione B/C"; aggiunta "Che cosa evitare" |
| T11 | Livelli di automazione (Parasuraman, Sheridan e Wickens 2000), OWASP, accumulo degli errori negli agenti. **Revisionato il 9 ottobre 2026:** OWASP aggiornato alla Top 10 LLM 2026 (prompt injection prima, eccesso di autonomia terzo); nota su MCP; tolti nove rimandi proiettati e l'etichetta "Integrazione C"; "Che cosa evitare" portata al formato standard a sei voci |
| T12 | Valore, waterfall da teorico a reale, paradosso di Solow, teoria dei vincoli. **Revisionato il 9 ottobre 2026:** studi di produttività aggiornati alle versioni pubblicate (Brynjolfsson QJE 2025: +15%, +36%; Dell'Acqua Organization Science 2026: +12,2%, +25,1%, +32%, -19 punti), coerenti con il T1; tolti i rimandi proiettati e le etichette "Integrazione A/B/C"; "Che cosa evitare" portata al formato standard a sei voci |

**Temi 13-18**

| Tema | Elementi notevoli |
|---|---|
| T13 | Compito, processo, ruolo; esposizione e trasformazione (Eloundou, Science 2024; analisi completa 2023); bancomat e cassieri (Bessen); Autor 2003. **Revisionato il 9 ottobre 2026:** tolti i rimandi proiettati (compresa la mappa competenze e temi della slide 48) e le etichette interne; aggiunta "Che cosa evitare" |
| T14 | Quattro condizioni (disponibilità, accessibilità, utilizzabilità, affidabilità); iceberg della conoscenza tacita; RAG concettuale; classificazione delle informazioni; oversharing; scenario a 5 errori. **Revisionato il 9 ottobre 2026:** fonti completate (Liu uniformato); tolti i rimandi proiettati e le etichette interne (A)-(D); grafico con percentuali inventate (slide 64) sostituito da un elenco senza numeri; "Che cosa evitare" nel formato standard a sei voci |
| T15 | Percorso individuare, descrivere, valutare, confrontare, verificare; scenario delle richieste commerciali; matrice valore e fattibilità; limiti dei punteggi; criteri di insuccesso definiti prima. **Revisionato il 9 ottobre 2026:** tolti i rimandi proiettati (anche nelle tabelle) e le etichette interne (A)-(D); grafici dello scenario mantenuti, perché calcoli dichiarati fittizi; "Che cosa evitare" nel formato standard a sei voci |
| T16 | Da disponibilità a valore; scenario A e B; Shadow AI; TAM e UTAUT; transfer della formazione; Kirkpatrick; sicurezza psicologica; diffusione rapida e graduale. **Revisionato il 9 ottobre 2026:** tolti i rimandi proiettati e le etichette interne (A)-(D); hype cycle solo richiamato (slide 31, grafico tolto); grafico dell'uso per funzione (slide 22) sostituito da un elenco senza numeri; dato del Work Trend Index 2024 precisato (78%); "Che cosa evitare" nel formato standard a sei voci |
| T17 | Esempi A-D (identificabilità, prompt injection, supervisione apparente, divulgazione via output); checklist in 5 domande; procedere, verificare, chiedere, interrompere. **Revisionato il 9 ottobre 2026:** OWASP 2026 come nel T11; tolti i rimandi proiettati e le lettere tra parentesi; lettere A-D mantenute come nome dei quattro esempi, ora "fittizi"; slide 68 rinominata "La checklist essenziale"; "Che cosa evitare" nel formato standard a sei voci |
| T18 | Verificato a ottobre 2026: AI Act modificato dal **Digital Omnibus**. Dettagli sotto. **Revisionato il 9 ottobre 2026:** dati normativi verificati sui testi ufficiali (EUR-Lex, Gazzetta Ufficiale); tolti i rimandi proiettati e le lettere tra parentesi; equivoci numerati da 1 a 4, lettere solo per gli esempi; tolta dalla slide 76 la nota di lavoro; "Che cosa evitare" nel formato standard a sei voci. **Corretta il 9 ottobre 2026 la slide 28 (L'alto rischio):** Allegato I diviso in sezione A e sezione B; le macchine sono passate nella sezione B con il Digital Omnibus (requisiti AI nel Regolamento Macchine 2023/1230, atti delegati entro il 2 agosto 2028) |

**Dettagli del Tema 18 (normativa verificata a ottobre 2026)**
- Il Digital Omnibus è il Reg. (UE) 2026/1744, pubblicato in GUUE (serie L) il 24 luglio 2026 e in vigore dal 27 luglio 2026. **Verificato sul testo ufficiale il 9 ottobre 2026** (EUR-Lex: considerando 38, 40 e 46; articolo 1, punto 5, per l'articolo 4).
- Alto rischio: Allegato III dal 2 dicembre 2027; Allegato I dal 2 agosto 2028 (considerando 40, verificato).
- Marcatura dei contenuti sintetici (art. 50, par. 2): transitorio di quattro mesi, fino al 2 dicembre 2026, per i sistemi già sul mercato prima del 2 agosto 2026 (considerando 38, verificato).
- Art. 3, punto 1 (definizione di sistema di AI): non modificato; le modifiche all'art. 3 riguardano i punti 14, 14 bis e 14 ter (verificato).
- Articolo 4 riscritto: obbligo di "sostenere lo sviluppo" dell'alfabetizzazione, senza garantire un livello individuale (verificato sul testo ufficiale).
- Nuovi divieti (art. 5, par. 1, lettere ba e bb: contenuti intimi senza consenso, materiale pedopornografico): esistenza verificata; **data di applicazione non verificata sul testo ufficiale, quindi non riportata nelle slide** (indicazione dell'utente: non usare dati senza riferimento ufficiale).
- Standard armonizzati: stato non verificato su fonte ufficiale; nelle slide "verificarne lo stato".
- Legge italiana 132/2025 (GU Serie Generale n. 223 del 25 settembre 2025), in vigore dal 10 ottobre 2025; artt. 7, 11, 13, 20 e 25 verificati sul testo; deleghe al Governo entro dodici mesi dall'entrata in vigore.
- Macchine (verificato sul testo ufficiale il 9 ottobre 2026): il Reg. 2026/1744 sopprime il punto 1 della sezione A dell'Allegato I e aggiunge il Reg. (UE) 2023/1230 come punto 21 della sezione B (art. 1, punto 41); per la sezione B l'AI Act si applica solo in parte (art. 2, par. 2, modificato); i requisiti per l'AI ad alto rischio nelle macchine entrano nel Regolamento Macchine con atti delegati applicabili entro il 2 agosto 2028 (art. 3; considerando 42). Stato degli atti delegati: da verificare.
- Esempi A-D, checklist di governance in 9 punti, esempio di policy di una pagina (fittizio).

---

## 5. Attività da svolgere per la revisione dell'intero percorso

Ordine consigliato: A, B e C prima di D; E ed F in parallelo dopo D. **Prima di iniziare, chiedere all'utente le priorità e confermare le risposte alle domande aperte della sezione 7.**

### A. Revisione trasversale dei 18 temi

È il passo indicato da tutti i documenti di perimetro. Per ogni punto: leggere i deck (estrazione testo con `python -m markitdown`), produrre un rapporto e proporre gli interventi prima di modificare.

**A1. Ridondanze già note da risolvere.** Decidere dove un contenuto è trattato e dove è solo richiamato.

| Contenuto | Dove compare |
|---|---|
| Automation bias e fiducia eccessiva (Parasuraman e Manzey 2010) | T5, T7, T17 (e T11 con Parasuraman 2000) |
| Prompt injection e OWASP | T11, T17 |
| Deepfake, casi WSJ 2019 e Arup 2024 | T10, T17 (nel T17 dovrebbe restare solo il richiamo) |
| Caso Amazon (Dastin 2018) | T3, T17 |
| Mata v. Avianca e piaggeria (Sharma 2023) | T3, T7 |
| Studi di produttività (Brynjolfsson, Dell'Acqua) | T1, T3, T12. **Deciso il 9 ottobre 2026 (punto 11):** introdotti nel T1 come segnale di rilevanza, richiamati nel T3 (frontiera frastagliata), approfonditi nel T12 (slide 28) per ragionare sul valore; stessi dati delle versioni pubblicate in tutti e tre |
| RAG e "Lost in the Middle" | T2, T8, T14 |
| Classificazione delle informazioni (pubbliche, interne, riservate, sensibili o personali) | T14, T17 |
| Shadow AI | T16 (adozione), T17 (rischio), T18 (governance) |
| Waterfall da beneficio teorico a reale | T12, T15 |
| Hype cycle | T1, T16. **Deciso il 9 ottobre 2026 (punto 11):** presentato per intero nel T1 (1.6, con lo schema); nel T16 solo richiamato nelle note della slide 31, senza grafico |
| Formazione | T16 come leva di adozione, T18 come misura di alfabetizzazione |
| Proporzionalità della verifica | T7, ripresa in T17 e T18 |

**A2. Lacune e prerequisiti.**
- Verificare che ogni concetto sia introdotto prima di essere usato.
- Esempi da controllare: il RAG nel T8 presuppone il T2; gli agenti nel T17 presuppongono il T11.
- Verificare i rimandi "(Tema N)" nelle slide e nelle note: devono puntare al tema giusto.

**A3. Coerenza terminologica.**
- Termini da uniformare: AI o IA; provider e deployer o fornitore e utilizzatore; prompt o richiesta; output o risultato; allucinazione.
- Nomi delle aree identici in tutti i deck.
- Formato delle citazioni uniforme. Liu et al. va citato come "(2024). Lost in the Middle: How Language Models Use Long Contexts. Transactions of the ACL, 12, 157-173": uniformato nel T2, nel T8 e nel T14 (9 ottobre 2026).

**A4. Coerenza dei passaggi tra temi.**
- Controllare in tutti i 18 deck le slide "Che cosa viene dopo" e "Il percorso del modulo".
- Il T2 rimandava all'AI Act "in un modulo dedicato": corretto con il rimando al Tema 18 (9 ottobre 2026).

**A5. Coerenza stilistica.**
- I Temi 1-7 non hanno l'indicatore a pillole e usano un set di helper più ridotto.
- Decidere se uniformarli. Le palette e i master sono gli stessi.

### B. Verifica delle fonti e dei fatti

Le fonti sono state citate a memoria e vanno verificate una per una, con WebSearch o WebFetch e le fonti primarie.

**Elenco per tema**

| Tema | Fonti da verificare |
|---|---|
| T1 | **Verificate il 9 ottobre 2026** (vedi registro). Restano da verificare solo i dati bibliografici aggiunti a memoria (Rosenblatt, Shortliffe, Rumelhart, Deng, Krizhevsky, Radford, Brown, Kaplan, Ouyang) |
| T2 | **Verificate il 9 ottobre 2026** (vedi registro). Confermato sul testo ufficiale (revisione del T18) che il Reg. 2026/1744 non modifica l'art. 3, punto 1 |
| T3 | **Verificate il 9 ottobre 2026** (vedi registro). Aggiunta la fonte Parasuraman e Manzey 2010 per l'automation bias |
| T4 | **Tutto il contenuto su prodotti, fornitori, modelli, prezzi e funzioni: rivedere integralmente, perché invecchia rapidamente.** La slide fonti non è stata estratta automaticamente: aprire il deck |
| T5 | **Verificate il 9 ottobre 2026** (vedi registro). Resta da confermare il DOI di Lee et al. 2025 (10.1145/3706598.3713778, nelle note della slide fonti) |
| T6 | **Verificate il 9 ottobre 2026** (vedi registro). Il deck cita le guide al prompting di Anthropic, OpenAI e Google; resta da confermare sulla guida ufficiale OpenAI (Reasoning best practices) l'indicazione sui modelli che ragionano, verificata solo su fonti secondarie |
| T7 | **Verificate il 9 ottobre 2026** (vedi registro). Restano da verificare le pagine di Reber e Schwarz 1999 (338-342) e di Parasuraman e Manzey 2010 (381-410), indicate a memoria |
| T8 | **Verificate il 9 ottobre 2026** (vedi registro): Liu uniformato al Tema 2, Lewis confermato |
| T9 | **Verificate il 9 ottobre 2026** (vedi registro): Anscombe (27(1), 17-21) e Vigen confermati |
| T10 | **Verificate il 9 ottobre 2026** (vedi registro): casi deepfake confermati (circa 220.000 euro; circa 25 milioni di dollari, Arup). Rinvio al 2 dicembre 2026 della marcatura (art. 50(2)) confermato sul testo ufficiale del Reg. 2026/1744 (considerando 38). Il codice di condotta sulla trasparenza di giugno 2026, non trovato su fonte ufficiale, è stato tolto dalle note (9 ottobre 2026) |
| T11 | **Verificate il 9 ottobre 2026** (vedi registro): Parasuraman, Sheridan e Wickens confermato (30(3), 286-297); OWASP Top 10 for LLM Applications 2026 (settembre 2026). Da verificare: la nota su MCP, citata a memoria |
| T12 | **Verificate il 9 ottobre 2026** (vedi registro): Brynjolfsson e Dell'Acqua nelle versioni pubblicate, Solow e Goldratt confermati. Da verificare: pagina dell'articolo di Solow (p. 36), citata a memoria |
| T13 | **Verificate il 9 ottobre 2026** (vedi registro): Eloundou citato nella versione Science 2024 con l'analisi completa del 2023; Bessen e Autor confermati. Da verificare: se la sintesi su Science riporta gli stessi valori (80% e 19%) |
| T14 | **Verificate il 9 ottobre 2026** (vedi registro): Polanyi con l'edizione Doubleday 1966 e la ristampa del 2009; Lewis, Liu e Saltzer e Schroeder con volumi e pagine; Nonaka e Takeuchi confermato. Da verificare: pagine di Lewis e di Saltzer e Schroeder, edizione di Polanyi |
| T15 | **Verificate il 9 ottobre 2026** (vedi registro): Popper 1959 (ed. orig. 1934); Brown 2009 e IDEO; Ohno 1988 (cinque perché); Nickerson 1998 con le pagine; effetto Hawthorne (citato con cautela, solo nelle note). Da verificare: pagine di Nickerson, editori di Popper, Brown e Ohno |
| T16 | Rogers; Davis 1989; Venkatesh 2003; Baldwin e Ford 1988; Kirkpatrick; Edmondson 1999; legge di Goodhart; Deming; modello 70-20-10; curva dell'oblio (Ebbinghaus); hype cycle (richiamo al T1); Work Trend Index 2024. **Verificate il 9 ottobre 2026** (vedi registro): Work Trend Index 2024 confermato (78% di chi usa l'AI al lavoro porta strumenti propri); aggiunte le pagine di Davis, Venkatesh, Baldwin e Ford, Edmondson. Da verificare: pagine ed editori |
| T17 | **Verificate il 9 ottobre 2026** (vedi registro): Greshake 2023 (AISec '23, 79-90); OWASP Top 10 for LLM Applications 2026 (prompt injection al primo posto, come nel T11); Sweeney 2000 (87%); Gender Shades 2018 (valori dello studio per il sistema peggiore: 0,3%, 7,1%, 12,0%, 34,7%; pagine 77-91); Parasuraman e Manzey 2010 (381-410); Reuters 2018; casi deepfake (2019 e Arup 2024). Da verificare: versione OWASP 2026 (fonti secondarie), pagine, dettagli dei casi deepfake |
| T18 | **Verificate il 9 ottobre 2026 sui testi ufficiali** (vedi registro): Reg. 2026/1744 (pubblicazione, entrata in vigore, date dell'alto rischio, transitorio art. 50, nuovo art. 4, art. 3 invariato); Legge 132/2025. Da verificare: data di applicazione dei nuovi divieti (non riportata), stato degli standard armonizzati e dei decreti attuativi della Legge 132/2025 |

**Correzione dei grafici.** I grafici con "dati inventati" sono dichiarati come tali; verificare che l'etichetta sia presente su ognuno. Se una fonte risulta sbagliata, correggere slide e note e annotarlo in un registro delle modifiche.

### C. Aggiornamenti per data e normativa

- Fissare una "data di validità" del percorso e aggiungerla nei deck sensibili al tempo: T1, T4 e T18 in particolare.
- Prima di ogni edizione, ricontrollare:
  - AI Act e Digital Omnibus (eventuali ulteriori modifiche, standard armonizzati, linee guida);
  - Legge 132/2025 e decreti attuativi;
  - GDPR e orientamenti delle autorità;
  - prodotti e modelli citati nel T4 e negli esempi.
- Verificare che nessun deck precedente al T18 contenga date dell'AI Act superate dal Digital Omnibus. Un primo controllo sui T1-T6 ha trovato solo riferimenti all'art. 3 e alla data di entrata in vigore, entrambi corretti.

### D. Metodo per derivare formazioni specifiche dalla base

La base è volutamente completa. Ogni formazione futura va progettata a partire da essa, in base a pubblico, obiettivi, durata e formato.

**Durate stimate della base**, calcolate dalle note del relatore: circa 196.000 parole, 140 parole al minuto, solo esposizione frontale.

| Area | Temi | Esposizione frontale |
|---|---|---|
| Comprendere l'AI | 1-4 | circa 4 h 30 min |
| Interagire con l'AI | 5-7 | circa 3 h 25 min |
| Esplorare le possibilità dell'AI | 8-11 | circa 6 h |
| Comprendere il valore per l'azienda | 12-16 | circa 6 h 40 min |
| Utilizzare l'AI responsabilmente | 17-18 | circa 2 h 55 min |
| **Totale** | 1-18 | **circa 23-25 h** |

- **Aula reale:** con domande, discussione e pause si aggiunge di norma il 40-60 per cento, cioè **circa 35-40 ore**.
- **Esercizi:** le note contengono almeno 101 "Esercizi suggeriti" (Temi 6-18). Svolgendone una parte, il percorso completo supera le **50-60 ore**.
- **Durata per tema:** quella di ciascun tema è indicata nella sezione 9.

**Procedura consigliata per una nuova formazione**
1. Chiedere all'utente:
   - pubblico (ruoli, livello di partenza, numero di partecipanti);
   - obiettivi;
   - durata e numero di incontri;
   - formato (aula, online, e-learning, misto);
   - eventuali vincoli, per esempio obblighi di alfabetizzazione o temi richiesti dal committente.
2. Selezionare i contenuti usando l'indice della sezione 9 e le priorità dei documenti di perimetro (Molto alta, Alta, Media, "solo accennare"). Distinguere:
   - **nucleo**, da trattare in aula;
   - **approfondimento**, come materiale di studio;
   - **riferimento**, come dispensa.
3. Ritmo realistico in aula: circa 15-20 slide all'ora, includendo interazione. Le slide chiave, gli scenari dei documenti e le schede pratiche sono di norma il nucleo.
4. Proporre un'agenda con tempi per blocco, pause ed esercitazioni, e farla validare prima di produrre i materiali.
5. Produrre i deck della formazione specifica come nuovi file, senza modificare la base:
   - selezionando e riordinando slide dei 18 deck;
   - oppure con nuovi deck sintetici generati dai sorgenti.
6. Annotare in un file dedicato a quella formazione le scelte fatte (pubblico, selezione, agenda), così la base resta neutra e riutilizzabile.

### E. Sviluppo degli esercizi

- Ogni slide chiave contiene un "Esercizio suggerito" nelle note.
- Raccoglierli tutti, estraendoli con markitdown e grep "Esercizio suggerito", in un elenco unico.
- Organizzarli come una libreria di esercizi riutilizzabili, da selezionare per ogni formazione specifica (attività D).
- Svilupparli come schede: obiettivo, durata, materiali, consegna, debriefing, materiale fittizio pronto.
- Tutti gli esempi devono restare fittizi.
- Considerare anche:
  - strumenti di verifica dell'apprendimento, in coerenza con il T16 (livelli di Kirkpatrick);
  - una registrazione della formazione, in coerenza con il T18, art. 4. Ricordare che la registrazione non prova la conformità.

### F. Brand e versione finale

- Chiedere all'utente se la base e le formazioni derivate debbano applicare il **brand NetAi**. È disponibile la skill `netai-brand:brand-identity-netai`.
- In caso affermativo, va sostituito il tema neutro (palette HEX e font nei sorgenti) e va riapplicato il pipeline di QA.

### G. Materiali complementari, da proporre all'utente

- Una dispensa per i partecipanti per ciascuna area, adattabile alle singole formazioni.
- Una pagina con le checklist: T15 (scheda opportunità), T17 (5 domande), T18 (governance in 9 punti).
- Un glossario unico del percorso, utile anche per l'attività A3.
- Una guida per il formatore con le avvertenze, in particolare quelle normative del T18.
- **Lacune emerse con la formazione Laser Srl (9 ottobre 2026):** NIS2 non compare in nessuno dei 18 deck; l'AI nel prodotto (manutenzione predittiva, qualità visiva, servitization) è solo accennata. Valutare se portare nella base le slide nuove create per Laser (vedi `Formazioni/2026-10_LaserSrl_AI_Adoption/note_scelte.md`).

---

## 6. Note tecniche per rigenerare o modificare i deck

### Sorgenti
- `Base/sorgenti_slide.zip` contiene tutti i file JavaScript usati.
- Composizione dei file:
  - `commonN.js`: setup, tema, master, helper di base;
  - `helpers.js`, `helpers4.js`, `extra5.js`, `extra7.js`, `extra8.js`, `charts11.js`, `helpers12.js`: helper condivisi;
  - `bodyN*.js`: contenuto di ciascun tema;
  - `buildN.js`: concatenazione già pronta.
- Il Tema 1 usa `build.js`.
- Comando di build, per esempio per il Tema 18:
  ```
  cat common18.js helpers.js helpers4.js extra5.js extra8.js charts11.js helpers12.js body18a.js body18b.js body18c.js > build18.js && node build18.js
  ```
- `commonN.js` richiede `apply_theme.js` della skill pptx, con un percorso assoluto dell'ambiente cloud. In una nuova sessione aggiornare quel percorso. Il percorso usato era `/root/.claude/skills/synced/089a5cb4-f32b-4603-aa0a-09878bdf984d_e1119d2b-6bf8-43fc-8ae3-be0bf12e39dd/pptx/scripts/apply_theme.js`.
- In alternativa, si possono modificare direttamente i .pptx con la skill pptx.

### Impostazioni dei deck
- **Libreria e formato:** pptxgenjs, LAYOUT_16x9.
- **Master:** TITOLO, SEZIONE, CONTENUTO, CHIAVE.
- **Palette neutra (HEX):** dk1 22262B, lt1 FFFFFF, dk2 4A515C, lt2 F2F3F5, a1 2E7D7A, a2 8A939E, a3 D5D9DE, a4 5B6573, a5 A86F1C, a6 E6F0EF. Toni aggiuntivi: D9ECEA, CFE6E4.
- **Icone:** react-icons/fi (Feather), renderizzate con sharp.
- **Grafici:** nativi di PowerPoint (barre, linee, torta, a cascata con serie base bianca), modificabili dall'utente.
- **Helper principali:**
  - `card`, `bullets`, `txt`, `arrow`, `shapeBox`, `iconCircle`, `section`, `content`, `divider`, `keySlide`;
  - `table`, `chip`, `chartBarH`, `iconGrid`, `banner`, `rowList`, `twoPanel`, `promptBox`, `qGrid`, `pathSlide`, `lineChart`, `docBox`, `numList`;
  - `rowsLabel`, che accetta anche le opzioni x e w.

### QA obbligatoria a ogni modifica
1. `python3 .../pptx/scripts/office/validate.py FILE.pptx` deve dare "All validations PASSED".
2. `python3 -m markitdown FILE.pptx > t.md` e poi `python3 -c "import sys;t=open(sys.argv[1]).read();print(t.count('\\u2013')+t.count('\\u2014'))" t.md`: deve dare 0.
3. Render: `soffice --headless --convert-to pdf`, poi `pdftoppm -r 50 -jpeg`, poi griglie 2x3 con PIL, controllate a vista.

### Errori ricorrenti già visti, da ricontrollare dopo ogni modifica
- **Titoli lunghi che si sovrappongono alle pillole** in alto a destra: tenere il titolo entro circa 5,5 pollici.
- **Titoli dei divisori che vanno a capo** sul sottotitolo.
- **Testo che esce da `twoPanel` o `card` basse**: sostituire con `docBox` o aumentare l'altezza.
- **Elementi coperti da `banner`.**
- **Legende ed etichette dei grafici tagliate** da elementi sottostanti.
- **Icone inesistenti** in react-icons/fi (esempio: FiMegaphone, sostituita da FiVolume2).

### Consegna
1. Inviare il file all'utente con SendUserFile (display attach).
2. Scrivere il file nella cartella giusta con device_commit_files, usando il fileUuid restituito:
   - `/Users/michelebarchi/Claude/Projects/Formazione AI Literacy Official/Base/<file>` per i file della base;
   - `/Users/michelebarchi/Claude/Projects/Formazione AI Literacy Official/Formazioni/<nome formazione>/<file>` per una formazione specifica.
3. Per sovrascrivere un file già presente serve `force: true`.

---

## 7. Domande aperte da porre all'utente all'inizio della revisione

1. Priorità tra le attività A-G, e se procedere tema per tema o per area.
2. Se la revisione riguarda solo la base, o anche una prima formazione specifica da progettare (in quel caso: pubblico, durata, formato).
3. Applicare il brand NetAi alla versione finale?
4. Formato preferito per le formazioni derivate: nuovi deck sintetici oppure selezione di slide dai 18 deck completi?
5. Chi valida le verifiche normative del Tema 18 (legale, DPO)?
6. Glossario unico: AI o IA, e altri termini preferiti.

---

## 8. Come iniziare la prossima sessione

1. Leggere questo file e verificare l'accesso alla cartella, con un elenco dei file di `Base/` e di `Formazioni/`.
2. Estrarre i 18 deck in testo con markitdown e tenerli nello scratchpad per le analisi.
3. Porre le domande della sezione 7. Chiedere anche del brand, come da preferenza.
4. Creare una lista di attività visibile all'utente e procedere con l'attività A, poi B e C, consegnando i rapporti prima di modificare i deck.
5. Tenere un registro delle modifiche in `Base/registro_revisione.md`. Non conservare copie delle versioni precedenti: le gestisce l'utente su GitHub.

---

## 9. Indice degli argomenti delle slide

Indice generato dai 18 deck. Per ogni tema: introduzione, sottotemi con i titoli delle slide e il messaggio della slide chiave, conclusioni. I numeri tra parentesi sono i numeri di slide. La durata è stimata dalle note del relatore (circa 140 parole al minuto, solo esposizione frontale).

### Tema 1 · Evoluzione e rilevanza dell'Intelligenza Artificiale
*Area: Comprendere l'AI · 59 slide · file `Tema1_Evoluzione_e_rilevanza_AI.pptx` · esposizione stimata circa 1 h 01 min*

- **Introduzione**: Obiettivo del modulo (2) · Sei domande guida per questo modulo (3) · Il filo conduttore (4) · Il percorso del modulo (5)
- **1.1 Storia ed evoluzione dell'AI**: Le origini: si possono costruire macchine che pensano? (7) · Oltre settant'anni di evoluzione (8) · L'AI simbolica: la conoscenza scritta in regole (9) · Cicli di entusiasmo e disillusione (10) · Dalle regole all'apprendimento dai dati (11) · Machine Learning e Deep Learning (12) · Dall'AI specializzata all'AI generativa (13)
  - *Messaggio chiave:* L'AI è il risultato di decenni di ricerca ed evoluzione tecnologica, non un'invenzione recente.
- **1.2 I fattori dell'accelerazione tecnologica**: Cinque fattori che si rafforzano a vicenda (16) · Potenza di calcolo (17) · Disponibilità di grandi quantità di dati (18) · Evoluzione degli algoritmi e delle architetture (19) · Lo sviluppo di modelli di grandi dimensioni (20) · Investimenti e infrastrutture tecnologiche (21)
  - *Messaggio chiave:* L'accelerazione deriva dalla convergenza di diversi fattori, non da una singola invenzione.
- **1.3 La svolta dell'AI generativa**: Dal classificare e prevedere al generare (24) · Il linguaggio naturale diventa l'interfaccia (25) · La diffusione di chatbot e assistenti AI (26) · Che cosa può generare l'AI (27) · Un'AI accessibile a tutti (28)
  - *Messaggio chiave:* L'AI generativa ha ampliato le persone e le attività che possono utilizzare direttamente capacità AI.
- **1.4 Dalla digitalizzazione all'Intelligenza Artificiale**: Quattro passaggi di un'evoluzione (31) · Un esempio: la gestione delle richieste dei clienti (32) · Software deterministico e sistemi probabilistici (33)
  - *Messaggio chiave:* Digitalizzazione, automazione e AI sono concetti collegati ma distinti; possono coesistere nello stesso processo aziendale.
- **1.5 Rilevanza dell'AI per le aziende**: Un'applicazione trasversale alle funzioni aziendali (36) · L'AI come tecnologia abilitante (37) · Capacità AI accessibili tramite strumenti commerciali (38) · Effetti potenziali: produttività, qualità, innovazione (39) · Come evolvono il lavoro e le competenze (40) · Possibili implicazioni competitive (41) · Dal potenziale tecnologico al valore realizzato (42)
  - *Messaggio chiave:* L'AI può abilitare cambiamenti in molte aree dell'impresa, ma il valore nasce da applicazioni appropriate a problemi reali.
- **1.6 Tra hype e realtà**: Aspettative, promesse e narrazioni mediatiche (45) · Dimostrazione tecnologica e uso aziendale continuativo (46) · Maturità delle capacità e limiti attuali (47) · Opportunità concrete o affermazioni non dimostrate? (48) · I benefici non sono uguali per tutti (49) · Velocità del cambiamento e incertezza sul futuro (50) · Competenze adattabili, non dipendenza dagli strumenti (51)
  - *Messaggio chiave:* Occorre valutare criticamente le promesse dell'AI, distinguendo possibilità tecniche, affidabilità e convenienza.
- **Conclusioni**: Le domande guida: le nostre risposte (53) · Che cosa portiamo a casa (54) · Davanti a una novità sull'AI: una scheda pratica (55) · Che cosa evitare (56) · Prossimo passo: il Tema 2 (57) · Fonti e riferimenti (1 di 2) (58) · Fonti e riferimenti (2 di 2) (59)

### Tema 2 · Fondamenti e funzionamento dell'Intelligenza Artificiale
*Area: Comprendere l'AI · 72 slide · file `Tema2_Fondamenti_e_funzionamento_AI.pptx` · esposizione stimata circa 1 h 18 min*

- **Introduzione**: Obiettivo del modulo (2) · Otto domande guida per questo modulo (3) · Il filo conduttore (4) · Il percorso del modulo (5)
- **2.1 Che cos'è l'Intelligenza Artificiale**: Una definizione operativa (7) · Intelligenza artificiale e intelligenza umana (8) · Sistemi specializzati e intelligenza artificiale generale (9) · Comprensione apparente: l'effetto ELIZA (10) · Che cosa osserviamo e che cosa possiamo concludere (11)
  - *Messaggio chiave:* L'AI non è un'unica tecnologia e le prestazioni osservabili non autorizzano automaticamente ad attribuirle caratteristiche umane.
- **2.2 Le principali categorie di AI**: Quattro criteri di classificazione diversi (14) · AI simbolica e Machine Learning (15) · Deep Learning e reti neurali (16) · AI predittiva, discriminativa e generativa (17) · AI multimodale (18) · Quale approccio per quale problema (19)
  - *Messaggio chiave:* Esistono approcci e capacità differenti, adatti a problemi differenti. Le categorie rispondono a criteri diversi e non sono tutte mutuamente esclusive.
- **2.3 Come un sistema AI apprende dai dati**: Che cosa significa apprendere dai dati (22) · Dati di addestramento ed esempi (23) · Individuare schemi e regolarità (24) · I parametri del modello (25) · Il ciclo di addestramento (26) · Generalizzare verso nuovi input (27) · Addestramento e inferenza (28)
  - *Messaggio chiave:* Nei sistemi di Machine Learning l'addestramento modifica i parametri del modello, mentre l'inferenza lo utilizza per elaborare nuovi input. Non tutti i sistemi AI apprendono dai dati.
- **2.4 Che cosa sono i Large Language Models**: Un modello linguistico di grandi dimensioni (31) · I token: come il modello vede il testo (32) · Rappresentare il significato (33) · Il Transformer e il meccanismo di attenzione (34) · Come viene generata una risposta (35) · Più di un completamento automatico (36) · Capacità linguistiche, di analisi e di ragionamento (37) · Perché un modello può affrontare compiti diversi (38)
  - *Messaggio chiave:* Gli LLM generano output usando regolarità apprese e il contesto disponibile; la spiegazione non va ridotta alla sola metafora del completamento automatico.
- **2.5 Come funziona un'interazione con l'AI**: Input, prompt e output (41) · Il percorso di una richiesta (42) · La finestra di contesto (43) · La cronologia conversazionale (44) · Contesto temporaneo e memoria persistente (45) · Il modello e l'applicazione (46)
  - *Messaggio chiave:* Il risultato dipende anche dalle informazioni rese disponibili durante l'interazione; il funzionamento del modello e quello del prodotto che lo utilizza non coincidono sempre.
- **2.6 Conoscenza e fonti informative**: Tre fonti di informazione (49) · Conoscenza incorporata e recupero di informazioni (50) · Aggiornamento dei dati e limiti temporali (51) · Grounding: ancorare le risposte alle fonti (52) · Introduzione alla Retrieval-Augmented Generation (53) · Adattare un sistema AI a un contesto specifico (54) · Tre equivoci frequenti (55)
  - *Messaggio chiave:* Fornire un documento o collegare una fonte a un sistema AI non significa necessariamente riaddestrare il modello.
- **2.7 Variabilità dei risultati**: Stessa richiesta, risposte diverse (58) · Che cosa influenza la variabilità (59) · I parametri di generazione: la temperatura (60) · Comportamento deterministico e probabilistico (61) · Riproducibilità dei risultati (62) · Variabilità non significa errore (63)
  - *Messaggio chiave:* Una stessa richiesta può produrre risposte differenti; la variabilità è distinta dalla questione della correttezza e dell'affidabilità.
- **Conclusioni**: Le domande guida: le nostre risposte (65) · Che cosa portiamo a casa (66) · Glossario essenziale (1 di 2) (67) · Glossario essenziale (2 di 2) (68) · Da dove viene questa risposta? Una scheda pratica (69) · Che cosa evitare (70) · Prossimo passo: il Tema 3 (71) · Fonti e riferimenti (72)

### Tema 3 · Capacità, limiti e affidabilità dell'Intelligenza Artificiale
*Area: Comprendere l'AI · 70 slide · file `Tema3_Capacita_limiti_affidabilita_AI.pptx` · esposizione stimata circa 1 h 15 min*

- **Introduzione**: Obiettivo del modulo (2) · Calibrare la fiducia (3) · Otto domande guida per questo modulo (4) · Il filo conduttore (5) · Il percorso del modulo (6)
- **3.1 Le principali capacità dell'AI**: Una mappa delle capacità (8) · Dalle capacità alle attività (9) · Non tutti i sistemi hanno le stesse capacità (10)
  - *Messaggio chiave:* Le capacità dell'AI sono ampie, ma variano in funzione dei sistemi e dei compiti; non tutti i prodotti AI dispongono delle stesse funzioni.
- **3.2 Ragionamento, problem solving e creatività**: Ragionamento logico, matematico e analitico (13) · Problemi strutturati e non strutturati (14) · Scomporre, pianificare, valutare alternative (15) · Generazione di idee e supporto creativo (16) · Limiti nelle situazioni nuove, ambigue o complesse (17)
  - *Messaggio chiave:* L'AI può supportare attività cognitive avanzate, ma non garantisce ragionamenti sempre corretti o coerenti.
- **3.3 Allucinazioni e informazioni false**: Che cos'è un'allucinazione (20) · Citazioni, riferimenti e fonti inesistenti (21) · Perché si verificano le allucinazioni (22) · Plausibilità linguistica e veridicità (23) · L'autorevolezza apparente (24) · Dove le allucinazioni sono più probabili (25)
  - *Messaggio chiave:* La fluidità o la sicurezza del tono non dimostra che un'affermazione sia corretta o verificata.
- **3.4 Bias e distorsioni nei risultati**: Che cosa sono bias e distorsioni (28) · Da dove nascono le distorsioni (29) · Stereotipi e rappresentazioni non equilibrate (30) · L'influenza del contesto e delle istruzioni (31) · Bias di conferma e tendenza ad assecondare (32) · Neutralità apparente e oggettività effettiva (33)
  - *Messaggio chiave:* I sistemi AI possono riprodurre o amplificare distorsioni; le risposte non devono essere considerate automaticamente imparziali.
- **3.5 Accuratezza, affidabilità e consistenza**: Quattro concetti da distinguere (36) · Prestazioni diverse in base al compito (37) · Coerenza, ripetibilità e robustezza (38) · I limiti di benchmark e dimostrazioni (39) · Valutare le prestazioni nel contesto reale (40) · Il modello e il sistema completo (41)
  - *Messaggio chiave:* L'affidabilità non è una proprietà unica e universale di un modello; deve essere valutata per compiti e condizioni d'uso specifici.
- **3.6 Verificabilità e controllo dei risultati**: Che cosa verificare (44) · Verificare fatti, fonti e riferimenti (45) · Controllare calcoli, dati e informazioni (46) · Completezza, coerenza e tracciabilità (47) · I limiti dell'autoverifica (48) · Supervisione umana e verifica proporzionata (49)
  - *Messaggio chiave:* La verifica è parte dell'uso consapevole dell'AI e deve essere proporzionata all'importanza del compito e alle possibili conseguenze di un errore.
- **3.7 I fattori che influenzano le prestazioni**: Sette fattori (52) · Tecnologia, informazioni e modalità operative (53) · Differenze tra ambiti applicativi (54)
  - *Messaggio chiave:* Le prestazioni derivano dall'interazione tra caratteristiche tecnologiche, qualità delle informazioni e modalità operative.
- **3.8 Quando utilizzare o limitare l'AI**: Possibilità tecnica e opportunità di utilizzo (57) · Le conseguenze di un errore (58) · Attività a basso e alto impatto (59) · Affidabilità adeguata allo scopo (60) · Supporto, supervisione e delega (61) · Quando limitare o evitare l'uso (62) · La responsabilità resta umana (63)
  - *Messaggio chiave:* L'AI va utilizzata quando le sue prestazioni e i controlli disponibili sono compatibili con il rischio del compito, non soltanto quando il sistema sembra capace di eseguirlo.
- **Conclusioni**: Le domande guida: le nostre risposte (65) · Che cosa portiamo a casa (66) · Prima di usare un risultato AI: una checklist (67) · Che cosa evitare (68) · Prossimo passo: il Tema 4 (69) · Fonti e riferimenti (70)

### Tema 4 · Ecosistema AI: modelli, strumenti e piattaforme
*Area: Comprendere l'AI · 70 slide · file `Tema4_Ecosistema_AI.pptx` · esposizione stimata circa 1 h 14 min*

- **Introduzione**: Obiettivo del modulo (2) · Dieci domande guida per questo modulo (3) · Il filo conduttore (4) · Il percorso del modulo (5)
- **4.1 La struttura dell'ecosistema AI**: Modello, sistema, applicazione, piattaforma (7) · Foundation models e modelli specializzati (8) · Gli attori dell'ecosistema (9) · Com'è fatta un'applicazione AI (10) · Più modelli, modelli che cambiano (11) · Ecosistemi integrati e soluzioni composte (12)
  - *Messaggio chiave:* Un'applicazione AI è spesso composta da più elementi tecnologici e non coincide necessariamente con il modello che utilizza.
- **4.2 Le principali famiglie di modelli AI**: Quattro famiglie di modelli (15) · Capacità, dimensioni e requisiti (16) · Modelli proprietari e modelli con pesi accessibili (17) · Open-weight non significa open-source (18) · Modelli aperti, chiusi e controllo tecnologico (19)
  - *Messaggio chiave:* Modelli differenti rispondono a esigenze differenti; non esiste un unico modello migliore per qualunque attività.
- **4.3 Le principali piattaforme e gli strumenti AI**: Gli assistenti AI generalisti (22) · Le categorie di strumenti (23) · Funzionalità comuni e differenze principali (24) · Capacità del modello e funzionalità dell'applicazione (25) · Disponibilità delle funzionalità (26) · Capacità dichiarate e funzionalità disponibili (27)
  - *Messaggio chiave:* Due prodotti dall'interfaccia simile possono offrire capacità, integrazioni, controlli e condizioni molto diversi.
- **4.4 AI generalista, specializzata e integrata**: Tre approcci (30) · L'AI nei software di produttività e nei gestionali (31) · Soluzioni pronte all'uso e personalizzate (32) · Vantaggi e limiti dei diversi approcci (33) · Usare uno strumento o integrare l'AI in un processo (34)
  - *Messaggio chiave:* Le capacità AI possono essere disponibili in prodotti generalisti, strumenti dedicati o software già presenti in azienda; adottare AI non richiede necessariamente un nuovo applicativo separato. Sottot
- **4.5 Chatbot, assistenti, agenti e automazioni**: Uno spettro di autonomia (37) · Chatbot e assistenti configurati (38) · Sistemi con strumenti e agenti (39) · Automazioni tradizionali e workflow con AI (40) · Livelli di autonomia e supervisione umana (41) · Una terminologia non standardizzata (42)
  - *Messaggio chiave:* Conversare, ricevere assistenza, automatizzare e delegare l'esecuzione di attività rappresentano modalità e livelli di autonomia differenti.
- **4.6 Modalità di accesso e utilizzo dell'AI**: Le principali modalità di accesso (45) · Applicazioni e API: due modi di usare lo stesso modello (46) · Cloud ed esecuzione locale (47) · Soluzioni individuali, team ed enterprise (48)
  - *Messaggio chiave:* Capacità analoghe possono essere rese disponibili attraverso modalità differenti, con implicazioni tecniche, economiche e organizzative diverse.
- **4.7 Criteri per confrontare e scegliere**: Undici criteri (51) · Adeguatezza, qualità e facilità d'uso (52) · Funzionalità, integrazione e costi complessivi (53) · Dati, sicurezza e controlli amministrativi (54) · Indipendenza tecnologica e vendor lock-in (55) · Verificare ciò che è davvero disponibile (56) · Una scheda di confronto (57)
  - *Messaggio chiave:* Lo strumento più noto o il modello più potente non è necessariamente la scelta migliore per l'azienda.
- **4.8 L'evoluzione e la dinamicità dell'ecosistema AI**: Che cosa cambia (60) · Obsolescenza di strumenti, procedure e competenze (61) · Competenze e conoscenze trasferibili (62) · Orientarsi senza inseguire ogni novità (63)
  - *Messaggio chiave:* I principi di funzionamento e valutazione hanno maggiore durata rispetto alle caratteristiche di una singola versione di un prodotto.
- **Conclusioni**: Le domande guida: le nostre risposte (65) · Che cosa portiamo a casa (66) · Prima di scegliere uno strumento AI: una checklist (67) · Che cosa evitare (68) · Prossimo passo: il Tema 5 (69) · Nota sull'aggiornamento dei contenuti (70)

### Tema 5 · Il dialogo uomo-AI
*Area: Interagire con l'AI · 63 slide · file `Tema5_Dialogo_uomo_AI.pptx` · esposizione stimata circa 1 h 04 min*

- **Introduzione**: Obiettivo del modulo (2) · Dieci domande guida per questo modulo (3) · Il filo conduttore (4) · Il percorso del modulo (5)
- **5.1 Il linguaggio naturale come interfaccia**: Dai comandi alle richieste (7) · Vantaggi e limiti della comunicazione conversazionale (8) · Flessibilità e ambiguità del linguaggio (9) · Testo, voce e immagini (10) · Cambia il rapporto tra utente e software (11)
  - *Messaggio chiave:* Il linguaggio naturale amplia l'accessibilità della tecnologia, ma richiede comunque obiettivi chiari e un'interpretazione critica delle risposte.
- **5.2 Dalla domanda alla conversazione**: Richiesta isolata e dialogo articolato (14) · Un processo progressivo e iterativo (15) · Un esempio di dialogo (16) · Il contesto della conversazione (17) · L'AI come interlocutore che può porre domande (18) · L'AI come supporto alla definizione dei problemi (19)
  - *Messaggio chiave:* Una buona interazione può svilupparsi attraverso più scambi e non richiede una richiesta iniziale perfetta.
- **5.3 I diversi ruoli che l'AI può assumere**: Sette ruoli possibili (22) · Fonte, assistente operativo, supporto creativo (23) · Analista, revisore, tutor (24) · L'AI come strumento di confronto critico (25) · Ruolo assegnato e competenza effettiva (26)
  - *Messaggio chiave:* Assegnare un ruolo all'AI può orientarne il comportamento, ma non garantisce che abbia le competenze richieste.
- **5.4 La collaborazione uomo-AI**: Ottenere una risposta o collaborare (29) · Suddividere le attività tra persona e sistema (30) · Capacità complementari (31) · Produrre, rivedere, migliorare (32) · Supporto al ragionamento e alla valutazione (33) · Competenze, contesto e responsabilità (34)
  - *Messaggio chiave:* Il valore dell'AI può nascere dalla combinazione delle capacità del sistema con quelle della persona, senza implicare la sostituzione del giudizio umano.
- **5.5 I livelli di delega all'Intelligenza Artificiale**: Cinque livelli di delega (37) · Che cosa fanno l'AI e la persona a ogni livello (38) · Assistenza, collaborazione, delega, automazione (39) · Come cambia il ruolo umano (40) · Responsabilità e controllo ai diversi livelli (41) · Scegliere il livello adeguato (42)
  - *Messaggio chiave:* Una maggiore autonomia non determina automaticamente risultati migliori: il livello di delega deve essere adeguato al compito, alle capacità del sistema, ai rischi e ai controlli disponibili.
- **5.6 La qualità dipende anche dalla persona**: Otto fattori che dipendono dalla persona (45) · Obiettivi chiari e comprensione del problema (46) · Contesto e competenze di dominio (47) · Domande, interpretazione e feedback (48) · Utilizzo passivo e utilizzo attivo (49)
  - *Messaggio chiave:* Le competenze umane restano determinanti per formulare problemi, interpretare risultati e riconoscere output inadeguati.
- **5.7 Limiti e rischi della relazione conversazionale**: Antropomorfizzazione (52) · Fiducia eccessiva e accettazione passiva (53) · Automation bias (54) · Il rischio della delega cognitiva (55) · Dipendenza e preservazione del giudizio (56)
  - *Messaggio chiave:* Un'interazione naturale e convincente non attribuisce al sistema intenzionalità, giudizio umano o responsabilità decisionale.
- **Conclusioni**: Le domande guida: le nostre risposte (58) · Che cosa portiamo a casa (59) · Principi per un dialogo consapevole (60) · Che cosa evitare (61) · Prossimo passo: il Tema 6 (62) · Fonti e riferimenti (63)

### Tema 6 · Prompting e tecniche di interazione con l'AI
*Area: Interagire con l'AI · 74 slide · file `Tema6_Prompting_tecniche_interazione.pptx` · esposizione stimata circa 1 h 14 min*

- **Introduzione**: Obiettivo del modulo (2) · Dieci domande guida per questo modulo (3) · Il filo conduttore (4) · Il percorso del modulo (5)
- **6.1 Fondamenti del prompting**: Che cos'è un prompt (7) · Domanda, istruzione, richiesta di esecuzione (8) · Richieste generiche e contestualizzate (9) · Chiarezza, specificità, pertinenza (10) · Qualità dell'input e utilità dell'output (11) · Prompting e programmazione tradizionale (12) · Prompting e limiti delle istruzioni (13)
  - *Messaggio chiave:* Il prompt comunica obiettivi e aspettative, ma non è un comando che assicura un risultato deterministico e corretto.
- **6.2 Gli elementi di una richiesta efficace**: Prima il problema, poi il prompt (16) · Otto elementi possibili (17) · Anatomia di una richiesta (18) · Vincoli, formato e criteri di qualità (19) · Ruoli e prospettive (20) · Non serve sempre un prompt lungo (21)
  - *Messaggio chiave:* Un prompt efficace rende espliciti i requisiti rilevanti; non deve necessariamente essere lungo o contenere tutti gli elementi in ogni situazione.
- **6.3 Il ruolo del contesto nel prompting**: Che cosa è contesto (24) · Distinguere informazioni, istruzioni, esempi (25) · Qualità del contesto: pertinente, completo, comprensibile (26) · Chiedere all'AI di esplicitare le informazioni mancanti (27) · Informazioni contraddittorie (28) · Gestire i limiti della finestra di contesto (29)
  - *Messaggio chiave:* Fornire più informazioni non produce automaticamente risultati migliori; è preferibile un contesto pertinente, sufficientemente completo e comprensibile.
- **6.4 Tecniche fondamentali di prompting**: Una cassetta degli attrezzi (32) · Zero-shot e few-shot (33) · Istruzioni strutturate e delimitazione (34) · Scomporre i compiti complessi (35) · Alternative e confronto con criteri (36) · Chiedere chiarimenti prima dell'esecuzione (37) · Scegliere la tecnica in base al compito (38)
  - *Messaggio chiave:* La complessità della tecnica deve essere proporzionata al compito; non esiste una strategia unica migliore in ogni situazione.
- **6.5 Prompting iterativo**: Il ciclo del miglioramento progressivo (41) · Feedback efficaci (42) · Raffinare, approfondire, riformulare (43) · Modificare la richiesta o ricominciare (44) · I limiti dell'iterazione (45)
  - *Messaggio chiave:* L'iterazione consente di migliorare l'aderenza al compito, ma la verifica indipendente della correttezza appartiene a una fase distinta.
- **6.6 Guidare il formato e la struttura degli output**: Definire il formato desiderato (48) · Report, documenti e comunicazioni professionali (49) · Dettaglio, tono e destinatario (50) · Introduzione agli output strutturati (51) · Vincoli di presentazione e criteri verificabili (52)
  - *Messaggio chiave:* La forma dell'output ne condiziona l'utilità nelle attività successive, ma la buona formattazione non dimostra la correttezza del contenuto.
- **6.7 Prompting per attività professionali**: Attività creative, analitiche e operative (55) · Scrittura e revisione di contenuti (56) · Analisi e sintesi documentale (57) · Informazioni e dati (58) · Ricerca, alternative, brainstorming e problem solving (59) · Report e comunicazioni (60)
  - *Messaggio chiave:* Il metodo deve adattarsi allo scopo e al contesto lavorativo; il tema insegna ad applicare i principi, non a memorizzare prompt universali.
- **6.8 Istruzioni riutilizzabili e standardizzazione**: Prompt occasionali e ricorrenti (63) · Template di prompt (64) · Librerie, istruzioni persistenti, assistenti configurati (65) · Standardizzare, versionare, manutenere (66) · I limiti della standardizzazione (67)
  - *Messaggio chiave:* Istruzioni riutilizzabili possono favorire coerenza e produttività, ma devono essere manutenute e non sostituiscono il controllo dei risultati.
- **Conclusioni**: Le domande guida: le nostre risposte (69) · Che cosa portiamo a casa (70) · Uno schema per le richieste importanti (71) · Che cosa evitare (72) · Prossimo passo: il Tema 7 (73) · Nota sulle fonti e sugli esempi (74)

### Tema 7 · Verifica degli output e pensiero critico nell'utilizzo dell'AI
*Area: Interagire con l'AI · 74 slide · file `Tema7_Verifica_output_pensiero_critico.pptx` · esposizione stimata circa 1 h 17 min*

- **Introduzione**: Obiettivo del modulo (2) · Undici domande guida per questo modulo (3) · Il filo conduttore: valutare, verificare, decidere (4) · Il percorso del modulo (5)
- **7.1 Il pensiero critico nell'interazione con l'AI**: Che cos'è il pensiero critico (7) · Ricevere informazioni o valutarle (8) · Fatti, opinioni, ipotesi, interpretazioni (9) · Le domande critiche (10) · Evidenze, giudizio e competenze (11) · Atteggiamento critico, non sfiducia (12)
  - *Messaggio chiave:* Pensare criticamente significa valutare informazioni e conclusioni alla luce delle evidenze, senza accettarle o respingerle automaticamente.
- **7.2 Valutare la qualità di un output**: Le dimensioni della qualità (15) · Qualità espressiva e qualità sostanziale (16) · Informazioni mancanti e omissioni (17) · Come cercare ciò che manca (18) · Incertezza e livello di fiducia (19) · Contenuti verificati e non verificati (20)
  - *Messaggio chiave:* Una risposta professionale nella forma può essere errata, incompleta o inadatta allo scopo.
- **7.3 Verifica delle informazioni e delle fonti**: Che cosa verificare: i punti critici (23) · Fonti primarie e secondarie (24) · Una fonte esistente non basta (25) · Attendibilità e fonti indipendenti (26) · Date, nomi, numeri e riferimenti (27) · Le informazioni non verificabili (28)
  - *Messaggio chiave:* Una citazione non costituisce automaticamente una prova: occorre controllare che la fonte sia autentica, pertinente e sostenga l'affermazione.
- **7.4 Valutare ragionamenti e conclusioni**: Premesse, dati e conclusioni (31) · Coerenza logica e passaggi deboli (32) · Correlazione e causalità (33) · Assunzioni e generalizzazioni indebite (34) · Alternative e omissioni nel ragionamento (35) · Conclusioni coerenti con le evidenze (36)
  - *Messaggio chiave:* Informazioni singolarmente corrette non assicurano che la conclusione tratta da esse sia giustificata.
- **7.5 Verifica di dati, calcoli e risultati quantitativi**: Dati di partenza, formule e unità (39) · Plausibilità e ordini di grandezza (40) · Dati osservati, stime e simulazioni (41) · Aggregazioni e confronti (42) · Leggere criticamente tabelle e grafici (43) · Tracciabilità e strumenti indipendenti (44)
  - *Messaggio chiave:* Un risultato quantitativo utile alle decisioni deve essere riconducibile a dati e procedimenti controllabili.
- **7.6 Tecniche di verifica e revisione assistite dall'AI**: Sei tecniche di revisione assistita (47) · Un esempio di richiesta di revisione (48) · Il confronto con altri modelli (49) · Verificare o chiedere conferma all'AI (50) · Autovalutazione e verifica indipendente (51)
  - *Messaggio chiave:* Una revisione assistita dall'AI è un supporto al controllo, non un sostituto delle evidenze indipendenti.
- **7.7 Bias cognitivi e fiducia nell'AI**: I bias che influenzano la valutazione (54) · Bias di conferma nella verifica (55) · Fluidità, sicurezza e autorevolezza (56) · Troppa fiducia, troppo poca fiducia (57) · Preservare l'autonomia cognitiva (58)
  - *Messaggio chiave:* L'affidabilità del processo dipende anche dall'atteggiamento di chi valuta il risultato e dalla capacità di riconoscere i propri bias.
- **7.8 Validazione e responsabilità nell'uso**: Plausibile, verificato, validato (61) · Adeguatezza allo scopo e conseguenze (62) · L'economia della verifica (63) · Rapporto tra costo della verifica e rischio (64) · Le incertezze residue (65) · Competenze specialistiche e decisione (66) · Documentare e assumere la responsabilità (67)
  - *Messaggio chiave:* Validare significa decidere se un output, con le verifiche appropriate e le incertezze residue, sia adeguato a uno specifico utilizzo.
- **Conclusioni**: Le domande guida: le nostre risposte (69) · Che cosa portiamo a casa (70) · Valutare, verificare, decidere: una scheda pratica (71) · Che cosa evitare (72) · Che cosa viene dopo (73) · Fonti e riferimenti (74)

### Tema 8 · AI per testi, documenti e conoscenza
*Area: Esplorare le possibilità dell'AI · 82 slide · file `Tema8_AI_testi_documenti_conoscenza.pptx` · esposizione stimata circa 1 h 32 min*

- **Introduzione**: Obiettivo del modulo (2) · Undici domande guida (3) · Il filo conduttore: quattro modalità (4) · Attività diverse, controlli diversi (5) · Il percorso del modulo (6)
- **8.1 Generazione di contenuti testuali**: Che cosa si può produrre (8) · Dalle istruzioni al testo (9) · Adattare il testo ai destinatari (10) · Tono, stile e registro (11) · Bozze e versioni alternative (12) · Automatica o supervisionata (13)
  - *Messaggio chiave:* L'AI può accelerare la produzione di contenuti, ma qualità, accuratezza e adeguatezza devono essere presidiate dal processo di revisione umano e organizzativo.
- **8.2 Revisione, riscrittura e trasformazione**: Generare o trasformare? (16) · Le principali trasformazioni (17) · Semplificare senza tradire (18) · Tradurre e localizzare (19) · Cambiare formato e struttura (20) · Modifiche formali e sostanziali (21) · Preservare il significato originale (22)
  - *Messaggio chiave:* Trasformare un testo richiede di controllare che la nuova formulazione non alteri significati, intenzioni o informazioni rilevanti.
- **8.3 Sintesi e analisi documentale**: Le possibilità su un documento (25) · Sintesi diverse per scopi diversi (26) · Tracciabilità: risalire alle fonti (27) · Riferimenti davvero controllabili (28) · Il rischio di perdita di significato (29) · Dove si perde il significato (30) · Controllare una sintesi (31) · Limiti con documenti complessi (32)
  - *Messaggio chiave:* Una sintesi utile deve rappresentare fedelmente gli elementi essenziali e consentire controlli sui contenuti originali quando richiesto dall'utilizzo previsto.
- **8.4 Estrazione e strutturazione delle informazioni**: Sintetizzare o estrarre? (35) · Che cosa si può estrarre (36) · Dal non strutturato al dato utilizzabile (37) · Classificare e trovare ricorrenze (38) · Campi mancanti o ambigui (39) · Accuratezza e completezza (40) · Dato estratto, dato validato (41)
  - *Messaggio chiave:* L'AI può rendere più utilizzabile il contenuto informativo dei documenti, ma un dato estratto non è automaticamente un dato validato.
- **8.5 Confronto e analisi di più documenti**: Tre tipi di confronto (44) · Identificare le modifiche (45) · La matrice comparativa (46) · Contraddizioni e lacune (47) · Differenze formali e sostanziali (48) · Tracciare le differenze (49)
  - *Messaggio chiave:* Un confronto documentale è utile se individua differenze rilevanti, ne distingue la natura e permette di verificarle nelle fonti.
- **8.6 Ricerca, approfondimento e organizzazione**: L'AI nel lavoro di ricerca (52) · Incorporata o recuperata? (53) · Attualità e attendibilità (54) · Organizzare: dossier e sintesi (55) · Confrontare fonti e prospettive (56) · Ricerca assistita e verifica (57)
  - *Messaggio chiave:* L'AI può sostenere ricerca e organizzazione della conoscenza, senza rendere automaticamente attendibili le informazioni trovate o generate.
- **8.7 AI e gestione della conoscenza**: Dati, informazioni, documenti (60) · Archivio o conoscenza interrogabile (61) · Come funziona per chi la usa (62) · Assistenti sulla documentazione (63) · Risposte collegate ai documenti (64) · Aggiornamento e versionamento (65) · Condizioni per risposte utili (66)
  - *Messaggio chiave:* L'AI può agevolare l'accesso alle informazioni documentali, ma non risolve da sola i problemi di organizzazione e qualità della conoscenza.
- **8.8 Limiti e condizioni di efficacia**: Caricare non significa elaborare (69) · Qualità e struttura dei documenti (70) · Digitali, scansionati, impaginati (71) · Documenti lunghi e copertura (72) · Linguaggio tecnico e riferimenti (73) · Omissioni e alterazioni (74) · Controlli proporzionati all'uso (75)
  - *Messaggio chiave:* Poter caricare un documento non garantisce che il sistema ne abbia elaborato tutte le parti, interpretato correttamente il contenuto e preservato il significato.
- **Conclusioni**: Le domande guida: le nostre risposte (77) · Che cosa portiamo a casa (78) · Quattro modalità: una scheda pratica (79) · Che cosa evitare (80) · Che cosa viene dopo (81) · Fonti e riferimenti (82)

### Tema 9 · AI per dati e analisi
*Area: Esplorare le possibilità dell'AI · 85 slide · file `Tema9_AI_dati_analisi.pptx` · esposizione stimata circa 1 h 37 min*

- **Introduzione**: Obiettivo del modulo (2) · Otto domande guida (3) · Il filo conduttore: quattro fasi (4) · Quattro tipi di analisi (5) · Il percorso del modulo (6)
- **9.1 L'AI come supporto all'analisi dei dati**: Dati, informazioni, conoscenza (8) · Analisi dei dati e BI (9) · Il ruolo dell'AI nel processo (10) · Domande in linguaggio naturale (11) · Analisi tradizionale e assistita (12) · La democratizzazione dell'analisi (13) · Competenze umane e dominio (14)
  - *Messaggio chiave:* Rendere più facile interrogare dati non equivale a rendere automaticamente corretta la loro interpretazione.
- **9.2 Comprensione, preparazione e qualità dei dati**: Tipi di dati e formati (17) · Comprendere la struttura (18) · Variabili e formati (19) · Mancanti, duplicati, anomali (20) · Pulizia e trasformazione (21) · Rappresentatività e distorsioni (22) · Definizioni e provenienza (23) · Dati, metriche e indicatori (24)
  - *Messaggio chiave:* Un dataset apparentemente ordinato non è necessariamente corretto, completo o rappresentativo del fenomeno analizzato.
- **9.3 Elaborazione e analisi quantitativa**: Le operazioni tipiche (27) · Percentuali, rapporti, variazioni (28) · Statistiche descrittive di base (29) · Le statistiche non bastano (30) · Formule e codice generati dall'AI (31) · Calcolo eseguito o numero generato (32) · Riconoscere un calcolo eseguito (33) · Tracciabilità delle operazioni (34)
  - *Messaggio chiave:* Metodo, dati e passaggi di elaborazione sono determinanti per l'affidabilità di un risultato numerico.
- **9.4 Pattern, tendenze e anomalie**: Andamenti nel tempo (37) · Anomalie e scostamenti (38) · Relazioni e correlazioni (39) · Correlazione e causalità nei dati (40) · Relazioni prive di significato (41) · Dati corretti, conclusioni sbagliate (42) · Verificare le ipotesi (43)
  - *Messaggio chiave:* Individuare una relazione nei dati non prova automaticamente l'esistenza di un nesso causale.
- **9.5 Visualizzazione e comunicazione dei risultati**: Che cosa può produrre l'AI (46) · Scegliere la rappresentazione (47) · Tabelle, dashboard e report (48) · Commenti generati e storytelling (49) · Grafici fuorvianti (50) · Dati e grafico coerenti (51) · Comunicare bene, interpretare bene (52)
  - *Messaggio chiave:* Una rappresentazione persuasiva non garantisce la validità dei dati né delle conclusioni.
- **9.6 AI, analisi predittiva e simulazioni**: Descrivere e prevedere (55) · Modelli previsionali e dati storici (56) · Stime, proiezioni, incertezza (57) · Simulazioni, scenari, what-if (58) · Le ipotesi alla base (59) · Calcolata o supposta? (60) · Validare le previsioni (61)
  - *Messaggio chiave:* Una previsione è una stima condizionata da dati, ipotesi e metodo, non una descrizione certa del futuro.
- **9.7 Interpretazione e decisioni**: Dai risultati al significato (64) · Confrontare alternative e scenari (65) · Evidenza e giudizio (66) · Analisi o raccomandazione (67) · Il rischio di falsa oggettività (68) · Assunzioni che sembrano fatti (69) · La responsabilità resta umana (70)
  - *Messaggio chiave:* La solidità di una decisione non dipende solo dalla correttezza aritmetica degli indicatori.
- **9.8 Limiti e condizioni di affidabilità**: Dove nascono gli errori (73) · Dati reali, stime, simulazioni (74) · Fondamento statistico (75) · Tracciabilità di dati ed elaborazioni (76) · L'apparenza non è affidabilità (77) · Validazione proporzionata all'uso (78)
  - *Messaggio chiave:* Un'analisi AI richiede controlli su dati, metodi e interpretazioni, proporzionati alle conseguenze dell'utilizzo.
- **Conclusioni**: Le domande guida: le nostre risposte (80) · Che cosa portiamo a casa (81) · Quattro fasi: una scheda pratica (82) · Che cosa evitare (83) · Che cosa viene dopo (84) · Fonti e riferimenti (85)

### Tema 10 · AI multimodale e creazione di contenuti
*Area: Esplorare le possibilità dell'AI · 75 slide · file `Tema10_AI_multimodale_contenuti.pptx` · esposizione stimata circa 1 h 25 min*

- **Introduzione**: Obiettivo del modulo (2) · Dieci domande guida (3) · Il filo conduttore (4) · Il percorso del modulo (5)
- **10.1 Fondamenti dell'AI multimodale**: Che cosa significa multimodale (7) · Testuali e multimodali (8) · Comprendere e generare (9) · Interazioni che combinano modalità (10) · Un modello o più modelli? (11) · Capacità che dipendono dal sistema (12)
  - *Messaggio chiave:* La multimodalità può essere realizzata con architetture differenti: capacità effettive e modalità supportate dipendono dal sistema impiegato.
- **10.2 Comprensione e analisi delle immagini**: Le possibilità su un'immagine (15) · Schermate e interfacce (16) · Diagrammi e testo nelle immagini (17) · Dettagli e relazioni spaziali (18) · Descrivere o comprendere (19) · Immagini e persone (20)
  - *Messaggio chiave:* Descrivere ciò che appare in un'immagine non equivale a comprenderne necessariamente il significato, la provenienza o il contesto.
- **10.3 Generazione e trasformazione delle immagini**: Dalla descrizione all'immagine (23) · Che cosa si può produrre (24) · Modificare immagini esistenti (25) · Applicazioni alla comunicazione (26) · Limiti di precisione e riproducibilità (27) · Requisiti professionali (28)
  - *Messaggio chiave:* La generazione visiva accelera l'esplorazione creativa ma non garantisce controllo completo, fedeltà ai riferimenti o conformità automatica a requisiti professionali.
- **10.4 AI per audio, voce e linguaggio parlato**: Le capacità vocali (31) · Riunioni, interviste, comunicazioni (32) · Errori di riconoscimento (33) · Chi ha detto che cosa (34) · Sintesi vocale e interazione (35) · Tradurre il parlato (36) · Uno strumento di accessibilità (37) · Registrare con consenso (38)
  - *Messaggio chiave:* L'accessibilità può migliorare grazie alle tecnologie vocali, ma trascrizioni e traduzioni richiedono controlli adeguati di accuratezza e contesto.
- **10.5 AI per comprensione e generazione video**: Comprendere i video (41) · Generare e modificare video (42) · Documentale o sintetico (43)
  - *Messaggio chiave:* Coerenza visiva e plausibilità di una sequenza video non dimostrano che gli eventi rappresentati siano realmente accaduti.
- **10.6 Presentazioni e materiali di comunicazione**: Dal testo alle slide (46) · Adattare ai destinatari (47) · Coerenza tra testo e visivo (48) · Estetica e accuratezza (49) · Valutare la qualità comunicativa (50)
  - *Messaggio chiave:* L'efficacia estetica di un materiale non garantisce accuratezza, completezza né coerenza narrativa.
- **10.7 Integrazione e trasformazione tra modalità**: La mappa delle conversioni (53) · Le catene di trasformazione (54) · Combinare più fonti (55) · Conversioni per l'accessibilità (56) · Coerenza tra modalità (57) · Confrontare con l'origine (58)
  - *Messaggio chiave:* Il valore delle conversioni è legato alla loro utilità e alla fedeltà delle informazioni, non soltanto alla comodità o alla rapidità del processo.
- **10.8 Limiti, autenticità e affidabilità**: Gli errori tipici (61) · Contenuti sintetici e deepfake (62) · Realismo, autenticità, accuratezza (63) · Provenienza e verifica (64) · Difendersi dalle frodi (65) · Comunicazione fuorviante (66) · Diritti su contenuti, immagini, voci (67) · Verifica e supervisione (68)
  - *Messaggio chiave:* Distinguere realismo, provenienza e accuratezza è essenziale per utilizzare in modo critico i contenuti multimodali.
- **Conclusioni**: Le domande guida: le nostre risposte (70) · Che cosa portiamo a casa (71) · Una scheda pratica (72) · Che cosa evitare (73) · Che cosa viene dopo (74) · Fonti e riferimenti (75)

### Tema 11 · Assistenti, agenti e automazioni con l'AI
*Area: Esplorare le possibilità dell'AI · 77 slide · file `Tema11_Assistenti_agenti_automazioni.pptx` · esposizione stimata circa 1 h 30 min*

- **Introduzione**: Obiettivo del modulo (2) · Nove domande guida (3) · Il filo conduttore (4) · Chatbot, assistenti, agenti, automazioni (5) · Il percorso del modulo (6)
- **11.1 Dalla conversazione all'azione**: Dai chatbot agli assistenti (8) · Assistenti integrati e copilot (9) · Suggerire, preparare, eseguire (10) · Capacità e limiti degli assistenti (11) · Nomi commerciali e funzionalità (12)
  - *Messaggio chiave:* Non tutti gli assistenti AI possono eseguire azioni: occorre distinguere ciò che il sistema può proporre da ciò che può realmente fare.
- **11.2 Strumenti, integrazioni e capacità operative**: Modello e sistema con strumenti (15) · Che cosa possono fare gli strumenti (16) · Leggere o modificare (17) · Identità, autorizzazioni, permessi (18) · Disponibile non è autorizzato (19) · Il contesto disponibile (20)
  - *Messaggio chiave:* La capacità di compiere operazioni dipende dagli strumenti e dai permessi realmente disponibili, non soltanto dalle capacità del modello linguistico.
- **11.3 Che cosa sono gli agenti AI**: Una definizione funzionale (23) · Il ciclo di un agente (24) · Un esempio passo per passo (25) · Agente, chatbot, workflow (26) · Limiti e incertezza (27) · L'accumulo degli errori (28) · Come si propaga un errore (29) · Gradi di autonomia operativa (30)
  - *Messaggio chiave:* Gli errori intermedi possono influenzare le operazioni successive: il successo di un singolo passaggio non garantisce l'affidabilità del processo completo.
- **11.4 Automazione tradizionale e intelligente**: Che cosa significa automatizzare (33) · La Robotic Process Automation (34) · L'AI nei processi automatizzati (35) · Regole e AI insieme (36) · Tre dimensioni distinte (37) · Quando l'AI non serve (38)
  - *Messaggio chiave:* Un processo può essere completamente automatizzato senza AI; un agente può effettuare scelte dinamiche pur richiedendo interventi umani.
- **11.5 Livelli di autonomia e supervisione umana**: Dalla risposta all'azione (41) · I livelli operativi di autonomia (42) · Nel ciclo o sul ciclo (43) · Punti di approvazione (44) · Interrompere, correggere, annullare (45) · Reversibili e irreversibili (46) · Controlli proporzionati al rischio (47)
  - *Messaggio chiave:* Dalla risposta all'azione cambia la natura del rischio: un'azione può avere conseguenze dirette su dati, comunicazioni e processi, anche difficili da annullare.
- **11.6 Attività e processi supportabili**: Che cosa si può supportare (50) · Un compito o un processo (51) · Eccezioni e casi non previsti (52) · Le attività più adatte (53) · Dalla dimostrazione all'esercizio (54)
  - *Messaggio chiave:* La riuscita di un'attività dimostrativa non equivale alla capacità di ripeterla in modo affidabile e continuativo in azienda.
- **11.7 Collaborazione tra persone, assistenti e agenti**: Distribuire il lavoro (57) · Ruoli delle persone (58) · Visibilità e consegne (59) · Più agenti e casi non previsti (60) · Chi risponde del risultato (61)
  - *Messaggio chiave:* Gli agenti sono componenti di un sistema di lavoro: il loro valore dipende anche dall'integrazione con attività, competenze e responsabilità umane.
- **11.8 Limiti, rischi e condizioni di affidabilità**: La mappa dei rischi (64) · Istruzioni nascoste nei contenuti (65) · Tracciabilità e verifica degli esiti (66) · Fallimenti e robustezza (67) · Monitorare e recuperare (68) · Prototipo o sistema affidabile (69) · Limiti operativi e supervisione (70)
  - *Messaggio chiave:* Le azioni possono produrre conseguenze dirette; gli errori intermedi possono accumularsi; un prototipo dimostrativo non prova l'affidabilità in esercizio.
- **Conclusioni**: Le domande guida: le nostre risposte (72) · Che cosa portiamo a casa (73) · Prima di affidare un'attività (74) · Che cosa evitare (75) · Che cosa viene dopo (76) · Fonti e riferimenti (77)

### Tema 12 · AI e creazione di valore per l'azienda
*Area: Comprendere il valore per l'azienda · 72 slide · file `Tema12_AI_creazione_valore_azienda.pptx` · esposizione stimata circa 1 h 22 min*

- **Introduzione**: Obiettivo del modulo (2) · Tre equivalenze da evitare (3) · Nove domande guida (4) · Il filo conduttore (5) · Il percorso del modulo (6)
- **12.1 Che cosa significa creare valore con l'AI**: Dalla capacità al valore (8) · L'AI come mezzo (9) · Per chi e a quale livello (10) · Percepito o effettivo (11) · Adozione non è impatto (12)
  - *Messaggio chiave:* Il valore non deriva dalla disponibilità di uno strumento, ma dal suo contributo a un obiettivo concreto e rilevante.
- **12.2 Le principali dimensioni del valore**: Una mappa delle dimensioni (15) · Tangibili e intangibili (16) · Compromessi tra dimensioni (17) · Un esempio con più dimensioni (18)
  - *Messaggio chiave:* Il valore è multidimensionale e non coincide soltanto con riduzione dei costi o risparmio di tempo.
- **12.3 AI, efficienza e produttività del lavoro**: Dove l'AI fa risparmiare tempo (21) · Efficienza e produttività (22) · Risparmiato o recuperato (23) · Il paradosso della produttività (24) · Valorizzare la capacità liberata (25) · Colli di bottiglia (26) · Individuale e organizzativa (27) · Che cosa dicono alcuni studi (28) · Velocità, qualità, carichi (29)
  - *Messaggio chiave:* Un risparmio di tempo locale non implica un beneficio equivalente per l'organizzazione; accelerare un'attività non migliora il processo se il collo di bottiglia è altrove.
- **12.4 AI, qualità e miglioramento delle prestazioni**: Dove migliora la qualità (32) · Qualità apparente ed effettiva (33) · Il rischio di errori sistematici (34) · Criteri osservabili (35)
  - *Messaggio chiave:* L'AI può migliorare alcune dimensioni della qualità ma introdurre nuovi errori: occorrono criteri osservabili per valutarne l'effetto.
- **12.5 AI come amplificatore delle competenze**: Persone con esperienze diverse (38) · Fare cose prima impossibili (39) · Competenze umane e capacità AI (40) · Dipendenza e competenze (41) · Amplificare o sostituire (42)
  - *Messaggio chiave:* Il valore dell'AI può derivare dal fare cose prima impossibili: alcuni benefici non sono risparmi di tempo, ma l'accesso ad attività prima troppo difficili, costose o poco praticabili.
- **12.6 AI, innovazione e nuove opportunità**: Ottimizzare o innovare (45) · Le forme dell'innovazione (46) · Fattibile non vuol dire desiderato (47) · Verificare la domanda reale (48)
  - *Messaggio chiave:* La possibilità tecnica di realizzare un nuovo servizio non dimostra da sola che il mercato lo desideri o che sia economicamente sostenibile.
- **12.7 Costi, compromessi e condizioni**: Diretti, indiretti, nascosti (51) · Il costo nascosto (52) · La curva dell'adozione (53) · Le condizioni per generare valore (54) · Beneficio lordo e beneficio netto (55) · Benefici locali, vincoli del processo (56)
  - *Messaggio chiave:* Il costo nascosto dell'AI: il prezzo dello strumento è soltanto una componente; occorre considerare formazione, controlli, errori, manutenzione e adattamenti operativi.
- **12.8 Dal valore potenziale al valore misurabile**: Ipotizzato, percepito, misurato (59) · Obiettivi e situazione iniziale (60) · Indicatori di risultato (61) · Con e senza AI (62) · Verso il beneficio netto (63) · Limiti delle misurazioni (64) · Adozione e impatto, di nuovo (65)
  - *Messaggio chiave:* Verificare che il tempo risparmiato si traduca in un beneficio effettivamente valorizzato, includendo i costi necessari per ottenere e mantenere il risultato.
- **Conclusioni**: Le domande guida: le nostre risposte (67) · Che cosa portiamo a casa (68) · Domande sul valore (69) · Che cosa evitare (70) · Che cosa viene dopo (71) · Fonti e riferimenti (72)

### Tema 13 · AI e trasformazione del lavoro e dei processi
*Area: Comprendere il valore per l'azienda · 64 slide · file `Tema13_AI_trasformazione_lavoro_processi.pptx` · esposizione stimata circa 1 h 14 min*

- **Introduzione**: Obiettivo del modulo (2) · Compito, processo, ruolo (3) · Nove domande guida (4) · Il filo conduttore (5) · Il percorso del modulo (6)
- **13.1 Come l'AI modifica la natura del lavoro**: Attività, compiti, mansioni, ruoli (8) · Tipi di lavoro (9) · Assistite, automatizzate, trasformate (10) · Il compito non è il ruolo (11) · Esposizione e trasformazione (12) · Effetti diversi, scelte decisive (13)
  - *Messaggio chiave:* Le capacità tecniche dell'AI non consentono, da sole, di dedurre effetti certi su professioni o occupazione.
- **13.2 Individuare le attività trasformabili**: Scomporre il lavoro in attività (16) · Le caratteristiche delle attività (17) · Informazioni, rischio, controllo (18) · Fattibile o trasformabile? (19)
  - *Messaggio chiave:* Non tutte le attività sono ugualmente adatte all'AI: qualità delle informazioni, variabilità, contesto, rischio e organizzazione ne condizionano l'applicazione.
- **13.3 Dal compito al processo**: Compito e processo (22) · Un processo trasformato (23) · Che cosa cambia nel processo (24) · Automatizzare l'inefficienza (25) · La trasformazione crea nuovo lavoro (26) · Ottimizzare o trasformare (27)
  - *Messaggio chiave:* Introdurre AI in un processo non equivale automaticamente a riprogettarlo o migliorarlo.
- **13.4 Collaborazione tra persone e AI**: Strumento personale o di processo (30) · Distribuire il lavoro (31) · Dall'esecuzione alla supervisione (32) · Autonomia e responsabilità (33)
  - *Messaggio chiave:* Le persone possono spostarsi verso interpretazione, verifica e supervisione, senza che questo elimini il bisogno di competenze professionali.
- **13.5 Evoluzione dei ruoli e delle responsabilità**: La composizione delle mansioni (36) · Competenze che cambiano peso (37) · Nuove attività e responsabilità (38) · Il supervisore inesperto (39) · Compiti e occupazione (40)
  - *Messaggio chiave:* Le conseguenze sui ruoli non sono predeterminate dalla tecnologia.
- **13.6 AI e collaborazione nei team e tra funzioni**: Dove la collaborazione migliora (43) · Usi diversi, frammentazione (44) · Individuale e collettivo (45)
  - *Messaggio chiave:* Un miglioramento individuale non produce automaticamente maggiore efficacia del team: il coordinamento rimane essenziale.
- **13.7 Competenze e modi di lavorare**: Le competenze per lavorare con l'AI (48) · Strumento o modo di lavorare (49) · La perdita delle competenze (50) · Meno pratica, più supervisione (51)
  - *Messaggio chiave:* Supervisione efficace e autonomia professionale richiedono competenze da preservare e sviluppare.
- **13.8 Condizioni e rischi della trasformazione**: Adozione e trasformazione effettiva (54) · Effetti inattesi sul lavoro (55) · Rischi strutturali (56) · Osservare il lavoro reale (57)
  - *Messaggio chiave:* L'impatto dell'AI va valutato osservando l'intero lavoro effettivamente svolto, non solo le prestazioni degli strumenti.
- **Conclusioni**: Le domande guida: le nostre risposte (59) · Che cosa portiamo a casa (60) · Domande sul cambiamento del lavoro (61) · Che cosa evitare (62) · Che cosa viene dopo (63) · Fonti e riferimenti (64)

### Tema 14 · AI, dati e conoscenza aziendale
*Area: Comprendere il valore per l'azienda · 78 slide · file `Tema14_AI_dati_conoscenza_aziendale.pptx` · esposizione stimata circa 1 h 26 min*

- **Introduzione**: Obiettivo del modulo (2) · Quattro condizioni distinte (3) · Otto domande guida (4) · Il filo conduttore (5) · Il percorso del modulo (6)
- **14.1 Il patrimonio informativo**: Dai dati alla conoscenza (8) · Strutturate e non strutturate (9) · Che cosa contiene il patrimonio (10) · Formalizzata e tacita (11) · Informazioni distribuite (12) · Possedere non è poter usare (13) · Il ruolo del patrimonio nell'AI (14)
  - *Messaggio chiave:* Avere molti dati non significa avere dati utilizzabili. E una parte della conoscenza aziendale non è scritta da nessuna parte.
- **14.2 Qualità e aggiornamento**: Le dimensioni della qualità (17) · Duplicati e contraddizioni (18) · Il problema dell'obsolescenza (19) · Parole diverse, stesse cose (20) · Provenienza e autorevolezza (21) · Chi aggiorna che cosa (22) · Che cosa l'AI non compensa (23)
  - *Messaggio chiave:* La quantità delle informazioni non compensa errori, incoerenze, lacune o obsolescenza. L'AI ha accesso alle fonti, non alla realtà.
- **14.3 Organizzazione e accessibilità**: Archivi e repository (26) · Classificazione e metadati (27) · Trovare e riconoscere la versione (28) · Frammentazione e silos (29) · Archivio o base di conoscenza (30) · I limiti della documentazione (31)
  - *Messaggio chiave:* Un'informazione che non si trova, o che non si distingue da quelle superate, è come se non ci fosse. E i documenti non contengono tutto ciò che l'azienda sa.
- **14.4 L'AI e le informazioni aziendali**: Modello e azienda (34) · Tre modi di fornire informazioni (35) · Il recupero, in sintesi (36) · Recuperare o modificare il modello (37) · Istruzioni, contesto e fonti (38) · Quando il recupero sbaglia (39) · Accessibili, recuperate, usate (40)
  - *Messaggio chiave:* Il modello non conosce l'azienda: legge le fonti che gli vengono recuperate. E ciò che è accessibile non è ciò che viene davvero usato nella risposta.
- **14.5 Integrazione con i sistemi**: Le applicazioni aziendali (43) · Documenti o dati operativi (44) · Leggere o anche modificare (45) · Integrazioni e interoperabilità (46) · Collegare non è aprire tutto (47)
  - *Messaggio chiave:* Collegare un'applicazione all'AI non significa aprirle tutto ciò che contiene.
- **14.6 Accessi, permessi e disponibilità**: Esistere non è essere autorizzati (50) · Livelli di classificazione (51) · Ruoli e minimo privilegio (52) · I permessi di chi? (53) · Il rischio di esposizione (54) · Separare i contesti (55) · Tracciabilità ed equilibrio (56)
  - *Messaggio chiave:* L'AI non deve sapere tutto ciò che l'azienda sa. Deve poter consultare soltanto ciò che è pertinente e autorizzato per il caso d'uso.
- **14.7 Affidabilità delle risposte**: Lo scenario: cinque modi di sbagliare (59) · Pertinenza e completezza (60) · Recuperato o interpretato? (61) · Contraddizioni e assenze (62) · Citare le fonti (63) · Apparentemente fondate (64) · Adeguata allo scopo (65)
  - *Messaggio chiave:* Una fonte corretta non garantisce una risposta corretta: il recupero può fallire, l'interpretazione può sbagliare, e ciò che manca non si vede.
- **14.8 Condizioni per valorizzare i dati**: Tre famiglie di condizioni (68) · Prototipo o servizio (69) · Gli ostacoli principali (70) · Partire dal caso d'uso (71)
  - *Messaggio chiave:* L'efficacia non richiede accesso illimitato, ma disponibilità mirata e controllata delle informazioni, curata nel tempo.
- **Conclusioni**: Le domande guida: le nostre risposte (73) · Che cosa portiamo a casa (74) · Domande su un assistente aziendale (75) · Che cosa evitare (76) · Che cosa viene dopo (77) · Fonti e riferimenti (78)

### Tema 15 · Individuazione e valutazione delle opportunità AI
*Area: Comprendere il valore per l'azienda · 76 slide · file `Tema15_Opportunita_valutazione_AI.pptx` · esposizione stimata circa 1 h 20 min*

- **Introduzione**: Obiettivo del modulo (2) · Dal bisogno, non dallo strumento (3) · Otto domande guida (4) · Il filo conduttore (5) · Il percorso del modulo (6) · Lo scenario del modulo (7)
- **15.1 Partire dai problemi**: Dal problema alla soluzione (9) · Dove cercare i problemi (10) · Il risultato desiderato (11) · Cause e sintomi (12) · Le alternative non AI (13) · Partire dalla tecnologia (14)
  - *Messaggio chiave:* Prima di scegliere l'AI occorre comprendere il problema, e chiedersi se una soluzione tradizionale, organizzativa o semplice non sia più adatta.
- **15.2 Descrivere un caso d'uso**: Che cos'è un caso d'uso (17) · Gli elementi della descrizione (18) · Un esempio compilato (19) · Idea generica o caso definito (20) · Le ipotesi da verificare (21)
  - *Messaggio chiave:* Un caso d'uso specifica chi svolge quale attività, su quali informazioni, con quale contributo dell'AI e per quale risultato. Il resto è ancora un'idea.
- **15.3 Opportunità promettenti**: Segnali di potenziale (24) · Profilo di un'opportunità (25) · Supporto o automazione parziale (26) · Complessità o utilità (27) · Alternative più semplici (28)
  - *Messaggio chiave:* L'opportunità più promettente non è necessariamente la più complessa o impressionante: una soluzione limitata e controllabile può generare più valore.
- **15.4 Il valore potenziale**: I benefici attesi (31) · Frequenza, volumi, diffusione (32) · Teorico o ottenibile? (33) · I costi da considerare (34) · Desiderabilità (35) · Benefici e costi, in sintesi (36)
  - *Messaggio chiave:* Un beneficio potenziale conta se è rilevante per il bisogno reale, realisticamente ottenibile, e superiore ai costi completi, anche con ipotesi prudenti.
- **15.5 Fattibilità tecnica e organizzativa**: Le domande della fattibilità (39) · Dati e integrazioni (40) · Tecnica, organizzativa, economica (41) · Fornitori e manutenzione (42) · Prototipo e uso operativo (43) · Alternative tecnologiche (44)
  - *Messaggio chiave:* Fattibilità tecnica, adozione organizzativa e sostenibilità economica non coincidono: una dimostrazione che funziona non basta.
- **15.6 Rischi e condizioni di controllo**: Che cosa può andare storto (47) · Supervisione e reversibilità (48) · Intrinseco e residuo (49) · Condizioni di esclusione (50) · Escludere o riprogettare (51)
  - *Messaggio chiave:* Alcuni rischi e vincoli sono condizioni di esclusione: un alto beneficio stimato non li rende automaticamente accettabili.
- **15.7 Confronto e priorità**: Individuare non è selezionare (54) · Criteri espliciti (55) · La matrice valore-fattibilità (56) · Quick win e strategiche (57) · I limiti dei punteggi (58) · Approfondire o investire? (59)
  - *Messaggio chiave:* Prioritizzare aiuta a decidere che cosa approfondire; non dimostra la convenienza di un investimento. E le condizioni non negoziabili stanno fuori dal punteggio.
- **15.8 Dall'idea alla verifica**: Ipotesi o risultato (62) · Assunzioni critiche (63) · Verifiche e sperimentazioni (64) · Successo e insuccesso, prima (65) · Il confronto giusto (66) · Cercare le evidenze contrarie (67) · Tre decisioni possibili (68) · Dimostrazione o validazione (69)
  - *Messaggio chiave:* La sperimentazione deve poter smentire l'idea iniziale: lo scopo di un test è imparare, non dimostrare a ogni costo che l'idea era valida.
- **Conclusioni**: Le domande guida: le nostre risposte (71) · Che cosa portiamo a casa (72) · La scheda dell'opportunità (73) · Che cosa evitare (74) · Che cosa viene dopo (75) · Fonti e riferimenti (76)

### Tema 16 · Adozione dell'AI e cambiamento organizzativo
*Area: Comprendere il valore per l'azienda · 76 slide · file `Tema16_Adozione_AI_cambiamento_organizzativo.pptx` · esposizione stimata circa 1 h 21 min*

- **Introduzione**: Obiettivo del modulo (2) · Dalla disponibilità al valore (3) · Otto domande guida (4) · Il filo conduttore (5) · Il percorso del modulo (6) · Lo scenario del modulo (7)
- **16.1 Che cosa significa adottare**: Disponibile, usato, adottato (9) · Individuale, team, organizzazione (10) · Spontanea o coordinata (11) · Utenti, qualità, impatto (12) · Un percorso, non un evento (13) · Lo Shadow AI (14) · Dal basso non è Shadow AI (15)
  - *Messaggio chiave:* Acquistare licenze e registrare accessi non equivale ad adottare l'AI: conta l'integrazione appropriata nel lavoro.
- **16.2 Fattori e ostacoli**: Utile e facile (18) · La mappa dei fattori (19) · Il tempo e le prime esperienze (20) · Quattro tipi di ostacoli (21) · Differenze tra gruppi (22) · Individuale o strutturale? (23) · Che cosa ci dicono i segnali (24)
  - *Messaggio chiave:* Una bassa adozione può dipendere dallo strumento o dalle condizioni operative, non dalla scarsa apertura al cambiamento.
- **16.3 Leadership e management**: Direzione: perché e verso dove (27) · I manager: creare condizioni (28) · Coerenza tra parole e priorità (29) · Incoraggiare o imporre (30) · Aspettative realistiche (31) · Una responsabilità condivisa (32)
  - *Messaggio chiave:* La leadership non deve solo promuovere l'AI: deve contribuire a rendere possibile il suo uso appropriato e utile.
- **16.4 Competenze e formazione**: Generali e per ruolo (35) · Le competenze che restano (36) · Come si impara davvero (37) · Dall'aula al lavoro (38) · Sapere, saper fare, fare (39) · Dopo la formazione (40)
  - *Messaggio chiave:* Un corso introduttivo avvia l'apprendimento: la competenza operativa si consolida con l'applicazione, il confronto e il supporto nel lavoro.
- **16.5 Sperimentazione e diffusione**: Dimostrazione, pilota, estensione (43) · Il ciclo del pilota (44) · Pratiche replicabili (45) · Locale o replicabile? (46) · I rischi della fretta (47)
  - *Messaggio chiave:* Un pilota riuscito non è automaticamente pronto per tutta l'organizzazione: si estende quando le condizioni del successo sono presenti anche altrove.
- **16.6 Cultura, fiducia, partecipazione**: Atteggiamenti diversi (50) · Fiducia informata (51) · Poter parlare di ciò che non va (52) · Opposizione o obiezione fondata? (53) · Partecipazione (54)
  - *Messaggio chiave:* Una cultura favorevole all'AI promuove confronto e fiducia informata, non entusiasmo obbligatorio. E le obiezioni sono spesso informazioni.
- **16.7 Supporto e coordinamento**: Che cosa si può usare, e come (57) · Materiali e referenti (58) · Raccogliere e coordinare (59) · Autonomia e pratiche comuni (60) · Gestire gli usi non autorizzati (61)
  - *Messaggio chiave:* L'autonomia individuale è più efficace quando esistono riferimenti operativi chiari e canali di aiuto accessibili.
- **16.8 Monitoraggio e sostenibilità**: Diffusione, intensità, qualità (64) · Adozione o impatto? (65) · Che cosa osservare (66) · Diffondere non è adottare (67) · Sostenibile nel tempo (68) · Che cosa decidere (69)
  - *Messaggio chiave:* Monitorare significa osservare non soltanto quanto l'AI viene usata, ma come, perché e con quali risultati. Diffondere rapidamente non è adottare efficacemente.
- **Conclusioni**: Le domande guida: le nostre risposte (71) · Che cosa portiamo a casa (72) · Domande per un'iniziativa di adozione (73) · Che cosa evitare (74) · Che cosa viene dopo (75) · Fonti e riferimenti (76)

### Tema 17 · Utilizzo consapevole e responsabile dell'AI
*Rischi, sicurezza e tutela delle informazioni · Area: Utilizzare l'AI responsabilmente · 75 slide · file `Tema17_Utilizzo_responsabile_rischi_sicurezza.pptx` · esposizione stimata circa 1 h 22 min*

- **Introduzione**: Obiettivo del modulo (2) · Da che cosa dipende il rischio (3) · Otto domande guida (4) · Il filo conduttore (5) · Il percorso del modulo (6)
- **17.1 Che cosa significa uso responsabile**: Può fare, è opportuno farle fare (8) · Chi può essere coinvolto (9) · Errore, danno, rischio (10) · Livelli di criticità (11) · Giudizio e responsabilità (12) · Proporzione, non rinuncia (13)
  - *Messaggio chiave:* Usare l'AI responsabilmente significa chiedersi non solo che cosa può fare, ma che cosa è opportuno farle fare, qui, con queste informazioni e queste conseguenze.
- **17.2 Protezione dei dati e riservatezza**: Quali informazioni (16) · Che cosa succede ai dati (17) · Condizioni e loro limiti (18) · Minimizzare (19) · Anonimo, pseudonimo, oscurato (20) · Esempio A: identificabile lo stesso (21) · Accedere non è poter divulgare (22) · Esempio D: attraverso la risposta (23)
  - *Messaggio chiave:* Prima di inserire informazioni: di che tipo sono, sono autorizzato, in quale strumento? E prima di condividere una risposta: che cosa contiene, e chi la riceve?
- **17.3 Sicurezza e rischi specifici**: Riservatezza e sicurezza (26) · Il prompt injection (27) · Esempio B: istruzioni nascoste (28) · Istruzioni e dati (29) · Che cosa può succedere (30) · Autorizzazioni e credenziali (31) · Notare, verificare, segnalare (32) · I limiti della prudenza (33)
  - *Messaggio chiave:* Un documento da analizzare non è una fonte di istruzioni. E la prudenza individuale è necessaria ma non sufficiente: servono controlli tecnici e organizzativi.
- **17.4 Bias, discriminazioni ed equità**: Che cos'è un bias (36) · Stereotipi e prestazioni diverse (37) · Discriminazione diretta e indiretta (38) · Plausibile, fondato, equo (39) · Situazioni sensibili (40) · Segnali e limiti della rilettura (41)
  - *Messaggio chiave:* Un output automatico non è necessariamente imparziale: le distorsioni possono venire dai dati, dal modello, dal problema posto o dal contesto d'impiego.
- **17.5 Trasparenza e contenuti sintetici**: Realistico non è autentico (44) · Deepfake e impersonificazione (45) · Comunicare senza ingannare (46) · Verificare provenienza e contesto (47)
  - *Messaggio chiave:* Realistico non significa autentico: evitare di produrre comunicazioni ingannevoli, e di fidarsi in modo acritico di contenuti plausibili.
- **17.6 Proprietà intellettuale**: Possedere non è poter usare (50) · Che cosa si dà all'AI (51) · Generabile non è impiegabile (52) · Condizioni, licenze, verifiche (53)
  - *Messaggio chiave:* I contenuti generati non sono automaticamente liberi da vincoli: dipende dai materiali di origine, dai servizi e dalle finalità d'uso.
- **17.7 Controllo umano e responsabilità**: Supporto o decisione (56) · Automation bias (57) · Quattro condizioni del controllo (58) · Esempio C: supervisione formale (59) · Controllo proporzionato (60) · Fermare e capire (61)
  - *Messaggio chiave:* La presenza di una persona nel processo non garantisce una supervisione efficace: servono competenze, informazioni, tempo e potere effettivo di intervento.
- **17.8 Buone pratiche per un uso sicuro**: Prima dell'uso (64) · Durante l'uso (65) · Dopo l'uso (66) · Quattro azioni possibili (67) · La checklist essenziale (68)
  - *Messaggio chiave:* L'uso responsabile deriva da comportamenti quotidiani, dalla valutazione del contesto e dalla capacità di riconoscere quando fermarsi.
- **Conclusioni**: Le domande guida: le nostre risposte (70) · Che cosa portiamo a casa (71) · I quattro esempi, in sintesi (72) · Che cosa evitare (73) · Che cosa viene dopo (74) · Fonti e riferimenti (75)

### Tema 18 · Normativa, regole e governance dell'AI
*Area: Utilizzare l'AI responsabilmente · 77 slide · file `Tema18_Normativa_regole_governance_AI.pptx` · esposizione stimata circa 1 h 31 min*

- **Introduzione**: Prima di cominciare (2) · Obiettivo del modulo (3) · Tre piani da distinguere (4) · Otto domande guida (5) · Il filo conduttore (6) · Il percorso del modulo (7)
- **18.1 Perché serve una governance**: Che cos'è la governance dell'AI (9) · Principi di riferimento (10) · Conformità e governo (11) · Il prezzo dell'assenza (12) · Lungo tutto il ciclo di vita (13) · Abilitante e proporzionata (14)
  - *Messaggio chiave:* Governare l'AI significa definire condizioni, responsabilità e verifiche che consentano usi appropriati e controllabili.
- **18.2 Il quadro normativo**: L'AI Act: obiettivi e impostazione (17) · Le grandi categorie di obblighi (18) · Un'applicazione progressiva (19) · AI Act e GDPR (20) · Non solo AI Act (21) · Il quadro italiano (22) · Che cosa obbliga, che cosa orienta (23)
  - *Messaggio chiave:* L'AI Act è centrale, ma non sostituisce le altre norme applicabili: GDPR, lavoro, consumatori, diritto d'autore, discipline settoriali, legge nazionale.
- **18.3 L'approccio basato sul rischio**: La logica della piramide (26) · Le pratiche vietate (27) · L'alto rischio (28) · Che cosa comporta l'alto rischio (29) · La finalità decide (30) · Esempio B: la selezione (31) · Trasparenza e modelli generali (32) · Generativa non è alto rischio (33)
  - *Messaggio chiave:* Il regime applicabile dipende dalla finalità e dalla qualificazione giuridica, non dalla presenza di un modello avanzato. E non essere ad alto rischio non significa non avere rischi né obblighi. Sotto
- **18.4 Ruoli e responsabilità**: I ruoli della filiera (36) · Le responsabilità del deployer (37) · Esempio A: il prodotto 'conforme' (38) · Quando cambia il ruolo (39) · Documentazione e contratti (40) · Chi fa che cosa, all'interno (41)
  - *Messaggio chiave:* Impiegare sistemi di terzi non elimina le responsabilità dell'organizzazione: il fornitore risponde di come il sistema è fatto, il deployer di come lo usa.
- **18.5 Politiche aziendali**: A che cosa serve una policy (44) · Gli elementi di una policy (45) · Quattro categorie di uso (46) · Scritta o praticata (47) · Un esempio di policy essenziale (48)
  - *Messaggio chiave:* Una policy è utile quando orienta decisioni e comportamenti concreti, non soltanto quando esiste come documento.
- **18.6 Rischi, controlli e supervisione**: Sapere che cosa c'è (51) · Valutare i rischi nel contesto (52) · Prevenire, rilevare, correggere (53) · Supervisione progettata (54) · Tracciare e gestire incidenti (55) · Riesame e rischio residuo (56)
  - *Messaggio chiave:* I controlli sono efficaci quando funzionano nella pratica e sono mantenuti nel tempo, non soltanto quando risultano descritti.
- **18.7 AI literacy e responsabilità**: Che cos'è l'AI literacy (59) · L'articolo 4, prima e dopo (60) · Misure commisurate (61) · Esempio C: il corso completato (62)
  - *Messaggio chiave:* Un corso di AI Awareness contribuisce all'alfabetizzazione, ma non equivale automaticamente alla conformità: le misure vanno commisurate a persone, ruoli, sistemi e contesti.
- **18.8 Una governance proporzionata**: I presidi essenziali (65) · Esempio D: aziende diverse (66) · Framework e standard volontari (67) · Formazione e governance (68) · La checklist essenziale (69) · Migliorare nel tempo (70)
  - *Messaggio chiave:* Non esiste un modello organizzativo unico, ma è necessario rispettare gli obblighi pertinenti e rendere effettivi i controlli scelti.
- **Conclusioni**: Le domande guida: le nostre risposte (72) · Che cosa portiamo a casa (73) · Quattro equivoci, quattro esempi (74) · Che cosa evitare (75) · Il percorso completato (76) · Fonti e riferimenti (77)

---

## 10. Mappa dei collegamenti tra temi

Serve all'agente per i controlli (attività A1, A2, A4) e per progettare le formazioni derivate (attività D): quando si selezionano slide o moduli, verificare qui che nessun concetto usato dia per scontato un tema escluso. Va compilata tema per tema durante la revisione. Nei deck i rimandi stanno solo nelle note (regola 11).

### Tema 1 (compilato il 9 ottobre 2026)
**Prerequisiti:** nessuno. **Concetti introdotti e ripresi in seguito:** software deterministico e sistemi probabilistici; digitalizzazione, automazione e AI; potenziale tecnologico e valore realizzato; frontiera frastagliata; possibile, affidabile, conveniente.

| Concetto | Nel Tema 1 | Approfondito o ripreso in |
|---|---|---|
| Funzionamento degli LLM, parametri, Transformer, apprendimento dai dati | accennato (1.1, 1.2) | Tema 2 |
| AGI | menzionata (1.1, 1.6) | Tema 2 (2.1) |
| AI predittiva, discriminativa e generativa | accennata (1.3) | Tema 2 (2.2) |
| Variabilità e sistemi probabilistici | introdotto (1.4) | Tema 2 (2.7), Tema 3 |
| Errori, allucinazioni, bias, affidabilità | accennato (1.6) | Tema 3; verifica nel Tema 7 |
| Prodotti, modelli e piattaforme | escluso | Tema 4 |
| Dialogo con l'AI e formulazione delle richieste | accennato (1.3) | Temi 5 e 6 |
| Applicazioni per tipo di attività | esempi indicativi (1.5) | Temi 8-11 |
| Valore, costi, ROI | potenziale e valore (1.5) | Temi 12 e 15 |
| Dati aziendali | accennato (1.2) | Tema 14 |
| Individuazione delle opportunità | accennato (1.5) | Tema 15 |
| Strategia e adozione | accennato (1.5) | Temi 12, 15 e 16 |
| Hype cycle | trattato (1.6) | richiamato nel Tema 16 (16.3, solo nelle note) |
| Studio Brynjolfsson (QJE 2025) | esempio (1.5) | Tema 12 |
| Studio Dell'Acqua (Organization Science 2026) | esempio (1.6) | Temi 3 e 12 |
| Shadow AI | accennato (1.5) | Temi 16, 17 e 18 |
| Rischi e regole d'uso | accennato (1.6) | Temi 17 e 18 |

### Tema 2 (compilato il 9 ottobre 2026)
**Prerequisiti:** nessuno obbligatorio; riprende brevemente dal Tema 1 AI simbolica e Machine Learning, retropropagazione, software deterministico e sistemi probabilistici. **Concetti introdotti e ripresi in seguito:** addestramento e inferenza; parametri; token e finestra di contesto; contesto temporaneo e memoria persistente; modello e applicazione; tre fonti di informazione; grounding e RAG; fine-tuning; data limite (cutoff); temperatura e variabilità.

| Concetto | Nel Tema 2 | Approfondito o ripreso in |
|---|---|---|
| Definizione di sistema di AI (AI Act, art. 3) | definizione operativa (2.1) | Tema 18 |
| AGI | trattata (2.1) | dibattito nel Tema 1 (1.6) |
| Antropomorfizzazione, effetto ELIZA | trattato (2.1) | Tema 5 (5.7) |
| Bias dai dati di addestramento | accennato (2.3) | Temi 3 e 17 |
| Uso delle conversazioni da parte del fornitore, memoria | accennato (2.3, 2.5, 2.6) | Temi 14 e 17; confronto tra strumenti nel Tema 4 |
| Modello e applicazione, prodotti | trattato (2.5) | Tema 4 |
| Tecniche di prompting, riproducibilità | accennato (2.5, 2.7) | Temi 5 e 6 |
| "Lost in the Middle" (Liu 2024) | citato (2.5) | Temi 8 e 14 |
| Grounding e RAG | introdotti (2.6) | Temi 8 e 14 |
| Allucinazioni, accuratezza, affidabilità | accennato (2.6, 2.7) | Tema 3; verifica nel Tema 7 |
| Variabilità e correttezza | trattato (2.7) | Temi 3 e 7 |
| Multimodalità | introdotta (2.2) | Tema 10 |
| Strumenti e azioni dei sistemi | accennato (2.5) | Tema 11 |

### Tema 3 (compilato il 9 ottobre 2026)
**Prerequisiti:** consigliato il Tema 2 per modello e applicazione, conoscenza incorporata, data limite, variabilità; le note richiamano brevemente questi concetti. **Concetti introdotti e ripresi in seguito:** calibrare la fiducia; allucinazione e sue forme; autorevolezza apparente; bias e sycophancy; accuratezza, affidabilità, consistenza, utilità; robustezza; verifica proporzionata; affidabilità adeguata allo scopo; supporto, supervisione, delega; responsabilità umana.

| Concetto | Nel Tema 3 | Approfondito o ripreso in |
|---|---|---|
| Frontiera frastagliata (Dell'Acqua 2026) | richiamata (3.5) | Temi 1 e 12 |
| Mata v. Avianca, citazioni inventate | trattato (3.3) | Tema 7 |
| Sycophancy (Sharma 2024) | trattata (3.4) | Tema 7 |
| Caso Amazon (Dastin 2018) | trattato (3.4) | Tema 17 |
| Automation bias (Parasuraman e Manzey 2010) | accennato (3.6, 3.8) | Temi 5, 7 e 17 |
| Verifica di fatti, fonti e numeri | principi (3.6) | Tema 7 (metodo); Tema 9 per i dati |
| Tecniche di formulazione delle richieste | accennate (3.4, 3.7) | Temi 5 e 6 |
| Valutare un sistema sui casi reali | approccio semplice (3.5) | Tema 15 |
| ROI e selezione dei progetti | escluso | Temi 12 e 15 |
| Dati riservati e strumenti autorizzati | accennato (3.8) | Temi 14 e 17 |
| Responsabilità, AI Act | accennato (3.8) | Tema 18 |
| Agenti e livelli di delega | accennato (3.8) | Temi 5 (5.5) e 11 |
| Benchmark e dimostrazioni | trattato (3.5) | Temi 1 (1.6) e 4 |

### Tema 4 (compilato il 9 ottobre 2026)
**Prerequisiti:** consigliati il Tema 2 (modello e applicazione, token, contesto) e il Tema 3 (affidabilità, benchmark e dimostrazioni), richiamati brevemente nelle note. **Concetti introdotti e ripresi in seguito:** modello, sistema, applicazione, piattaforma; foundation models; open-weight e open-source; generalista, specializzata, integrata; spettro chatbot, assistente, sistema con strumenti, agente, automazione; persona nel, sopra e fuori dal ciclo; app, API, cloud, locale; versioni individuali, team, enterprise; undici criteri di scelta; vendor lock-in e portabilità. **Contenuto più sensibile al tempo dell'intera base: esempi da ricontrollare prima di ogni edizione (slide 70).**

| Concetto | Nel Tema 4 | Approfondito o ripreso in |
|---|---|---|
| Modello e applicazione | trattato (4.1, 4.3) | introdotto nel Tema 2 (2.5) |
| Affidabilità come criterio di scelta, benchmark | usato (4.7) | Tema 3 (3.5) |
| Assistenti configurati, prompt e istruzioni riutilizzabili | accennato (4.4, 4.5) | Temi 5 e 6 (6.8) |
| Agenti, workflow con AI, livelli di autonomia | categorie (4.5) | Tema 11; livelli di delega nei Temi 3 (3.8) e 5 (5.5) |
| RAG e assistenti su documenti aziendali | accennato (4.4) | Temi 2, 8 e 14 |
| Applicazioni per tipo di attività | esempi (4.3, 4.4) | Temi 8-11 |
| Processi e trasformazione | accennato (4.4) | Tema 13 |
| Scelta del caso d'uso, pilota, criteri di successo | escluso o accennato (4.7) | Temi 15 e 16 |
| Costi complessivi | criterio (4.7) | Tema 12 |
| Account personali e Shadow AI | accennato (4.6) | Temi 16, 17 e 18 |
| Dati, sicurezza, permessi minimi, prompt injection | criteri (4.5, 4.7) | Temi 11, 14 e 17 |
| Normativa e governance | escluso | Tema 18 |
| Competenze trasferibili | trattato (4.8) | Tema 1 (1.6) |

### Tema 5 (compilato il 9 ottobre 2026)
**Prerequisiti:** consigliati il Tema 2 (contesto, effetto ELIZA), il Tema 3 (affidabilità, compiacenza, automation bias) e il Tema 4 (categorie di sistemi), richiamati brevemente nelle note. **Concetti introdotti e ripresi in seguito:** linguaggio naturale come interfaccia; richiesta isolata e dialogo progressivo; contesto della conversazione; sette ruoli dell'AI; ruolo assegnato e competenza effettiva; AI come interlocutore critico (avvocato del diavolo, pre-mortem); suddivisione delle attività tra persona e sistema; cinque livelli di delega; assistenza, collaborazione, delega, automazione; otto fattori che dipendono dalla persona; utilizzo passivo e attivo; antropomorfizzazione; delega cognitiva.

| Concetto | Nel Tema 5 | Approfondito o ripreso in |
|---|---|---|
| Effetto ELIZA, antropomorfizzazione | ripreso (5.7) | introdotto nel Tema 2 (2.1) |
| Contesto della conversazione | ripreso (5.2) | Tema 2 |
| Compiacenza, autorevolezza apparente | richiamato (5.3) | Tema 3 |
| Automation bias, fiducia calibrata | trattato (5.7) | Temi 3 (3.8), 7 e 17 |
| Chatbot, assistenti, agenti come categorie | richiamato (5.5) | Tema 4 (4.5) |
| Tecniche di formulazione, ruoli e formati nel prompt | escluso (5.2, 5.3, 5.6) | Tema 6 |
| Procedure di verifica degli output | escluso (5.4, 5.7) | Tema 7 |
| Livelli di delega e progettazione di agenti e workflow | livelli trattati (5.5) | Tema 11 |
| Riprogettazione di processi e ruoli | escluso (5.4) | Temi 13 e 16 |
| Ruoli e responsabilità organizzative | escluso (5.5) | Temi 13, 16 e 18 |
| Condivisione di dati riservati con l'AI | accennato (5.7) | Temi 14 e 17 |

### Tema 6 (compilato il 9 ottobre 2026)
**Prerequisiti:** consigliati il Tema 2 (prompt, istruzioni di sistema, finestra di contesto), il Tema 3 (allucinazioni, compiacenza, autorevolezza apparente) e il Tema 5 (dialogo, ruoli, interlocutore critico), richiamati brevemente nelle note. **Concetti introdotti e ripresi in seguito:** prompt come comunicazione di obiettivi, aspettative, informazioni; prima il problema, poi il prompt; otto elementi di una richiesta; qualità del contesto; informazioni, istruzioni, esempi; zero-shot e few-shot; delimitazione; scomposizione; chiarimenti prima dell'esecuzione; ciclo iterativo e feedback efficace; aderenza e correttezza; formati strutturati (CSV, JSON); requisiti verificabili; template, librerie, istruzioni persistenti, assistenti configurati; manutenzione delle istruzioni. **Nota di attualità:** indicazioni sui modelli che ragionano prima di rispondere (note della slide 38), da ricontrollare prima di ogni edizione.

| Concetto | Nel Tema 6 | Approfondito o ripreso in |
|---|---|---|
| Prompt, istruzioni di sistema, finestra di contesto | applicato (6.1, 6.3) | introdotto nel Tema 2 |
| Allucinazioni, "sei sicuro?", calcoli con codice | richiamato (6.1, 6.5, 6.7) | Tema 3 |
| Dialogo iterativo, ruoli, interlocutore critico | applicato (6.2, 6.4, 6.7) | Tema 5 |
| Verifica della correttezza | escluso (6.1, 6.5, 6.6) | Tema 7 |
| Testi, documenti, dati, contenuti per attività | esempi (6.7) | Temi 8-11 |
| Assistenti configurati, agenti, flussi di lavoro | accennato (6.4, 6.8) | Tema 11; categorie nel Tema 4 |
| Cambiamento dei modelli e manutenzione dei template | accennato (6.8) | Tema 4 (4.8) |
| Librerie condivise, standard aziendali | accennato (6.8) | Temi 14 e 16 |
| Dati riservati e strumenti autorizzati | avvertenza ricorrente | Temi 14, 17 e 18 |

### Tema 7 (compilato il 9 ottobre 2026)
**Prerequisiti:** consigliati il Tema 3 (allucinazioni, compiacenza, autorevolezza apparente, caso Avianca, conseguenze degli errori), il Tema 5 (delega cognitiva, automation bias) e il Tema 6 (aderenza e correttezza, richieste di chiarimento), richiamati brevemente nelle note. **Concetti introdotti e ripresi in seguito:** valutare, verificare, decidere; fatti, opinioni, ipotesi, interpretazioni; dimensioni della qualità; qualità espressiva e sostanziale; omissioni; livelli di certezza; fonti primarie e secondarie; tre controlli sulla fonte (autentica, pertinente, di supporto); premesse e conclusioni; correlazione e causalità; verifica di dati e calcoli; revisione assistita dall'AI e verifica indipendente; bias di conferma e fluidità; plausibile, verificato, validato; economia della verifica; incertezze residue.

| Concetto | Nel Tema 7 | Approfondito o ripreso in |
|---|---|---|
| Allucinazioni, fonti inventate, caso Avianca | richiamato (7.3, 7.6) | Tema 3 |
| Compiacenza, "sei sicuro?" | trattato (7.6) | introdotto nel Tema 3 |
| Automation bias, delega cognitiva | trattato (7.7) | Temi 3 (3.8), 5 (5.7) e 17 |
| Aderenza e correttezza, richieste di chiarimento | ripreso (7.2, 7.6) | Tema 6 |
| Conseguenze degli errori (gravità, reversibilità) | applicato (7.8) | Tema 3 (3.8) |
| Fedeltà delle sintesi, tracciabilità verso le fonti | principi (7.2, 7.3) | Temi 8 e 14 |
| Verifica di dati, grafici, paradosso di Simpson | trattato (7.5) | Tema 9 |
| Contenuti generati e deepfake | escluso | Tema 10 |
| ROI e valore | escluso | Tema 12 |
| Responsabilità giuridica, obblighi normativi | escluso | Tema 18 |

### Tema 8 (compilato il 9 ottobre 2026)
**Prerequisiti:** consigliati il Tema 2 (contesto, RAG in sintesi, "Lost in the Middle"), il Tema 3 (fonti inventate), il Tema 6 (prompting, formati strutturati) e il Tema 7 (verifica delle fonti, controlli proporzionati), richiamati brevemente nelle note. **Concetti introdotti e ripresi in seguito:** quattro modalità (produrre, trasformare, analizzare e strutturare, recuperare conoscenza); generare o trasformare; modifiche formali e sostanziali; sintesi per scopi diversi; tracciabilità e riferimenti controllabili; perdita di significato; sintetizzare ed estrarre; dato estratto e dato validato; matrice comparativa; conoscenza incorporata e recuperata; archivio e conoscenza interrogabile; versionamento dei documenti; caricare non significa elaborare.

| Concetto | Nel Tema 8 | Approfondito o ripreso in |
|---|---|---|
| Finestra di contesto, "Lost in the Middle" | applicato (8.3, 8.8) | introdotto nel Tema 2 |
| Fonti e citazioni inventate | richiamato (8.3, 8.6) | Tema 3 |
| Formati strutturati, istruzioni riutilizzabili | applicato (8.4) | Tema 6 |
| Verifica delle fonti, controlli proporzionati | applicato (8.6, 8.8) | Tema 7 (7.3, 7.8) |
| Dati estratti verso l'analisi | accennato (8.4) | Tema 9 |
| Scansioni, immagini, multimodalità | impatto sui documenti (8.8) | Tema 10 |
| Assistenti documentali, flussi di estrazione automatica | accennato (8.7) | Tema 11 |
| RAG, conoscenza aziendale su larga scala, permessi | accennato (8.7) | Tema 14 |
| Dati riservati e strumenti autorizzati | avvertenza | Temi 14 e 17 |

### Tema 9 (compilato il 9 ottobre 2026)
**Prerequisiti:** consigliati il Tema 2 (machine learning, generazione del testo), il Tema 3 (numeri e calcoli generati), il Tema 7 (verifica di dati e calcoli, correlazione e causalità) e il Tema 8 (estrazione di dati da documenti), richiamati brevemente nelle note. **Concetti introdotti e ripresi in seguito:** quattro fasi (comprendere e preparare, elaborare e analizzare, rappresentare e prevedere, interpretare e valutare); analisi descrittiva, diagnostica, predittiva, prescrittiva; dati, metriche, indicatori; qualità e rappresentatività dei dati; calcolo eseguito e numero generato; tracciabilità delle operazioni; quartetto di Anscombe; correlazioni spurie e confronti multipli; grafici fuorvianti; previsioni, scenari e incertezza; falsa oggettività.

| Concetto | Nel Tema 9 | Approfondito o ripreso in |
|---|---|---|
| Machine learning e previsione | richiamato (9.6) | Tema 2 |
| Numeri generati, calcoli con codice | trattato (9.3) | introdotto nel Tema 3 |
| Verifica di dati, calcoli e grafici | applicato (9.3, 9.5, 9.8) | Tema 7 (7.5) |
| Correlazione e causalità | trattato (9.4) | Tema 7 (7.4) |
| Dati estratti da documenti | richiamato (9.2) | Tema 8 (8.4) |
| Grafici e contenuti visivi generati | accennato (9.5) | Tema 10 |
| Analisi automatizzate e agenti | escluso | Tema 11 |
| Valore e scelta dei progetti | escluso | Temi 12 e 15 |
| BI, integrazioni, governance dei dati aziendali | accennato (9.1) | Tema 14 |
| Decisioni sulle persone, vincoli etici e normativi | accennato (9.7) | Temi 17 e 18 |

### Tema 10 (compilato il 9 ottobre 2026)
**Prerequisiti:** consigliati il Tema 2 (modelli e generazione), il Tema 6 (principi di una buona richiesta), il Tema 7 (verifica e controlli proporzionati) e il Tema 8 (tracciabilità, perdita di significato), richiamati brevemente nelle note. **Concetti introdotti e ripresi in seguito:** modalità (testo, immagini, audio, video); interpretare, generare, trasformare; modello multimodale nativo e catene di modelli; descrivere e comprendere un'immagine; generazione e modifica di immagini; trascrizione, attribuzione, traduzione del parlato; accessibilità; contenuto documentale e sintetico; catene di trasformazione; realismo, autenticità, accuratezza; provenienza (metadati, filigrane, C2PA); frodi con voce e volto; obblighi di trasparenza sui deepfake (AI Act, art. 50).

| Concetto | Nel Tema 10 | Approfondito o ripreso in |
|---|---|---|
| Principi di formulazione delle richieste | applicato (10.3) | Tema 6 |
| Controlli proporzionati all'uso | applicato (10.8) | Tema 7 (7.8) |
| Tracciabilità, perdita di significato nelle trasformazioni | applicato (10.7) | Tema 8 (8.3) |
| Scansioni e immagini nei documenti | ripreso (10.2) | Tema 8 (8.8) |
| Grafici e infografiche coerenti con i dati | applicato (10.6) | Tema 9 (9.5) |
| Flussi automatizzati tra modalità, agenti | escluso | Tema 11 |
| Valore e casi d'uso | escluso | Temi 12 e 15 |
| Frodi, sicurezza, dati personali in immagini e registrazioni | accennato (10.2, 10.4, 10.8) | Tema 17 |
| Diritti, consenso, obblighi di trasparenza (AI Act, art. 50) | introdotto (10.3, 10.8) | Tema 18 |

### Tema 11 (compilato il 9 ottobre 2026)
**Prerequisiti:** consigliati il Tema 3 (livelli di delega, automation bias), il Tema 4 (chatbot, assistenti, agenti come categorie), il Tema 5 (delega cognitiva, livelli di delega) e il Tema 7 (verifica, controlli proporzionati), richiamati brevemente nelle note. **Concetti introdotti e ripresi in seguito:** chatbot, assistente, agente, automazione; rispondere, suggerire, preparare, eseguire; modello, applicazione e strumenti; operazioni informative e operazioni che modificano; principio del privilegio minimo; disponibile non è autorizzato; ciclo di un agente; accumulo degli errori; automazione tradizionale, RPA e automazione con AI; automazione, autonomia, supervisione; livelli operativi di autonomia; human-in-the-loop e human-on-the-loop; punti di approvazione; reversibilità; prompt injection ed eccesso di autonomia; dalla demo all'esercizio.

| Concetto | Nel Tema 11 | Approfondito o ripreso in |
|---|---|---|
| Livelli di delega, automation bias | ripreso (11.5) | Temi 3 (3.8) e 5 (5.5) |
| Categorie di sistemi, denominazioni commerciali | ripreso (11.1) | Tema 4 (4.5) |
| Istruzioni riutilizzabili, assistenti configurati | ripreso (11.1) | Tema 6 (6.8) |
| Verifica e controlli proporzionati | applicato ad azioni e processi (11.5, 11.8) | Tema 7 |
| Estrazione e flussi documentali | esempi (11.4) | Tema 8 |
| Valore, convenienza, selezione dei casi d'uso | escluso | Temi 12 e 15 |
| Trasformazione di processi e ruoli | accennato (11.6, 11.7) | Temi 13 e 16 |
| Architetture e integrazioni aziendali | escluso | Tema 14 |
| Sicurezza, prompt injection, permessi | introdotto (11.2, 11.8) | Tema 17 |
| Responsabilità giuridica, obblighi normativi | escluso | Tema 18 |

### Tema 12 (compilato il 9 ottobre 2026)
**Prerequisiti:** consigliati il Tema 1 (studi di produttività in sintesi), il Tema 3 (frontiera frastagliata, affidabilità) e i Temi 8-11 (che cosa l'AI può fare), richiamati brevemente nelle note. **Concetti introdotti e ripresi in seguito:** dalla capacità al valore; l'AI come mezzo; percepito ed effettivo; adozione e impatto; otto dimensioni del valore; tangibile e intangibile; compromessi; efficienza e produttività; risparmio apparente ed effettivo; paradosso della produttività (Solow); colli di bottiglia (teoria dei vincoli); qualità apparente ed effettiva; errori sistematici; amplificare o sostituire; ottimizzare o innovare; costi diretti, indiretti, nascosti; curva a J; beneficio lordo e netto; valore ipotizzato, percepito, misurato; legge di Goodhart.

| Concetto | Nel Tema 12 | Approfondito o ripreso in |
|---|---|---|
| Studi di produttività (Brynjolfsson, Dell'Acqua) | approfondito (12.3) | introdotti nel Tema 1, richiamati nel Tema 3 |
| Frontiera frastagliata | ripresa (12.3) | Temi 1 e 3 |
| Capacità degli strumenti su testi, dati, contenuti, agenti | presupposto | Temi 8-11 |
| Riorganizzazione del lavoro, ruoli, competenze | accennato (12.3, 12.5, 12.7) | Tema 13 |
| Dati e conoscenza come condizione del valore | accennato (12.7) | Tema 14 |
| ROI analitico, business case, selezione dei casi d'uso | escluso | Tema 15 |
| Waterfall da beneficio teorico a reale | introdotto (12.7, 12.8) | Tema 15 |
| Curva di adozione, gestione del cambiamento | accennato (12.7) | Tema 16 |
| Normativa, sicurezza, governance | escluso | Temi 17 e 18 |

### Tema 13 (compilato il 9 ottobre 2026)
**Prerequisiti:** consigliati il Tema 5 (collaborazione e delega), il Tema 11 (livelli di autonomia, supervisione) e il Tema 12 (valore, colli di bottiglia, indicatori), richiamati brevemente nelle note. **Concetti introdotti e ripresi in seguito:** compito, mansione, ruolo, processo; attività assistite, automatizzate, trasformate; il compito non è il ruolo (bancomat e cassieri); esposizione e trasformazione; scomposizione del lavoro in attività; variabilità e giudizio; ottimizzazione locale e trasformazione del processo; automatizzare l'inefficienza; nuovo lavoro creato dalla trasformazione; dall'esecuzione alla supervisione; paradosso del supervisore inesperto; collaborazione nei team; competenze per lavorare con l'AI; adozione e trasformazione effettiva.

| Concetto | Nel Tema 13 | Approfondito o ripreso in |
|---|---|---|
| Competenze per lavorare con l'AI (literacy, prompting, verifica, supervisione) | sintesi (13.7) | Temi 1-7, 9, 11 e 12 (corrispondenza nelle note della slide 48) |
| Delega cognitiva e perdita delle competenze | ripreso (13.7) | Tema 5 (5.7) |
| Livelli di autonomia, supervisione, eccezioni | ripreso (13.1, 13.4) | Tema 11 |
| Valore, colli di bottiglia, indicatori di risultato | ripreso (13.3, 13.8) | Tema 12 |
| Informazioni e conoscenza come condizione | accennato (13.2) | Tema 14 |
| Scelta e priorità delle attività da trasformare | escluso | Tema 15 |
| Diffusione, accompagnamento del cambiamento, coinvolgimento | accennato (13.6, 13.8) | Tema 16 |
| Responsabilità e controllo nei processi automatizzati | accennato (13.8) | Temi 17 e 18 |

### Tema 14 (compilato il 9 ottobre 2026)
**Prerequisiti:** consigliati il Tema 2 (conoscenza del modello), il Tema 7 (verifica) e il Tema 8 (documenti e conoscenza), richiamati brevemente nelle note. **Concetti introdotti e ripresi in seguito:** dati, informazioni, documenti, conoscenza; strutturate e non strutturate; conoscenza formalizzata e tacita; quattro condizioni (disponibilità, accessibilità, utilizzabilità, affidabilità); qualità e obsolescenza delle fonti; responsabili delle fonti; recupero e modifica del modello; accessibili, recuperate, usate; sola lettura e modifica; minimo privilegio; condivisioni eccessive; fonte corretta e risposta errata; prototipo e servizio.

| Concetto | Nel Tema 14 | Approfondito o ripreso in |
|---|---|---|
| Conoscenza del modello, addestramento e data di riferimento | ripreso (14.4) | Tema 2 |
| Risposte plausibili ma inventate | ripreso (14.4) | Tema 3 |
| Verifica proporzionata, fluidità e affidabilità | ripreso (14.7) | Tema 7 |
| Documenti, allegati, "Lost in the Middle" | ripreso (14.1, 14.4) | Temi 2 e 8 |
| Sola lettura e modifica, rischio operativo | accennato (14.5) | Tema 11 |
| Trasmissione della conoscenza tacita | ripreso (14.3) | Tema 13 |
| Condizioni informative come criterio di scelta | accennato (14.8) | Tema 15 |
| Classificazione delle informazioni, aspetti giuridici degli accessi | accennato (14.6) | Temi 17 e 18 |

### Tema 15 (compilato il 9 ottobre 2026)
**Prerequisiti:** consigliati il Tema 12 (valore, costi, colli di bottiglia), il Tema 13 (attività trasformabili) e il Tema 14 (condizioni informative), richiamati brevemente nelle note. **Concetti introdotti e ripresi in seguito:** partire dal problema; cause e sintomi; alternative non AI; descrizione di un caso d'uso; ipotesi da verificare; supporto o automazione parziale; complessità e utilità; valore teorico e ottenibile; costi completi; desiderabilità, fattibilità, sostenibilità; intrinseco e residuo; condizioni di esclusione; matrice valore e fattibilità; limiti dei punteggi; ipotesi verificabili; criteri di successo e insuccesso decisi prima; baseline; evidenze contrarie; tre decisioni possibili.

| Concetto | Nel Tema 15 | Approfondito o ripreso in |
|---|---|---|
| Allucinazioni, omissioni, errori dell'AI | ripreso (15.6) | Temi 3 e 7 |
| Ecosistema e dipendenza dai fornitori | ripreso (15.5) | Tema 4 |
| Verifica realistica degli output | ripreso (15.6) | Tema 7 |
| Automazione tradizionale e livelli di autonomia | accennato (15.3) | Tema 11 |
| Valore, costi, colli di bottiglia | ripreso (15.4) | Tema 12 |
| Attività trasformabili, nuovo lavoro | ripreso (15.4) | Tema 13 |
| Dati e informazioni come condizione di fattibilità | ripreso (15.2, 15.5, 15.6) | Tema 14 |
| Dalla sperimentazione all'adozione | accennato (15.8) | Tema 16 |
| Condizioni di esclusione legali e di sicurezza | accennato (15.6) | Temi 17 e 18 |

### Tema 16 (compilato il 9 ottobre 2026)
**Prerequisiti:** consigliati il Tema 12 (valore e indicatori), il Tema 13 (trasformazione del lavoro) e il Tema 15 (scelta e verifica delle opportunità), richiamati brevemente nelle note. **Concetti introdotti e ripresi in seguito:** disponibilità, uso, adozione, valore; adozione individuale, di team, organizzativa; spontanea o coordinata; curva a S (Rogers); Shadow AI e adozione dal basso; utilità e facilità percepite (TAM, UTAUT); ostacoli individuali e strutturali; ruolo della leadership e dei manager; transfer della formazione; modello 70-20-10; curva dell'oblio; pilota ed estensione; sicurezza psicologica; obiezione fondata; indicazioni d'uso operative; metriche di adozione e di impatto; sostenibilità.

| Concetto | Nel Tema 16 | Approfondito o ripreso in |
|---|---|---|
| Hype cycle | richiamato (16.3, nelle note) | Tema 1 (1.6) |
| Fiducia calibrata, limiti e verifica | ripreso (16.6) | Temi 3 e 7 |
| Prompting e uso efficace dell'AI generativa | accennato (16.2) | Temi 5 e 6 |
| Valore e indicatori di impatto | ripreso (16.1, 16.8) | Tema 12 |
| Competenze, esperienza, carichi aggiuntivi | ripreso (16.4, 16.6) | Tema 13 |
| Strumenti senza informazioni adeguate | accennato (16.2, 16.8) | Tema 14 |
| Scelta delle iniziative, evidenze, condizioni di esclusione | ripreso (16.3, 16.8) | Tema 15 |
| Shadow AI come rischio, regole formali, governance | escluso | Temi 17 e 18 |

### Tema 17 (compilato il 9 ottobre 2026)
**Prerequisiti:** consigliati il Tema 3 (limiti e spiegazioni), il Tema 7 (verifica proporzionata) e il Tema 11 (agenti e azioni), richiamati brevemente nelle note. **Concetti introdotti e ripresi in seguito:** può fare ed è opportuno; errore, danno, rischio; livelli di criticità; servizi personali, aziendali, gestiti; limiti dell'esclusione dall'addestramento; minimizzazione; oscuramento, pseudonimizzazione, anonimizzazione; identificabilità indiretta; prompt injection diretto e indiretto; autorizzazioni e credenziali; bias, stereotipi, prestazioni diverse; discriminazione diretta e indiretta; deepfake e procedure di verifica; diritti sui contenuti; supporto o decisione; automation bias; quattro condizioni del controllo; checklist in cinque domande; quattro esempi A-D.

| Concetto | Nel Tema 17 | Approfondito o ripreso in |
|---|---|---|
| Spiegazioni del modello e allucinazioni | ripreso (17.7) | Tema 3 |
| Verifica proporzionata alla criticità | ripreso (17.1, 17.5, 17.7, 17.8) | Tema 7 |
| Contenuti sintetici e deepfake (art. 50 AI Act) | ripreso (17.5) | Temi 10 e 18 |
| Agenti, azioni, prompt injection, come fermare un processo | ripreso (17.3, 17.7) | Tema 11 |
| Assistenti collegati a fonti ampie | ripreso (17.2) | Tema 14 |
| Shadow AI, strumenti approvati, segnalazioni | ripreso (17.1, 17.3, 17.8) | Tema 16 |
| Definizioni giuridiche, contratti, alto rischio, responsabilità formali | escluso | Tema 18 |

### Tema 18 (compilato il 9 ottobre 2026)
**Prerequisiti:** consigliati il Tema 17 (rischi e precauzioni del singolo) e il Tema 16 (adozione e Shadow AI), richiamati brevemente nelle note. **Concetti introdotti:** governance e conformità; tre piani (obblighi, responsabilità, policy); ciclo di vita; AI Act e applicazione progressiva; Digital Omnibus; AI Act e GDPR; altre norme; Legge 132/2025; approccio basato sul rischio; pratiche vietate; alto rischio (Allegati I e III); trasparenza e modelli per finalità generali; ruoli della filiera (fornitore, deployer); policy aziendali; inventario, valutazione e controlli; incidenti; AI literacy e articolo 4; governance proporzionata; framework e standard volontari; quattro equivoci e quattro esempi.

| Concetto | Nel Tema 18 | Approfondito o ripreso in |
|---|---|---|
| Contenuti sintetici e deepfake (art. 50) | ripreso (18.3) | Temi 10 e 17 |
| Agenti, capacità operative, ciclo di vita | ripreso (18.1) | Tema 11 |
| Assistenti collegati ai documenti, permessi | ripreso (18.4, 18.6) | Tema 14 |
| Scelta delle opportunità, rischio residuo | ripreso (18.4, 18.6) | Tema 15 |
| Shadow AI, formazione come leva di adozione | ripreso (18.1, 18.5, 18.7) | Tema 16 |
| Precauzioni del singolo, bias, riservatezza, supervisione | ripreso (18.1, 18.2, 18.6) | Tema 17 |

