# Scheda formazione · Laser Srl · AI Adoption

Ultimo aggiornamento: 9 ottobre 2026 · Stato: **agenda in progettazione** (scheda e agenda da validare prima di produrre i deck)

## Committente

| Voce | Dato |
|---|---|
| Ragione sociale | Laser S.r.l. (marchio Laser Biscuit), P.IVA 02640680233 |
| Sede | Via Saturno 36, 37059 Santa Maria di Zevio (VR); nuova unità produttiva a Buttapietra |
| Attività | Progetta e costruisce forni a tunnel, impastatrici, tunnel di raffreddamento, linee di sfogliatura e linee complete per biscotti, cracker, pasticceria, prodotti da forno e petfood; lavorazioni meccaniche interne; installazione, avviamento e formazione presso i clienti, anche esteri |
| ATECO | 28.93.00 · Fabbricazione di macchine per l'industria alimentare, delle bevande e del tabacco |
| Dimensione | Fatturato 2025 circa 32,3 milioni di euro (2024 circa 30,1); da 100 a 249 dipendenti; costo del personale 2025 circa 6,1 milioni. **Media impresa** |
| Fonti | [laserbiscuit.com](https://www.laserbiscuit.com/); [fatturatoitalia.it](https://www.fatturatoitalia.it/laser-srl-02640680233) (fonte non ufficiale: confermare sul bilancio se servono i dati precisi) |

**Da scoprire in aula (sessione 1):** se le macchine raccolgono dati (PLC, sensori, teleassistenza); quale Copilot è in uso (Copilot Chat o Microsoft 365 Copilot, con quali licenze e impostazioni sui dati); se esiste già una policy sull'uso dell'AI; se l'azienda si è già registrata come soggetto NIS2.

## Riferimenti contrattuali

- Preventivo NetAi "Percorso formativo AI Adoption per l'impresa", 9 luglio 2026, versione 1.0.
- 3 sessioni da 4 ore in presenza, 12 ore in totale.
- **Incongruenza da correggere nel preventivo:** il testo indica trasferta di 100 euro a sessione, la tabella 80 euro a sessione (3 x 80 = 240 euro; totale 1.200 euro coerente con la tabella).

## Pubblico

- Reparti indicati nel preventivo: tecnico, produzione, qualità, service, commerciale, amministrazione, HR.
- Livello di partenza: misto, da rilevare con il sondaggio iniziale.
- Numero di partecipanti: **da definire**.

## Obiettivi (dal preventivo)

Al termine del percorso il team avrà:
1. un linguaggio comune sull'AI;
2. un portfolio di casi d'uso prioritizzati;
3. una proposta di roadmap con 1-2 schede progetto pronte da avviare.

## Formato

| Voce | Scelta |
|---|---|
| Modalità | Aula, 3 sessioni da 4 ore |
| Percorsi | **Due percorsi alternativi**, sugli stessi argomenti: **A interattivo** (`agenda.md`, esercizi, gara di prompt, workshop) e **B frontale** (`agenda_B_frontale.md`, parla solo il formatore, esempi guidati al posto delle attività). Si sceglie in base alla risposta dell'aula, anche durante la sessione |
| Date | **da definire** |
| Strumento per le demo | Microsoft Copilot, usato dal formatore. Nessun PC richiesto ai partecipanti |
| Demo | Preparate in anticipo; una dal vivo, le altre in video di 2-3 minuti; screenshot nelle slide come riserva |
| Materiali d'aula | Post-it, bollini colorati per la matrice, schede stampate |
| Lavagna digitale | **AFFiNE**, app desktop con spazio di lavoro locale (gratuito, dati solo sul PC del formatore). In aula si lavora su carta; il formatore trascrive in pausa o a fine sessione; nel workshop la board si proietta. Export in PDF per Laser a fine percorso. Schema in `board_affine.md` |
| Brand | **Neutro**, nessun brand NetAi (scelta dell'utente) |
| Deck | Un deck per sessione: slide selezionate dai 18 deck della base più slide nuove per le parti mancanti |
| Esempi | Sempre fittizi e dichiarati come tali, ambientati in un costruttore di forni e linee per prodotti da forno |

## Filo conduttore del percorso

Il **parcheggio dei casi d'uso**: un cartellone fisico in aula, riportato nella board AFFiNE, che si riempie in tutte e tre le sessioni (sprechi informativi nella sessione 1, idee dalle demo e shortlist nella sessione 2) e diventa la materia prima del workshop finale.

## Punti normativi specifici per Laser (da presentare come sintesi, non parere legale)

1. **AI Act e macchine.** Il Digital Omnibus (Reg. UE 2026/1744, art. 1, punto 41, e art. 3) ha spostato il Regolamento Macchine (UE) 2023/1230 nella sezione B dell'Allegato I dell'AI Act. Per l'AI usata come componente di sicurezza di una macchina, i requisiti entreranno nel Regolamento Macchine con atti delegati applicabili entro il 2 agosto 2028. Verificato sul testo ufficiale (cartella `Normative/AIAct`).
2. **Regolamento Macchine (UE) 2023/1230.** Data di applicazione generale indicata di norma al 20 gennaio 2027, ma risulta una rettifica delle date: **da verificare su EUR-Lex**.
3. **NIS2.** Con ATECO 28.93 (NACE C28) e dimensione media, Laser rientrerebbe tra i **soggetti importanti** (Allegato II, punto 5, lettera d, fabbricazione di macchinari e apparecchiature). In Italia: D.Lgs. 138/2024. Fonte secondaria ([nisd2.eu](https://nisd2.eu/it/wiki/scope/am-i-machinery-manufacturer-nis2)): **da verificare sul testo e con l'azienda**.
4. **Cyber Resilience Act** (Reg. UE 2024/2847). Riguarda i prodotti con elementi digitali; segnalazione di vulnerabilità e incidenti dall'11 settembre 2026, applicazione generale dall'11 dicembre 2027 ([CMS](https://cms.law/en/bel/legal-updates/ready-respond-report-the-cyber-resilience-act-s-reporting-regime-is-here)). Pertinente se le macchine hanno componenti digitali connessi: **da verificare caso per caso**.
5. **AI Act per l'uso interno.** Laser è deployer degli strumenti che usa (Copilot); attenzione all'HR (Allegato III, selezione e gestione dei lavoratori, dal 2 dicembre 2027) e all'articolo 4 sull'alfabetizzazione, come riscritto dall'Omnibus.

## Prodotti da consegnare

- `agenda.md` (percorso A, interattivo) e `agenda_B_frontale.md` (percorso B, frontale)
- `note_scelte.md` (questa cartella)
- 3 deck, uno per sessione (dopo la validazione dell'agenda)
- Materiali fittizi per le demo e gli esercizi
- Schede stampabili: esercizio sprechi, shortlist, matrice, scheda progetto
- Board AFFiNE (`board_affine.md`) ed export PDF finale per Laser
- Facoltativi: video delle demo (a cura del formatore), dispensa per i partecipanti
