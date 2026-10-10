# Portfolio di casi d'uso · Laser Srl · AI Adoption

Ultimo aggiornamento: 10 ottobre 2026

**Portfolio indicativo, preparato dal formatore.** I casi sono tipici di un costruttore di macchine per prodotti da forno, ma valori, fattibilità e rischi sono **valutazioni illustrative**, non dati di Laser. Vanno verificati con l'azienda.

Usi:
- **Percorso A:** spunti per il formatore se la shortlist della sessione 2 resta povera; base di confronto per il workshop.
- **Percorso B:** contenuto delle slide B8, B9 (portfolio), B11 (matrice), B12 e B13 (schede progetto), B14 (roadmap).

## 1. I casi d'uso

Legenda. **Luogo:** I = AI interna, C = AI per i clienti, M = AI nella macchina. **Valore** e **fattibilità:** alto, medio, basso. **Rischio:** basso, medio, alto, con il motivo principale.

| # | Reparto | Caso d'uso | Luogo | Valore | Fattibilità | Rischio | Prerequisiti e note |
|---|---|---|---|---|---|---|---|
| C01 | Tecnico | Ricerca in specifiche, disegni e documenti di commessa ("dove abbiamo già risolto questo problema?") | I | Alto | Media | Medio: disegni e know-how riservati | Documenti ordinati e con versioni chiare; strumento autorizzato con permessi |
| C02 | Tecnico | Bozze di manuali d'uso e manutenzione a partire da schede tecniche e manuali precedenti | I, C | Alto | Media | Medio: un errore nel manuale arriva al cliente | Revisione tecnica obbligatoria; i contenuti di sicurezza restano scritti e approvati da persone |
| C03 | Produzione | Istruzioni di lavoro e liste di controllo per il montaggio, dalle distinte e dai disegni | I | Medio | Media | Basso | Distinte e cicli aggiornati |
| C04 | Produzione | Sintesi dei passaggi di turno e dei problemi in officina | I | Basso | Alta | Basso | Note di turno scritte o dettate |
| C05 | Qualità | Analisi delle non conformità e bozze di rapporti 8D | I | Medio | Alta | Medio: conclusioni sulle cause da verificare | Storico delle non conformità; l'analisi delle cause resta delle persone |
| C06 | Qualità | Controllo di completezza del fascicolo tecnico di commessa (documenti presenti o mancanti) | I | Medio | Media | Alto: la conformità CE è responsabilità del fabbricante | Solo come lista di controllo; **mai** come valutazione di conformità |
| C07 | Service | Assistente per il troubleshooting, che risponde citando manuali e ticket storici | I (poi C) | Alto | Media | Medio: risposte sbagliate su interventi in campo | Manuali e ticket ordinati; risposte sempre con la fonte; sicurezza esclusa |
| C08 | Service | Report d'intervento dettato a voce dal tecnico e strutturato in automatico | I | Medio | Alta | Basso | Modello di report concordato; il tecnico rilegge prima dell'invio |
| C09 | Service e ricambi | Identificazione del ricambio da foto o descrizione del cliente | C | Medio | Bassa | Medio: ricambio sbagliato, costi e fermi | Catalogo ricambi con immagini e codici puliti |
| C10 | Commerciale | Bozza d'offerta strutturata dal capitolato del cliente, con l'elenco delle informazioni mancanti | I | Alto | Alta | Medio: prezzi e condizioni | L'AI non scrive prezzi né condizioni; il commerciale completa e approva |
| C11 | Commerciale | Traduzione e adattamento di offerte, email e documentazione per clienti esteri | I | Medio | Alta | Medio: errori di traduzione su dati tecnici | Glossario tecnico multilingua; rilettura dei dati numerici |
| C12 | Amministrazione | Bozze di solleciti e supporto alle riconciliazioni | I | Basso | Alta | Medio: dati di clienti e fornitori | Strumento autorizzato; nessun invio automatico |
| C13 | HR | Materiali di onboarding e formazione interna a partire da manuali e procedure | I | Medio | Alta | Basso | **Escluso** l'uso per selezionare o valutare le persone (AI Act, Allegato III) |
| C14 | Prodotto | Controllo qualità visivo dei prodotti all'uscita del forno (colore, dimensione, rotture) | M | Alto | Bassa | Medio: responsabilità sul prodotto, dati del cliente | Telecamere, immagini etichettate, partner tecnologico; verificare il quadro normativo |
| C15 | Prodotto e service | Monitoraggio delle anomalie e manutenzione predittiva (temperature, bruciatori, nastri, motori) | M, C | Alto | Bassa | Medio: dipende dai dati e dall'uso | Le macchine raccolgono dati? (da scoprire in sessione 1); connessione e consenso del cliente; CRA e NIS2 |
| C16 | Prodotto | Ottimizzazione dei consumi energetici del forno | M | Medio | Bassa | Basso | Dati di consumo e di processo; valore per il cliente da verificare |

**Lettura per luogo (slide B9):** 12 casi di AI interna (si possono iniziare con gli strumenti già disponibili), 4 casi per i clienti, 3 nella macchina (richiedono dati, investimenti e attenzione normativa). Alcuni casi stanno in più luoghi.

**Che cosa non mettere nel portfolio:** usi su decisioni sulle persone (selezione, valutazione delle prestazioni); AI come componente di sicurezza della macchina senza un progetto dedicato (Regolamento Macchine e AI Act); invii automatici a clienti senza revisione.

## 2. Matrice di esempio (slide B11)

Otto casi posizionati. **Valutazioni illustrative**, da rifare con Laser.

| Quadrante | Casi | Perché |
|---|---|---|
| **Quick win** (valore alto, fattibilità alta) | C10 Bozza d'offerta · C08 Report d'intervento · C11 Traduzioni | Strumenti già disponibili (Copilot), dati poco critici, revisione umana semplice |
| **Strategiche** (valore alto, fattibilità bassa o media) | C07 Assistente per il troubleshooting · C15 Manutenzione predittiva · C14 Qualità visiva | Valore alto, ma richiedono dati ordinati, integrazioni, investimenti; C14 e C15 toccano il prodotto |
| **Facili ma modeste** | C12 Solleciti | Facile, ma il beneficio è piccolo |
| **Da usare solo come supporto** | C06 Fascicolo tecnico | Condizione di esclusione: la valutazione di conformità non si delega. Resta solo la lista di controllo |

**Bollino rosso (rischio da approfondire):** C06, C14, C15.

Messaggio della slide: **combinare** alcune quick win per imparare (C10, C08, C11) e preparare le condizioni per una strategica (C07 prima, perché porta a C15).

## 3. Scheda progetto di esempio 1 (slide B12) · Assistente per il troubleshooting del service (C07)

Campi della scheda dell'opportunità (T15·73). **Esempio fittizio: i numeri sono da stimare con Laser.**

| Fase | Domanda | Risposta di esempio |
|---|---|---|
| Individuare | Problema, per chi? | I tecnici del service, in sede e in campo, perdono tempo a cercare nei manuali e nei ticket passati come è stato risolto un guasto simile; le risposte dipendono da chi è disponibile al telefono |
| | Risultato desiderato? | Trovare in pochi minuti le soluzioni già documentate, con il riferimento al documento |
| | Alternative non AI? | Riordinare l'archivio dei manuali; una FAQ interna dei guasti più frequenti. **Da fare comunque:** sono prerequisiti |
| Descrivere | Chi, attività, informazioni? | Tecnici service; diagnosi a distanza e preparazione degli interventi; manuali delle macchine, ticket chiusi degli ultimi anni, report d'intervento |
| | Ruolo dell'AI, supervisione? | Cerca e propone soluzioni **citando la fonte**; il tecnico decide. Non risponde su sicurezza, gas, interventi elettrici: rimanda al manuale e al responsabile |
| | Volume, confini, ipotesi? | Volume: numero di richieste di assistenza al mese (da stimare). Confini: solo uso interno nella prima fase. Ipotesi critica: i ticket storici sono scritti in modo utilizzabile |
| Valutare | Beneficio realistico? | Meno tempo di ricerca, diagnosi più rapide, meno dipendenza dai tecnici più esperti. Da misurare sul pilota |
| | Costi completi? | Licenze o piattaforma, riordino dei documenti, tempo dei tecnici senior per verificare le risposte, manutenzione delle fonti |
| | Desiderabile, fattibile, sostenibile? | Desiderabile: sì, se fa risparmiare tempo vero. Fattibile: dipende dallo stato dei documenti. Sostenibile: serve un responsabile delle fonti |
| | Esclusioni? | Informazioni di sicurezza e procedure su gas ed elettricità: solo dal manuale approvato |
| Confrontare | Posizione nella matrice? | Strategica: valore alto, fattibilità media |
| Verificare | Verifica più leggera? | Pilota di 6-8 settimane con 3-4 tecnici, su una sola famiglia di macchine, con Copilot e una cartella di documenti selezionati |
| | Criteri decisi prima? | **Successo:** almeno il 70% delle risposte, su un campione di 50 domande reali, giudicate corrette e con la fonte giusta dai tecnici senior. **Zona intermedia:** 50-70%, si riordinano le fonti e si riprova. **Insuccesso:** sotto il 50%. **Limite da non superare:** una risposta sbagliata su un tema di sicurezza non segnalata come tale |

## 4. Scheda progetto di esempio 2 (slide B13) · Bozza d'offerta dal capitolato del cliente (C10)

**Esempio fittizio: i numeri sono da stimare con Laser.**

| Fase | Domanda | Risposta di esempio |
|---|---|---|
| Individuare | Problema, per chi? | I commerciali e l'ufficio tecnico ricevono capitolati e richieste in lingue e formati diversi; estrarre i requisiti e capire che cosa manca richiede tempo e giri di email |
| | Risultato desiderato? | Una scheda dei requisiti ordinata e un elenco delle domande da fare al cliente, il giorno stesso della richiesta |
| | Alternative non AI? | Un modulo standard di raccolta requisiti da mandare ai clienti. **Utile comunque:** è la struttura che l'AI deve compilare |
| Descrivere | Chi, attività, informazioni? | Commerciali e ufficio tecnico; prima analisi della richiesta; email, capitolato, disegni del layout del cliente |
| | Ruolo dell'AI, supervisione? | Estrae i requisiti, segnala contraddizioni e informazioni mancanti, prepara la bozza della risposta. **Non scrive prezzi, tempi di consegna né condizioni.** Il commerciale completa e invia |
| | Volume, confini, ipotesi? | Volume: richieste d'offerta al mese (da stimare). Confini: niente invio automatico; i dati economici restano fuori. Ipotesi critica: la scheda requisiti standard copre la maggior parte delle richieste |
| Valutare | Beneficio realistico? | Prima risposta più rapida al cliente, meno requisiti dimenticati, meno rilavorazioni dell'ufficio tecnico |
| | Costi completi? | Tempo per definire la scheda requisiti e i prompt; formazione dei commerciali; revisione |
| | Desiderabile, fattibile, sostenibile? | Fattibile subito con Copilot e documenti del cliente; attenzione alla riservatezza dei capitolati |
| | Esclusioni? | Capitolati sotto accordo di riservatezza che vieta strumenti esterni: verificare con l'ufficio legale e con le impostazioni dello strumento |
| Confrontare | Posizione nella matrice? | Quick win |
| Verificare | Verifica più leggera? | 4 settimane, 2 commerciali, le richieste reali in arrivo, confronto con il metodo attuale |
| | Criteri decisi prima? | **Successo:** almeno l'80% dei requisiti estratti correttamente e almeno una lacuna utile trovata in metà delle richieste. **Insuccesso:** sotto il 60%, o più tempo di revisione che di lavoro risparmiato. **Limite da non superare:** un dato tecnico sbagliato inviato al cliente |

## 5. Proposta di roadmap (slide B14 e N33)

**Da validare con la direzione di Laser.**

| Fase | Quando | Che cosa |
|---|---|---|
| 0 · Regole e prime prove | Primo mese | Policy minima d'uso e strumenti autorizzati (sessione 3); referente interno per l'AI; uso individuale di Copilot sulle quick win C08 e C11 |
| 1 · Primo pilota | Mesi 1-3 | Pilota C10 (bozza d'offerta) con criteri decisi prima; in parallelo, riordino dei manuali e dei ticket per C07 |
| 2 · Pilota strategico | Mesi 3-6 | Pilota C07 (assistente per il troubleshooting); indagine sui dati che le macchine raccolgono, per valutare C15 |
| 3 · Decidere | Mesi 6-12 | Estendere, modificare o fermare i piloti; valutare un progetto sul prodotto (C14 o C15) con un partner, verificando Regolamento Macchine, AI Act, Cyber Resilience Act |

Ad ogni fase: misurare con gli indicatori decisi prima, raccogliere i riscontri delle persone, aggiornare la policy.
