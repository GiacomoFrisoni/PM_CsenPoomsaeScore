# WBS

Tutte le attività di seguito riportate comprendono anche lo sviluppo della relativa parte grafica, ove questo non sia esplicitamente specificato.

## App Android

### 1.1.1 Menù Principale

L'applicazione deve prevedere una schermata iniziale, nella quale selezionare la modalità di utilizzo: registrazione punteggio, storico o impostazioni.

### 1.1.2.1 Registrazione Accuratezza

Realizzazione di una schermata con controlli che abilitano la detrazione o l'incremento del punteggio dell'atleta svolgente la poomsae durante la fase di valutazione dell'accuratezza.

### 1.1.2.2 Registrazione Presentazione

Realizzazione di una schermata con controlli che abilitano la detrazione o l'incremento del punteggio dell'atleta svolgente la poomsae durante la fase di presentazione.

### 1.1.2.3 Visualizzazione Riepilogo

Realizzazione di una schermata che visualizzi i punteggi progressivi e quello totale, dopo che l'atleta ha concluso di esibirsi.

### 1.1.3 Gestione Navigazione
Realizzazione di una navigazione efficiente tra le varie schermate previste dall'applicazione (con particolare attenzione a quelle dedicate alle fasi di raccolta punti durante l'esibizione di un atleta). Tenere in considerazione la voce delle impostazioni per l'abilitazione o meno della possibilità - a partire dalla schermata di riepilogo - di far ritorno alla modifica dei parametri.

### 1.1.4 Invio Punteggio

Realizzazione di una schermata abilitante il giudice ad inviare i punteggi acquisiti al software del quadrato. Lato backend, studio del protocollo da utilizzare per l'invio dei dati.

### 1.1.5 Storico

Sviluppo di una schermata riepilogativa con lo storico dei punteggi assegnati agli atleti, in ordine cronologico. Ci dev'essere possibilità di azzerare questa lista. Non è importante che sia permanente.

### 1.1.6 Impostazioni

Sviluppo di una schermata con delle impostazioni per l'applicazione e per il device, quali:
- regolazione della luminosità dello schermo,
- abilitazione / disabilitazione della retro-modifica dei punteggi assegnati,
- abilitazione dell'invio dei punteggi, a fronte di inserimento di un indirizzo IP valido.


## Software Gestione Quadrato

### 1.2.1 Menù Principale

Realizzazione della schermata d'apertura del software contenente il menù per l'accesso alle funzionalità di avvio di una nuova competizione e impostazioni.

### 1.2.2 Ricezione Tornei

Raccolta dal server dell'elenco di tornei che il software di quadrato deve gestire. Qualora la rete non sia disponibile, prevedere il caricamento di tali dati da file.

### 1.2.3 Selezione Torneo

Sviluppo dei filtri attraverso cui selezionare un torneo, specificando i parametri identificativi del torneo stesso sulla base della sua tipologia (individuali, coppie o team).

### 1.2.4.1.1 Selezione Atleta

Visualizzazione delle poomsae degli atleti partecipanti a una gara interna a un torneo e gestione della loro selezione. Inserire nelle preview il numero d'ordine, il nome e il cognome dell'atleta, il punteggio eventualmente associato e un semaforo (rosso: non ancora svolta; arancione: in svolgimento; verde: completata).

### 1.2.4.1.2.1 Gestione Timer

Realizzazione del timer attraverso cui registrare il tempo impiegato da un atleta per lo svolgimento della sua poomsae.

### 1.2.4.1.2.2 Raccolta Punteggi Giudici

Raccolta wireless dei punteggi (accuratezza, presentazione e totale) assegnati dai giudici alla poomsae svolta dall'atleta. In caso di malfunzionamenti di rete o modalità offline, prevedere il loro inserimento manuale.

### 1.2.4.1.2.3 Raffinamento Punteggio

Sviluppo della schermata attraverso cui gestire la registrazione di errori (di grave entità, 0.3; o di lieve entità, 0.1) e il loro undo, a partire dalla media calcolata dai punteggi totali dei giudici.

### 1.2.4.1.2.4 Visualizzazione Risultati

Realizzazione di una schermata di riepilogo, illustrante il nome dell'atleta, il nome e la nazionalità della palestra, il punteggio finale assegnato alla poomsae dell'atleta stesso e il relativo tempo di esecuzione.

### 1.2.4.1.2.5 Gestione Poomsae Finali

Gestione dello svoglimento di due poomsae da parte di ogni atleta all'interno della gara finale, con il relativo intervallo temporale richiesto tra la loro esecuzione (sulla base di quanto specificato nelle impostazioni).

### 1.2.4.1.3 Gestione Ballottaggi

Individuazione di ballottaggi (punteggi uguali - anche nella componente di errori - su soglie critiche) all'atto di completamento di una gara, sia per il passaggio di turno che per l'assegnamento delle medaglie. In caso di una loro presenza, prevedere lo svogimento di una nuova poomsae da parte degli atleti coinvolti. Qualora la situazione di pareggio si ripresenti, considerare la vittoria di tutti gli atleti in ballottaggio (passaggio turno o ricezione di medaglie exaequo).

### 1.2.4.1.4 Gestione Ritiri ed Eliminazioni

Gestione del possibile ritiro da parte di un atleta in qualsiasi momento, mantenendone traccia all'interno del sistema ma non considerandolo per il passaggio alla gara successiva o per l'assegnazione delle medaglie.
In caso di torneo non avviato, gestire l'eventuale eliminazione di atleti.

### 1.2.4.1.5 Gestione Azzeramenti

Gestione degli azzeramenti per le seconde poomsae di poomsae finali e per le poomsae di ballottaggio (consolidando il risultato precedente).

### 1.2.4.1.6 Gestione Ripetizioni

Gestione della possibile ripetizione della poomsae svolta da un atleta (in caso di distrazione o altri motivi).
In caso di poomsae finale, una richiesta di ripetizione durante lo svolgimento della seconda poomsae determina la sola riesecuzione di quest'ultima parte.

### 1.2.4.1.7.1 Gestione Passaggio Turno

Calcolo del turno (ovvero della gara) di partenza in base al numero di partecipanti al torneo.
Applicazione delle regole per la determinazione degli atleti vincitori del passaggio da eliminatorie a semifinali o da semifinali a finali.

### 1.2.3.1.7.2 Gestione Assegnazione Medaglie

Calcolo dei vincitori del torneo e relativa assegnazione delle medaglie (calcolo della classifica locale).

### 1.2.4.2.1 Salvataggio su file

Gestione del salvataggio consistente su file .json di tutti i dati relativi ai tornei in carico al quadrato (serializzazione).

### 1.2.4.2.2 Invio Risultati al Server

Invio al server del punteggio finale di ogni poomsae al completamento della sua valutazione, invio delle casistiche di ritiro e invio della classifica locale di un torneo all'atto della sua chisura.

### 1.2.5 Impostazioni
Sviluppo della schermata dedicata alla gestione dell'associazione coi tablet dei giudici (necessaria per la raccolta wireless dei punteggi). Deve essere mostrato il riepilogo dei dispositivi attualmente connessi, permettendo eventualmente il loro disaccoppiamento.

### 1.2.6.1 Monitor Poomsae

Gestione della finestra da visualizzare sul monitor di poomsae. Mostrare i dati del torneo, l'anagrafica dell'atleta, il tempo trascorso dall'avvio della poomsae, i punteggi dei giudici man mano che questi vengono registrati.
Sviluppo anche della funzionalità relativa al suo oscuramento.

### 1.2.6.2.1 Elenco Atleti

Gestione della schermata da visualizzare sulla finestra del monitor di torneo dedicata all'elenco degli atleti presenti nell'attuale gara. Realizzare sul piano grafico una preview per ogni atleta contenente il suo numero d'ordine, il nome, il cognome, la palestra di appartenenza, il punteggio ottenuto per la sua poomsae principale ed eventualmente quello di ballottaggio.
Utilizzo di colorazioni diverse per le preview di atleti con poomsae completate, in svolgimento e non completate.

### 1.2.6.2.2 Classifica Torneo

Gestione della schermata da visualizzare sulla finestra del monitor di torneo dedicata alla classifica locale di quest'ultimo. Mostrare gli atleti in ordine di posizione sulla base del punteggio da loro ottenuto. A parità di punteggio considerare l'ordine alfabetico del nome e del cognome. Evidenziare graficamente gli atleti vincitori di medaglia.

## Server

### 1.3.1 Menù Principale
Realizzazione della schermata d'apertura del software contenente il menù per l'accesso alle funzionalità di creazione di una nuova competizione, apertura di una competizione già esistente e impostazioni.

### 1.3.2.1.1 Inserimento Anagrafica

Registrazione dell'anagrafica della competizione (nome della competizione e numero di giudici nei quadrati di gara).

### 1.3.2.1.2.1 Parsing da File Excel

Sviluppo del parsing per il caricamento dei dati a partire dal file Excel degli atleti. Creazione automatica dei tornei (di ogni tipologia) e dei relativi partecipanti in base ai parametri di ogni atleta.

### 1.3.2.1.2.2 Apertura Competizione Esistente

Deserializzazione del file .json contenente tutti i dati della competizione selezionata, consentendo la scelta tra quelli presenti all'interno della directory di default o il caricamento di quello desiderato da file system.

### 1.3.2.1.2.3 Validazione dei Dati Importati

Sviluppo della schermata riepilogativa per quanto concerne i tornei automaticamente creati e l'elenco dei rispettivi atleti partecipanti, ottenuta a partire dal file Excel. Ottenimento della conferma da parte dell'utente per la loro validazione.

### 1.3.2.2.1.1 Gestione Atleti

Realizzazione delle funzionalità di inserimento, modifica ed eliminazione di atleti.

### 1.3.2.2.1.2 Gestione Trasferimenti

Gestione dei trasferimenti degli atleti tra tornei. Per facilitare tale operazione, si prevede anche lo sviluppo di una funzionalità per l'individuazione automatica di atleti con un solo partecipante e la visualizzazione ordinata dei tornei in base al numero di partecipanti.

### 1.3.2.2.2 Partizionamento Tornei - Quadrati

Divisione dei tornei da gestire tra i vari software di quadrato di gara e realizzazione della relativa comunicazione wireless. In caso di assenza di rete, prevedere il salvataggio di tali informazioni su file per consentire un loro caricamento manuale.

### 1.3.3.1 Raccolta Puntegggi e Classifiche Locali

Gestione della raccolta dei punteggi legati a ogni poomsae e delle classifiche di fine torneo, da parte dei software di gestione di gara (con caricamento manuale di questi ultimi in caso di assenza di rete).

### 1.3.3.2 Gestione Classifica Globale

Elaborazione della classifica globale dedicata alle palestre sulla base delle medaglie ricevute dai loro atleti. Gestire l'aggiornamento di quest'ultima ogni qualvolta venga ricevuta una classifica locale all'atto di completamento di un torneo. 

### 1.3.4 Gestione Salvataggio

Gestione del salvataggio consistente su file .json di tutti i dati legati alla competizione.

### 1.3.5 Impostazioni
Sviluppo della schermata dedicata alla gestione delle impostazioni generali per un qualunque torneo interno alla competizione. Le voci previste devono essere le seguenti:
- soglia di passaggio da eliminatorie a semifinali;
- soglia di passaggio da semifinali a finali;
- tempo di attesa tra prima e seconda poomsae.
L'apportamento di modifiche deve essere possibile solo prima dell'avvio di una competizione.

### 1.3.6.1 Legame Atleta - Quadrato

Gestione della schermata da visualizzare sulla finestra del monitor esterno dedicata alla composizione di ogni quadrato in termini di atleti.

### 1.3.6.2 Classifica Globale

Gestione della schermata da visualizzare sulla finestra del monitor esterno dedicata alla classifica globale delle palestre.
