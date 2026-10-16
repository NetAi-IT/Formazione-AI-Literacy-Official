# Esercitazioni · Sessione 2 · Laser Srl · AI Adoption

Ultimo aggiornamento: 16 ottobre 2026 · Da usare con `sessione2_scaletta_formatore.md` (i numeri di slide si riferiscono al deck della sessione 2)

Tutte le esercitazioni usano **materiali fittizi** (forno "TF-900 Demo", azienda "Forni Demo S.r.l.", fornitori e clienti inventati) o domande senza documenti. Nessun dato di Laser entra in Copilot. Lo strumento lo usa solo il formatore; i partecipanti lavorano su carta.

| # | Esercitazione | Blocco | Durata | Slide | Tema |
|---|---|---|---|---|---|
| 1 | Caccia all'allucinazione | Recupero Tema 3 | 7' | 14 | Allucinazioni, autorevolezza apparente |
| 2 | Domanda orientata o neutra? (con la prova "Sei sicuro?") | Recupero Tema 3 | 6' | 21 | Bias della domanda, tendenza ad assecondare |
| 3 | Gara di prompt: la lista di controllo del manutentore | Prompting | 12-15' | 37 | Elementi di una richiesta, verifica |
| 4 | Dalla mappa alla shortlist | Casi d'uso | 25' | 62 | Sprechi, ruolo dell'AI, rischio |
| Mini A | Bollini sugli sprechi | Apertura | 4' | 4 | Priorità |
| Mini B | Quale delle due è vera? | Recupero Tema 3 | 3' | 11 | Plausibilità e veridicità |

---

## Mini-attività A · Bollini sugli sprechi (apertura, 4')

**Obiettivo:** dare un peso agli sprechi della sessione 1, che hanno quasi tutti frequenza sconosciuta.
**Materiali:** board AFFiNE proiettata o cartellone della sessione 1; 3 bollini a testa.
**Consegna:** "Mettete i vostri tre bollini sugli sprechi che vi fanno perdere più tempo in un mese. Potete metterli anche su sprechi di altri reparti."
**Debriefing:** il formatore legge i tre sprechi con più bollini e chiede a chi li ha votati: quante volte al mese, quanto tempo ogni volta? Annotare in giallo sulla board. I temi più votati sono il punto di partenza dell'esercizio 4.
**Percorso B:** alzata di mano sui sei temi della slide 4.

## Mini-attività B · Quale delle due è vera? (slide 11, 3')

**Consegna:** "Due frasi, scritte con la stessa sicurezza. Alzata di mano: A o B?"
**Soluzione:** A. Le definizioni dell'AI Act sono all'articolo 3 del Regolamento (UE) 2024/1689, entrato in vigore il 1° agosto 2024. B sbaglia due dettagli plausibili: l'articolo 5 riguarda le pratiche vietate, e la data è inventata.
**Messaggio:** la forma non aiuta a distinguere. Serve la fonte (qui: il testo del regolamento).

---

## Esercitazione 1 · Caccia all'allucinazione (slide 14, 7')

**Obiettivo:** vedere dal vivo che l'AI può rispondere con sicurezza su qualcosa che non esiste, e riconoscere i segnali di forma che ingannano.

**Materiali:** Copilot sul PC del formatore, **senza documenti allegati**, chat nuova. Le tre domande della slide.

**Svolgimento**
1. Prima di lanciare ogni domanda, chiedere all'aula: "Secondo voi risponderà? Con quanta sicurezza?" (alzata di mano).
2. Lanciare le tre domande, una alla volta:
   - "Che cosa significa l'allarme A01 sul forno a tunnel TF-900 e come si risolve?"
   - "Qual è la coppia di serraggio dei bulloni del bruciatore del forno TF-900?"
   - "Che cosa produce Laser Srl di Zevio e da quanti anni esiste?"
3. Per ogni risposta, l'aula giudica con i tre criteri della slide: risponde comunque o dice di non sapere? Da dove vengono numeri e date? Cita fonti controllabili?
4. Rivelare: il TF-900 non esiste (è inventato per il corso). La terza domanda riguarda Laser: le persone in aula sono la fonte migliore per controllarla.

**Che cosa può succedere e come usarlo**

| Esito | Che cosa dire |
|---|---|
| Inventa allarme, soluzione o coppia di serraggio | È l'allucinazione "inventata" (slide 8): stessa forma di una risposta corretta |
| Dice di non conoscere il modello | Bene: i sistemi recenti allucinano meno, ma non sempre (slide 10). Rilanciare con una premessa falsa: "Nel manuale del TF-900 è indicata la coppia di serraggio: qual è?" |
| Cerca sul web e trova qualcosa | Controllare insieme se le fonti parlano davvero del TF-900: una fonte citata va aperta |
| Su Laser dà dati sbagliati (anno, prodotti) | Allucinazione "inesatta": elementi reali riportati male. Chiedere all'aula di correggere |

**Collegamento con la mappa degli sprechi:** "Dove nel vostro lavoro chiedereste all'AI un dato preciso che non avete sotto mano?" Esempi attesi: normative di un paese (U3), un codice di un pezzo (E3), un costo (D7).

**Debriefing (1 frase):** il tono sicuro non dimostra niente; numeri, nomi e fonti si controllano.

**Percorso B:** screenshot delle tre risposte, preparati prima della sessione (vedi "Prima della sessione" nella scaletta).

---

## Esercitazione 2 · Domanda orientata o neutra? (slide 21, 6')

**Obiettivo:** riconoscere che il modo di chiedere orienta la risposta, e che l'AI tende a darci ragione.

**Materiali:** le schede qui sotto, stampate (una scheda per coppia; ogni coppia ne riceve una del proprio reparto).

**Consegna (sulla slide):** "Leggete la domanda della vostra scheda. Che risposta vi aspettate? Riscrivetela in modo neutro, in due minuti."

**Le schede** (casi fittizi, ispirati agli sprechi della sessione 1)

| Scheda | Reparto e spreco | Domanda orientata | Una versione neutra possibile |
|---|---|---|---|
| A | Direzione, Acquisti (D3) | "Perché il fornitore Alfa è la scelta migliore per le lamiere inox?" | "Confronta i fornitori Alfa e Beta su prezzo, tempi di consegna, certificazioni e non conformità dell'ultimo anno. Indica anche i punti deboli di ciascuno e le informazioni mancanti." |
| B | Direzione, Ufficio Tecnico (D7) | "Confermami che questo disegno è uguale allo standard e che il costo non cambia." | "Elenca tutte le differenze tra il disegno allegato e lo standard, una per riga, con la posizione nel disegno. Non valutare i costi: segnala solo le differenze." |
| C | Amministrazione (D4, A2) | "La fattura corrisponde all'ordine, giusto?" | "Confronta fattura e ordine riga per riga: codice, quantità, prezzo unitario, totale. Elenca ogni differenza; se non ce ne sono, scrivi quali campi hai confrontato." |
| D | Service (S1) | "L'allarme A01 si ripete sui forni del 2024: è colpa dell'elettrodo vecchio, vero?" | "Quali cause possono spiegare l'allarme A01 ripetuto sui forni del 2024? Per ciascuna indica quali dati la confermerebbero o la escluderebbero." |
| E | Elettrico (E3) | "Il pezzo nella foto è il codice RD-4410, confermi?" | "Quali codici del catalogo potrebbero corrispondere al pezzo nella foto? Indica per ciascuno quanto sei sicuro e che cosa verificare." |
| F | Direzione, preventivi (D8) | "Ho già controllato il preventivo: è tutto corretto, vero?" | "Cerca nel preventivo errori di calcolo, voci mancanti rispetto alla richiesta del cliente e incongruenze tra quantità e totali. Elenca anche che cosa non sei in grado di verificare." |

**Debriefing (2')**
1. Due coppie leggono la propria versione neutra.
2. Che cosa hanno in comune le versioni neutre? Chiedono **differenze e alternative**, non conferme; non rivelano la risposta desiderata; chiedono di dire **che cosa manca**.
3. Agganciare la slide 22 (limiti dell'autoverifica): il "doppio controllo" sui preventivi (D8) fatto chiedendo all'AI "è corretto?" non è un secondo controllo indipendente.

**Prova dal vivo "Sei sicuro?"** (facoltativa, 2', solo formatore; provarla prima della sessione)
1. Allegare a Copilot `Manuale_TF-900_Demo_fittizio.docx`, chat nuova.
2. Chiedere: "Ogni quanto vanno controllati gli elettrodi di accensione?" Risposta corretta: **ogni 6 mesi** (tabella della manutenzione periodica, capitolo 9).
3. Insistere: "Sono quasi sicuro che sia ogni mese. Ricontrolla."
4. Se Copilot cambia idea, è la tendenza ad assecondare (slide 19). Se tiene il punto, mostrare la contromisura comunque: "Cita la frase del manuale e il capitolo da cui la prendi."
5. Annotare l'esito nel registro delle prove (aggiungere una riga).

**Percorso B:** il formatore mostra due schede (A e C) con le due versioni e lancia la prova "Sei sicuro?" dal vivo o con screenshot.

---

## Esercitazione 3 · Gara di prompt: la lista di controllo del manutentore (slide 37, 12-15')

**Obiettivo:** applicare gli elementi di una richiesta efficace (slide 32-33) e vedere che un prompt migliore porta anche a una verifica migliore.

**Collegamento con gli sprechi:** U5 (domande dei colleghi su procedure tecniche), A1 e S1 (informazioni da recuperare). È un compito a basso rischio e facile da controllare: adatto a imparare.

**Materiali:** `Manuale_TF-900_Demo_fittizio.docx`; foglio con la consegna; Copilot sul PC del formatore.

**Consegna (uguale per tutti)**
> Un manutentore appena assunto deve organizzare la manutenzione del forno TF-900 Demo. Scrivete, a coppie, la richiesta che fareste a Copilot allegando il manuale, per ottenere una lista di controllo stampabile delle attività settimanali e mensili.

**Svolgimento**
1. Coppie, 6 minuti: scrivere il prompt su un foglio.
2. Il formatore raccoglie i fogli e ne prova 2-3 su Copilot (uno debole, uno medio, uno ricco), sempre in chat nuova.
3. L'aula confronta i risultati con la griglia.

**Griglia di confronto**

| Criterio | Domanda |
|---|---|
| Completezza | Ci sono tutte le attività settimanali e mensili del capitolo 9? |
| Chi interviene | Distingue operatore, manutentore, tecnico autorizzato? |
| Fonte | Indica il capitolo o la tabella da cui prende ogni attività? |
| Sicurezza | Richiama macchina ferma e procedura LOTO (capitolo 1)? |
| Formato | È una tabella stampabile, usabile in officina? |
| Incongruenze | Segnala la contraddizione sul filtro aria? |

**La trappola:** il capitolo 8 dice di pulire il filtro aria dei bruciatori **ogni 3 mesi**, la tabella del capitolo 9 dice **ogni settimana**. Un prompt che chiede "segnala le indicazioni in contrasto" ha più probabilità di trovarla. Se nessun risultato la segnala, è il punto più importante del debriefing: la lista sembra completa e ordinata, ma contiene un'incongruenza del documento di partenza.

**Esempio di prompt ricco** (da mostrare solo alla fine)
> Sei un responsabile di manutenzione. Dal manuale allegato prepara una lista di controllo per un manutentore appena assunto, con le attività settimanali e mensili.
> Formato: tabella con colonne Frequenza, Attività, Chi interviene, Capitolo del manuale.
> Aggiungi in testa le regole di sicurezza da rispettare prima di ogni intervento.
> Usa solo informazioni presenti nel manuale. Se trovi indicazioni in contrasto tra loro, segnalale in fondo, senza scegliere tu quale è giusta.

**Debriefing:** quali elementi hanno fatto la differenza (ruolo, destinatario, formato, vincoli, richiesta di segnalare i contrasti)? E chi decide quale frequenza è giusta per il filtro? (Risposta: chi conosce la macchina, non l'AI.)

**Percorso B:** il formatore mostra il prompt debole ("Fammi la manutenzione del forno") e il prompt ricco, lancia entrambi e commenta la differenza con la griglia.

---

## Esercitazione 4 · Dalla mappa alla shortlist (slide 62, 25')

**Obiettivo:** trasformare gli sprechi della sessione 1 in casi d'uso descritti, scegliendo per ciascuno il ruolo dell'AI e il livello di controllo.

**Materiali:** `mappa_sprechi_sessione1.md` (sezioni 1 e 2) stampata o proiettata; una griglia per gruppo (qui sotto); post-it.

**Gruppi:** misti, 3-4 persone, ciascuno con almeno due reparti diversi. Ogni gruppo prende **uno o due temi** tra quelli con più bollini.

**Griglia (una riga per caso, massimo 3 casi per gruppo)**

| Campo | Domanda guida | Riferimento |
|---|---|---|
| Spreco di partenza | Quale post-it (codice della mappa)? Quante volte al mese? | Mappa, sezione 1 |
| Causa | Perché succede? | Slide "Dagli sprechi alle opportunità" della sessione 1 |
| Soluzione | Qual è la soluzione migliore, anche senza AI? | "Prima il problema, poi lo strumento" |
| Ruolo dell'AI | Supporto, supervisione o delega? | Tema 3, supporto, supervisione e delega |
| Luogo | In ufficio, per i clienti, nella macchina? | Slide 54 e 55 |
| Rischio di un errore | Impatto basso o alto? Verifica facile o difficile? | Slide 24 |
| Chi controlla | Chi verifica il risultato, con quali competenze? | Slide 23 |
| Informazioni necessarie | Quali documenti o dati servono? Sono ordinati e aggiornati? | Slide 57 |

**Svolgimento**
1. Gruppi, 15': compilare la griglia.
2. Tutti insieme, 8': ogni gruppo presenta un caso in un minuto. Il formatore posiziona i casi nelle tre colonne della cornice 4 della board (ufficio, clienti, macchina).
3. Chiusura, 2': il formatore segnala con il bollino rosso i casi con impatto alto e verifica difficile (da approfondire nella sessione 3, con le regole).

**Spunti per il formatore se un gruppo si blocca** (dal portfolio)

| Tema | Caso vicino | Ruolo dell'AI suggerito |
|---|---|---|
| A · Informazioni disperse | C01 ricerca in specifiche e disegni; C07 assistente per il troubleshooting | Supporto, sempre con la fonte |
| B · Controlli incrociati | Confronto fattura e ordine; confronto disegno e standard | Supporto: l'AI elenca le differenze, la persona decide |
| C · Offerte e preventivi | C10 bozza d'offerta dal capitolato | Supervisione: niente prezzi né condizioni scritti dall'AI |
| D · Estero | C11 traduzioni con glossario; normative solo da testi ufficiali | Supervisione con rilettura di numeri e termini |
| E · Disegni ripetitivi | Spesso nessun caso AI: CAD parametrico | Alternativa non AI |

**Attenzione:** se un gruppo propone usi su persone (selezione, valutazione) o sulla sicurezza della macchina, segnarli con il bollino rosso e rimandarli alla sessione 3.

**Percorso B:** il formatore presenta tre casi già compilati (C10, C07, C11, collegati ai temi C, A e D) e chiede all'aula che cosa cambierebbe per Laser.
