# Istruzioni per Claude · Percorso di formazione AI Literacy

> **Leggi questo file per intero prima di lavorare sul percorso.** Riassume il lavoro fatto nella conversazione di produzione delle slide (8 e 9 ottobre 2026), le regole da rispettare, le attività che restano per la revisione dell'intero percorso e, nella sezione 9, l'indice completo degli argomenti delle slide.

Ultimo aggiornamento: 9 ottobre 2026 (indice degli argomenti; base indipendente da singole formazioni; nuova struttura con le cartelle `Base/` e `Formazioni/`; cartella di lavoro spostata in `Formazione AI Literacy Official`).

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
    - Se l'utente lo chiede, git può sostituire la cartella `_versioni_precedenti/` per conservare la storia delle modifiche.
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
  └── Formazioni/                                 (da creare alla prima formazione)
      └── <nome formazione>/                      una sottocartella per ciascuna formazione
  ```
  - I **18 documenti di perimetro** sono la fonte primaria dei contenuti, già "consolidati" dall'utente.
  - Le **18 presentazioni** sono una per tema, prodotte nella conversazione di produzione.
  - `sorgenti_slide.zip` contiene i sorgenti JavaScript (vedi sezione 6).
- **Regole di organizzazione dei file:**
  1. **La cartella `Base/` non si modifica**, salvo una revisione della base richiesta esplicitamente dall'utente (attività A, B, C, E, F della sezione 5).
     - In quel caso, prima di sovrascrivere un file, conservarne la versione precedente: per esempio in `Base/_versioni_precedenti/` con la data nel nome.
     - Annotare ogni modifica in `Base/registro_revisione.md`.
  2. **Ogni nuova formazione ha una sottocartella propria** in `Formazioni/`, con un nome breve e la data, per esempio `Formazioni/2026-11_Management_AI_Awareness/`. Contiene:
     - `scheda_formazione.md`: committente, pubblico, obiettivi, durata, formato, date, brand;
     - `agenda.md`: blocchi, tempi, slide e temi usati, esercizi;
     - i deck e i materiali prodotti per quella formazione (dispense, esercizi, checklist);
     - `note_scelte.md`: che cosa è stato preso dalla base, che cosa adattato e perché.
  3. I file delle formazioni si creano come **nuovi file**: si copiano o si selezionano contenuti dalla base, senza spostare né rinominare i file di `Base/`.
  4. Questo file di istruzioni resta nella cartella principale. Va aggiornato quando cambia la struttura o la base. Dopo ogni modifica, aggiornare anche la copia nei documenti del progetto Claude: `Formazione AI Literacy Official/ISTRUZIONI_CLAUDE_Percorso_AI_Literacy.md`.
- **Stato:** tutte le 18 presentazioni sono state prodotte e consegnate. **Il passo successivo, indicato dai documenti di perimetro, è la revisione trasversale dei 18 temi.** Dopo la revisione, la base potrà essere usata per progettare formazioni specifiche.

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
6. **Esercizi rimandati:** nelle note compare solo un suggerimento "Esercizio suggerito: ..." nella slide chiave di ogni sottotema. Gli esercizi veri vanno sviluppati in seguito (vedi attività E).
7. **Esempi aziendali sempre fittizi e dichiarati come tali.** Nessun dato riservato. I casi reali citati, come Mata v. Avianca, Arup o Amazon, sono indicati con la loro fonte.
8. **Riferimenti citati a memoria:** vanno segnalati all'utente come "da verificare".
9. **Temi normativi:** precisare sempre che non si tratta di un parere legale. Verificare le date sulle fonti ufficiali e non presentare mai una data unica come scadenza universale.
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
| 1 | Comprendere l'AI | Evoluzione e rilevanza dell'AI | Tema1_Evoluzione_e_rilevanza_AI.pptx | 55 |
| 2 | Comprendere l'AI | Fondamenti e funzionamento | Tema2_Fondamenti_e_funzionamento_AI.pptx | 69 |
| 3 | Comprendere l'AI | Capacità, limiti, affidabilità | Tema3_Capacita_limiti_affidabilita_AI.pptx | 68 |
| 4 | Comprendere l'AI | Ecosistema AI | Tema4_Ecosistema_AI.pptx | 68 |
| 5 | Interagire con l'AI | Dialogo uomo e AI | Tema5_Dialogo_uomo_AI.pptx | 61 |
| 6 | Interagire con l'AI | Prompting e tecniche di interazione | Tema6_Prompting_tecniche_interazione.pptx | 72 |
| 7 | Interagire con l'AI | Verifica degli output e pensiero critico | Tema7_Verifica_output_pensiero_critico.pptx | 73 |
| 8 | Esplorare le possibilità | Testi, documenti, conoscenza | Tema8_AI_testi_documenti_conoscenza.pptx | 81 |
| 9 | Esplorare le possibilità | Dati e analisi | Tema9_AI_dati_analisi.pptx | 84 |
| 10 | Esplorare le possibilità | AI multimodale e contenuti | Tema10_AI_multimodale_contenuti.pptx | 74 |
| 11 | Esplorare le possibilità | Assistenti, agenti, automazioni | Tema11_Assistenti_agenti_automazioni.pptx | 77 |
| 12 | Valore per l'azienda | Creazione di valore | Tema12_AI_creazione_valore_azienda.pptx | 72 |
| 13 | Valore per l'azienda | Trasformazione del lavoro e dei processi | Tema13_AI_trasformazione_lavoro_processi.pptx | 63 |
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
| T1 | Storia (Turing, Dartmouth), transformer, crescita del calcolo (Epoch AI), studi di produttività (Brynjolfsson 2023, Dell'Acqua 2023), hype cycle |
| T2 | Definizione AI Act (art. 3) e OCSE, ELIZA, transformer, RLHF (Ouyang 2022), RAG (Lewis 2020), "Lost in the Middle" (Liu) |
| T3 | Allucinazioni (Mata v. Avianca, Kalai 2025), piaggeria (Sharma 2023), bias (caso Amazon), frontiera irregolare. Esempio didattico di frase vera e falsa sull'AI Act |
| T4 | Ecosistema di prodotti e fornitori. **Contenuto molto sensibile al tempo** |
| T5 | ELIZA, automation bias (Parasuraman e Manzey 2010), Lee et al. 2025 sul pensiero critico |
| T6 | Tecniche di prompting |

**Temi 7-12**

| Tema | Elementi notevoli |
|---|---|
| T7 | Fluidità e verità (Reber e Schwarz 1999), proporzionalità della verifica. "Che cosa viene dopo" aggiornato al Tema 8 |
| T8 | Uso dell'AI su documenti, RAG solo accennato |
| T9 | Quartetto di Anscombe, correlazioni spurie (Vigen) |
| T10 | Deepfake (casi WSJ 2019 e Arup 2024), C2PA |
| T11 | Livelli di automazione (Parasuraman, Sheridan e Wickens 2000), OWASP, accumulo degli errori negli agenti |
| T12 | Valore, waterfall da teorico a reale, paradosso di Solow, teoria dei vincoli |

**Temi 13-18**

| Tema | Elementi notevoli |
|---|---|
| T13 | Compito, processo, ruolo; esposizione e trasformazione (Eloundou 2023); bancomat e cassieri (Bessen); Autor 2003 |
| T14 | Quattro condizioni (disponibilità, accessibilità, utilizzabilità, affidabilità); iceberg della conoscenza tacita; RAG concettuale; classificazione delle informazioni; oversharing; scenario a 5 errori |
| T15 | Percorso individuare, descrivere, valutare, confrontare, verificare; scenario delle richieste commerciali; matrice valore e fattibilità; limiti dei punteggi; criteri di insuccesso definiti prima |
| T16 | Da disponibilità a valore; scenario A e B; Shadow AI; TAM e UTAUT; transfer della formazione; Kirkpatrick; sicurezza psicologica; diffusione rapida e graduale |
| T17 | Esempi A-D (identificabilità, prompt injection, supervisione apparente, divulgazione via output); checklist in 5 domande; procedere, verificare, chiedere, interrompere |
| T18 | Verificato a ottobre 2026: AI Act modificato dal **Digital Omnibus**. Dettagli sotto |

**Dettagli del Tema 18 (normativa verificata a ottobre 2026)**
- Il Digital Omnibus è il Reg. (UE) 2026/1744, pubblicato in GUUE il 24 luglio 2026 e in vigore dal 27 luglio 2026.
- Alto rischio: Allegato III dal 2 dicembre 2027; Allegato I dal 2 agosto 2028.
- Articolo 4 riscritto: obbligo di "sostenere lo sviluppo" dell'alfabetizzazione, senza garantire un livello individuale.
- Nuovi divieti dal 2 dicembre 2026.
- Legge italiana 132/2025, in vigore dal 10 ottobre 2025.
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
| Studi di produttività (Brynjolfsson, Dell'Acqua) | T1, T3, T12 |
| RAG e "Lost in the Middle" | T2, T8, T14 |
| Classificazione delle informazioni (pubbliche, interne, riservate, sensibili o personali) | T14, T17 |
| Shadow AI | T16 (adozione), T17 (rischio), T18 (governance) |
| Waterfall da beneficio teorico a reale | T12, T15 |
| Hype cycle | T1, T16 |
| Formazione | T16 come leva di adozione, T18 come misura di alfabetizzazione |
| Proporzionalità della verifica | T7, ripresa in T17 e T18 |

**A2. Lacune e prerequisiti.**
- Verificare che ogni concetto sia introdotto prima di essere usato.
- Esempi da controllare: il RAG nel T8 presuppone il T2; gli agenti nel T17 presuppongono il T11.
- Verificare i rimandi "(Tema N)" nelle slide e nelle note: devono puntare al tema giusto.

**A3. Coerenza terminologica.**
- Termini da uniformare: AI o IA; provider e deployer o fornitore e utilizzatore; prompt o richiesta; output o risultato; allucinazione.
- Nomi delle aree identici in tutti i deck.
- Formato delle citazioni uniforme. Esempio di incoerenza già nota: Liu et al. è "2023 / TACL 2024" nel T2 e "2024" nel T8 e T14.

**A4. Coerenza dei passaggi tra temi.**
- Controllare in tutti i 18 deck le slide "Che cosa viene dopo" e "Il percorso del modulo".
- Il T2 dice che il quadro dell'AI Act "sarà eventualmente approfondito in un modulo dedicato": aggiornare con il rimando al Tema 18.

**A5. Coerenza stilistica.**
- I Temi 1-7 non hanno l'indicatore a pillole e usano un set di helper più ridotto.
- Decidere se uniformarli. Le palette e i master sono gli stessi.

### B. Verifica delle fonti e dei fatti

Le fonti sono state citate a memoria e vanno verificate una per una, con WebSearch o WebFetch e le fonti primarie.

**Elenco per tema**

| Tema | Fonti da verificare |
|---|---|
| T1 | Turing 1950; proposta di Dartmouth 1955; Vaswani 2017; Epoch AI 2024 (crescita 4-5x all'anno); Brynjolfsson, Li e Raymond 2023; Dell'Acqua 2023; Reuters febbraio 2023 (stima UBS sugli utenti di ChatGPT) |
| T2 | AI Act art. 3; OCSE 2023; Weizenbaum 1966; Brown 2020; Ouyang 2022; Lewis 2020; Liu (anno) |
| T3 | Mata v. Avianca 2023; Kalai et al. 2025; Sharma 2023; Dastin 2018; Doshi e Hauser 2024; Dell'Acqua 2023 |
| T4 | **Tutto il contenuto su prodotti, fornitori, modelli, prezzi e funzioni: rivedere integralmente, perché invecchia rapidamente.** La slide fonti non è stata estratta automaticamente: aprire il deck |
| T5 | Parasuraman e Manzey 2010; Lee et al. 2025 (CHI) |
| T6 | Verificare le fonti nel deck (non estratte automaticamente) |
| T7 | Reber e Schwarz 1999 |
| T8 | Liu 2024; Lewis 2020 |
| T9 | Anscombe 1973; Vigen 2015 |
| T10 | Casi deepfake del 2019 e 2024 (cifre); C2PA |
| T11 | Parasuraman, Sheridan e Wickens 2000; OWASP (versione corrente) |
| T12 | Brynjolfsson 2023; Dell'Acqua 2023; Solow 1987; Goldratt e Cox 1984 |
| T13 | Eloundou 2023 (80% e 19%); Bessen 2015 (bancomat e cassieri); Autor, Levy e Murnane 2003 |
| T14 | Polanyi 1966; Nonaka e Takeuchi 1995; Lewis 2020; Liu 2024; Saltzer e Schroeder 1975 |
| T15 | Popper; Brown 2009 e IDEO; Ohno 1988 (cinque perché); Nickerson 1998; effetto Hawthorne (citato con cautela) |
| T16 | Rogers; Davis 1989; Venkatesh 2003; Baldwin e Ford 1988; Kirkpatrick; Edmondson 1999; legge di Goodhart; Deming; modello 70-20-10; curva dell'oblio (Ebbinghaus); hype cycle; Work Trend Index 2024 (cifre) |
| T17 | Greshake 2023; OWASP; Sweeney 2000 (87%); Gender Shades 2018 (valori del grafico approssimati: 0,3%, 7,1%, 12%, 34,7%); Parasuraman e Manzey 2010; Reuters 2018; casi deepfake |
| T18 | Testo ufficiale del Reg. 2026/1744 in GUUE (le sintesi vengono da fonti secondarie); calendario completo; nuovo art. 4; art. 50 e periodo transitorio; nuovi divieti; Legge 132/2025 e stato dei decreti attuativi; linee guida della Commissione; ISO/IEC 42001 e 23894; NIST AI RMF |

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
5. Tenere un registro delle modifiche in `Base/registro_revisione.md`, conservando le versioni precedenti in `Base/_versioni_precedenti/`.

---

## 9. Indice degli argomenti delle slide

Indice generato dai 18 deck. Per ogni tema: introduzione, sottotemi con i titoli delle slide e il messaggio della slide chiave, conclusioni. I numeri tra parentesi sono i numeri di slide. La durata è stimata dalle note del relatore (circa 140 parole al minuto, solo esposizione frontale).

### Tema 1 · Evoluzione e rilevanza dell'Intelligenza Artificiale
*Area: Comprendere l'AI · 55 slide · file `Tema1_Evoluzione_e_rilevanza_AI.pptx` · esposizione stimata circa 0 h 54 min*

- **Introduzione**: Obiettivo del modulo (2) · Sei domande guida per questo modulo (3) · Il percorso del modulo (4)
- **1.1 Storia ed evoluzione dell'AI**: Le origini: si possono costruire macchine che pensano? (6) · Oltre settant'anni di evoluzione (7) · L'AI simbolica: la conoscenza scritta in regole (8) · Cicli di entusiasmo e disillusione (9) · Dalle regole all'apprendimento dai dati (10) · Machine Learning e Deep Learning (11) · Dall'AI specializzata all'AI generativa (12)
  - *Messaggio chiave:* L'AI è il risultato di decenni di ricerca ed evoluzione tecnologica, non un'invenzione recente.
- **1.2 I fattori dell'accelerazione tecnologica**: Cinque fattori che si rafforzano a vicenda (15) · Potenza di calcolo (16) · Disponibilità di grandi quantità di dati (17) · Evoluzione degli algoritmi e delle architetture (18) · Lo sviluppo di modelli di grandi dimensioni (19) · Investimenti e infrastrutture tecnologiche (20)
  - *Messaggio chiave:* L'accelerazione deriva dalla convergenza di diversi fattori, non da una singola invenzione.
- **1.3 La svolta dell'AI generativa**: Dal classificare e prevedere al generare (23) · Il linguaggio naturale diventa l'interfaccia (24) · La diffusione di chatbot e assistenti AI (25) · Che cosa può generare l'AI (26) · Un'AI accessibile a tutti (27)
  - *Messaggio chiave:* L'AI generativa ha ampliato le persone e le attività che possono utilizzare direttamente capacità AI.
- **1.4 Dalla digitalizzazione all'Intelligenza Artificiale**: Quattro passaggi di un'evoluzione (30) · Un esempio: la gestione delle richieste dei clienti (31) · Software deterministico e sistemi probabilistici (32)
  - *Messaggio chiave:* Digitalizzazione, automazione e AI sono concetti collegati ma distinti; possono coesistere nello stesso processo aziendale.
- **1.5 Rilevanza dell'AI per le aziende**: Un'applicazione trasversale alle funzioni aziendali (35) · L'AI come tecnologia abilitante (36) · Capacità AI accessibili tramite strumenti commerciali (37) · Effetti potenziali: produttività, qualità, innovazione (38) · Come evolvono il lavoro e le competenze (39) · Possibili implicazioni competitive (40) · Dal potenziale tecnologico al valore realizzato (41)
  - *Messaggio chiave:* L'AI può abilitare cambiamenti in molte aree dell'impresa, ma il valore nasce da applicazioni appropriate a problemi reali.
- **1.6 Tra hype e realtà**: Aspettative, promesse e narrazioni mediatiche (44) · Dimostrazione tecnologica e uso aziendale continuativo (45) · Maturità delle capacità e limiti attuali (46) · Opportunità concrete o affermazioni non dimostrate? (47) · I benefici non sono uguali per tutti (48) · Velocità del cambiamento e incertezza sul futuro (49) · Competenze adattabili, non dipendenza dagli strumenti (50)
  - *Messaggio chiave:* Occorre valutare criticamente le promesse dell'AI, distinguendo possibilità tecniche, affidabilità e convenienza.
- **Conclusioni**: Le domande guida: le nostre risposte (52) · Che cosa portiamo a casa (53) · Prossimo passo: il Tema 2 (54) · Fonti e riferimenti (55)

### Tema 2 · Fondamenti e funzionamento dell'Intelligenza Artificiale
*Area: Comprendere l'AI · 69 slide · file `Tema2_Fondamenti_e_funzionamento_AI.pptx` · esposizione stimata circa 1 h 13 min*

- **Introduzione**: Obiettivo del modulo (2) · Otto domande guida per questo modulo (3) · Il percorso del modulo (4)
- **2.1 Che cos'è l'Intelligenza Artificiale**: Una definizione operativa (6) · Intelligenza artificiale e intelligenza umana (7) · Sistemi specializzati e intelligenza artificiale generale (8) · Comprensione apparente: l'effetto ELIZA (9) · Che cosa osserviamo e che cosa possiamo concludere (10)
  - *Messaggio chiave:* L'AI non è un'unica tecnologia e le prestazioni osservabili non autorizzano automaticamente ad attribuirle caratteristiche umane.
- **2.2 Le principali categorie di AI**: Quattro criteri di classificazione diversi (13) · AI simbolica e Machine Learning (14) · Deep Learning e reti neurali (15) · AI predittiva, discriminativa e generativa (16) · AI multimodale (17) · Quale approccio per quale problema (18)
  - *Messaggio chiave:* Esistono approcci e capacità differenti, adatti a problemi differenti. Le categorie rispondono a criteri diversi e non sono tutte mutuamente esclusive.
- **2.3 Come un sistema AI apprende dai dati**: Che cosa significa apprendere dai dati (21) · Dati di addestramento ed esempi (22) · Individuare schemi e regolarità (23) · I parametri del modello (24) · Il ciclo di addestramento (25) · Generalizzare verso nuovi input (26) · Addestramento e inferenza (27)
  - *Messaggio chiave:* Nei sistemi di Machine Learning l'addestramento modifica i parametri del modello, mentre l'inferenza lo utilizza per elaborare nuovi input. Non tutti i sistemi AI apprendono dai dati.
- **2.4 Che cosa sono i Large Language Models**: Un modello linguistico di grandi dimensioni (30) · I token: come il modello vede il testo (31) · Rappresentare il significato (32) · Il Transformer e il meccanismo di attenzione (33) · Come viene generata una risposta (34) · Più di un completamento automatico (35) · Capacità linguistiche, di analisi e di ragionamento (36) · Perché un modello può affrontare compiti diversi (37)
  - *Messaggio chiave:* Gli LLM generano output usando regolarità apprese e il contesto disponibile; la spiegazione non va ridotta alla sola metafora del completamento automatico.
- **2.5 Come funziona un'interazione con l'AI**: Input, prompt e output (40) · Il percorso di una richiesta (41) · La finestra di contesto (42) · La cronologia conversazionale (43) · Contesto temporaneo e memoria persistente (44) · Il modello e l'applicazione (45)
  - *Messaggio chiave:* Il risultato dipende anche dalle informazioni rese disponibili durante l'interazione; il funzionamento del modello e quello del prodotto che lo utilizza non coincidono sempre.
- **2.6 Conoscenza e fonti informative**: Tre fonti di informazione (48) · Conoscenza incorporata e recupero di informazioni (49) · Aggiornamento dei dati e limiti temporali (50) · Grounding: ancorare le risposte alle fonti (51) · Introduzione alla Retrieval-Augmented Generation (52) · Adattare un sistema AI a un contesto specifico (53) · Tre equivoci frequenti (54)
  - *Messaggio chiave:* Fornire un documento o collegare una fonte a un sistema AI non significa necessariamente riaddestrare il modello.
- **2.7 Variabilità dei risultati**: Stessa richiesta, risposte diverse (57) · Che cosa influenza la variabilità (58) · I parametri di generazione: la temperatura (59) · Comportamento deterministico e probabilistico (60) · Riproducibilità dei risultati (61) · Variabilità non significa errore (62)
  - *Messaggio chiave:* Una stessa richiesta può produrre risposte differenti; la variabilità è distinta dalla questione della correttezza e dell'affidabilità, approfondita nel Tema 3.
- **Conclusioni**: Le domande guida: le nostre risposte (64) · Che cosa portiamo a casa (65) · Glossario essenziale (1 di 2) (66) · Glossario essenziale (2 di 2) (67) · Prossimo passo: il Tema 3 (68) · Fonti e riferimenti (69)

### Tema 3 · Capacità, limiti e affidabilità dell'Intelligenza Artificiale
*Area: Comprendere l'AI · 68 slide · file `Tema3_Capacita_limiti_affidabilita_AI.pptx` · esposizione stimata circa 1 h 12 min*

- **Introduzione**: Obiettivo del modulo (2) · Calibrare la fiducia (3) · Otto domande guida per questo modulo (4) · Il percorso del modulo (5)
- **3.1 Le principali capacità dell'AI**: Una mappa delle capacità (7) · Dalle capacità alle attività (8) · Non tutti i sistemi hanno le stesse capacità (9)
  - *Messaggio chiave:* Le capacità dell'AI sono ampie, ma variano in funzione dei sistemi e dei compiti; non tutti i prodotti AI dispongono delle stesse funzioni.
- **3.2 Ragionamento, problem solving e creatività**: Ragionamento logico, matematico e analitico (12) · Problemi strutturati e non strutturati (13) · Scomporre, pianificare, valutare alternative (14) · Generazione di idee e supporto creativo (15) · Limiti nelle situazioni nuove, ambigue o complesse (16)
  - *Messaggio chiave:* L'AI può supportare attività cognitive avanzate, ma non garantisce ragionamenti sempre corretti o coerenti.
- **3.3 Allucinazioni e informazioni false**: Che cos'è un'allucinazione (19) · Citazioni, riferimenti e fonti inesistenti (20) · Perché si verificano le allucinazioni (21) · Plausibilità linguistica e veridicità (22) · L'autorevolezza apparente (23) · Dove le allucinazioni sono più probabili (24)
  - *Messaggio chiave:* La fluidità o la sicurezza del tono non dimostra che un'affermazione sia corretta o verificata.
- **3.4 Bias e distorsioni nei risultati**: Che cosa sono bias e distorsioni (27) · Da dove nascono le distorsioni (28) · Stereotipi e rappresentazioni non equilibrate (29) · L'influenza del contesto e delle istruzioni (30) · Bias di conferma e tendenza ad assecondare (31) · Neutralità apparente e oggettività effettiva (32)
  - *Messaggio chiave:* I sistemi AI possono riprodurre o amplificare distorsioni; le risposte non devono essere considerate automaticamente imparziali.
- **3.5 Accuratezza, affidabilità e consistenza**: Quattro concetti da distinguere (35) · Prestazioni diverse in base al compito (36) · Coerenza, ripetibilità e robustezza (37) · I limiti di benchmark e dimostrazioni (38) · Valutare le prestazioni nel contesto reale (39) · Il modello e il sistema completo (40)
  - *Messaggio chiave:* L'affidabilità non è una proprietà unica e universale di un modello; deve essere valutata per compiti e condizioni d'uso specifici.
- **3.6 Verificabilità e controllo dei risultati**: Che cosa verificare (43) · Verificare fatti, fonti e riferimenti (44) · Controllare calcoli, dati e informazioni (45) · Completezza, coerenza e tracciabilità (46) · I limiti dell'autoverifica (47) · Supervisione umana e verifica proporzionata (48)
  - *Messaggio chiave:* La verifica è parte dell'uso consapevole dell'AI e deve essere proporzionata all'importanza del compito e alle possibili conseguenze di un errore.
- **3.7 I fattori che influenzano le prestazioni**: Sette fattori (51) · Tecnologia, informazioni e modalità operative (52) · Differenze tra ambiti applicativi (53)
  - *Messaggio chiave:* Le prestazioni derivano dall'interazione tra caratteristiche tecnologiche, qualità delle informazioni e modalità operative.
- **3.8 Quando utilizzare o limitare l'AI**: Possibilità tecnica e opportunità di utilizzo (56) · Le conseguenze di un errore (57) · Attività a basso e alto impatto (58) · Affidabilità adeguata allo scopo (59) · Supporto, supervisione e delega (60) · Quando limitare o evitare l'uso (61) · La responsabilità resta umana (62)
  - *Messaggio chiave:* L'AI va utilizzata quando le sue prestazioni e i controlli disponibili sono compatibili con il rischio del compito, non soltanto quando il sistema sembra capace di eseguirlo.
- **Conclusioni**: Le domande guida: le nostre risposte (64) · Che cosa portiamo a casa (65) · Prima di usare un risultato AI: una checklist (66) · Prossimo passo: il Tema 4 (67) · Fonti e riferimenti (68)

### Tema 4 · Ecosistema AI: modelli, strumenti e piattaforme
*Area: Comprendere l'AI · 68 slide · file `Tema4_Ecosistema_AI.pptx` · esposizione stimata circa 1 h 09 min*

- **Introduzione**: Obiettivo del modulo (2) · Dieci domande guida per questo modulo (3) · Il percorso del modulo (4)
- **4.1 La struttura dell'ecosistema AI**: Modello, sistema, applicazione, piattaforma (6) · Foundation models e modelli specializzati (7) · Gli attori dell'ecosistema (8) · Com'è fatta un'applicazione AI (9) · Più modelli, modelli che cambiano (10) · Ecosistemi integrati e soluzioni composte (11)
  - *Messaggio chiave:* Un'applicazione AI è spesso composta da più elementi tecnologici e non coincide necessariamente con il modello che utilizza.
- **4.2 Le principali famiglie di modelli AI**: Quattro famiglie di modelli (14) · Capacità, dimensioni e requisiti (15) · Modelli proprietari e modelli con pesi accessibili (16) · Open-weight non significa open-source (17) · Modelli aperti, chiusi e controllo tecnologico (18)
  - *Messaggio chiave:* Modelli differenti rispondono a esigenze differenti; non esiste un unico modello migliore per qualunque attività.
- **4.3 Le principali piattaforme e gli strumenti AI**: Gli assistenti AI generalisti (21) · Le categorie di strumenti (22) · Funzionalità comuni e differenze principali (23) · Capacità del modello e funzionalità dell'applicazione (24) · Disponibilità delle funzionalità (25) · Capacità dichiarate e funzionalità disponibili (26)
  - *Messaggio chiave:* Due prodotti dall'interfaccia simile possono offrire capacità, integrazioni, controlli e condizioni molto diversi.
- **4.4 AI generalista, specializzata e integrata**: Tre approcci (29) · L'AI nei software di produttività e nei gestionali (30) · Soluzioni pronte all'uso e personalizzate (31) · Vantaggi e limiti dei diversi approcci (32) · Usare uno strumento o integrare l'AI in un processo (33)
  - *Messaggio chiave:* Le capacità AI possono essere disponibili in prodotti generalisti, strumenti dedicati o software già presenti in azienda; adottare AI non richiede necessariamente un nuovo applicativo separato. Sottot
- **4.5 Chatbot, assistenti, agenti e automazioni**: Uno spettro di autonomia (36) · Chatbot e assistenti configurati (37) · Sistemi con strumenti e agenti (38) · Automazioni tradizionali e workflow con AI (39) · Livelli di autonomia e supervisione umana (40) · Una terminologia non standardizzata (41)
  - *Messaggio chiave:* Conversare, ricevere assistenza, automatizzare e delegare l'esecuzione di attività rappresentano modalità e livelli di autonomia differenti.
- **4.6 Modalità di accesso e utilizzo dell'AI**: Le principali modalità di accesso (44) · Applicazioni e API: due modi di usare lo stesso modello (45) · Cloud ed esecuzione locale (46) · Soluzioni individuali, team ed enterprise (47)
  - *Messaggio chiave:* Capacità analoghe possono essere rese disponibili attraverso modalità differenti, con implicazioni tecniche, economiche e organizzative diverse.
- **4.7 Criteri per confrontare e scegliere**: Undici criteri (50) · Adeguatezza, qualità e facilità d'uso (51) · Funzionalità, integrazione e costi complessivi (52) · Dati, sicurezza e controlli amministrativi (53) · Indipendenza tecnologica e vendor lock-in (54) · Verificare ciò che è davvero disponibile (55) · Una scheda di confronto (56)
  - *Messaggio chiave:* Lo strumento più noto o il modello più potente non è necessariamente la scelta migliore per l'azienda.
- **4.8 L'evoluzione e la dinamicità dell'ecosistema AI**: Che cosa cambia (59) · Obsolescenza di strumenti, procedure e competenze (60) · Competenze e conoscenze trasferibili (61) · Orientarsi senza inseguire ogni novità (62)
  - *Messaggio chiave:* I principi di funzionamento e valutazione hanno maggiore durata rispetto alle caratteristiche di una singola versione di un prodotto.
- **Conclusioni**: Le domande guida: le nostre risposte (64) · Che cosa portiamo a casa (65) · Prima di scegliere uno strumento AI: una checklist (66) · Prossimo passo: il Tema 5 (67) · Nota sull'aggiornamento dei contenuti (68)

### Tema 5 · Il dialogo uomo-AI
*Area: Interagire con l'AI · 61 slide · file `Tema5_Dialogo_uomo_AI.pptx` · esposizione stimata circa 1 h 01 min*

- **Introduzione**: Obiettivo del modulo (2) · Dieci domande guida per questo modulo (3) · Il percorso del modulo (4)
- **5.1 Il linguaggio naturale come interfaccia**: Dai comandi alle richieste (6) · Vantaggi e limiti della comunicazione conversazionale (7) · Flessibilità e ambiguità del linguaggio (8) · Testo, voce e immagini (9) · Cambia il rapporto tra utente e software (10)
  - *Messaggio chiave:* Il linguaggio naturale amplia l'accessibilità della tecnologia, ma richiede comunque obiettivi chiari e un'interpretazione critica delle risposte.
- **5.2 Dalla domanda alla conversazione**: Richiesta isolata e dialogo articolato (13) · Un processo progressivo e iterativo (14) · Un esempio di dialogo (15) · Il contesto della conversazione (16) · L'AI come interlocutore che può porre domande (17) · L'AI come supporto alla definizione dei problemi (18)
  - *Messaggio chiave:* Una buona interazione può svilupparsi attraverso più scambi e non richiede una richiesta iniziale perfetta.
- **5.3 I diversi ruoli che l'AI può assumere**: Sette ruoli possibili (21) · Fonte, assistente operativo, supporto creativo (22) · Analista, revisore, tutor (23) · L'AI come strumento di confronto critico (24) · Ruolo assegnato e competenza effettiva (25)
  - *Messaggio chiave:* Assegnare un ruolo all'AI può orientarne il comportamento, ma non garantisce che abbia le competenze richieste.
- **5.4 La collaborazione uomo-AI**: Ottenere una risposta o collaborare (28) · Suddividere le attività tra persona e sistema (29) · Capacità complementari (30) · Produrre, rivedere, migliorare (31) · Supporto al ragionamento e alla valutazione (32) · Competenze, contesto e responsabilità (33)
  - *Messaggio chiave:* Il valore dell'AI può nascere dalla combinazione delle capacità del sistema con quelle della persona, senza implicare la sostituzione del giudizio umano.
- **5.5 I livelli di delega all'Intelligenza Artificiale**: Cinque livelli di delega (36) · Che cosa fanno l'AI e la persona a ogni livello (37) · Assistenza, collaborazione, delega, automazione (38) · Come cambia il ruolo umano (39) · Responsabilità e controllo ai diversi livelli (40) · Scegliere il livello adeguato (41)
  - *Messaggio chiave:* Una maggiore autonomia non determina automaticamente risultati migliori: il livello di delega deve essere adeguato al compito, alle capacità del sistema, ai rischi e ai controlli disponibili. Sottotem
- **5.6 La qualità dipende anche dalla persona**: Otto fattori che dipendono dalla persona (44) · Obiettivi chiari e comprensione del problema (45) · Contesto e competenze di dominio (46) · Domande, interpretazione e feedback (47) · Utilizzo passivo e utilizzo attivo (48)
  - *Messaggio chiave:* Le competenze umane restano determinanti per formulare problemi, interpretare risultati e riconoscere output inadeguati.
- **5.7 Limiti e rischi della relazione conversazionale**: Antropomorfizzazione (51) · Fiducia eccessiva e accettazione passiva (52) · Automation bias (53) · Il rischio della delega cognitiva (54) · Dipendenza e preservazione del giudizio (55)
  - *Messaggio chiave:* Un'interazione naturale e convincente non attribuisce al sistema intenzionalità, giudizio umano o responsabilità decisionale.
- **Conclusioni**: Le domande guida: le nostre risposte (57) · Che cosa portiamo a casa (58) · Principi per un dialogo consapevole (59) · Prossimo passo: il Tema 6 (60) · Fonti e riferimenti (61)

### Tema 6 · Prompting e tecniche di interazione con l'AI
*Area: Interagire con l'AI · 72 slide · file `Tema6_Prompting_tecniche_interazione.pptx` · esposizione stimata circa 1 h 10 min*

- **Introduzione**: Obiettivo del modulo (2) · Dieci domande guida per questo modulo (3) · Il percorso del modulo (4)
- **6.1 Fondamenti del prompting**: Che cos'è un prompt (6) · Domanda, istruzione, richiesta di esecuzione (7) · Richieste generiche e contestualizzate (8) · Chiarezza, specificità, pertinenza (9) · Qualità dell'input e utilità dell'output (10) · Prompting e programmazione tradizionale (11) · Prompting e limiti delle istruzioni (12)
  - *Messaggio chiave:* Il prompt comunica obiettivi e aspettative, ma non è un comando che assicura un risultato deterministico e corretto.
- **6.2 Gli elementi di una richiesta efficace**: Prima il problema, poi il prompt (15) · Otto elementi possibili (16) · Anatomia di una richiesta (17) · Vincoli, formato e criteri di qualità (18) · Ruoli e prospettive (19) · Non serve sempre un prompt lungo (20)
  - *Messaggio chiave:* Un prompt efficace rende espliciti i requisiti rilevanti; non deve necessariamente essere lungo o contenere tutti gli elementi in ogni situazione.
- **6.3 Il ruolo del contesto nel prompting**: Che cosa è contesto (23) · Distinguere informazioni, istruzioni, esempi (24) · Qualità del contesto: pertinente, completo, comprensibile (25) · Chiedere all'AI di esplicitare le informazioni mancanti (26) · Informazioni contraddittorie (27) · Gestire i limiti della finestra di contesto (28)
  - *Messaggio chiave:* Fornire più informazioni non produce automaticamente risultati migliori; è preferibile un contesto pertinente, sufficientemente completo e comprensibile.
- **6.4 Tecniche fondamentali di prompting**: Una cassetta degli attrezzi (31) · Zero-shot e few-shot (32) · Istruzioni strutturate e delimitazione (33) · Scomporre i compiti complessi (34) · Alternative e confronto con criteri (35) · Chiedere chiarimenti prima dell'esecuzione (36) · Scegliere la tecnica in base al compito (37)
  - *Messaggio chiave:* La complessità della tecnica deve essere proporzionata al compito; non esiste una strategia unica migliore in ogni situazione.
- **6.5 Prompting iterativo**: Il ciclo del miglioramento progressivo (40) · Feedback efficaci (41) · Raffinare, approfondire, riformulare (42) · Modificare la richiesta o ricominciare (43) · I limiti dell'iterazione (44)
  - *Messaggio chiave:* L'iterazione consente di migliorare l'aderenza al compito, ma la verifica indipendente della correttezza appartiene a una fase distinta.
- **6.6 Guidare il formato e la struttura degli output**: Definire il formato desiderato (47) · Report, documenti e comunicazioni professionali (48) · Dettaglio, tono e destinatario (49) · Introduzione agli output strutturati (50) · Vincoli di presentazione e criteri verificabili (51)
  - *Messaggio chiave:* La forma dell'output ne condiziona l'utilità nelle attività successive, ma la buona formattazione non dimostra la correttezza del contenuto.
- **6.7 Prompting per attività professionali**: Attività creative, analitiche e operative (54) · Scrittura e revisione di contenuti (55) · Analisi e sintesi documentale (56) · Informazioni e dati (57) · Ricerca, alternative, brainstorming e problem solving (58) · Report e comunicazioni (59)
  - *Messaggio chiave:* Il metodo deve adattarsi allo scopo e al contesto lavorativo; il tema insegna ad applicare i principi, non a memorizzare prompt universali.
- **6.8 Istruzioni riutilizzabili e standardizzazione**: Prompt occasionali e ricorrenti (62) · Template di prompt (63) · Librerie, istruzioni persistenti, assistenti configurati (64) · Standardizzare, versionare, manutenere (65) · I limiti della standardizzazione (66)
  - *Messaggio chiave:* Istruzioni riutilizzabili possono favorire coerenza e produttività, ma devono essere manutenute e non sostituiscono il controllo dei risultati.
- **Conclusioni**: Le domande guida: le nostre risposte (68) · Che cosa portiamo a casa (69) · Uno schema per le richieste importanti (70) · Prossimo passo: il Tema 7 (71) · Nota sulle fonti e sugli esempi (72)

### Tema 7 · Verifica degli output e pensiero critico nell'utilizzo dell'AI
*Area: Interagire con l'AI · 73 slide · file `Tema7_Verifica_output_pensiero_critico.pptx` · esposizione stimata circa 1 h 15 min*

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
- **Conclusioni**: Le domande guida: le nostre risposte (69) · Che cosa portiamo a casa (70) · Valutare, verificare, decidere: una scheda pratica (71) · Che cosa viene dopo (72) · Fonti e riferimenti (73)

### Tema 8 · AI per testi, documenti e conoscenza
*Area: Esplorare le possibilità dell'AI · 81 slide · file `Tema8_AI_testi_documenti_conoscenza.pptx` · esposizione stimata circa 1 h 31 min*

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
- **Conclusioni**: Le domande guida: le nostre risposte (77) · Che cosa portiamo a casa (78) · Quattro modalità: una scheda pratica (79) · Che cosa viene dopo (80) · Fonti e riferimenti (81)

### Tema 9 · AI per dati e analisi
*Area: Esplorare le possibilità dell'AI · 84 slide · file `Tema9_AI_dati_analisi.pptx` · esposizione stimata circa 1 h 35 min*

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
- **Conclusioni**: Le domande guida: le nostre risposte (80) · Che cosa portiamo a casa (81) · Quattro fasi: una scheda pratica (82) · Che cosa viene dopo (83) · Fonti e riferimenti (84)

### Tema 10 · AI multimodale e creazione di contenuti
*Area: Esplorare le possibilità dell'AI · 74 slide · file `Tema10_AI_multimodale_contenuti.pptx` · esposizione stimata circa 1 h 22 min*

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
- **Conclusioni**: Le domande guida: le nostre risposte (70) · Che cosa portiamo a casa (71) · Una scheda pratica (72) · Che cosa viene dopo (73) · Fonti e riferimenti (74)

### Tema 11 · Assistenti, agenti e automazioni con l'AI
*Area: Esplorare le possibilità dell'AI · 77 slide · file `Tema11_Assistenti_agenti_automazioni.pptx` · esposizione stimata circa 1 h 28 min*

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
*Area: Comprendere il valore per l'azienda · 72 slide · file `Tema12_AI_creazione_valore_azienda.pptx` · esposizione stimata circa 1 h 20 min*

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
*Area: Comprendere il valore per l'azienda · 63 slide · file `Tema13_AI_trasformazione_lavoro_processi.pptx` · esposizione stimata circa 1 h 12 min*

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
- **Conclusioni**: Le domande guida: le nostre risposte (59) · Che cosa portiamo a casa (60) · Domande sul cambiamento del lavoro (61) · Che cosa viene dopo (62) · Fonti e riferimenti (63)

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
- **17.8 Buone pratiche per un uso sicuro**: Prima dell'uso (64) · Durante l'uso (65) · Dopo l'uso (66) · Quattro azioni possibili (67) · La checklist del documento (68)
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
- **18.8 Una governance proporzionata**: I presidi essenziali (65) · Esempio D: aziende diverse (66) · Framework e standard volontari (67) · Formazione e governance (68) · La checklist del documento (69) · Migliorare nel tempo (70)
  - *Messaggio chiave:* Non esiste un modello organizzativo unico, ma è necessario rispettare gli obblighi pertinenti e rendere effettivi i controlli scelti.
- **Conclusioni**: Le domande guida: le nostre risposte (72) · Che cosa portiamo a casa (73) · Quattro equivoci, quattro esempi (74) · Che cosa evitare (75) · Il percorso completato (76) · Fonti e riferimenti (77)
