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
  - [3.7. Classificazione del progetto](#37-Classificazione-del-progetto)
  - [3.8. Scelta del Core Team](#38-Scelta-del-Core-Team)
- [4. Planning](#4-Planning)
  - [4.1 Joint Project Planning Session](#41-Joint-Project-Planning-Session)
    - [4.1.1 Sessione #1](#411-Sessione-1)
    - [4.1.2 Sessione #2](#412-Sessione-2)
    - [4.1.3 Sessione #3](#413-Sessione-3)
  - [4.2 Prioritizzazione dei requisiti](#42-Prioritizzazione-dei-requisiti)
  - [4.3 Work Breakdown Structure (WBS)](#43-Work-Breakdown-Structure-WBS)
  - [4.4 Stima delle risorse necessarie](#44-Stima-delle-risorse-necessarie)
    - [4.4.1 Valutazione delle skill richieste dai task](#441-Valutazione-delle-skill-richieste-dai-task)
    - [4.4.2 Assegnamento membri dello staff ai task](#442-Assegnamento-membri-dello-staff-ai-task)
    - [4.5 Stima della durata dei task](#45-Stima-della-durata-dei-task)
    - [4.6 Stima dei costi](#46-Stima-dei-costi)
  - [4.7 Diagramma di Gantt](#47-Diagramma-di-Gantt)
  - [4.8 Diagramma di PERT](#48-Diagramma-di-PERT)
  - [4.9 Analisi dei Rischi](#49-Analisi-dei-Rischi)
  - [4.10 Project Definition Statement (PDS)](#410-Project-Definition-Statement-PDS)
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
- **GitHub Desktop** per la gestione del repository.
  
<!--- **TeXstudio** per la generazione di parte della documentazione tramite il linguaggio LaTeX;-->

[//]: # (-------------------------------------------------------------------------)

# 2. Introduzione
In questa sezione sono fornite informazioni di carattere generale relative all'esecutore e al committente. Viene analizzato il rapporto tra queste due entità, con lo scopo di fornire una larga veduta sull'intera struttura su cui il progetto si basa e di comprendere le ragioni che hanno portato a intraprendere determinate scelte a discapito di altre. Si illustrano inoltre le competenze dei singoli membri facenti parte del team dell'azienda fornitrice, scendendo anche nel dettaglio delle politiche aziendali.

## 2.1. Azienda esecutrice
L'esecutore del progetto è la startup "**PunchCode**". Essa è un'azienda informatica specializzata nella costruzione di soluzioni software, composta da due soli dipendenti neo-laureati. Essendosi appena costituita, non presenta esperienza pregressa in altri progetti e conseguentemente non possiede un know-how in alcuna area di mercato. Considerando l'esiguo numero di persone interne all'azienda, quest'ultima non è al momento decomposta in specifiche aree funzionali sul piano organizzativo; tuttavia è in espansione e prevede l'acqusizione nel breve termine di nuovo personale con competenze tecniche specializzate. Il principale motivo per cui l'azienda è stata scelta dal committente, oltre ad aver presentato un'offerta più aggressiva rispetto ai principali concorrenti, è da ricercarsi nella sua propensione all'uso di tecnologie innovative che l'hanno portata ad acquisire un'indubbia fama sul territorio e a ottenere un alto livello di attenzione sul panorama mediatico per mezzo dell'incubatore nel quale è localizzata.

### 2.1.1. Startup Team

PunchCode è formata da due soli membri ricoprenti entrambi il ruolo di Project Manager. Le competenze di ogni dipendente sono tracciate dall'azienda all'interno di un apposito [documento](project_docs/startup_team_skills/startup_team_skills.md), tenendo conto sia di *pre skill* (o soft skill) che di *pro skill* (o hard skill). Le prime si riferiscono alle capacità inerenti alla sfera interpersonale e della comunicazione, indipendenti dalla specifica mansione lavorativa e pertanto trasversali. Le seconde sono quelle competenze tecniche relative allo svolgimento di una certa professione, acquisibili tramite lo studio e certificabili. Nell'ottica di andare a delineare un valido strumento di appoggio per un Project Manager ai fini della futura assegnazione delle attività ai membri dello staff in fase di Planning, si è infatti ritenuto utile includere la valutazione di ambo le tipologie di abilità. Per quanto concerne l'assegnazione dei punteggi, si è voluta considerare una scala di valori numerici adimensionali compresa tra 1 e 5 (preferendola ad alternative misure non numeriche che avrebbero impedito la valutazione delle competenze in media di tutto il team su un certo parametro).

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
Al fine di motivare gli impiegati e rendere le loro attività quotidiane meno frustranti nella loro percezione, PunchCode si avvale di tecniche di Gamification all'interno dei propri progetti di sviluppo software di durata massima stimata non superiore ai 5 mesi. Questa scelta è frutto di approfondite [ricerche in letteratura](#bibliography-1)<sup>1</sup> che testimoniano come esse influenzino positivamente i risultati di un gruppo di lavoro.  
PunchCode - sotto questo punto di vista - si avvale di un proprio sistema di login per il tracciamento delle attività compiute dai dipendenti, premiandoli con dei *punti* (come componente di gioco) in caso di:
- lettura di codice / documentazione di colleghi con invio di feedback (in forma di rating);
- ricezione di feedback positivi da parte di un collega.

L'uso di una metodologia di questo tipo porta a diversi vantaggi:
- stimola i dipendenti a revisionare il lavoro realizzato dagli altri;
- abilita una forma di trasferimento di conoscenza a partire da esempi positivi forniti dai colleghi.

##### 2.1.2.2.2. Documentazione

- **Sviluppo**  
PunchCode riversa sulla documentazione un ruolo di primaria importanza per numerose ragioni (tra cui riusabilità, manutenibilità, condivisione e storico sia in termini di problematiche che di soluzioni).
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

PunchCode considera lo svolgimento di Problem Resolution Meeting per la discussione di problematiche riscontrate durante lo svolgimento di un progetto. L'azienda prevede nello specifico che questi siano organizzati qualora si ritengano necessari a fronte dell'individuazione di attività fuori controllo durante uno Stand-up Meeting. In queste riunioni per la risoluzione di un problema l'agenda deve prevedere:
- la partecipazione dei soli sviluppatori coinvolti nel problema;
- la determinazione del/i proprietario/i (owner) del problema (potenzialmente molteplici da punti di vista diversi);
- l'identificazione della soluzione;
- la determinazione delle modalità (come e quando) attraverso cui stabilire che il problema è da considerarsi risolto.

Preme tuttavia sottolineare come - a causa del ridotto personale attualmente presente nella startup - tali meeting richiedano necessariamente la presenza di entrambi i membri.

##### 2.1.2.3.4. Project Review Meeting

In concomitanza col raggiungimento di una milestone, l'azienda svolge un Project Review Meeting. Durante questi eventi formali:
- si svolge la presentazione dello stato del progetto in corrispondenza della milestone e si effettua una sua revisione critica;
- partecipano il project manager, il senior management, lo sponsor, il committente, gli stakeholder e 2-3 tecnici esperti dell'ambito di progetto della milestone. PunchCode richiede pertanto obbligatoriamente la presenza del cliente in questi incontri (ove non sia possibile, è sufficiente un suo referente);
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
Il committente è alla ricerca di un fornitore innovativo e giovane, puntando sulle startup locali emergenti. Le due parti non si conoscono e non hanno mai collaborato a nessun progetto, ma grazie alla crescente notorietà nel campo di programmazione di PunchCode, essa è stata presa in considerazione sin da subito come un potenziale appaltatore.

[//]: # (-------------------------------------------------------------------------)

# 3. Scoping
In questa sezione sono riportate tutte le scelte intraprese durante la fase di scoping. Dopo una sintetica spiegazione sul come sia avvenuto il primo contatto, gli argomenti sono proposti in base ai deliverable coinvolti da questo gruppo di processo. Inoltre, è anche discussa l'organizzazione dei meeting (documentando l'ordine del giorno, i partecipanti e una sintesi dell'ipotetico svolgimento).

## 3.1. Primo contatto
Il primo contatto tra il committente e l'esecutore avviene utilizzando la mail aziendale. Il committente, dopo una breve presentazione di CSEN, esprime subito la sua volontà di informatizzare il processo di gestione delle gare di Taekwondo organizzate da CSEN, senza adottare in questa sua richiesta una descrizione di dettaglio. La startup, seguendo le buone pratiche descritte in precedenza, decide di proporre al committente un Project Scoping Meeting, al fine di chiarire tutte le ambiguità e valutare la fattibilità della proposta. In base alla disponibilità del cliente viene stabilito che l'incontro si svolgerà il lunedì 11 marzo, alle ore 09:00, all'interno della sala riunioni di PunchCode. A rappresentare l'azienda cliente vi sarà il relativo Project Manager: Enrico Comando.

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

Nell'intervallo di tempo compreso tra una sessione e la successiva, PunchCode si impegna anche alla realizzazione di mockup (sottoposti al giudizio del committente tramite email), sia per quanto riguarda [l'applicazione Android](project_docs/csen_poomsae_score/project_scoping_meeting/session_14_03_19_res/mockup) in esecuzione sui tablet dei giudici, sia per i [software di gestione del quadrato di gara](project_docs/csen_poomsae_score/project_scoping_meeting/session_18_03_19_res/mockup) per i computer in dotazione.

Dopo aver discusso nel dettaglio di ogni sottosistema (comprendendo problematiche, desiderata e modalità di raccolta dei requisiti), si è infine pianificato un ultimo meeting (successivo all'applicazione delle tecniche finalizzate alla raccolta dei requisiti, alla classificazione del progetto e all'identificazione dei rischi) per la scelta del PMLC Model (descritta nella [prossima sezione](#34-scelta-del-pmlc-model)) che meglio si adattasse alla chiusura del gap individuato (tenendo chiaramente conto anche della disponibilità del cliente). In questa occasione si è anche effettuata la stesura di una bozza del POS (con relativa approvazione):

 - 01/04/2019 - [agenda del meeting conclusivo per la definizione dello scope](project_docs/csen_poomsae_score/project_scoping_meeting/session_01_04_19.md)

Per quanto concerne il budget e la durata del progetto, si è prevista una discussione iniziale di questi aspetti - condotta da parte del Project Manager del cliente - già all'interno della prima sessione (in modo tale da non considerare nemmeno la pianificazione delle riunioni successive in assenza delle condizioni per farlo). Si osserva inoltre come si sia organizzata un'ulteriore e analoga discussione di questi temi all'interno dell'ultima sessione, condotta però da parte del Project Manager dell'azienda (ora consapevole di tutti i dettagli del progetto e in grado di fare una reale valutazione dal suo punto di vista).

Unendo tutte le informazioni raccolte sui bisogni del cliente, il documento di descrizione dell'intero progetto è disponibile al seguente [allegato](project_docs/csen_poomsae_score/project_scoping_meeting/project_description.md).

## 3.3. Resources Breakdown Structure (RBS)

### 3.3.1. Raccolta dei requisiti

In ogni Project Scoping Meeting dedicato a uno specifico sottosistema, si sono discusse e definite le modalità di acquisizione dei relativi requisiti (con approcci ulteriori alla singola riunione). Dopo un'attenta analisi, considerando la disponibilità manifestata dal cliente, si è deciso di optare per **Interviste** e **Osservazioni**. Altri metodi, come il "Requirements Reuse" e il "Prototyping" non sono stati adottati dal momento che non si verificano le condizioni necessarie alla loro attuazione (l'azienda non ha esperienza su progetti precedenti da cui riprendere parte di implementazione e la realizzazione di un prototipo si rivela eccessivamente costosa e rischiosa).

#### 3.3.1.1 Interviste
Al fine di avere una descrizione dei processi e delle problematiche attuali direttamente da chi li gestisce, si è ritenuto opportuno prevedere *tre interviste*: due per gli addetti responsabili alle gestione dei quadrati e una per il gestore del server.

Essendo PunchCode formata da due soli membri, per compensare l'assenza di un analista interno all'azienda, viene presa la decisione di far rivestire il ruolo di intervistatore a entrambi i membri (formulando e sottoponendo le domande agli intervistati in coppia). Questa scelta va anche nella direzione di ridurre il rischio di un'interpretazione errata delle risposte, nonostante si sia consapevoli che un simile approcio potrebbe scoraggiare l'intervistato ad esprimersi in piena libertà.

Un ulteriore motivo che ha portato alla scelta di questo metodo è da ricercarsi nel fatto che l'esecutore non ha mai condotto progetti antecedenti simili a quello in esame. Di conseguenza potrebbe per lui risultare difficile dedurre ciò di cui il committente ha bisogno solamente attraverso le discussioni svolte durante i meeting.

L'intervistato potrebbe distorcere la realtà, avere difficoltà a esprimersi o, in preda ad agitazione, fornire informazioni poco precise.
Una possibile soluzione a questo problema consiste normalmente nell'adozione di un approccio deduttivo, chiamato "ad imbuto".
L'intervistatore parte da domande molto generali per poi restringere l'argomento dell'intervista a temi specifici. Il carattere generale dei quesiti iniziali (normalmente in forma aperta), infatti, allieva la tensione dell'intervistato (che potrebbe altrimenti essere emozionato o eccessivamente deferente).

Per la definizione delle domande legate a ogni intervista, inoltre, si è ritenuto fondamentale tener conto della posizione ricoperta e delle mansioni svolte dell'intervistato (ricercando sempre un focus preciso).

Un esempio di intervista realizzata da PunchCode al gestore del sistema software dedicato ai quadrati di gara è disponibile al seguente [allegato](project_docs/csen_poomsae_score/rbs/interview_26_03_19.md).

#### 3.3.1.2 Osservazioni
Per risolvere ulteriormente i tipici problemi di un'intervista, si è scelto di integrare quest'ultima con un'osservazione. Questo ulteriore approccio è molto educativo e permette di comprendere al meglio il modo di lavorare del cliente, dimostrandosi di conseguenza utile per rilevare requisiti del sistema che altrimenti rischierebbero di non emergere da domande.  

Grazie agli accordi presi durante i meeting, i membri di PunchCode hanno così potuto partecipare direttamente a una delle gare svolte dallo CSEN.

### 3.3.2. Costruzione
Al fine di esprimere all'utente in maniera chiara, intuitiva e significativa i requsiti raccolti, si è scelto di costruire un RBS, in linea con le buone pratiche del PMBOK proposto da PMI. Nel far ciò, si è prestata attenzione nel non definire attività con una granularità troppo fine (che avrebbe altrimenti portato ad alti costi in fase di monitoraggio e controllo).   

Nella stestura dell'[RBS](project_docs/csen_poomsae_score/rbs/rbs.png), PunchCode ha ritenuto opportuno affrontare la decomposizione gerarchica dei requisiti tenendo conto di tre macro-aree (rappresentanti i tre principali sottosistemi del progetto).

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
  
  - *Creazione*, stabilendo i parametri generici (anagrafica) della competizione stessa e importando i dati degli atleti dall'apposito file;
  
  - *Aggiornamento*, consentendo la *manipolazione dei tornei* interni alla competizione nei momenti antecedenti alla sua inizializzazione e il *partizionamento* sul piano gestionale dei tornei definiti ai vari software di quadrato.

- *Inizializzazione Competizione*  
  Dopo averla opportunamente configurata, la competizione può essere avviata. Durante tutta la sua durata, il server rimane in ascolto sull'avanzamento di stato di ogni singolo torneo (*raccogliendo sia i punteggi legati alle varie poomsae che le classifiche locali al termine di ogni torneo*). Questo processo permette di elaborare la classifica globale delle singole palestre.

- *Gestione Salvataggio*  
  Procedura permettente di mantenere integro e recuperabile lo stato e l'avanzamento dell'intera competizione.

- *Visualizzazione*  
  Il server è connesso ad un monitor, consentendo al pubblico sia di consultare informazioni generali legate ai quadrati di gara che i risultati ottenuti a partire dai dati raccolti.

## 3.4. Scelta del PMLC Model

Per quanto riguarda la scelta del modello per il ciclo di vita del progetto, i Project Manager di PunchCode hanno deciso - dopo un'attenta analisi - di adottare una modalità **incrementale**. Le principali ragioni che hanno portato a questa scelta scaturiscono direttamente dalle caratteristiche del progetto stesso e dalle esigenze del cliente:
- i requisiti sono stati chiaramente definiti (così come le loro priorità);
- non sono previste modifiche rilevanti allo scope (anche se ci sono delle probabilità che ciò accada);
- il cliente desidera ricevere business value presto e con una certa frequenza.

Dal momento che vi è una qualche probabilità che lo scope subisca delle modifiche, un approccio incrementale fornisce della flessibilità per accettare cambiamenti di scope (che comunque dovrebbero essere molto ridotti). L'identificazione di più sottosistemi interni al progetto, inoltre, favorisce il progressivo rilascio di incrementi usabili da parte dell'utente.

Si sono immaginate tre major-release, considerando i sottosistemi identificati, le dipendenze tra loro e le priorità assegnate da parte del committente. Oltre a queste, vengono previsti anche dei rilasci incrementali minori, a scopo di ottenere man mano un diretto riscontro dal cliente (che nel corso delle sessioni del Project Scoping Meeting ha manifestato più volte la sua disponibilità a essere contattato per il rilascio di feedback).

## 3.5. Budget e tempi
Durante l'ultima sessione del Project Scoping Meeting si è arrivati al compromesso di 8000€ e un tempo di realizzazione pari ad un anno. Sotto quest'ultimo punto di vista si tenga presente come si sia scelto di ricorrere ad un modello incrementale, garantendo di conseguenza al cliente rilasci graduali e continui durante questo arco temporale. Il tempo e budget qui discussi tengono anche conto delle operazioni di installazione, manutenzione, monitoraggio e formazione del personale.

## 3.6. Project Overview Statement (POS)

La stesura della bozza del [POS](project_docs/csen_poomsae_score/pos/pos.md) è stata fatta iterativamente (assieme al raffinamento delle Condition of Satisfaction e del RBS), con l'avanzare delle sessioni di Project Scoping Meeting (giungendo infine alla sua approvazione). Esso rappresenta una dichiarazione generale che descrive sinteticamente in cosa consiste il progetto, fungendo da riferimento per il team di pianificazione e costituendo un valido aiuto per le decisioni riguardanti il progetto stesso. È infatti utilizzato come nulla osta a procedere con la pianificazione.  

Gli aspetti principali che si sono considerati per la creazione del documento sono di seguito riportati.
- Chiarire cosa è incluso nel progetto e cosa invece non lo è (delineando pertanto obiettivi necessari e sufficienti).

- Includere solo gli elementi di interesse ai fini dell'approvazione, rimandando gli aspetti specifici e di dettaglio al PDS.

- Prestare attenzione a specificare dei sucess criteria strettamente correlati al business value (IR - Increase Revenue, AC - Avoid Costs, IS - Improve Service) e ben misurabili (facendo esclusivamente uso di metriche quantitative):
  - per definire dei KPI, attraverso cui misurare il raggiungimento di un business value, si è optato anche per l'utilizzo di diverse tabelle comparative;
  - ogni tabella confronta i risultati forniti dal cliente durante la fase di Project Scoping Meeting (relativamente la situazione attuale oggetto del problema) con quelli posti come obiettivo di miglioramento;
  - dal momento che non è realistico ipotizzare che tutti i tempi a seguito dell'introduzione del sistema software rispecchino sempre quelli attesi, si è scelto di quantificare non solo il tempo medio desiderato, ma anche il massimo tempo accettabile e la massima deviazione standard (come misura di dispersione dei dati temporali rispetto alla media aritmetica). La deviazione standard (o scarto quadratico medio), infatti, possiede il vantaggio - rispetto alla varianza - di avere la stessa unità di misura dei valori osservati;
  - poichè si prevede che i singoli obiettivi possano essere soddisfatti con un graduale rilascio delle major-release, si è specificato per ciascuno di essi il momento da cui si prevede di poterne trarre beneficio.
  
- Mostrare solo i rischi più importanti che si sono individuati e quantificati già alla fine della fase di scoping, che potrebbero portare PunchCode a scegliere di non continuare il progetto.
  
- Inserire un glossario al fine di evitare ambiguità e chiarire i principali concetti di dominio.

## 3.7. Classificazione del progetto
Al fine di avere una prima indicazione dell'overhead (ovvero del tempo di gestione da dedicare al progetto), si è realizzata anche una classificazione di Csen Poomsae Score. Per far ciò, PunchCode si appoggia a un proprio [template](project_docs/project_classification/project_classification.md), basandosi su caratteristiche quali durata in ordine di grandezza, classe di rischio, livello di complessità (determinato, ad esempio, dal numero di persone che vi lavorano e dal conseguenziale bisogno di comunicazione), tecnologia impiegata e probabilità di problemi.
Tale classificazione è svolta con la partecipazione di entrambi i dipendenti di PunchCode (che rappresentano sia i Project Manager - con l'impersonificazione da parte di uno del ruolo di Architetto, che il team). Si osserva quindi come la sua funzione sia anche quella di comprendere se valga la pena approfondire o meno (dal momento che anche tale operazione ha un costo).

Nonostante si sia classificato il progetto con un rischio medio-alto (tipo B), PunchCode decide comunque di assumersi il rischio di proseguirlo nella sua gestione, considerando questa opportunità come base per lanciarsi in un nuovo mercato ed acquisire esperienza (know how).

## 3.8. Scelta del Core Team
Una volta conclusa la fase di Scoping (raggiunti e consolidati tutti i suoi deliverable) - prima di iniziare il Planning - è necessario definire i membri del Core Team (o addirittura di tutto il team, ove possibile) per il progetto. Questo passaggio è molto importante dal momento che la partecipazione del Core Team alla fase di pianificazione sarà fondamentale per il successo del progetto. Dato che sarà poi impegnato nell'esecuzione del progetto stesso, infatti, il suo contributo sarà fondamentale nella stima della durata delle attività e nella previsione delle risorse necessarie.  
Disponendo di due soli dipendenti, questa fase si rivela automatica per PunchCode che è costretta a scegliere sotto questo punto di vista entrambe le sue risorse: Giacomo Frisoni e Marcin Pabich.  
Si sottolinea comunque come, disponendo di più personale, tale decisione possa cambiare in progetti futuri (andando a selezionare solo le figure maggiormente motivate, flessibili, con esperienza, abili nel rispettare i tempi e i vincoli previsti, con responsabilità frammentata, propense a concedere fiducia e supporto reciproco, team-oriented, open-minded e con capacità nell'utilizzo di strumenti - anche software - per il Project Management).  

# 4. Planning

Un corretto svolgimento della fase di Scoping non è sufficiente: con esso si sa il *cosa* fare, ma non si conosce ancora le attività (che richiedono l'aver stabilito il *come*) e i tempi stimati per la loro realizzazione. Oltre che per la definizione del calendario delle attività, il Planning rappresenta anche un'ulteriore occasione per verificare la piena comprensione del progetto. Durante l'approfondimento delle attività, infatti, potrebbero venir fuori aspetti tralasciati o errati al momento della definizione del *cosa* (portando alla estensione o alla modifica sia del RBS che del POS).

Come evidenziato dalla "*pain curve*" descritta da Wysocki, la pianificazione costituisce un processo frustrante e richiedente tempo, ma va nella direzione di evitare l'insorgere di problemi, panico e risorse fuori controllo (che potrebbero rappresentare un alto rischio di non convergenza con la fine del progetto). Faticare pertanto nella sua realizzazione all'inizio del progetto, serve per evitare la formazione di difficoltà in seguito.

La fase di Planning è, quindi, di primaria importanza per il buon esito di un progetto e consente di:
- ridurre l'incertezza, dal momento che con la presenza di un piano si sa cosa accadrà in seguito;
- aumentare la comprensione, facendo domande e comprendendo in misura maggiore cosa il cliente vuole;
- migliorare l'efficienza, facendo sì che ogni membro del team sia a conoscenza del lavoro da svolgere in una determinata giornata.

PunchCode decide di far uso di pacchetti software di supporto alla pianificazione, specie considerando come al progetto sia stata attribuita una classe B in termini di complessità (nonostante non preveda la presenza di team diversi e di parti di lavoro in appalto).

A fronte di una stima iniziale, si suppone che il tempo richiesto per la pianificazione sia di 3/4 giorni.

Per maggior chiarezza vengono elencati i deliverable che la fase di Planning deve produrre:
- Project Definition Statement (PDS);
- Work Breakdown Structure (WBS);
- Risorse necessarie;
- Stima della durata delle attività;
- Project network schedule;
- Schedulazione delle attività;
- Assegnamento delle risorse;
- Project Notebook;
- Project proposal.

## 4.1 Joint Project Planning Session
Le riunioni sono uno strumento di base per il Planning. Una JPPS è una sessione di lavoro realizzata con lo scopo di attuare la panificazione del progetto. Durante le JPPS vengono così definite le attività volte a soddisfare le esigenze del cliente, stabilendo dei vincoli in termini di tempo, di budget e di risorse disponibili. Un meeting si basa sulla definizione di alcuni elementi di principale importanza, quali:
 - i partecipanti;
 - le facility;
 - la strumentazione;
 - l'agenda;
 - i deliverable;
 - la proposta di progetto.

Generalmete, le attività da svolgere durante la sessione superano di gran lunga l'arco temporale di una giornata, per cui si preferisce intraprendere più sessioni. La startup pianifica dunque 3 meeting, sollecitando il Project Manager del cliente a partecipare soltanto alla prima sessione.
I partecipanti a questi incontri dovrebbero essere: il/i Project Manager dell'esecutore e del committente, il Core Project Team, il rappresentante del cliente, il Resource Manager, il Facilitatore e il Tecnografo.
A causa del ridotto numero del personale, la figura del Resource Manager non si rivela necessaria e PunchCode decide far partecipare entrambi i membri del team agli incontri, cercando di coprire le figure mancanti basandosi sulle skill dei dipendenti.

I meeting si terranno nelle giornate dell'8, 9 e 10 aprile presso la sede di PunchCode. Lo svolgimento avverrà all'interno di una stanza, dotata di una lavagna bianca, proiettore, computer e, all'occorrenza, carta e penna.  
Le agende delle tre sessioni sono di seguito riportate:

 - 08/04/2019 - [agenda sessione 1](project_docs/csen_poomsae_score/joint_project_planning_session/session_08_04_19.md)  
 - 09/04/2019 - [agenda sessione 2](project_docs/csen_poomsae_score/joint_project_planning_session/session_09_04_19.md)  
 - 10/04/2019 - [agenda sessione 3](project_docs/csen_poomsae_score/joint_project_planning_session/session_10_04_19.md) 

### 4.1.1 Sessione #1
Alla prima sessione vi partecipano i due membri di PunchCode (sia nel ruolo di Project Manager che di Core Team), il Project Manager del cliente e la sua rappresentanza.
Questo è l'unico JPPS in cui è presente il team di lavoro lato committente, in quanto necessario per definire le priorità dei vari requisiti.

La startup ha preferito non dedicare interamente la prima riunione alla revisitazione apposita dei CoS, del RBS e del POS (appena conclusi in forma non definitiva al termine della fase di Scoping, con la relativa approvazione del cliente). Si è ritenuto opportuno, piuttosto, procedere con una pianificazione in dettaglio delle attività da svolgere (WBS), in quanto il cliente si è reso disponibile fin dal Project Scoping Meeting ad un alto coinvolgimento durante l'intera pianificazione. 
È proprio durante la definizione delle attività a partire dal RBS che i partecipanti al meeting possono eventualmente constatare la presenza di elementi trascurati o di errori compiuti al momento della stesura dei deliverable della fase precedente (provvedendo di conseguenza alla loro risoluzione, avvalendosi di un diretto confronto con il cliente). Rimettere 

Lo scopo del primo incontro dovrebbe essere anche quello di introdurre i vari soggetti che seguiranno l'intero progetto, pur considerando come il team di sviluppo possa essere scelto soltanto nella fase di Launching (a causa della distanza temporale potenzialmente presente tra la pianificazione e l'avvio effettivo del contratto). Tuttavia, dal momento che il Core Team di PunchCode è formato dagli stessi Project Manager, il cliente ha già avuto modo di conoscere tali figure.
Una volta concluse le presentazioni, è discussa la prioritizzazione dei requisiti definiti durante le sessioni di Project Scoping Meeting. Soltanto in seguito viene ampliato l'RBS per dar vita alla [Work Breakdown Structure (WBS)](project_docs/csen_poomsae_score/planning/wbs.png) precedentemente citata (che è pertanto realizzata da tutti i membri del team nell'obiettivo di giungere a una soluzione migliore, nonostante ciò sia più dispendioso). Rimettere mano allo scoping adesso, infatti, è molto meno costoso che farlo in seguito (nonostante tale operazione debba comunque avvenire il meno possibile).

### 4.1.2 Sessione #2
Alla seconda sessione partecipano soltanto i membri di PunchCode.

L'incontro ha inizio con la stima della quantità di lavoro, della durata e delle risorse richieste per lo svolgimento delle singole attività che si sono individuate con la WBS. Si giunge così alla costruzione del [Gantt](project_docs/csen_poomsae_score/gantt/gantt.png).

Successivamente si procede alla definizione delle dipendenze tra le varie attività, ottenendo il diagramma di [PERT](project_docs/csen_poomsae_score/pert/pert.png) e continuando con la parte centrale del meeting: l'individuazione e la discussione del *critical path*, delle date previste per il completamente del progetto e delle diverse milestone. Se necessario, si considera una compressione della schedula a fini di ottimizzazione. Una scelta non corretta delle date di completamento di una o più milestone potrebbe originare un malcontento da parte del committente e la crescita di stress all'interno del gruppo di lavoro.

<!-- Microsoft Project -->

### 4.1.3 Sessione #3
Alla terza sessione prendono parte gli stessi partecipanti della seconda.

L'obiettivo principale dell'incontro riguarda l'identificazione dei [rischi](project_docs/csen_poomsae_score/wbs/wbs.png), la loro valutazione e l'individuazione di eventuali piani di mitigazione (valutando alternative e soluzioni per eliminare o ridurre le perdite).
La gestione del rischio costituisce un argomento fondamentale e può rivelarsi anche molto complessa. Una non corretta individuazione dei rischi in fase di Planning potrebbe portare a scontrarsi con problematiche più o meno gravi durante le successive fasi del ciclo di vita del progetto (non prevedendo eventi con conseguenze negative sul progetto stesso o compiendo errori nella valutazione del loro impatto). Sotto quest'ultimo punto di vista, occorre anche osservare come una sovrastima dell'impatto di un rischio possa determinare l'inserimento di complessità non necessaria in termini di monitoraggio e controllo, capace di rendere difficoltosa la gestione del progetto e di far lievitare al tempo stesso anche budget e tempistiche.

La fase successiva riguarda l'ottenimento dell'approvazione da parte di tutti i partecipanti sui contenuti del piano (facendo emergere eventuali perplessità). Ciò è molto importante in quanto una volta arrivati a questo punto eventuali modifiche si ripercuoteranno su un gran numero di attività. 

L'ultimo obiettivo della sessione si riferisce alla redazione del [Project Definition Statement (PDS)](project_docs/csen_poomsae_score/pds/pds.md), con la partecipazione di tutto il team.

## 4.2 Prioritizzazione dei requisiti

Non tutti i requisiti vengono trattati con le stesse priorità, in quanto vi è un processo di classificazione (o meglio, prioritizzazione) dei requisiti. Esistono diversi approci nell'eseguire quest'attività; quello adottato dall'azienda risulta essere **MoSCoW**, che è basato su una categorizzazione in 4 classi:

- *Must*: requisiti che **devono** essere soddisfatti per ritenere il progetto completato con successo.
- *Should*: requisiti che **dovrebbero** essere inclusi nella soluzione. Sono abbastanza critici da essere considerati necessari, ma è possibile sostituirli con dei requisiti alternativi.
- *Could*: requisiti che **potrebbero** essere inclusi alla consegna, ma non sono strettamente necessari, in quanto considerati soltanto in caso di disponibilità del tempo e delle risorse.
- *Won't*: requisiti che **sarebbero** da includere, ma vengono rinviati per una futura release, in quanto non strettamente necessari.

PunchCode, nello specifico, decide di assegnare una priorità ai soli requisiti "foglia" del RBS. Il risultato di questa fase è osservabile al seguente [allegato](project_docs/csen_poomsae_score/moscow_prioritisation/moscow_prioritisation.md).


## 4.3 Work Breakdown Structure (WBS)

Consiste nella suddivisione tassonomica di tutte le singole attività che devono essere svolte all'interno del progetto per soddisfare i bisogni del cliente (rappresentando una mappa gerarchica di tutto il lavoro).

È generata e validata nella JPPS, subito dopo la prioritizzazione MoSCoW dei requisiti.

Uno dei principali motivi per cui PunchCode ne fa uso è che - oltre a essere uno strumento di reporting - facilita la definizione dell'architettura (dal momento che attività ripetute sono infatti indice di componenti che, a causa di un loro molteplice uso, necessitano di essere progettati con cura).
La WBS è usata anche nel seguente modo:
- aiuta i Project Manager e il team a visualizzare esattamente come il lavoro sia definito e debba essere gestito efficientemente;
- consente di non dimenticare parti di lavoro ed evitare duplicazioni (assegnando una numerazione univoca a tutte le attività);
- facilita la comunicazione tra gli stakeholder (permettendo a tutti di riferirsi in maniera omogenea ed inequivocabile al lavoro da eseguirsi);
- consente la realizzazione di valutazioni di costo o di tempo aggregate, seguendo la struttura gerarchica definita.

La WBS inizia là dove finisce l'RBS. PunchCode, infatti, la ricava considerando le foglie dell'RBS e decomponendole ulteriormente (approccio classico). Si presta inoltre attenzione a non spingersi troppo nel dettaglio, per evitare di dover fare un numero elevato di stime (richiedenti tempo e costi); allo stesso tempo si cerca di non avere nemmeno una granularità troppo grande, in modo da ridurre il rischio che le attività siano difficili da stimare e pericolose da monitorare.  
Per comprendere quando arrestarsi a causa del raggiungimento di un adeguato livello di decomposizione che decreti il completamento della WBS, PunchCode adotta 6+1 criteri:

1) lo stato e il completamento sono misurabili (si deve essere in grado di indicare la percentuale di completamento);
2) le attività sono ben delimitate (con un inizio e una fine definiti);
3) le attività hanno associato un deliverable;
4) i tempi e i costi sono facilmente stimabili;
5) la durata delle attività rientra in un limite accettabile;
6) ciascun task è considerato come un'attività non interrompibile;
7) qualora il *cosa* sia chiaro ma il *come* no, il Project Manager deve gestire tale incertezza.

Per convertire la RBS in WBS, PunchCode utilizza il *Team Approach* (prevedendo cioè la partecipazione di tutto il team alla definizione dell'intera WBS). La ragione di questa scelta è nuovamente da ricercarsi nel ridotto numero di membri interni alla startup, che impedisce al momento l'adozione di una modalità di lavoro parallela a sotto-team.

Confermando un modello PMLC incrementale, la WBS è necessariamente completa.

Infine, si osserva come la WBS non abbia alcuna logica temporale e conseguentemente non imponga un ordine cronologico. Il rapporto delle attività rispetto al tempo è introdotto col diagramma di Gantt e col diagramma di PERT.

<!-- Spiegare attività in arancione scuro e task in arancione -->
<!-- Link a WBS.png e a indice (wbs.md) -->

## 4.4 Stima delle risorse necessarie

La stima delle risorse che potrebbero essere necessarie all'esecuzione dei task rappresenta un passaggio essenziale per la buona riuscita del progetto. Col termine "risorse" non si fa riferimento alle sole persone fisiche, ma anche alle facility, all'attrezzatura, ai materiali e al costo. Nei paragrafi di seguito proposti ci si focalizza tuttavia sui soli processi legati all'assegnamento delle risorse umane ai task (la stima dei costi sarà discussa in una [successiva sezione](#46-stima-dei-costi)).  
PunchCode sceglie pertanto di stimare prima le risorse in termini di personale da assegnare alle varie attività e soltanto dopo la durata dei task in funzione di esse. Questa decisione ha come obiettivo la produzione di stime temporali più accurate che tengano conto sin da subito sia delle persone incaricate per la realizzazione dei task stessi che delle loro singole capacità.

### 4.4.1 Valutazione delle skill richieste dai task

Per assegnare i membri dello staff ai task della WBS nel modo più efficace possibile, PunchCode sviluppa prima una [matrice "skill-need" (need inventory)](project_docs/csen_poomsae_score/staff_skills_assignments/needs_inventory.md) con un'indicazione delle skill richieste da ciascuno di essi.  
Nel far ciò, la startup considera tutte le pro skill e le sole pre skill effettivamente legate a tale passaggio. Inoltre, si è ritenuto non necessario adottare una valutazione numerica, preferendo di conseguenza un semplice indicatore booleano (per esprimere la necessità o meno di una certa skill da parte di un task).

### 4.4.2 Assegnamento membri dello staff ai task

Tenendo conto delle skill possedute dallo staff ([skills inventory](project_docs/startup_team_skills/startup_team_skills.md)) e di quelle realmente richieste dai task da svolgere ([need inventory](project_docs/csen_poomsae_score/staff_skills_assignments/needs_inventory.md)), PunchCode incrocia le due matrici al fine di individuare i corretti match. 
Ad ogni dipendente si assegnano quindi i task da svolgere che meglio si adattano alle sue abilità.

È importante sottolineare la necessità di parallerizarre molti dei task da svolgere, a causa del limitato numero dei membri del team e delle loro capacità diversificate. Nella risultante tabella di [staff assignment](project_docs/csen_poomsae_score/staff_skills_assignments/staff_assignment.md) (ove non vi è presente una "X" simboleggiante una completa gestione da parte di un solo membro) sono state indicate le skill effettivamente sfruttate dai dipendenti durante lo svolgimento di una determinata attività.

### 4.5 Stima della durata dei task

La stima della durata dei task costituisce la parte centrale del Planning, nonchè quella in cui spesso le aziende falliscono. Tale fase, infatti, è molto complicata: in aggiunta al già difficile compito della stima in quanto tale, si deve anche considerare come si possa non andare alla velocità prevista o come si possano verificare interruzioni non prevedibili anche a fronte di una valutazione corretta. L'importanza di questa operazione è anche legata al fatto che permette di costruire la schedula e di determinare i tempi necessari al raggiungimento delle varie milestone e al completamento del progetto.

Dal momento che la persona che meglio può entrare nel merito di un'attività è chi la realizza, PunchCode decide di far svolgere questa fase a entrambi i membri del team. La stima della durata richiede tuttavia l'aver prima scelto il come svolgerla.

La durata di un task può variare per diverse ragioni, tra cui livelli di esperienza e competenza differenti da parte dello staff stesso. Un'altra scelta della startup è pertanto quella di tener conto al momento della stima, oltre che del numero di risorse assegnate al task in esame (osservabile dallo [staff assignment](project_docs/csen_poomsae_score/staff_skills_assignments/staff_assignment.md)), anche delle singole capacità del/i membro/i assegnato/i (indicate nello [skills inventory](project_docs/startup_team_skills/startup_team_skills.md)), in modo da dedurre le velocità di lavoro di ogni persona sulla base delle varie skill. Occorre comunque sottolineare come tutti i processi abbiano una durata variabile per cause comuni: non esiste una sola attività (anche operativa) che svolta tutti i giorni impieghi sempre lo stesso tempo.

Non avendo esperienza con progetti precedenti, PunchCode non può ricorrere all'analisi di dati storici o all'uso di estrapolazioni basate su attività simili per la costruzione delle stime. Inoltre, non avendo le risorse economiche necessarie, preferisce non affidarsi a terzi per avvalersi del giudizio di un esperto.  
La startup decide pertanto di ricorrere all'applicazione di una tecnica "**consensus-based**". Disponendo in tale fase di due sole figure interne al team, metodologie quali *Three-point technique* e l'uso di indici statistici come la mediana non risultano applicabili. Non potendo poi usufruire di anonimato, PunchCode ha scelto di far riferimento a una versione modificata della *Delphi Technique* nell'obiettivo di favorire sin da subito l'insorgere di interazioni atte a comprendere le ragioni alla base di stime ottimistiche o pessimistiche.  
Il metodo richiede ai due membri del team di effettuare segretamente le stime ad ogni round (in un numero compreso tra 1 e 3, sulla base delle necessità). Al termine di ogni round, le durate stimate vengono rivelate e ogni partecipante è così incoraggiato a rivedere la propria stima in base a quella rilasciata dall'altro e alle motivazioni che l'accompagnano. Il processo termina quando si soddisfa un criterio di stop, consistente nel raggiungimento del numero massimo di round pari a 3 o di un consenso unanime). La stima finale è rappresentata dalla media. Si osserva dunque come durante questo processo il gap tra le stime si dovrebbe ridurre, portando alla convergenza verso un valore condiviso.  
Nonostante spesso si preferisca adottare una misura adimensionale (distaccata sia dai tempi che dai costi), PunchCode preferisce adottare un'unità di misura tradizionale in *giorni/uomo*. Ciò è anche legato all'inesperienza dell'azienda con tali aspetti metodologici, dove vi sarebbe il rischio di non essere in grado di quantificare opportunamente il lavoro da svolgere a partire da una misura adimensionale (come una carta poker, un numero di Fibonacci o una taglia T-shirt).  
Infine, si evidenzia come una stima non debba considerare solo il tempo di scrittura del codice, ma quello per la costruzione di una soluzione robusta che sia completa e funzionante (che comprenda quindi anche la scrittura dei rispettivi test e il loro superamento).

Il documento contenente le stime in termini di effort giorni/uomo rilasciate da parte del team per le varie attività presenti in WBS è disponibile nel relativo [allegato](project_docs/csen_poomsae_score/task_duration_estimate/task_duration_estimate.md).
È interessante osservare come i membri del team siano generalmente molto in sintonia (probabilmente a causa della loro profonda esperienza nel lavorare assieme, che li ha di fatto spinti alla costituzione di PunchCode). In talune circostanze si evince tuttavia come le stime iniziali sarebbero state molto diverse senza essere condizionati. In alcuni casi si osserva anche la presenza di un'oscillazione (1° round: ottimistico, 2° round: pessimistico, 3° round: valutazione intermedia).

### 4.6 Stima dei costi

<!--
Per quanto riguarda i costi delle singole attivita' ci si basera' molto su:

Esperienze Precedenti
Risorse Particolari (licenze, consulenti..)
Personale Coinvolto
Altro

Al termine di ogni stima il tutto viene formalizzato attraverso l'apposito template che indichera' effettivamente il tempo che si e' deciso e il costo ad esso associato. Quindi l'analisi dei costi viene effettuata nello stesso momento delle stime delle tempistiche delle singole attivita'. Il calcolo e' agevolato dalla scelta dell'unita' di misura classica (giorni/uomo) che, anche se risulta non proprio ottimale per una stima corretta, puo' essere facilmente intuibile anche da reparti amministrativi, a cui puo' essere delegata la stima dei costi stessa, e da eventuali consulenti esterni o altri che non conoscono eventuali misurazioni alternative. Inoltre si riduce il trade off data da un'eventuale conversione da un'unita' di misura personalizzata adimensionale.
-->

## 4.7 Diagramma di Gantt

<!--
Nella sua versione base, consiste semplicemente nel prendere le attività previste dalla WBS e posizionarle sull'asse temporale, capendo cioè quando iniziano e quando finiscono.

Assieme al PERT è lo strumento principale con cui si comprende lo stato di avanzamento del progetto. Viene infatti mantenuto aggiornato dal Project Manager durante lo svolgimento del progetto stesso. Man mano che esso progredisce, delle barre colorate possono essere aggiunte al diagramma per indicare le attività completate o una porzione completata di queste.
Es. l'attività 3 è svolta al 70%
Non solo... Il Project Manager potrebbe anche dire "questa attività è in ritardo, allora l'altra la sposto più avanti".

Il diagramma di Gantt è lo strumento ufficiale per gestire la pianificazione temporale del progetto.


Aggiungere la spiegazione del perchè abbiamo differenziato tra X, UI/UX e coding
-->

## 4.8 Diagramma di PERT
<!--
A differenza del diagramma di Gantt che non considera la presenza di legami tra le varie attività, col diagramma di PERT ci si arricchisce e si vanno a identificare tutte le relazioni di precedenza tra le attività stesse.

La sua rappresentazione interna è quella di un grafo, con le attività come i nodi e gli archi come legami di vario tipo:
1) Finish to Start
2) Start to Start
3) Start to Finish
4) Finish to Finish

A partire dal diagramma di PERT è possibile riconoscere - attraverso un Forward pass (->) e un Backward pass (<-) - la presenza di percorsi critici (insiemi di attività in cui un ritardo su una singola attività determina un ritardo sull'intero progetto).
Un percorso critico è pertanto caratterizzato dall'assenza di margine (Total Float = Late Start - Early Start = 0).
I percorsi critici o quelli con basso margine (es. pochi giorni) sono gli insiemi di attività che devo monitorare con maggiore attenzione.

Non ci lavoro solo in fase di PIANIFICAZIONE, ma anche in OTTIMIZZAZIONE (es. voglio che il progetto finisca prima -> aggiungo risorse con l'obiettivo di ridurre la durata delle attività sul percorso critico) e in CONTROLLO.
-->

## 4.9 Analisi dei Rischi

<!--
- 4 categorie.
- Nel valutare l'impatto si è ragionato tenendo conto del caso peggiore.
- Ogni quanto ri-identificare e rivalutare i rischi (approccio dinamico).
-->

## 4.10 Project Definition Statement (PDS)

Il [PDS](project_docs/csen_poomsae_score/pds/pds.md) è una versione estesa del POS a uso del team di progetto. In esso si sono riportati elementi di maggior dettaglio, costituenti un ottimo input per le fasi successive e per approfondimenti. Il PDS rappresenta così un punto di riferimento anche per eventuali nuovi membri del team, consentendo loro di rimanere focalizzati sulla corretta direzione e sugli aspetti importanti per il successo del progetto.



<!--
- *Applicazione Android*.  
Per automatizzare la valutazione delle poomsae svolte dagli atleti da parte dei giudici.

- *Software per la gestione del quadrato di gara abbinato all'applicazione Android*.  
Per la gestione dei tornei interni a una competizione su un quadrato di gara e la raccolta dei punteggi da parte delle applicazioni in esecuzione sui tablet dei giudici, anticipando alcune funzionalità lato server (importazione dati da file Excel, creazione della competizione, gestione dei trasferimenti ed elaborazione classifica globale localmente al quadrato).

- *Sistema software completo*  
Per l'integrazione del server, spostando la configurazione delle competizioni su un unico nodo, gestendo il partizionamento dei tornei tra i vari quadrati al fine di evitare sovrapposizioni e raccogliendo i dati elaborati da ogni software di gestione di quadrato.

Si vuole sottolineare come - per garantire i rilasci intermedi di cui il committente necessita - si sia scelto di anticipare funzionalità di sottosistemi ancora non realizzati (con la consapevolezza che ciò richieda un ulteriore lavoro in termini di modifiche e integrazione).
-->

# 5. Bibliografia

[1]<a id="bibliography-1"></a> [Platonova, Valērija & Bērziša, Solvita. "Gamification in Software Development Projects". *Information Technology and Management Science*. Dec 2017.](https://www.researchgate.net/publication/322409704_Gamification_in_Software_Development_Projects)  
[2]<a id="bibliography-1"></a> [Senthil Rajamarthandan. "Using Gamification to Build a Passionate and Quality-Driven Software Development Team". *Cognizant 20-20 Insights*. Feb 2014.](https://www.cognizant.com/InsightsWhitepapers/Using-Gamification-to-Build-a-Passionate-and-Quality-Driven-Software-Development-Team.pdf)