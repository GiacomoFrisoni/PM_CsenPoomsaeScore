# Indice <!-- omit in toc -->

- [1. Descrizione dell'Approccio Utilizzato](#1-Descrizione-dellApproccio-Utilizzato)
- [2. Introduzione](#2-Introduzione)
  - [2.1. Azienda esecutrice](#21-Azienda-esecutrice)
    - [2.1.1. Startup Team](#211-Startup-Team)
    - [2.1.2. Politiche aziendali](#212-Politiche-aziendali)
      - [2.1.2.1. Orari lavorativi](#2121-Orari-lavorativi)
      - [2.1.2.2. Modalità di lavoro](#2122-Modalit%C3%A0-di-lavoro)
        - [2.1.2.2.1. Gamification](#21221-Gamification)
        - [2.1.2.2.2. Documentazione](#21222-Documentazione)
      - [2.1.2.3. Project Meeting](#2123-Project-Meeting)
        - [2.1.2.3.1. Project Scoping Meeting](#21231-Project-Scoping-Meeting)
        - [2.1.2.3.2. Daily Status Meeting](#21232-Daily-Status-Meeting)
        - [2.1.2.3.3. Problem Resolution Meeting](#21233-Problem-Resolution-Meeting)
        - [2.1.2.3.4. Project Review Meeting](#21234-Project-Review-Meeting)
      - [2.1.2.4. Gestione delle comunicazioni](#2124-Gestione-delle-comunicazioni)
  - [2.2. Committente](#22-Committente)
  - [2.3. Relazione esecutore-committente](#23-Relazione-esecutore-committente)
- [3. Scoping](#3-Scoping)
  - [3.1. Primo contatto](#31-Primo-contatto)
  - [3.2. Project Scoping Meeting](#32-Project-Scoping-Meeting)
  - [3.3. Resources Breakdown Structure (RBS)](#33-Resources-Breakdown-Structure-RBS)
    - [3.3.1. Raccolta dei requisiti](#331-Raccolta-dei-requisiti)
      - [3.3.1.1 Interviste](#3311-Interviste)
      - [3.3.1.2 Osservazioni](#3312-Osservazioni)
    - [3.3.2. Costruzione](#332-Costruzione)
      - [3.3.2.1 App Android](#3321-App-Android)
      - [3.3.2.2 Software Gestione Quadrato](#3322-Software-Gestione-Quadrato)
      - [3.3.2.3 Server](#3323-Server)
  - [3.4. Scelta del PMLC Model](#34-Scelta-del-PMLC-Model)
  - [3.5. Budget e tempi](#35-Budget-e-tempi)
  - [3.6. Project Overview Statement (POS)](#36-Project-Overview-Statement-POS)
  - [3.7. Project Definition Statement (PDS)](#37-Project-Definition-Statement-PDS)
    - [3.7.1. Analisi dei rischi](#371-Analisi-dei-rischi)
- [4. Planning](#4-Planning)
- [5. Bibliografia](#5-Bibliografia)

[//]: # (-------------------------------------------------------------------------)

# 1. Descrizione dell'Approccio Utilizzato
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

[//]: # (-------------------------------------------------------------------------)

# 2. Introduzione
In questa sezione sono fornite informazioni di carattere generale relative all'esecutore e al committente. Viene analizzato il rapporto tra queste due entità, con lo scopo di fornire una larga veduta sull'intera struttura su cui il progetto si basa e di comprendere le ragioni che hanno portato a intraprendere determinate scelte a discapito di altre. Si illustrano inoltre le competenze dei singoli membri facenti parte del team dell'azienda fornitrice, scendendo anche nel dettaglio delle politiche aziendali.

## 2.1. Azienda esecutrice
L'esecutore del progetto è la startup "**Punch Code**". Essa è un'azienda informatica specializzata nella costruzione di soluzioni software, composta da due soli dipendenti neo-laureati. Essendosi appena costituita, non presenta esperienza pregressa in altri progetti e conseguentemente non possiede un know-how in alcuna area di mercato. Considerando l'esiguo numero di persone interne all'azienda, quest'ultima non è al momento decomposta in specifiche aree funzionali sul piano organizzativo; tuttavia è in espansione e prevede l'acqusizione nel breve termine di nuovo personale con competenze tecniche specializzate. Il principale motivo per cui l'azienda è stata scelta dal committente, oltre ad aver presentato un'offerta più aggressiva rispetto ai principali concorrenti, è da ricercarsi nella sua propensione all'uso di tecnologie innovative che l'hanno portata ad acquisire un'indubbia fama sul territorio e a ottenere un alto livello di attenzione sul panorama mediatico per mezzo dell'incubatore nel quale è localizzata.

### 2.1.1. Startup Team

"Punch Code" è formata da due soli membri ricoprenti entrambi il ruolo di Project Manager. Le competenze di ogni dipendente sono tracciate dall'azienda all'interno di un apposito [documento](project_docs/startup_team_skills/startup_team_skills.md), tenendo conto sia di *pre skill* (o soft skill) che di *pro skill* (o hard skill). Le prime si riferiscono alle capacità inerenti alla sfera interpersonale e della comunicazione, indipendenti dalla specifica mansione lavorativa e pertanto trasversali. Le seconde sono quelle competenze tecniche relative allo svolgimento di una certa professione, acquisibili tramite lo studio e certificabili. Nell'ottica di andare a delineare un valido strumento di appoggio per un Project Manager ai fini della futura assegnazione delle attività ai membri dello staff in fase di Planning, si è infatti ritenuto utile includere la valutazione di ambo le tipologie di abilità. Per quanto concerne l'assegnazione dei punteggi, si è voluta considerare una scala di valori numerici adimensionali compresa tra 1 e 5 (preferendola ad alternative misure non numeriche che avrebbero impedito la valutazione delle competenze in media di tutto il team su un certo parametro).

Il team è consapevole dell'assenza di una figura interna rivestente il ruolo di Architetto. Per consentire comunque l'instaurazione di dibattiti costruttivi si è scelto - in base alle pre-skill e alle pro-skill - di far sì che un membro difendesse gli interessi legati al ruolo di un architetto (impersonandolo).
Sotto questo punto di vista, è Marcin Pabich (specie grazie alle sue maggiori capacità creative) ad occuparsi anche di questo aspetto.

### 2.1.2. Politiche aziendali

Per far fronte ipoteticamente a più progetti in parallelo, l'azienda decide di adottare delle buone pratiche di natura generale al fine di uniformare alcuni degli aspetti più critici della gestione dei gruppi di processo (lasciando comunque spazio a eventuali personalizzazioni dettate dalle esigenze di specifici progetti, qualora si dovessero rivelare necessari).
Si sottolinea come tali politiche aziendali possano subire modifiche a fronte della review operata al termine di ogni progetto, nell'intento di un continuo processo di miglioramento. Un ulteriore motivo di cambiamento potrebbe essere anche la futura evoluzione dell'organizzazione aziendale a causa del maggior numero di dipendenti e di una migliore suddivisione delle responsabilità.

#### 2.1.2.1. Orari lavorativi
La startup segue un comune modello di suddivisione delle giornate e dell'orario lavorativo, cosiderando la produzione attiva dal lunedì al venerdì, dalle ore 09:00 alle ore 18:00, con una pausa pranzo intermedia nella fascia 12:00-13:00. La disponibilità del team permette di essere comunque molto flessibili, consentendo eventuali modifiche agli orari e/o giornate lavorative (assecondando eventualmente le esigenze del committente).

#### 2.1.2.2. Modalità di lavoro
L'azienda consente lo svolgimento del lavoro in forma telematica direttamente da casa, ad eccezzione dei Project Meeting di diversa natura, come discusso in dettaglio nella [prossima sezione](#2123-project-meeting). Inoltre, per la risoluzione dei problemi complessi e per un maggiore coinvolgimento dei dipendenti, il team di sviluppo può avvalersi anche di tecniche di lavoro denominate *Pair Programming*, sia in remoto che in loco; quest'ultime possono essere utilizzate sia in fase di coding, che nella stesura della documentazione. Esse infatti stimolano utili brainstorming e danno la possibilità al management e agli sviluppatori di capire dove siano stati apportati eventuali cambiamenti di rotta e quali questi siano.

##### 2.1.2.2.1. Gamification
Al fine di motivare gli impiegati e rendere le loro attività quotidiane meno frustranti nella loro percezione, "PunchCode" si avvale di tecniche di Gamification all'interno dei propri progetti di sviluppo software di durata massima stimata non superiore ai 5 mesi. Questa scelta è frutto di approfondite [ricerche in letteratura](#bibliography-1)<sup>1</sup> che testimoniano come esse influenzino positivamente i risultati di un gruppo di lavoro.  
"Punch Code" - sotto questo punto di vista - si avvale di un proprio sistema di login per il tracciamento delle attività compiute dai dipendenti, premiandoli con dei *punti* (come componente di gioco) in caso di:
- lettura di codice / documentazione di colleghi con invio di feedback (in forma di rating);
- ricezione di feedback positivi da parte di un collega.

L'uso di una metodologia di questo tipo porta a diversi vantaggi:
- stimola i dipendenti a revisionare il lavoro realizzato dagli altri;
- abilita una forma di trasferimento di conoscenza a partire da esempi positivi forniti dai colleghi.

##### 2.1.2.2.2. Documentazione

- **Sviluppo**  
"Punch Code" riversa sulla documentazione un ruolo di primaria importanza per numerose ragioni (tra cui riusabilità, manutenibilità, condivisione e storico sia in termini di problematiche che di soluzioni).
Rientra pertanto nelle politiche aziendali la volontà di dedicarsi alla scrittura di quest'ultima non a progetto finito, ma costantemente nel corso della sua evoluzione. L'overhead legato all'operazione di aggiornamento continuo è così giustificato dall'obiettivo di minimizzare il senso di frustrazione in fase di stesura (partizionando il carico di lavoro complessivo) e di voler risparmiare tempo in futuro.

- **Mantenimento**
L'azienda utilizza un repository online come **workbook** per conservare l'insieme della documentazione relativa ai vari progetti, anche a fini legali. Per consentire un facile reperimento delle informazioni, i file vengono suddivisi in directory in base alla loro tipologia e al progetto di appartenenza.

#### 2.1.2.3. Project Meeting

##### 2.1.2.3.1. Project Scoping Meeting

Al fine di entrare in contatto col cliente e iniziare a delineare lo scope del progetto, l'azienda prevede un Project Scoping Meeting organizzato come di seguito descritto.
Sul piano dello schema, l'obiettivo delle varie riunioni che compongono tale processo consiste nella produzione dei seguenti deliverable:
- Conditions of Satisfaction (CoS), con match tra richieste del committente e reali esigenze;
- Requirements Breakdown Structure (RBS);
- PMLC Model;
- Project Overview Statement (POS).

L'elenco dei partecipanti prevede la presenza delle seguenti figure.
- Lo *staff aziendale* col ruolo di Project Manager.
- Il *Client Group* (con l'eventuale presenza sollecitata di personale legato ad aree funzionali o ad attività in discussione con l'agenda odierna). Come per il gruppo di lavoro dell'esecutore, anche quello del committente è già stato definito antecedentemente allo scoping.

Non disponendo delle risorse necessarie, i ruoli di *Facilitatore* e *Tecnografo* sono temporaneamente ricoperti dai membri del team aziendale che cercheranno conseguentemente di dare valore al tempo, evitare discussioni inutili, convergere su tutti gli argomenti in agenda, raccogliere le informazioni in forma documentale (verbale) e strutturarle in modo tale da facilitare il loro reperimento. L'azienda prevede tuttavia di integrare un *Facilitatore* non appena ne avrà le possibilità, poichè - nonostante i maggiori costi che ne deriveranno - la figura di un mediatore imparziale tra le parti è da considerarsi centrale e potrebbe costituire un valore aggiunto significativo, anche nell'intento di evitare problematiche dovute a fraintendimenti e tensioni tra chi gestirà e svilupperà il progetto e il committente.

Dal momento che il Project Scoping Meeting può comprendere numerose sessioni in giornate diverse, l'azienda preferisce intraprendere una sola riunione di partenza, valutandone eventualmente altre in base alle necessità. Tra due sessioni è richiesto un intervallo di tempo pari a una settimana, al fine di analizzare e organizzare le informazioni raccolte, oltre che preparare la prossima agenda. In ogni caso, una sessione si conclude sempre con la definizione dei punti che occorrerà discutere durante la successiva.

L'azienda è anche interessata a fare una breve review al termine di ogni sessione di Project Scoping Meeting per valutare il rispetto dell'agenta, il livello di partecipazione e altri parametri utili per un miglioramento continuo.

##### 2.1.2.3.2. Daily Status Meeting

L'azienda prevede la presenza di riunioni giornaliere per mantenere monitorato lo stato di avanzamento dei task. Nello specifico adotta la forma di Stand-up Meeting, preferendola ad alternative come resoconti di fine giornata.

Tali incontri avvengono alle ore 09:00 del mattino e hanno una durata massima di 20 minuti, nei quali si riporta sinteticamente lo stato di ciascuna attività e ci si concentra sugli aspetti maggiormenti critici.
In queste occasioni, si associa inoltre a ogni task un colore in linea col Spotlight Report allo scopo di creare un comodo strumento visuale capace di offrire in breve tempo una panoramica sull'andamento di un certo progetto. L'azienda consiglia inoltre ai dipendenti di valutare sempre se sia il caso di considerare una riunione specifica a fronte della presenza di task fuori controllo (etichettati come rossi).

Lo svolgimento degli Stand-Up Meeting dovrebbe sempre avvenire dal vivo, anche se, in via del tutto eccezzionale, è possibile svolgerlo in via telematica: in questo caso, però, è strettamente necessario l'utilizzo di una WebCam per un rapporto semi-diretto con gli interlocutori (che secondo degli studi sociologici favorirebbe lo sviluppo della discussione). Data la natura informale degli incontri, è preferibile parteciparvi "*in piedi*" per stimolare una maggior attenzione e minimizzare la durante del meeting stesso.

##### 2.1.2.3.3. Problem Resolution Meeting

"PunchCode" considera lo svolgimento di Problem Resolution Meeting per la discussione di problematiche riscontrate durante lo svolgimento di un progetto. L'azienda prevede nello specifico che questi siano organizzati qualora si ritengano necessari a fronte dell'individuazione di attività fuori controllo durante uno Stand-up Meeting. In queste riunioni per la risoluzione di un problema l'agenda deve prevedere:
- la partecipazione dei soli sviluppatori coinvolti nel problema;
- la determinazione del/i proprietario/i (owner) del problema (potenzialmente molteplici da punti di vista diversi);
- l'identificazione della soluzione;
- la determinazione delle modalità (come e quando) attraverso cui stabilire che il problema è da considerarsi risolto.

Preme tuttavia sottolineare come - a causa del ridotto personale attualmente presente nella startup - tali meeting richiedano necessariamente la presenza di entrambi i membri.

##### 2.1.2.3.4. Project Review Meeting

In concomitanza col raggiungimento di una milestone, l'azienda svolge un Project Review Meeting. Durante questi eventi formali:
- si svolge la presentazione dello stato del progetto in corrispondenza della milestone e si effettua una sua revisione critica;
- partecipano il project manager, il senior management, lo sponsor, il committente, gli stakeholder e 2-3 tecnici esperti dell'ambito di progetto della milestone. "PunchCode" richiede pertanto obbligatoriamente la presenza del cliente in questi incontri (ove non sia possibile, è sufficiente un suo referente);
- si presentano le performance fornite dal progetto fino a quel momento;
- si identificano eventuali problemi e si propongono anche azioni correttive.

Come già evidenziato, le attuali ridotte dimensioni della startup potrebbero avere un impatto sulle figure partecipanti.

#### 2.1.2.4. Gestione delle comunicazioni

- L'accettazione di ogni informazione da parte del destinatario (cliente o figura aziendale) avviene esclusivamente per mezzo di feedback scritto in formato elettronico. Il cliente interagisce direttamente col/i Project Manager dell'azienda e a fronte di ogni comunicazione (anche di tipo one-to-one) viene redatto un documento riassuntivo, seguendo uno specifico [template](project_docs/request_acknowledge_template/request_acknowledge_template.md). Questo viene successivamente inviato al richiedente, il quale dovrà rispondere per iscritto confermando o rifiutando il contenuto. In questo modo si cercano di evitare pericolosi scenari che potrebbero essere dettati dalla presenza di una regola di silenzio assenso, da fenomeni di incomprensione o da rinnegamenti. Solo al sopraggiungere della conferma, il documento riassuntivo viene inserito nel workbook e - qualora si tratti di un interrogativo o di una richiesta - preso in carico da parte del Project Manager (scatenando eventualmente ulteriori processi basati su documenti con altri template specifici, come il Project Impact Statement per le richieste di cambiamento di scoping - ad esempio). L'azienda considera pertanto richieste solo all'ottenimento del feedback loro associato.  
Per quanto concerne le comunicazioni interne all'azienda, queste vengono formalizzate solo se rilevanti per il progetto o di interesse (per altri dipendenti, come storico per miglioramento della gestione interna o per progetti futuri) utilizzando lo stesso template. L'azienda tuttavia sollecita i dipendenti a esprimere le proprie idee / osservazioni durante gli Stand-up Meeting approfittando della presenza di tutti gli interessati.

- A fronte di ogni Stand-up Meeting, viene redatta una documentazione scritta soltanto per le attività cui è stata assegnata una colorazione gialla o rossa attraverso lo Spotlight Report da parte del responsabile dello specifico task (concentrandosi sulle sole attività oggetto di scostamenti dal piano o rappresentanti scenari fuori controllo), raccogliendo informazioni motivazionali utili ed evitando di investire tempo nella produzione di comunicazioni scritte per le attività in schedula (verdi). Terminato l'incontro, il documento viene caricato nel repository dell'azienda.

## 2.2. Committente
Il committente è CSEN (Centro Sportivo Educativo Nazionale), un ente di elevate dimensioni operante su tutto il territorio nazionale senza finalità di lucro e avente come obiettivo principale quello di perseguire una propaganda sportiva di alto valore sociale. CSEN contribuisce pertanto allo sviluppo della pratica sportiva e a una sua miglior accessibiltà da parte delle persone, creando le condizioni per una più larga crescita dell'educazione fisica, dello sport stesso e della salute. Collabora inoltre con il C.O.N.I. e le Federazioni Sportive, con la Scuola, con le Regioni e gli Enti Locali, con le forze sociali e politiche e con le libere associazioni di altri Paesi.
Esso è organizzato come segue:
- 1.650.000 Soci Dirigenti, Tecnici, Atleti, Amatori;
- 15.540 Associazioni Sportive A.S.D. / S.S.D.;
- 4.300 Associazioni Sportive (Basi Associative Sportive);
- 2.000 Associazioni Promozione Sociale e Tempo Libero;
- 1.300.000 Tesserati Sportivi;
- 500.000 Tesserati del Tempo Libero;
- 20 Comitati Regionali;
- 106 Comitati Provinciali;
- 25 Comitati di Zona.

Il progetto è stato assegnato da Enrico Comando (nome di fantasia), che ne ricopre anche il ruolo di Project Manager. Enrico Comando è stato scelto poichè qualificato sia in termini di competenze informatiche che di dominio, oltre che dotato di una profonda esperienza nella coordinazione di ulteriori progetti per conto di CSEN - comunque legati a quello che verrà successivamente esposto.

## 2.3. Relazione esecutore-committente
Il committente è alla ricerca di un fornitore innovativo e giovane, puntando sulle startup locali emergenti. Le due parti non si conoscono e non hanno mai collaborato a nessun progetto, ma grazie alla crescente notorietà nel campo di programmazione di "PunchCode", essa è stata presa in considerazione sin da subito come un potenziale appaltatore.

[//]: # (-------------------------------------------------------------------------)

# 3. Scoping
In questa sezione sono riportate tutte le scelte intraprese durante la fase di scoping. Dopo una sintetica spiegazione sul come sia avvenuto il primo contatto, gli argomenti sono proposti in base ai deliverable coinvolti da questo gruppo di processo. Inoltre, è anche discussa l'organizzazione dei meeting (documentando l'ordine del giorno, i partecipanti e una sintesi dell'ipotetico svolgimento).

## 3.1. Primo contatto
Il primo contatto tra il committente e l'esecutore avviene utilizzando la mail aziendale. Il committente, dopo una breve presentazione di CSEN, esprime subito la sua volontà di informatizzare il processo di gestione delle gare di Taekwondo organizzate da CSEN, senza adottare in questa sua richiesta una descrizione di dettaglio. La startup, seguendo le buone pratiche descritte in precedenza, decide di proporre al committente un Project Scoping Meeting, al fine di chiarire tutte le ambiguità e valutare la fattibilità della proposta. In base alla disponibilità del cliente viene stabilito che l'incontro si svolgerà il lunedì 11 marzo, alle ore 09:00, all'interno della sala riunioni di "PunchCode". A rappresentare l'azienda cliente vi sarà il relativo Project Manager: Enrico Comando.

## 3.2. Project Scoping Meeting

Il Project Scoping Meeting costituisce la prima occasione d'incontro tra il fornitore e il committente. Applicando le politiche aziendali, si è svolta una prima sessione seguendo l'agenda disponibile nel relativo [allegato](project_docs/csen_poomsae_score/project_scoping_meeting/session_11_03_19.md).
Tale file è distribuito a tutte le figure aziendali presenti alla riunione e - come è possibile dedurre dal suo contenuto - prevede degli appositi campi "note" compilabili digitalmente al fine di tener traccia delle varie osservazioni emerse in ogni fase di cui il meeting è composto. Prevede inoltre una sezione dedicata alla valutazione dell'incontro e alla pianificazione del successivo.
Nella costruzione dell'agenda descritta nel documento in oggetto si sono effettuate le seguenti considerazioni.
- Non disponendo al momento di un Facilitatore, tale ruolo è ricoperto dal Project Manager aziendale con le soft skill più idonee ai suoi compiti (quali organizzazione, comunicazione ed empatia). Tenendo inoltre conto di come Marcin Pabich sia anche incaricato di riflettere gli interessi di un Architetto (interessandosi più della bellezza della soluzione che del costo a essa associata), si è ritenuto che Giacomo Frisoni fosse il membro più idoneo.
- I tempi relativamente le durate di ogni argomento in agenda sono stimati a partire dal contenuto della mail di contatto pervenuta da CSEN, ricordando tuttavia l'alta probabilità di discostamento a causa della non esperienza di PunchCode.
- Dal momento che la discussione delle Condition of Satisfaction (CoS) non viene fatta in un unico punto, si è scelto di prevedere un'apposita area all'interno del template del documento in cui annotare man mano gli obiettivi del progetto.
- Dato che il cliente può fornire materiale di varia natura all'interno di un meeting, si predispone anche un'apposita sezione in cui tener traccia dei riferimenti a quanto fornito.
- La compilazione digitale del documento è stata scelta per diverse ragioni:
  - facilita un eventuale processamento automatico delle informazioni in esso contenute;
  - velocizza il processo di annotazione (anche considerando come un membro dello staff aziendale sia frequentemente impegnato nel dirigire la discussione)
  - rende il contenuto del documento maggiormente fruibile da parte di tutti gli interessati.

Un esempio di documento compilato per quanto concerne la prima sessione è disponibile nel seguente [allegato](project_docs/csen_poomsae_score/project_scoping_meeting/session_11_03_19_marcin_pabich.md).

A causa della complessità del progetto, durante il primo incontro si è subito manifestata la necessità di pianificarne altri. Nello specifico, riconoscendo la presenza di vari sottosistemi, si è pertanto preferito organizzare un meeting per entrare nei dettagli di ciascuno di questi (sollecitando di volta in volta la partecipazione delle figure coinvolte lato committente da parte di quel sottosistema) e limitarsi con la prima riunione a inquadrare il problema solo in termini generali. Tenendo conto di come il cliente abbia manifestato fin da subito la sua disponibilità a più incontri nell'arco di una settimana, l'elenco delle successive sessioni svolte è di seguito riportato (specificando per ognuna data e agenda):

 - 14/03/2019 - [agenda per il sottosistema dedicato ai tablet dei giudici](project_docs/csen_poomsae_score/project_scoping_meeting/session_14_03_19.md)  
 - 18/03/2019 - [agenda per il sottosistema dedicato al software per la gestione di un quadrato di gara](project_docs/csen_poomsae_score/project_scoping_meeting/session_18_03_19.md)  
 - 22/03/2019 - [agenda per il sottosistema dedicato alla gestione di un torneo lato server](project_docs/csen_poomsae_score/project_scoping_meeting/session_22_03_19.md)  

Nell'intervallo di tempo compreso tra una sessione e la successiva, PunchCode si impegna anche alla realizzazione di mockup, sia per quanto riguarda i [tablet](project_docs/csen_poomsae_score/project_scoping_meeting/session_14_03_19), sia per i [computer](project_docs/csen_poomsae_score/project_scoping_meeting/session_18_03_19) (sottoposti al giudizio del committente tramite email).

Dopo aver discusso nel dettaglio di ogni sottosistema (comprendendo problematiche, desiderata e modalità di raccolta dei requisiti), si è infine pianificato un ultimo meeting (successivo all'applicazione delle tecniche finalizzate alla raccolta dei requisiti, alla classificazione del progetto e all'identificazione dei rischi) per la scelta del PMLC Model (descritta nella [prossima sezione](#34-scelta-del-pmlc-model)) che meglio si adattasse alla chiusura del gap individuato (tenendo chiaramente conto anche della disponibilità del cliente). In questa occasione si è anche effettuata la stesura di una bozza del POS (con relativa approvazione):

 - 01/04/2019 - [agenda del meeting conclusivo per la definizione dello scope](project_docs/csen_poomsae_score/project_scoping_meeting/session_01_04_19.md)

Per quanto concerne il budget e la durata del progetto, si è prevista una discussione iniziale di questi aspetti - condotta da parte del Project Manager del cliente - già all'interno della prima sessione (in modo tale da non considerare nemmeno la pianificazione delle riunioni successive in assenza delle condizioni per farlo). Si osserva inoltre come si sia organizzata un'ulteriore e analoga discussione di questi temi all'interno dell'ultima sessione, condotta però da parte del Project Manager dell'azienda (ora consapevole di tutti i dettagli del progetto e in grado di fare una reale valutazione dal suo punto di vista).

Unendo tutte le informazioni raccolte sui bisogni del cliente, il documento di descrizione dell'intero progetto è disponibile al seguente [allegato](project_docs/csen_poomsae_score/project_scoping_meeting/project_description.md).

## 3.3. Resources Breakdown Structure (RBS)

### 3.3.1. Raccolta dei requisiti

In ogni Project Scoping Meeting dedicato a uno specifico sottosistema, si sono discusse e definite le modalità di acquisizione dei relativi requisiti (con approcci ulteriori alla singola riunione). Dopo un'attenta analisi, considerando la disponibilità manifestata dal cliente, si è deciso di optare per **Interviste** e **Osservazioni**. Altri metodi, come il "Requirements Reuse" e il "Prototyping" non sono stati adottati dal momento che non si verificano le condizioni necessarie alla loro attuazione (l'azienda non ha esperienza su progetti precedenti da cui riprendere parte di implementazione e la realizzazione di un prototipo si rivela eccessivamente costosa e rischiosa).

#### 3.3.1.1 Interviste
Al fine di avere una descrizione dei processi e delle problematiche attuali direttamente da chi li gestisce, si è ritenuto opportuno prevedere *tre interviste*: due per gli addetti responsabili alle gestione dei quadrati e una per il gestore del server.

Essendo "PunchCode" formata da due soli membri, per compensare l'assenza di un analista interno all'azienda, viene presa la decisione di far rivestire il ruolo di intervistatore a entrambi i membri (formulando e sottoponendo le domande agli intervistati in coppia). Questa scelta va anche nella direzione di ridurre il rischio di un'interpretazione errata delle risposte, nonostante si sia consapevoli che un simile approcio potrebbe scoraggiare l'intervistato ad esprimersi in piena libertà.

Un ulteriore motivo che ha portato alla scelta di questo metodo è da ricercarsi nel fatto che l'esecutore non ha mai condotto progetti antecedenti simili a quello in esame. Di conseguenza potrebbe per lui risultare difficile dedurre ciò di cui il committente ha bisogno solamente attraverso le discussioni svolte durante i meeting.

L'intervistato potrebbe distorcere la realtà, avere difficoltà a esprimersi o, in preda ad agitazione, fornire informazioni poco precise.
Una possibile soluzione a questo problema consiste normalmente nell'adozione di un approccio deduttivo, chiamato "ad imbuto".
L'intervistatore parte da domande molto generali per poi restringere l'argomento dell'intervista a temi specifici. Il carattere generale dei quesiti iniziali (normalmente in forma aperta), infatti, allieva la tensione dell'intervistato (che potrebbe altrimenti essere emozionato o eccessivamente deferente).

Per la definizione delle domande legate a ogni intervista, inoltre, si è ritenuto fondamentale tener conto della posizione ricoperta e delle mansioni svolte dell'intervistato (ricercando sempre un focus preciso).

Un esempio di intervista realizzata da "PunchCode" al gestore del sistema software dedicato ai quadrati di gara è disponibile al seguente [allegato](project_docs/csen_poomsae_score/rbs/interview_26_03_19.md).

#### 3.3.1.2 Osservazioni
Per risolvere ulteriormente i tipici problemi di un'intervista, si è scelto di integrare quest'ultima con un'osservazione. Questo ulteriore approccio è molto educativo e permette di comprendere al meglio il modo di lavorare del cliente, dimostrandosi di conseguenza utile per rilevare requisiti del sistema che altrimenti rischierebbero di non emergere da domande.  

Grazie agli accordi presi durante i meeting, i membri di "PunchCode" hanno così potuto partecipare direttamente a una delle gare svolte dallo CSEN.

### 3.3.2. Costruzione
Al fine di esprimere all'utente in maniera chiara, intuitiva e significativa i requsiti raccolti, si è scelto di costruire un RBS, in linea con le buone pratiche del PMBOK proposto da PMI. Nel far ciò, si è prestata attenzione nel non definire attività con una granularità troppo fine (che avrebbe altrimenti portato ad alti costi in fase di monitoraggio e controllo).   

Nella stestura dell'[RBS](project_docs/csen_poomsae_score/rbs/rbs.png), "PunchCode" ha ritenuto opportuno affrontare la decomposizione gerarchica dei requisiti tenendo conto di tre macro-aree (rappresentanti i tre principali sottosistemi del progetto).

#### 3.3.2.1 App Android
È il sottosistema incentrato sullo sviluppo dell'applicazione Android per la registrazione dei punteggi associati alle poomsae da parte dei giudici.

- *Registrazione Punteggio*  
  Deve essere possibile registrare il punteggio per una determinata poomsae, attraverso step successivi e tenendo conto di parametri diversi.
  
- *Invio Punteggio*  
  Il punteggio calcolato dal giudice necessita - qualora ci si trovi in modalità online - di essere inviato al software per la gestione del quadrato di gara. 

- *Storico*  
  Si deve mantenere traccia di tutti i punteggi registrati attraverso l'uso dell'applicazione.

- *Impostazioni*  
  L'applicazione deve prevedere un'area dedicata al settaggio di impostazioni di utilità.

#### 3.3.2.2 Software Gestione Quadrato
È il sottosistema incentrato sullo sviluppo della soluzione software atta a gestire i tornei all'interno di un quadrato.

- *Ricezione Tornei*  
  Ogni quadrato, all'inizio di una competizione, riceve una serie di tornei da gestire (sulla base della decomposizione realizzata dal server).

- *Selezione Torneo*  
  Prima di procedere alla selezione degli alteti, è necessario selezionare il torneo dal quale sceglierli.

- *Gestione Torneo*  
  Prevede la gestione delle singole poomsae nelle diverse **gare** e il mantenimento in forma permanente dei dati acquisiti (**salvataggio**).

- *Visualizzazione*
  I dati acquisiti dai quadrati devono essere visualizzati al pubblico su appositi monitor.

#### 3.3.2.3 Server  
È il sottosistema software rappresentante la parte centrale nella gestione di competizioni. Esso consente di crearle e configurarle, oltre che gestirle una volta inizializzate.

- *Configurazione Competizione*  
  Prima di essere operativa, la competizione dev'essere opportunamente *configurata*. La configurazione avviene attraverso due macro-fasi:
  
  - *Creazione*, stabilendo i parametri generici della competizione stessa e importando i dati degli atleti dall'apposito file;
  
  - *Aggiornamento*, consentendo la *manipolazione dei tornei* interni alla competizione nei momenti antecedenti alla sua inizializzazione e il *partizionamento* sul piano gestionale dei tornei definiti ai vari software di quadrato.

- *Inizializzazione Competizione*  
  Dopo averla opportunamente configurata, la competizione può essere avviata. Durante tutta la sua durata, il server rimane in ascolto sull'avanzamento di stato di ogni singolo torneo (*raccogliendo sia i punteggi legati alle varie poomsae che le classifiche locali al termine di ogni torneo*). Questo processo permette di elaborare la classifica globale delle singole palestre.

- *Gestione Salvataggio*  
  Procedura permettente di mantenere integro e recuperabile lo stato e l'avanzamento dell'intera competizione.

- *Visualizzazione*  
  Il server è connesso ad un monitor, consentendo al pubblico sia di consultare informazioni generali legate ai quadrati di gara che i risultati ottenuti a partire dai dati raccolti.

## 3.4. Scelta del PMLC Model

Per quanto riguarda la scelta del modello per il ciclo di vita del progetto, i Project Manager di "PunchCode" hanno deciso - dopo un'attenta analisi - di adottare una modalità **incrementale**. Le principali ragioni che hanno portato a questa scelta scaturiscono direttamente dalle caratteristiche del progetto stesso e dalle esigenze del cliente:
- i requisiti sono stati chiaramente definiti (così come le loro priorità);
- non sono previste modifiche rilevanti allo scope (anche se ci sono delle probabilità che ciò accada);
- il cliente desidera ricevere business value presto e con una certa frequenza.

Dal momento che vi è una qualche probabilità che lo scope subisca delle modifiche, un approccio incrementale fornisce della flessibilità per accettare cambiamenti di scope (che comunque dovrebbero essere molto ridotti). L'identificazione di più sottosistemi interni al progetto, inoltre, favorisce il progressivo rilascio di incrementi usabili da parte dell'utente.

Si sono immaginate tre major-release, considerando i sottosistemi identificati, le dipendenze tra loro e le priorità assegnate da parte del committente. Oltre a queste, vengono previsti anche dei rilasci incrementali minori, a scopo di ottenere man mano un diretto riscontro dal cliente (che nel corso delle sessioni del Project Scoping Meeting ha manifestato più volte la sua disponibilità a essere contattato per il rilascio di feedback).

## 3.5. Budget e tempi
Durante l'ultima sessione del Project Scoping Meeting si è arrivati al compromesso di 8000€ e un tempo di realizzazione pari ad un anno. Sotto quest'ultimo punto di vista si tenga presente come si sia scelto di ricorrere ad un modello incrementale, garantendo di conseguenza al cliente rilasci graduali e continui durante questo arco temporale. Il tempo e budget qui discussi tengono anche conto delle operazioni di installazione, manutenzione, monitoraggio e formazione del personale.

## 3.6. Project Overview Statement (POS)
Ottenuta a fronte di un ulteriore raffinamento della bozza approvata con l'ultima sessione di Project Scoping Meeting.

[//]: # (Spiegare la scelta di mettere il Glossiario nel POS)

## 3.7. Project Definition Statement (PDS)

### 3.7.1. Analisi dei rischi
Spiegare il perchè dell'uso di un diagramma rispetto a un altro.

# 4. Planning

- *Applicazione Android*.  
Per automatizzare la valutazione delle poomsae svolte dagli atleti da parte dei giudici.

- *Software per la gestione del quadrato di gara abbinato all'applicazione Android*.  
Per la gestione dei tornei interni a una competizione su un quadrato di gara e la raccolta dei punteggi da parte delle applicazioni in esecuzione sui tablet dei giudici, anticipando alcune funzionalità lato server (importazione dati da file Excel, creazione della competizione, gestione dei trasferimenti ed elaborazione classifica globale localmente al quadrato).

- *Sistema software completo*  
Per l'integrazione del server, spostando la configurazione delle competizioni su un unico nodo, gestendo il partizionamento dei tornei tra i vari quadrati al fine di evitare sovrapposizioni e raccogliendo i dati elaborati da ogni software di gestione di quadrato.

Si vuole sottolineare come - per garantire i rilasci intermedi di cui il committente necessita - si sia scelto di anticipare funzionalità di sottosistemi ancora non realizzati (con la consapevolezza che ciò richieda un ulteriore lavoro in termini di modifiche e integrazione).

# 5. Bibliografia

[1]<a id="bibliography-1"></a> [Platonova, Valērija & Bērziša, Solvita. "Gamification in Software Development Projects". *Information Technology and Management Science*. Dec 2017.](https://www.researchgate.net/publication/322409704_Gamification_in_Software_Development_Projects)  
[2]<a id="bibliography-1"></a> [Senthil Rajamarthandan. "Using Gamification to Build a Passionate and Quality-Driven Software Development Team". *Cognizant 20-20 Insights*. Feb 2014.](https://www.cognizant.com/InsightsWhitepapers/Using-Gamification-to-Build-a-Passionate-and-Quality-Driven-Software-Development-Team.pdf)