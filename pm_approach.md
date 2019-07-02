# Descrizione dell'Approccio Utilizzato
In questo documento sono presentate tutte le scelte effettuate durante la simulazione di progetto, motivandone l'adozione. È pertanto descritto l'approccio di Project Management che si è deciso di applicare sulla base delle conoscenze apprese durante il corso universitario. La descrizione è articolata seguendo il tipico ordine dei gruppi di processo, che si susseguono in termini di picchi di attività. 

Il progetto è stato strutturato in modo tale da permettere una fluida navigazione tra questa guida e i documenti relativi al vero processo di Project Management: in ogni sezione verranno infatti proposti collegamenti agli allegati, ai quali verrà rimandata nelle successive sezioni la dettagliata descrizione di cosa è avvenuto al momento della loro stesura.

La scelta di pubblicare questa simulazione su un repository è dovuta a diversi fattori:
- offre un unico spazio condiviso tra i membri, dove poter collaborare anche a distanza;
- dispone di un sistema di versioning dei file, permettendo di avere un pieno controllo sullo storico delle modifiche apportate ai documenti pubblicati;
- abilita l'utilizzo di collegamenti diretti tra i documenti non solo tramite link url, ma percorsi relativi all'interno dello stesso repository;
- simula perfettamente lo spazio che una fantomatica azienda dovrebbe predisporre per gestire i propri progetti;
- facilita la stesura della documentazione e permette un'immediata esplorazione di essa direttamente dal browser, anche grazie all'utilizzo di MarkDown.

Per la stesura della documentazione si è fatto uso di diversi software:
- **Skype**, per la comunicazione a distanza (ove non era possibile un incontro dal vivo), abilitato anche alla condivisione dello schermo, per un maggiore coinvolgimento;
- **Trello**, per l'organizzazione e il tracciamento del lavoro ([link alla bacheca](https://trello.com/b/dfDeDMvi/pm-project));
- **Visual Studio Code** per la stesura della documentazione in MarkDown, anche in modalità "Live Sharing" (per permettere la contemporanea stesura del documento da parte di entrambi i membri);
- **Microsoft Project** (in versione di prova) per ...;
- **TeXstudio** per la generazione di parte della documentazione tramite il linguaggio LaTeX;
- **GitHub Desktop** per la gestione del repository.

# Introduzione
In questa sezione sono fornite informazioni di carattere generale relative all'esecutore e al committente. Viene analizzato il rapporto tra queste due entità, con lo scopo di fornire una larga veduta sull'intera struttura su cui il progetto si basa e di comprendere le ragioni che hanno portato a intraprendere determinate scelte a discapito di altre. Si illustrano inoltre le competenze dei singoli membri facenti parte del team dell'azienda fornitrice, scendendo anche nel dettaglio delle politiche aziendali.

## Azienda esecutrice
L'esecutore del progetto è la startup "**Punch Code**". Essa è un'azienda informatica specializzata nella costruzione di soluzioni software, composta da due soli dipendenti neo-laureati. Essendosi appena costituita, non presenta esperienza pregressa in altri progetti e conseguentemente non possiede un know-how in alcuna area di mercato. Considerando l'esiguo numero di persone interne all'azienda, quest'ultima non è al momento decomposta in specifiche aree funzionali sul piano organizzativo; tuttavia è in espansione e prevede l'acqusizione nel breve termine di nuovo personale con competenze tecniche specializzate. Il principale motivo per cui l'azienda è stata scelta dal committente, oltre ad aver presentato un'offerta più aggressiva rispetto ai principali concorrenti, è da ricercarsi nella sua propensione all'uso di tecnologie innovative che l'hanno portata ad acquisire un'indubbia fama sul territorio e a ottenere un alto livello di attenzione sul panorama mediatico per mezzo dell'incubatore nel quale è localizzata.

### Startup Team

"Punch Code" è formata da due soli membri ricoprenti entrambi il ruolo di Project Manager. Le competenze di ogni dipendente sono tracciate dall'azienda all'interno di un apposito [documento](project_docs/startup_team_skills.md), tenendo conto sia di *pre skill* (o soft skill) che di *pro skill* (o hard skill). Le prime si riferiscono alle capacità inerenti alla sfera interpersonale e della comunicazione, indipendenti dalla specifica mansione lavorativa e pertanto trasversali. Le seconde sono quelle competenze tecniche relative allo svolgimento di una certa professione, acquisibili tramite lo studio e certificabili. Nell'ottica di andare a delineare un valido strumento di appoggio per un Project Manager ai fini della futura assegnazione delle attività ai membri dello staff in fase di Planning, si è infatti ritenuto utile includere la valutazione di ambo le tipologie di abilità. Per quanto concerne l'assegnazione dei punteggi, si è voluta considerare una scala di valori numerici adimensionali compresa tra 1 e 5 (preferendola ad alternative misure non numeriche che avrebbero impedito la valutazione delle competenze in media di tutto il team su un certo parametro).

[//]: # (TODO: uno dei due potrebbe lavorare difendendo gli interessi legati al ruolo di un architetto, impersonandolo, per originare conflitti costruttivi)

### Politiche aziendali

Per far fronte ipoteticamente a più progetti in parallelo, l'azienda decide di adottare delle buone pratiche di natura generale al fine di uniformare alcuni degli aspetti più critici della gestione dei gruppi di processo (lasciando comunque spazio a eventuali personalizzazioni dettate dalle esigenze di specifici progetti, qualora si dovessero rivelare necessari).
Si sottolinea come tali politiche aziendali possano subire modifiche a fronte della review operata al termine di ogni progetto, nell'intento di un continuo processo di miglioramento. Un ulteriore motivo di cambiamento potrebbe essere anche la futura evoluzione dell'organizzazione aziendale a causa del maggior numero di dipendenti e di una migliore suddivisione delle responsabilità.

#### Documentazione

##### Sviluppo
"Punch Code" riversa sulla documentazione un ruolo di primaria importanza per numerose ragioni (tra cui riusabilità, manutenibilità, condivisione e storico sia in termini di problematiche che di soluzioni).
Rientra pertanto nelle politiche aziendali la volontà di dedicarsi alla scrittura di quest'ultima non a progetto finito, ma costantemente nel corso della sua evoluzione. L'overhead legato all'operazione di aggiornamento continuo è così giustificato dall'obiettivo di minimizzare il senso di frustrazione in fase di stesura (partizionando il carico di lavoro complessivo) e di voler risparmiare tempo in futuro.

[//]: # (TODO: tecniche di gamification per rendere la scrittura della documentazione un'attività meno pesante?)
[//]: # (TODO: anche in pair programming / con più addetti per sollecitare la generazione di utili brainstorming. Nell'aggiornare la documentazione, infatti, il management e gli sviluppatori capiscono dove sono stati apportati eventuali cambiamenti di rotta e quali questi siano)

##### Mantenimento
L'azienda utilizza un repository online come **workbook** per conservare l'insieme della documentazione relativa ai vari progetti, anche a fini legali. Per consentire un facile reperimento delle informazioni, i file vengono suddivisi in directory in base alla loro tipologia e al progetto di appartenenza.

#### Orari lavorativi e modalità
La startup segue un comune modello di suddivisione delle giornate e dell'orario lavorativo, cosiderando la produzione attiva dal lunedì al venerdì, dalle ore 09:00 alle ore 18:00, con una pausa pranzo intermedia nella fascia 12:00-13:00. La disponibilità del team permette di essere comunque molto flessibili, consentendo eventuali modifiche agli orari e/o giornate lavorative (assecondando eventualmente le esigenze del committente) e consentendo lo svolgimento del lavoro in forma telematica direttamente da casa.

#### Project Meeting

##### Project Scoping Meeting

Al fine di entrare in contatto col cliente e iniziare a delineare lo scope del progetto, l'azienda prevede un Project Scoping Meeting organizzato come di seguito descritto.
Sul piano dello schema, l'obiettivo delle varie riunioni che compongono tale processo consiste nella produzione dei seguenti deliverable:
- Conditions of Satisfaction (CoS), con match tra richieste del committente e reali esigenze;
- Requirements Breakdown Structure (RBS);
- PMLC Model;
- Project Overview Statement (POS).

L'elenco dei partecipanti prevede la presenza delle seguenti figure:
- lo *staff aziendale* col ruolo di Project Manager;
- il *Client Group* (con l'eventuale presenza sollecitata di personale legato ad aree funzionali o ad attività in discussione con l'agenda odierna);

Non disponendo delle risorse necessarie, i ruoli di *Facilitatore* e *Tecnografo* sono temporaneamente ricoperti dai membri del team aziendale che cercheranno conseguentemente di dare valore al tempo, evitare discussioni inutili, convergere su tutti gli argomenti in agenda, raccogliere le informazioni in forma documentale (verbale) e strutturarle in modo tale da facilitare il loro reperimento.

Dal momento che il Project Scoping Meeting può comprendere numerose sessioni in giornate diverse, l'azienda preferisce intraprendere una sola riunione di partenza, valutandone eventualmente altre in base alle necessità. Tra due sessioni è richiesto un intervallo di tempo pari a una settimana, al fine di analizzare e organizzare le informazioni raccolte, oltre che preparare la prossima agenda. In ogni caso, una sessione si conclude sempre con la definizione dei punti che occorrerà discutere durante la successiva.

[//]: # (Regole operative per il team)

##### Daily Status Meeting

L'azienda prevede la presenza di riunioni giornaliere per mantenere monitorato lo stato di avanzamento dei task. Nello specifico adotta la forma di Stand-up Meeting, preferendola ad alternative come resoconti di fine giornata.

Tali incontri avvengono alle ore 09:00 del mattino e hanno una durata massima di 20 minuti, nei quali si riporta sinteticamente lo stato di ciascuna attività e ci si concentra sugli aspetti maggiormenti critici.
In queste occasioni, si associa inoltre a ogni task un colore in linea col Spotlight Report allo scopo di creare un comodo strumento visuale capace di offrire in breve tempo una panoramica sull'andamento di un certo progetto. L'azienda consiglia inoltre ai dipendenti di valutare sempre se sia il caso di considerare una riunione specifica a fronte della presenza di task fuori controllo (etichettati come rossi).

Lo svolgimento degli Stand-Up Meeting dovrebbe sempre avvenire dal vivo, anche se, in via del tutto eccezzionale, è possibile svolgerlo in via telematica: in questo caso, però, è strettamente necessario l'utilizzo di una WebCam per un rapporto semi-diretto con gli interlocutori (che secondo degli studi sociologici favorirebbe lo sviluppo della discussione). Data la natura informale degli incontri, è preferibile parteciparvi "*in piedi*" per stimolare una maggior attenzione e minimizzare la durante del meeting stesso.

##### Problem Resolution Meeting

##### Project Review Meeting

#### Gestione delle comunicazioni

- L'accettazione di ogni informazione da parte del destinatario (cliente o figura aziendale) avviene esclusivamente per mezzo di feedback con uno specifico [template](project_docs/feedback_template.md), in modo da evitare pericolosi scenari che potrebbero essere dettati dalla presenza di una regola di silenzio assenso;
- A fronte di ogni Stand-up Meeting, viene redatta una documentazione scritta soltanto per le attività cui è stata assegnata una colorazione gialla o rossa attraverso lo Spotlight Report da parte del responsabile dello specifico task (concentrandosi sulle sole attività oggetto di scostamenti dal piano o rappresentanti scenari fuori controllo), raccogliendo informazioni motivazionali utili ed evitando di investire tempo nella produzione di comunicazioni scritte per le attività in schedula (verdi). Terminato l'incontro, il documento viene caricato nel repository dell'azienda.

## Committente
Csen.

## Relazione esecutore-committente
Csen.


# Scoping
In questa sezione...

## Project Scoping Meeting

- Applicando le politiche aziendali, si è reso necessario lo svolgimento di tale fase (che costituisce la prima occasione d'incontro tra il fornitore e il committente) su più giornate (sessioni)
- Ne sono state realizzate X (es. 5) e gli argomenti trattati in ciascuna con le rispettive date sono disponibili al seguente documento Y. 1° incontro: generale + 2° incontro: tablet + 3° incotro: sw quadrato + 4° incontro: server + comunicazione wireless
- il cliente ha dato disponibilità a contatti frequenti

[//]: # (Ricordarsi della discussione budget e tempo alla prima sessione)
[//]: # (Non sono spiegati ulteriori incontri, in quanto sono presenti nel doc ufficialmente linkato)

## Resources Breakdown Structure (RBS)

### Raccolta dei requisiti

- interviste ai vari stackholder lato cliente (specificando il tipo di intervista: es. imbuto + esempi domande in base al ruolo)
    - ad Andrea (il PM del committente)
    - ai futuri utilizzatori del sw (gestori gare e giudici)
- osservazioni sul campo (durante i tornei) per una comprensione più chiara delle esigenze

### Costruzione
Spiegazione dei vari requisiti sui rami.

## Scelta del PMLC Model
- siamo pochi, non possiamo avere uno scrum master: ha poco senso essere agili.
(perchè non possiamo essere agili, ma perchè facciamo di tutto per esserlo nelle nostre possibilità)
- dato che il cliente si è dimostrato molto disponibile a frequenti feedback nonchè felice di ciò...

## Project Overview Statement (POS)
C'è qualcosa da spiegare (?)

[//]: # (Spiegare la scelta di mettere il Glossiario nel POS)

## Project Definition Statement (PDS)
C'è qualcosa da spiegare (?)

### Analisi dei rischi
Spiegare solo il perchè dell'uso di un diagramma rispetto a un altro.

##