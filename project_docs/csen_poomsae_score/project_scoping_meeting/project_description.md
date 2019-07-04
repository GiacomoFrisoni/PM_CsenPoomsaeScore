# Descrizione del progetto

## Introduzione

CSEN (Centro Sportivo Educativo Nazionale) è un ente di elevate dimensioni incentrato sullo sviluppo della pratica sportiva e sulla sua accessibilità. CSEN ha avuto una forte crescita negli ultimi 10 anni a cui non è seguita una razionalizzazione delle procedure operative. Recentemente ha deciso di informatizzare il proprio processo di gestione dei tornei di Taekwondo, organizzati nelle varie competizioni svolte sul territorio nazionale. Loro attribuiscono questa esigenza a due fattori principali: l'inefficienza legata a una completa gestione manuale e la presenza di soluzioni software già in uso da parte di aziende competitor. 
La Direzione Aziendale si è rivolta alla nostra startup per commissionare la realizzazione di un sistema software, in grado di migliorare la situazione attuale del cliente, fornendo una soluzione capace di coprire le esigenze avvertite.
Enrico Comando, Project Manager di CSEN, afferma come i principali obiettivi dell'intervento siano sviluppare un'applicazione Android per automatizzare l'assegnamento dei punteggi da parte dei giudici e la loro raccolta / elaborazione, introdurre un software per la completa gestione di un quadrato di gara e un'applicazione lato server per la configurazione dei tornei e l'elaborazione delle classifiche. Il cliente vuole che il team si impegni a ricercare una soluzione efficace ed efficiente per la realizzazione dei tre sottosistemi.

## Sottosistema 1 - Tablet
Il primo è un sottosistema software incentrato sulla realizzazione di un'applicazione Android da installare sui tablet aziendali e messi a disposizione dei giudici per l'assegnazione del punteggio complessivo di ogni poomsae svolta da un atleta. Questo è determinato dalla somma di due valutazioni:

- *Accuratezza*  
    - Range: 0.0 - 4.0
    - Valore inziale: 4.0
    - Modalità di assegnazione: presenza di quattro pulsanti per la registrazione di errori di scarsa entità (-0.1) e di grave entità (-0.3), consentendo anche il loro "undo" (+0.1 e +0.3)
  
- *Presentazione*  
  - Range: 0.0 - 6.0
  - Valore iniziale: 6.0
  - Modalità di assegnazione: presenza di 3 slider, ognuno riferito ad una diversa categoria di valutazione (velocità e potenza, forza e ritmo, espressione di energia); ognuno di essi parte con un punteggio iniziale di 2.0 e può essere diminuito a scaglioni di 0.2 punti.

Al termine della valutazione, deve essere mostrata una schermata riepilogativa contenenti il punteggio totale e le sue due componenti.
Il cliente richiede che i dati in essa contenuti siano ben visibili anche ad una distanza di circa 10 metri.

L'applicazione deve poter funzionare in due modalità: offline (default) e online. La seconda richiede una configurazione consistente nella specifica dell'indirizzo IP della macchina su cui è in esecuzione il software di gestione del quadrato, associato al giudice in possesso del tablet.
In modalità online, inoltre, a seguito della visualizzazione dei punteggi, deve essere possibile inviarli al software del quadrato precedentemente configurato (consentendo anche molteplici invii per far fronte a eventuali perdite di pacchetti lungo la rete). Si sottolinea come debba essere possibile in ogni caso far ritorno alla schermata riepilogativa per consentire il proseguio della gara (con un inserimento manuale dei punteggi sull'applicativo del quadrato) anche nell'eventualità di un crollo della rete.

Si richiede inoltre che l'applicazione sia in grado di:
- mantenere lo storico dei punteggi assegnati dal giudice in possesso del tablet;
- consentire la specifica di impostazioni quali cancellazione dello storico, regolazione della luminosità, abilitazione del pulsante per il ritorno alla schermata dei punteggi (consentendo la possibilità di modifiche).

## Sottosistema 2 - PC

## Sottosistema 3 - Server e comunicazione wireless
