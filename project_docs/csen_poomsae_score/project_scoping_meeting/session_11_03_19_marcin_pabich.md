# Project Scoping Meeting Agenda

**Dipendente**: Marcin Pabich  
**Data**: 11 marzo 2019  
**Orario**: 09:00  
**Luogo**: Sala Riunioni PunchCode  
**Materiale**:
- [Immagini del software usato da aziende competitor](./session_11_03_19_res/competitor)
- [Architettura immaginata dal cliente](./session_11_03_19_res/customer_architecture_idea.pdf)

## Oggetto
Primo incontro conoscitivo con CSEN

## Partecipanti
- **Project Manager fornitore:**
    - Giacomo Frisoni
    - Marcin Pabich
- **Project Manager cliente:**
    - Enrico Comando

<br/>

<table>
    <tr>
        <th colspan="3">Prima del meeting</th>
        <th colspan="1">Durante il meeting</th>
    </tr>
    <tr>
        <th width="20%">Argomento in agenda</th>
        <th width="15%">Orario</th>
        <th width="20%">Direttore della discussione</th>
        <th width="35%">Note</th>
    </tr>
    <tr>
        <td>Introduzione</td>
        <td align="center">09:00 - 09:15</td>
        <td align="center">Giacomo Frisoni</td>
        <td>CSEN fa parte di una realtà molto grande. Il Project Manager ci comunica sin da subito il loro interesse verso il nostro modo di lavorare.</td>
    </tr>
    <tr>
        <td>Scopo del meeting</td>
        <td align="center">09:15 - 09:20</td>
        <td align="center">Giacomo Frisoni</td>
        <td>-</td>
    </tr>
    <tr>
        <td>Descrizione dello stato corrente e del problema</td>
        <td align="center">09:20 - 11:00</td>
        <td align="center">Enrico Comando</td>
        <td>CSEN ha un problema molto complesso dovuto alla scarsa digitalizzazione dei processi che riguardano le competizioni di Taekwondo. I punteggi vengono presi e gestiti in formato cartaceo, con evidenti difficoltà di gestione. I tempi risultano pertanto molto lunghi e spesso si incorre in errori a causa della pressione con cui si è chiamati a preoccuparsi manualmente dell'avanzamento degli atleti nelle varie gare (eliminatorie, semifinali e finali) che compongono un torneo. Sotto questo punto di vista infatti le regole da considerare sono molteplici e il numero di atleti che passano il turno varia sulla base della gara in cui ci si trova. Inoltre, la gara di partenza per un torneo è determinata dal numero di partecipanti a esso.
        CSEN sottolinea come l'elenco degli atleti partecipanti sia già disponibile sotto forma di file Excel alcuni giorni prima di ogni competizione e come questo sia elaborato da una soluzione software (con lo scopo di aggregare le registrazioni dei singoli atleti compiute dalle palestre tramite un loro portale web) di cui sono già in possesso presso la loro sede di Roma. 
        CSEN sottolinea anche come la partecipazione di atleti non previamente registrati sia spesso causa di confusione. L'individuazione del torneo di appartenenza per un atleta avviene sulla base della tripla categoria-sesso-grado di quest'ultimo. Gli atleti possono esibirsi da soli, in coppia o in team (formati al massimo da 5 persone). Antecedentemente alla competizione, un responsabile si riserva la possibilità di realizzare dei trasferimenti per l'accorpamento di tornei altrimenti composti singolarmente da un numero molto ridotto di atleti.</td>
    </tr>
    <tr>
        <td>Descrizione dello stato finale che si vuole raggiungere</td>
        <td align="center">11:00 - 12:00</td>
        <td align="center">Enrico Comando</td>
        <td> CSEN ci comunica che l'idea di ricorrere a una soluzione software sia nata anche osservando la gestione di tornei fatta da un competitor in altri paesi. Sotto questo punto di vista, l'organizzazione ci rilascia del materiale per comprendere meglio le loro esigenze o su cui eventualmente ispirarci. La società - prendendo come riferimento questo approccio - ha pensato a una soluzione nella quale i giudici facciano uso di un'applicazione Android su dei tablet per esprimere le loro votazioni. I punteggi vengono poi catturati da un software su dei PC centrali (uno per ogni quadrato di gara), incaricati di raccoglierli e mostrarli al pubblico tramite dei monitor esterni. Si pensa già alla presenza di un server per la gestione dei vari tornei che compongono una competizione, sia in fase preparatoria che in termini di calcolo classifiche.</td>
    </tr>
    <tr>
        <td>Discussione dei requisiti e delle modalità di raccolta</td>
        <td align="center">12:00 - 13:00</td>
        <td align="center">Giacomo Frisoni</td>
        <td>
        I macro requisiti sono di seguito riportati.
        <ul>
            <li>Applicazione Android per tablet finalizzata all'assegnazione di punteggi a ogni atleta da parte dei giudici.</li>
            <li>Software per la gestione delle poomsae fatte su un quadrato, incaricato di raccogliere i punteggi di ogni atleta nelle varie fasi di gara che compongono un torneo.</li>
            <li>Server per la gestione dei tornei previsti da una competizione odierna (con un partizionamento dei tornei stessi tra i vari quadrati) e per l'elaborazione di classifiche sia locali ai tornei che globali sull'intera competizione in base alle medaglie guadagnate dalle palestre.</li>
        </ul>
        È evidente che i problemi da risolvere siano numerosi per un singolo incontro, per cui i requisiti vengono stabiliti solo "approsimativamente". Sarà svolta una riunione per ogni sottosistema. Anche la scelta degli approcci con cui realizzare la raccolta dei requisiti più dettagliati è pertanto rimandata. Le prossime sessioni verranno realizzate il prima possibile, in base alla disponibilità del cliente. A causa delle numerose osservazioni, abbiamo concluso in ritardo alle 13:25.</td>
    </tr>
    <tr>
        <td>Budget e tempi</td>
        <td align="center">14:00 - 14:30</td>
        <td align="center">Enrico Comando</td>
        <td>Il cliente non può sostenere costi eccessivamente alti e il budget è stimato essere di circa 6000€. Si rimanderà ad una valutazione più congrua, una volta definiti tutti i dettagli del progetto con le prossime sessioni. Per quanto concerne le tempistiche, il cliente è disposto ad attendere diversi mesi per la soluzione software completa ma necessita al più presto del sottosistema incentrato sui tablet per la raccolta dei voti da parte dei giudici. Il cliente inoltre osserva come il numero delle gare sia destinato a intensificarsi entro la fine dell'estate e come necessiti di almeno un primo rilascio entro breve termine.</td>
    </tr>
    <tr>
        <td>Domande varie</td>
        <td align="center">14:30 - 15:00</td>
        <td align="center">Giacomo Frisoni</td>
        <td>
        <ul>
            <li>Il procurement dell'hardware non è affidato a noi. L'azienda possiede già computer portatili, monitor esterni e altri componenti correlati. Per quanto concerne i tablet, al momento CSEN non li ha già in dotazione ma prevede di comprarli a breve. Sotto questo punto di vista la scelta del dispositivo è già stata fatta e di conseguenza non abbiamo libertà di manovra. CSEN si promette di portarci al prossimo incontro le caratteristiche tecniche di tali tablet.</li>
            <li>Per ogni atleta si possiedono le seguenti informazioni (disponibili nel documento excel rilasciato): nome, cognome, categoria, grado, sesso, nazionalità, palestra di appartenenza e nazionalità della palestra.</li>
            <li>Una palestra è normalmente suddivisa in 4 quadrati di gara. La competizione svolta in un certo giorno è l'insieme di tutti i tornei che devono essere intrapresi. Ogni torneo si compone di 3 gare (eliminatorie, semifinali e finali), alcune delle quali potrebbero non essere effettuate qualora il numero dei partecipanti sia ridotto (es. partire direttamente dalle finali). I tornei sono suddivisi tra i 4 quadrati di gara (tipicamente in base all'età degli atleti e al loro grado di cintura), in modo da poterli portare avanti in contemporanea. La gestione di un torneo non può essere fatta su più quadrati di gara: inizia su uno e lì finisce.</li>
        </ul>
        </td>
    </tr>
    <tr>
        <td>Documentazione</td>
        <td align="center">15:00 - 15:30</td>
        <td align="center">Giacomo Frisoni</td>
        <td>Non essendo del tutto chiari i requisiti, non è possibile stendere la documentazione in ogni singolo dettaglio: vengono descritti aspetti generali ma è probabile che ci saranno modifiche sostanziali durante i prossimi incontri.</td>
    </tr>
</table>

<br/>

## Conditions of Satistaction (CoS)

<!--
Il cliente vuole gestire digitalmente tutti i processi che compongono una gara di Taekwondo, attraverso l'uso di tre categorie di dispositivi elettronici:

- **Tablet**  
  Servirà ai giudici per acquisire punteggi in modo semplice e intuitivo. 

- **PC/Server**  
  Raccoglierà i punteggi inviati dai tablet. Farà controlli ed elaborerà dati che verranno poi memorizzati e visualizzati.

- **Monitor**  
  Visualizzeranno al pubblico i dettagli delle gare e i punteggi raccolti.

Il cliente esige che il sistema progettato:
- sia compliant con regole ufficiali di Taekwondo, rispettando nomenclature e i minimali e massimali dei punti;
- sia facile da utilizzare, a causa della presenza di potenziali utilizzatori con scarse conoscenze tecnologiche e/o con problemi di vista;
- sia compatibile con l'attuale sistema, che fornisce i dati degli atleti e palestre in mediante l'utilizzo di un foglio elettronico (formato Excel);
- possa automatizzare l'importazione dei dati citati sopra nel nuovo sistema;
- preveda un meccanismo di backup in caso di blackout;
- non arrechi ritardi, blocchi o perdite di dati durante la gara.


 Gli atleti che si esibiscono fanno parte di diversi gruppi, suddivisi in tre macro-gruppi:

- categoria
  - junior;
  - senior;
  - altro
  - altro
  - altro
  - altro
  - altro
- sesso
  - maschio;
  - femmina;
- grado
  - cup
  - dan
  - altro
  - altro
  - altro
  - altro
-->

## Valutazione del Meeting
 - L'agenda è stata rispettata? [NO]
 - Tutti i partecipanti hanno interagito? [YES]
 - L'obiettivo del meeting è stato raggiunto? [NO]
 - Abbiamo chiarito i prossimi step? [YES]
 - Questo meeting è stato utile? [YES]
 - Come potrebbe migliorare il prossimo meeting? *Si punterà a discutere soltanto di una parte del progetto per delimitare meglio le problematiche da affrontare*

## Pianificazione del prossimo meeting
 - **Obiettivo:** Discussione del primo sottosistema (applicazione Android per i tablet utilizzati dai giudici)
 - **Data**: 14/03/19
 - **Luogo**: Sala Riunioni della "PunchCode"
 - **Partecipanti:** Giacomo Frisoni, Marcin Pabich, Enrico Comando, 2 giudici

<br/>


## 
*Firma*: Marcin Pabich  
*Data*: 11/03/19