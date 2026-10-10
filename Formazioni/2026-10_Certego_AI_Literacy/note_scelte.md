# Note sulle scelte · Certego · AI Literacy, consapevolezza e normativa

Ultimo aggiornamento: 10 ottobre 2026

## Decisioni prese con l'utente (10 ottobre 2026)

1. **Formazione autonoma:** non deriva da altre formazioni (Laser Srl, Energia); si parte direttamente dalla base.
2. **Impostazione:** corso di consapevolezza generica con i temi normativi, più un **workshop collegato alla definizione delle policy di reparto**.
3. **Reparti:** Amministrazione, Legal, **Customer Care** (al posto della Progettazione, ipotizzata all'inizio).
4. **Formato:** due mezze giornate da 4 ore, con un compito tra i due incontri.
5. **ISO/IEC 42001:** solo un **accenno di 10'** (una slide, insieme a T18·67 sugli standard volontari). L'utente non è pronto per una formazione sulla norma (decisione del 10 ottobre 2026, che sostituisce la prima ipotesi di un blocco di 30' e di un modello di policy agganciato ai controlli della norma). I 20' liberati vanno al quadro normativo (+10') e al Workshop 3 (+15'), con 5' tolti dal margine finale.
6. **Brand:** tema neutro.
7. **Percorso di riserva tutto frontale** (`agenda_B_frontale.md`): stessi argomenti e stesso formato, 142 slide della base e 16 nuove, con i punti di passaggio tra i due percorsi. Con il percorso B le policy di reparto sono esempi del formatore e non bozze scritte dai partecipanti.

## Perché questa impostazione

- **Pubblico già sensibile alla sicurezza:** Certego è un'azienda di cyber security. La consapevolezza si concentra sui rischi **nuovi** dell'AI (perdita di dati tramite prompt, prompt injection, deepfake, automation bias, Shadow AI) invece che sulla sicurezza generica.
- **Dati di terzi molto delicati:** report di incidente, log e contratti dei clienti. Per questo il Workshop 1 "Posso caricarlo?" produce subito la tabella dati e strumenti, che diventa il **quadro comune** delle tre policy.
- **ISO 27001 già certificata:** nell'accenno si dice soltanto che la ISO/IEC 42001 ha la stessa struttura delle norme che Certego già applica e che le policy scritte in aula sarebbero un punto di partenza riutilizzabile. Il modello di policy segue gli elementi del T18 (T18·45), senza riferimenti ai controlli della norma.
- **Policy di reparto e politica aziendale:** la politica aziendale sull'uso dell'AI spetta alla direzione. Il corso produce **bozze di reparto** e un elenco di punti aperti per la direzione; questo evita di presentare il corso come la soluzione della conformità.
- **Prova incrociata:** una policy si giudica dalla capacità di rispondere a situazioni concrete (T18·47 "Scritta o praticata"). La rotazione tra reparti fa emergere lacune e linguaggio poco chiaro.

## Che cosa è preso dalla base

| Blocco | Temi | Perché |
|---|---|---|
| Come funziona l'AI | T2 (2.1, 2.4, 2.5, 2.6, 2.7) | Il minimo per capire dove vanno i dati e perché l'output varia |
| Capacità e limiti | T3 (3.3, 3.4, 3.8) | Allucinazioni, compiacenza, conseguenze degli errori: base delle regole di verifica |
| Verificare | T7 (7.3, 7.8), T5 (5.7), T17 (17.7) | Sezione "Verifica e controllo umano" della policy |
| Rischi per le informazioni | T17 (17.2, 17.3, 17.6), T10 (10.8), T16 (16.1) | Sezioni dati, usi vietati, segnalazioni |
| Workshop 1 | T14 (14.6) | Classificazione e minimo privilegio |
| Normativa | T18 (18.2, 18.3, 18.4, 18.7) | Quadro essenziale, ruoli, art. 4 |
| Dalla norma alla policy | T18 (18.5, 18.8) | Elementi di una policy, quattro categorie d'uso, checklist |

**Rimandi tra temi** (mappa della sezione 10 delle istruzioni): il T17 presuppone il T11 per gli agenti; qui gli agenti non sono trattati, quindi le slide T17·27 e T17·28 vanno presentate restando sul caso di documenti ed email analizzati, senza entrare nelle azioni automatiche. Il T18 presuppone T16 e T17, entrambi coperti in parte nell'incontro 1.

## Che cosa è stato escluso, e perché

- **T4 (ecosistema e prodotti):** contenuto molto sensibile al tempo e poco utile per le policy; basta la distinzione modello e applicazione (T2·46).
- **T6 (prompting) e Temi 8-11 (applicazioni):** il corso non ha obiettivi di produttività. Eventuale modulo successivo.
- **Temi 12-16 (valore e adozione):** fuori dall'obiettivo, salvo lo Shadow AI (T16·14).
- **Alto rischio in dettaglio (T18·28-29):** per i tre reparti non è centrale; resta T18·30 "La finalità decide" con l'esempio della selezione del personale, utile all'Amministrazione se gestisce candidature.

## Lacune della base colmate con slide nuove

| Slide | Contenuto | Nota |
|---|---|---|
| C9 | NIS2 e uso dell'AI | NIS2 assente nella base (già segnalato con la formazione Laser). I fornitori di servizi di sicurezza gestiti rientrano tra i settori della direttiva: **inquadramento di Certego da verificare** |
| C10 | Contratti con i clienti e fornitori di AI | Clausole di riservatezza, subfornitori, trasferimenti di dati |
| C11 | ISO/IEC 42001 in una slide | Assente nella base (il T18 ha solo un cenno agli standard volontari, slide 67). Solo informativa: che cos'è, legame con la ISO 27001, esistenza della certificazione accreditata in Italia |
| C4 | Dati tipici di Certego | Esempi fittizi |

**Proposta per la base:** valutare se portare nella base, dopo l'edizione, la slide sulla NIS2 e l'accenno alla ISO/IEC 42001, eventualmente nel T18.

## Fonti da verificare

- ISO/IEC 42001:2023: contenuto della slide C11 (struttura della norma).
- Accredia, Circolare tecnica DC 08/2026 sull'accreditamento per la certificazione dei sistemi di gestione per l'AI: https://accredia.it/wp-content/uploads/2026/02/Circolare_tecnica_DC_08-2026_ITA-Accreditamento-MS-per-la-certificazione-dei-sistemi-di-gestione-IA.pdf
- Certificazioni di Certego (ISO 27001, ISO 9001), dal sito aziendale: https://www.certego.net/iso/Cert_3917107_iso_27001_it.pdf
- NIS2 (Direttiva (UE) 2022/2555) e D.Lgs. 138/2024: settore dei servizi gestiti di sicurezza.
- AI Act, art. 50 (trasparenza dei sistemi che interagiscono con persone), per l'eventuale assistente rivolto ai clienti del Customer Care.
- Date dell'AI Act dopo il Reg. (UE) 2026/1744: ricontrollare prima dell'edizione.

## Possibili sviluppi

- **Terzo incontro facoltativo di 2 ore,** dopo 4-6 settimane: riesame delle policy approvate e dei primi casi reali.
- **Eventuale percorso ISO/IEC 42001** in futuro, per direzione, responsabile del sistema di gestione e Legal, se Certego lo chiederà e quando il materiale sarà pronto. Le bozze di policy ne sarebbero il punto di partenza.
