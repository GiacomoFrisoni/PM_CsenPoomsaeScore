# Descrizione del progetto

## Introduzione

CSEN (Centro Sportivo Educativo Nazionale) è un ente di elevate dimensioni incentrato sullo sviluppo della pratica sportiva e sulla sua accessibilità. CSEN ha avuto una forte crescita negli ultimi 10 anni a cui non è seguita una razionalizzazione delle procedure operative. Recentemente ha deciso di informatizzare il proprio processo di gestione dei tornei di Taekwondo, organizzati nelle varie competizioni svolte sul territorio nazionale. Loro attribuiscono questa esigenza a due fattori principali: l'inefficienza legata a una completa gestione manuale e la presenza di soluzioni software già in uso da parte di aziende competitor. CSEN ha inizialmente valutato l'acquisizione di soluzioni già esistenti ma, non riscontrando in queste le caratteristiche richieste in termini di funzionalità e usabilità, ha preferito considerare la costruzione di un nuovo sistema personalizzato per far fronte alle proprie esigenze.  
La Direzione Aziendale si è rivolta alla nostra startup per commissionare la realizzazione di un sistema software, in grado di migliorare la situazione attuale del cliente, fornendo una soluzione capace di coprire le esigenze avvertite.
Enrico Comando, Project Manager di CSEN, afferma come i principali obiettivi dell'intervento siano sviluppare un'applicazione Android per automatizzare l'assegnamento dei punteggi da parte dei giudici e la loro raccolta / elaborazione, introdurre un software per la completa gestione di un quadrato di gara e un'applicazione lato server per la configurazione dei tornei e l'elaborazione delle classifiche. Il cliente vuole che il team si impegni a ricercare una soluzione efficace ed efficiente per la realizzazione dei tre sottosistemi.

## Sottosistema 1 - Tablet dei giudici
Il primo è un sottosistema software incentrato sulla realizzazione di un'applicazione Android da installare sui tablet aziendali e messi a disposizione dei giudici per l'assegnazione del punteggio complessivo di ogni poomsae svolta da un atleta. Questo è determinato dalla somma di due valutazioni:

- *Accuratezza*  
    - Range: 0.0 - 4.0
    - Valore inziale: 4.0
    - Modalità di assegnazione: presenza di quattro pulsanti per la registrazione di errori di scarsa entità (-0.1) e di grave entità (-0.3), consentendo anche il loro "undo" (+0.1 e +0.3)
  
- *Presentazione*  
  - Range: 0.0 - 6.0
  - Valore iniziale: 6.0
  - Modalità di assegnazione: presenza di 3 slider, ognuno riferito ad una diversa categoria di valutazione (velocità e potenza, forza e ritmo, espressione di energia); ciascuno parte con un punteggio iniziale di 2.0 e può essere diminuito a scaglioni di 0.2 punti

Al termine della valutazione, deve essere mostrata una schermata riepilogativa contenenti il punteggio totale e le sue due componenti.
Il cliente richiede che i dati in essa contenuti siano ben visibili anche ad una distanza di circa 10 metri.

L'applicazione deve poter funzionare in due modalità: offline (default) e online. La seconda richiede una configurazione consistente nella specifica dell'indirizzo IP della macchina su cui è in esecuzione il software di gestione del quadrato, associato al giudice in possesso del tablet.
In modalità online, inoltre, a seguito della visualizzazione dei punteggi, deve essere possibile inviarli al software del quadrato precedentemente configurato (consentendo anche molteplici invii per far fronte a eventuali perdite di pacchetti lungo la rete). Si sottolinea come debba essere possibile in ogni caso far ritorno alla schermata riepilogativa per consentire il proseguio della gara (con un inserimento manuale dei punteggi sull'applicativo del quadrato) anche nell'eventualità di un crollo della rete.

Si richiede inoltre che l'applicazione sia in grado di:
- mantenere lo storico dei punteggi assegnati dal giudice in possesso del tablet;
- consentire la specifica di impostazioni quali cancellazione dello storico, regolazione della luminosità, abilitazione del pulsante per il ritorno alla schermata dei punteggi (consentendo così la possibilità di modifiche).

## Sottosistema 2 - Gestione del quadrato
Il secondo è un sottosistema software per la gestione di tutti i tornei svolti su un determinato quadrato di gara.

### Organizzazione di un torneo
Esistono tre tipologie di torneo in base al numero di atleti che compongono i gruppi partecipanti: individuali (un solo atleta), coppie (due atleti) e team (più di 2 atleti, fino ad un massimo di 5).  
Ogni torneo è identificato da una serie di parametri con specifici range di possibili valori:
- *TORNEI INDIVIDUALI*
  - Categoria
    - NOVIZI
    - ESORDIENTI
    - CADETTI 1
    - CADETTI 2
    - JUNIOR
    - SENIOR 1
    - SENIOR 2
    - MASTER 1
    - MASTER 2
  
  - Sesso
    - M (per maschi)
    - F (per femmine)
  
  - Gruppo di grado
    - 10-9 KUP
    - 8-7 KUP
    - 6-5 KUP
    - 4-3 KUP
    - 2-1 KUP
    - POOM
    - DAN

- *TORNEI DI COPPIE O TEAM*
    - Classe
      - A
      - B
      - C
  
    - Gruppo di grado
      - 10/5 KUP
      - 4/1 KUP
      - POMM
      - NERE

Un torneo si compone di tre gare: eliminatorie, semifinali e finali (necessariamente svolte nell'ordine presentato). La gara di partenza è dettata dal numero di atleti registrati al torneo; di conseguenza non tutte le gare sono necessariamente svolte. I criteri per la determinazione della gara inziale e per il passaggio da una gara alla successiva sono di seguito riportati:

 - *ELIMINATORIE*
   - Atleti richiesti: più di 18 atleti;
   - Passaggio a semifinali: 50% + 1 degli atleti con punteggio totale più alto;
 - *SEMIFINALI*
   - Atleti richiesti: tra i 9 e i 18 atleti (compresi); 
   - Passaggio a finali: i primi 5 atleti con punteggio totale più alto;
 - *FINALI*
   - Atleti richiesti: meno di 9 atleti;

L'esibizione di forma fatta da un atleta è chiamata "poomsae".
Nel momento in cui un atleta inizia a esibirsi, viene avviato un timer per misurare il tempo impiegato per lo svolgimento della forma.  
Al termine della poomsae, vengono raccolte le votazioni assegnate dai giudici per l'atleta. Il punteggio totale è così calcolato come media delle singole votazioni. Questo può essere ulteriormente oggetto di correzioni, registrando penalità di scarsa entità (-0.1) o di grave entità (-0.3) - similarmente al calcolo della componente di accuratezza da parte di un singolo giudice.

Un atleta in eliminatorie o in semifinali è chiamato a svolgere una sola poomsae; durante la fase finale, invece, ne vengono richieste due (separate da un intervallo temporale, fissato a 30 secondi). In quest'ultimo caso, il punteggio totale è dato dalla somma dei singoli punteggi totali ottenuti attraverso le due poomsae.
Le regole appena presentate per il calcolo della gara di partenza, per il passaggio da una all'altra e per l'arco temporale tra lo svolgimento della prima e della seconda poomsae finale sono quelle attualmente in vigore. Si sottolinea tuttavia come CSEN possa apportare dei cambiamenti a esse di anno in anno e di come, quindi, il sistema debba prevedere il loro aggiornamento da parte dell'utente.

Giunti al termine della gara finale, avviene l'assegnamento delle medaglie (oro, argento, bronzo). Se il torneo è costituito da un unico atleta, egli - dolo lo svolgimento della sua poomsae - ha automaticamente diritto alla medaglia (oro singolo).

Alla fine dello svolgimento di una gara (sia per il passaggio alla gara successiva che per l'assegnamento delle medaglie) è possibile che più atleti abbiano lo stesso punteggio totale. Qualora tale scenario impedisca la determinazione degli atleti passanti il turno (o riceventi una determinata medaglia) a causa di un pari merito in punti critici (es. sulla soglia semifinali &rarr; finali), si osserva chi possiede la componente di accuratezza più alta. Qualora anche l'accuratezza non dovesse essere un parametro discriminante, gli atleti sono invitati a eseguire un'ulteriore poomsae di ballottaggio. Il nuovo punteggio totale così ottenuto viene confrontato con quello degli avversari per stabilire il vincitore. È previsto un solo ballottaggio: qualora una situazione di pari merito si dovesse nuovamente ripetere, tutti gli atleti coinvolti dal ballottaggio stesso passano il turno o ricevono la medesima medaglia in forma ex aequo. Quest'ultimo, inoltre, non può essere mai ripetuto. 

Prima dell'inizio di un torneo, viene fatto un appello per verificare la presenza degli atleti partecipanti: gli atleti non presenti vengono eliminati dal sistema. Specularmente, se il torneo non è ancora stato avviato, deve essere possibile poter aggiungere atleti non previsti. L'eliminazione e l'aggiunta di atleti sono operazioni che hanno chiaramente effetto sul numero iniziale di membri per il torneo e in quanto tali possono alterare la gara di partenza per quest'ultimo. Nello specifico, è sia possibile avanzare di gara (eliminando atleti) che retrocedere di gara (aggiungendone di nuovi).

Un atleta può essere ritirato da un torneo avviato durante una qualsiasi gara. Gli atleti ritirati sono evidenziati dal sistema e non vengono presi in considerazione per il passaggio di gara o per l'assegnamento delle medaglie. I loro punteggi non concorrono pertanto all'elaborazione delle classifiche, ma vengono comunque tracciati.
Si sottolinea come il ritiro o l'eliminazione di un atleta siano azioni definitive, in quanto non possono essere in nessun modo revocate.

Qualora non sia possibile svoltere la seconda parte di una poomae finale (o un ballottaggio) viene assegnato un'operazione di "assegnamento di punteggio zero". In entrambi i casi, infatti, si consolida il punteggio precedente dell'atleta (quello della prima poomsae) per la poomsae finale, o quello del punteggio che ha determinato il ballottaggio. Un atleta con punteggio azzerato può comunque passare il turno e ricevere medaglie, a differenza di un atleta ritirato.

### Gestione dei tornei del quadrato di gara
Al primo avvio il software riceve i dati della competizione (nome e numero di giudici) e i tornei da gestire con l'elenco dei relativi partecipanti dal server.

L'utente deve poter ricercare un torneo attraverso delle caselle a scelta multipla rappresentanti i parametri che lo identificano (varianti sulla base della tipologia).  
Selezionado correttamente i filtri viene visualizzato l'elenco degli atleti corrispondente al torneo scelto, navigabile anche nelle gare che compongono il torneo stesso.

A fronte della scelta di un atleta, sono resi disponibili i controlli per la gestione della sua poomsae. Il sistema deve prevedere quindi un bottone per l'avvio e l'arresto del timer, nonchè la visualizzazione del tempo trascorso, con precisione al millisecondo. Alla conclusione della poomsae viene visualizzata una schermata dedicata alla raccolta delle votazioni dei giudice (manuale o wireless). È quindi calcolato il punteggio medio, con la possibilità di registrare ulteriori penalità a partire da esso.
Si osserva come sia sempre possibile ripetere una poomsae iniziata per far fronte a scenari pratici quali la distrazione dell'atleta in esame, per esempio.

Al completamento della poomsae, in base alla fase del torneo attualmente occupata dall'atleta, possono essere visualizzate due schermate:
 - nelle gare *eliminatorie* e *semifinali*, si passa immediatamente ad una schermata riepilogativa, illustrante i dettagli della prova stessa e consentente l'annullamento della poomsae (abilitando conseguentemente la possibilità di ripeterla);

 - nella gara delle *finali* - se la poomsae terminata è la prima delle due - viene mostrato un timer (con la possibilità di saltarlo), allo scadere del quale l'atleta è invitato ad eseguire la poomsae successiva (ripetendo, di conseguenza, tutte le schermate precedenti). Alla chiusura della seconda poomsae, invece, viene mostrata la schermata riepilogativa.

Ogni tal volta che una poomsae giunge in uno stato consistente (tempo registrato, voti dei giudici ricevuti, correzzione al punteggio medio applicata, completamento), viene effettuato anche il salvataggio dello stato attuale del torneo cui questa appartiene in maniera permanente sul disco rigido. Ciò consente di affrontare gli eventuali disagi che potrebbero emergere durante la gestione. Il file risultante può essere utilizzato successivamente per riprendere l'avanzamento della gara da dove la si era lasciata. Tutte le volte in cui una poomsae viene portata a termine, i dati di quest'ultima sono anche inviati al server centrale. Il software di gestione del quadrato, inoltre, deve notificare il server con la classifica parziale ottenuta a fronte di ogni chiusura di torneo (per consentire l'aggiornamento della classifica globale delle palestre).

### Monitor esterni
Il software per la gestione del quadrato di gara è connesso mediante cavi HDMI a 2 monitor esterni:

- **Monitor di torneo**  
    - Mostra l'elenco degli atleti nella gara corrente del torneo, abilitando uno scorrimento verticale, nel caso in cui le preview dei partecipanti non siano visualizzabili interamente sul monitor esterno.
    - Il sistema deve prevedere una diversificazione grafica atta a distinguere le poomsae già svolte, da quelle che non lo sono ancora e da quella attualmente in gestione.
    - Ogni preview fa riferimento a un atleta (e non a una singola poomsae). Essa deve riportare le seguenti informazioni: ordine in lista, nome e cognome, nazionalità e nome della palestra, punteggio totale ed eventuale punteggio di ballottaggio.
    - Nel momento in cui un torneo giunge al termine, viene mostrata la classifica ottenuta, evidenziando gli atleti che hanno ottenuto una medaglia.

- **Monitor di poomsae**  
    - Mostra i dettagli della poomsae correntemente in esecuzione: timer (anche in fase di aggiornamento), nome e cognome dell'atleta, nazionalità e nome della palestra, punteggio totale (con le due componenti per poomsae finali).
    - Deve essere possibile oscurare il monitor in qualunque momento.

In entrambi i casi, qualora il torneo si riferisca a coppie o team, le informazioni anagrafiche dell'atleta sono sostituite con quelle dei membri che compongono il gruppo (prestando attenzione a denominare i team con il nome della palestra per cui partecipano).
Sia nel monitor di torneo che in quello di poomsae, inoltre, la tipologia e i parametri che identificano il torneo devono essere visibili nell'area superiore dello schermo. Sotto questo punto di vista CSEN raccomando l'uso del seguente sistema di colori:
 - **ELIMINATORIE** - verde;
 - **SEMIFINALI** - arancione;
 - **FINALI** - rosso.
  
Sul piano dei requisiti non funzionali, il cliente ribadisce inoltre come tutte le informazioni presentate sui monitor esterni appena discussi debbano essere ben visibili anche da circa 15 metri di distanza.

## Sottosistema 3 - Server
Il terzo è il sottosistema software rappresentante il server. Esso deve consentire la creazione e la configurazione di un'intera competizione.

Per creare una competizione occorre specificare il nome di quest'ultima e il numero di giudici che concorrono alla valutazione degli atleti in torneo, in ogni quadrato di gara.

Il sistema deve prevedere il caricamento di tutti gli atleti, realizzando un parsing a partire dal contenuto del file Excel fornito (con una struttura diversa per ogni tipologia di torneo, su uno specifico foglio). Durante il caricamento di queste informazioni, gli atleti devono essere già inseriti (in ordine alfabetico) all'interno del loro torneo di appartenenza (non specificato su file ma desumibile a partire dai parametri dell'atleta stesso o del gruppo di atleti in caso di coppie o team). A seguito del caricamento degli atleti e dell'iniziale costruzione automatica dei tornei, deve essere visualizzata una schermata riepilogativa per validare i dati raccolti (assieme alla visualizzazione di alcune statistiche, quali il numero di atleti e di palestre partecipanti alla competizione).  

Il sistema deve anche consentire la gestione di eventuali trasferimenti (spostando cioè tutti o alcuni degli atleti facenti parte di un torneo all'interno di un altro). 
Se a fronte di un trasferimento un torneo rimane senza partecipanti, questo deve essere eliminato.

Completati i trasferimenti, deve essere possibile assegnare a ogni quadrato di gara i tornei che questo deve prendere in carico. Uno stesso torneo chiaramente non può essere gestito da più quadrati.

Dal momento che queste operazioni di configurazione possono essere realizzate anche in sessioni diverse nei giorni antecedenti alla gara, è necessario salvare i dati di ogni competizione. È infatti possibile predisporre più competizioni concorrentemente, e non necessariamente gestirle una alla volta. Il software lato server deve pertanto prevedere anche la possibilità di aprire una competizione già creata in precedenza, per riprendere il lavoro da dove lo si era lasciato.

Nel momento in cui la configurazione della competizione è completata e la si avvia, il server è incaricato di accogliere i risultati delle poomsae registrate dai vari software di gestione dei quadrati di gara man mano che questi divengono disponibili. Nell'eventualità in cui per problematiche di rete non sia possibile svolgere l'aggregazione di queste informazioni mediante una comunicazione wireless tra i quadrati e il server stesso, il sistema deve prevedere la possibilità di caricare i file contenenti i dati di tutti i tornei gestiti da ogni quadrato di gara (e prodotti dal rispettivo software) per fondere le varie informazioni in un'unica soluzione.

I punteggi totali delle varie poomsae vengono inviati al server al fine di costruire lo storico completo della competizione. Inoltre, man mano che i tornei vengono completati, il server viene notificato dai quadrati al fine di aggiornare la classifica globale delle varie palestre (elaborata sulla base delle medaglie ricevute dai propri atleti sui vari tornei). Tale classifica è mostrata in tempo reale su un apposito monitor esterno (dedicato anche alla visualizzazione degli atleti partecipanti a tornei correntemente in svolgimento sui quadrati di gara disponibili, permettendo loro di sapere dove recarsi).

### Note

Sul piano dei requisiti, CSEN richiede inoltre che l'interfaccia grafica di tutti i sottosistemi sia semplice, intuitiva e utilizzabile anche dal persona aziendale senza profonda esperienza nel campo dell'informatica.