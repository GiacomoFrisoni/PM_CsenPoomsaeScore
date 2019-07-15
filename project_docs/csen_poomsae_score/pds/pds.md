<table>
    <tr>
        <th rowspan="2" width="15%" align="left">PROJECT DEFINITION STATEMENT</th>
        <th width="30%">Project Name</th>
        <th width="30%">Project No.</th>
        <th width="30%">Project Manager</th>
    </tr>
    <tr>
        <td align="center">CSEN Poomsae Score</td>
        <td align="center">1</td>
        <td align="center">Giacomo Frisoni<br/>Marcin Pabich</td>
    </tr>
</table>

<br/>


<table>
    <tr>
        <td>
            <b>Problem/Opportunity</b><br/><br/>
            Dopo una forte crescita a cui non è seguita una razionalizzazione dei processi operativi, CSEN ha necessità di informatizzare il proprio processo di gestione dei tornei di Taekwondo; l'esigenza è data dall'inefficienza legata a una completa gestione manuale e dalla presenza di soluzioni software già in uso da parte di aziende competitor.
        </td>
    </tr>
    <tr>
        <td>
            <b>Goal</b><br/><br/>
            Implementare una soluzione software che sia in grado di migliorare la gestione delle competizioni di Taekwondo, sia in termini di efficacia che di efficienza.
        </td>
    </tr>
    <tr>
        <td>
            <b>Objectives</b><br/><br/>
            <ul>
                <li>
                    Sviluppare un'applicazione Android per automatizzare la valutazione di poomsae da parte dei giudici.
                    <ul>
                        <li>
                        Prevedere la realizzazione delle schermate seguendo i <a href="../project_scoping_meeting/session_14_03_19_res/mockup">mockup</a> definiti nel Project Scoping Meeting.
                        </li>
                        <li>
                        Porre una particolare attenzione all'usabilità dei controlli, in quanto potrebbero essere fruiti anche da persone con scarse competenze informatiche.
                        </li>
                    </ul>
                </li>
                <br/>
                <li>
                    Sviluppare un sistema software per la gestione dei tornei nei quadrati di gara.
                    <ul>
                        <li>
                        Prevedere la realizzazione delle schermate seguendo i <a href="../project_scoping_meeting/session_18_03_19_res/mockup">mockup</a> definiti nel Project Scoping Meeting.
                        </li>
                        <li>
                        Trarre ispirazione dalle <a href="../project_scoping_meeting/session_11_03_19_res/competitor">soluzioni software già esistenti</a> e comunicate dal committente.
                        </li>
                        <li>
                        Tenere in considerazione che i laptop montano tutti Windows 10 come sistema operativo.
                        </li>
                        <li>
                        La visualizazzione dei dati sui monitor esterni non richiede la realizzazione di ulteriori applicazioni, ma consiste semplicemente in finestre secondarie, aperte e gestite dal software.
                        </li>
                    </ul>
                </li>
                <br/>
                <li>
                    Realizzare un server capace di creare, configurare e gestire competizioni.
                    <ul>
                        <li>
                        Il file con gli atleti arriva in formato Excel (.xls).
                        </li>
                        <li>
                        Tenere in considerazione che i laptop montano tutti Windows 10 come sistema operativo.
                        </li>
                        <li>
                        La visualizazzione della classifica globale e degli atleti partecipanti ai vari quadrati sul monitor esterno non richiede la realizzazione di ulteriori applicazioni, ma consiste semplicemente in finestre secondarie, aperte e gestite dal software.
                        </li>
                    </ul>
                </li>
                <br/>
                <li>
                    Provvedere all'implementazione di una forma di comunicazione tra i vari sottosistemi.
                    <ul>
                        <li>
                        Non è sempre garantito un accesso a Internet: la comunicazione si svolge pertanto via LAN, utilizzando sia collegamenti fisici che rete wireless (e comunque attraverso tramite un router). 
                        </li>
                        <li>
                        Tutte le funzionalità dipendenti dalla comunicazione in rete devono essere progettate per funzionare anche in assenza di quest'ultima (ad esempio, permettendo il caricamento dei dati da file)
                        </li>
                    </ul>
                </li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <b>Success Criteria</b><br/><br/>
            <ul>
                <li>
                    Diminuire i tempi per la raccolta dei punteggi espressi dai giudici per le singole poomsae, in base alla seguente tabella:
                    <table>
                        <tr>
                            <th rowspan="2">N° giudici</th>
                            <th align="center">Attuale</th>
                            <th colspan="3" align="center">Desiderato</th>
                        </tr>
                        <tr>
                            <th>Tempo medio attuale (secondi)</th>
                            <th>Tempo medio desiderato (secondi)</th>
                            <th>Massima deviazione standard (secondi)</th>
                            <th>Tempo massimo (secondi)</th>
                        </tr>
                        <tr>
                            <td>3</td>
                            <td>120</td>
                            <td>5</td>
                            <td>5</td>
                            <td>15</td>
                        </tr>
                        <tr>
                            <td>5</td>
                            <td>240</td>
                            <td>5</td>
                            <td>5</td>
                            <td>15</td>
                        </tr>
                        <tr>
                            <td>7</td>
                            <td>360</td>
                            <td>5</td>
                            <td>5</td>
                            <td>15</td>
                        </tr>
                    </table>
                    <i>Miglioramento percepibile a partire dalla prima major-release relativa ai tablet con l'applicazione Android.</i>
                </li>
                <br/>
                <li>
                    Ridurre i tempi medi di preparazione di un torneo secondo la seguente tabella:
                    <table>
                        <tr>
                            <th rowspan="2">Range di partecipanti</th>
                            <th align="center">Attuale</th>
                            <th colspan="3" align="center">Desiderato</th>
                        </tr>
                        <tr>
                            <th>Tempo medio attuale (minuti)</th>
                            <th>Tempo medio desiderato (minuti)</th>
                            <th>Massima deviazione standard (minuti)</th>
                            <th>Tempo massimo (minuti)</th>
                        </tr>
                        <tr>
                            <td>0-8</td>
                            <td>7</td>
                            <td>2</td>
                            <td>2</td>
                            <td>5</td>
                        </tr>
                        <tr>
                            <td>9-18</td>
                            <td>13</td>
                            <td>5</td>
                            <td>3</td>
                            <td>9</td>
                        </tr>
                        <tr>
                            <td>19+</td>
                            <td>26</td>
                            <td>10</td>
                            <td>4</td>
                            <td>16</td>
                        </tr>
                    </table>
                    <i>Miglioramento percepibile a partire dalla seconda major-release relativa alla soluzione software per la gestione dei quadrati di gara, integrata con l'applicazione Android.</i>
                </li>
                <br/>
                <li>
                    Ridurre i tempi medi per la determinazione degli atleti che passano alla gara successiva o che ricevano una medaglia (comprensivi dell'individuazione di ballottaggi):
                    <table>
                        <tr>
                            <th rowspan="2">Range di partecipanti</th>
                            <th align="center">Attuale</th>
                            <th colspan="3" align="center">Desiderato</th>
                        </tr>
                        <tr>
                            <th>Tempo medio attuale (secondi)</th>
                            <th>Tempo medio desiderato (secondi)</th>
                            <th>Massima deviazione standard (secondi)</th>
                            <th>Tempo massimo (secondi)</th>
                        </tr>
                        <tr>
                            <td>0-8</td>
                            <td>100</td>
                            <td>2</td>
                            <td>2</td>
                            <td>5</td>
                        </tr>
                        <tr>
                            <td>9-18</td>
                            <td>300</td>
                            <td>2</td>
                            <td>2</td>
                            <td>5</td>
                        </tr>
                        <tr>
                            <td>19+</td>
                            <td>500</td>
                            <td>2</td>
                            <td>2</td>
                            <td>5</td>
                        </tr>
                    </table>
                    <i>Miglioramento percepibile a partire dalla seconda major-release relativa alla soluzione software per la gestione dei quadrati di gara, integrata con l'applicazione Android.</i>
                </li>
                <br/>
                <li>
                    Nell'elaborazione della classifica globale delle palestre, ridurre i tempi medi per l'attribuzione di punti a una palestra a partire da un suo atleta vincitore da 10 secondi per ogni atleta con medaglia a 2 secondi per l'intero processo, con massima deviazione standard di 3 secondi e tempo massimo pari a 7 secondi.<br/>
                    <i>Miglioramento percepibile a partire dalla release finale.</i>
                </li>
                <br/>
                <li>
                    Incremento della percentuale delle iscrizioni ai tornei del 15% nel primo semestre, rispetto al numero d'iscrizioni dell'ultimo anno (pari a 1200).<br/>
                    <i>Miglioramento percepibile a partire dalla release finale.</i>
                </li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <b>Assumbtions / Risks / Obstacles</b><br/><br/>
            <i>Assunzioni</i>
            <ul>
                <li>
                Il committente è già in possesso della dotazione tecnica (quali tablet, computer, monitor e dispositivi per l'interconnessione).
                </li>
                <li>
                Il numero ridotto degli atleti partecipanti, rispetto alla concorrenza, è causato dall'obsolescenza dell'azienda nel gestire le competizioni.
                </li>
                <li>
                Le soluzioni software sono limitate esclusivamente ai due sistemi operativi citati (Android e Windows), pertanto non devono essere Cross-Platform.
                </li>
            </ul>
            <br/>
            <i>Rischi</i>
            <ul>
                <li>
                Le caratterristiche tecniche dei laptop e del server in dotazione al cliente potrebbero incidere sull'usabilità delle soluzioni software, limitandone le performance.
                </li>
                <li>
                A causa dell'anticipazione di alcune funzionalità per il rilascio di release intermedie, la loro futura integrazione potrebbe richiedere di svolgere nuovamente alcune parti di lavoro.
                </li>
                <li>
                Bisogno inaspettato di acquistare software.
                </li>
                <li>
                PunchCode potrebbe riscontrare difficoltà nella gestione delle comunicazioni a causa della sua inesperienza coi protocolli di rete.
                </li>
                <li>
                Le stime delle durate dei task potrebbero essere inaccurate (ottimistiche o pessimistiche) a causa dell'inesperienza di PunchCode. 
                </li>
                <li>
                L'assenza di dati storici da parte di PunchCode potrebbe causare un'errata quantificazione delle probabilità di perdite associate ai rischi.
                </li>
                <li>
                Le richieste di cambiamento di scope da parte del committente potrebbero essere frequenti e significative.
                </li>
                <li>
                Le assunzioni potrebbero essere inaccurate.
                </li>
                <li>
                La mancanza di figure specializzate nella conduzione e gestione dei meeting potrebbe rendere quest'ultimi inefficienti.
                </li>
                <li>
                L'interpretazione del ruolo di Architetto da parte di un Project Manager potrebbe non portare ai vantaggi attesi (anche a causa dell'inesperienza).
                </li>
                <li>
                La scarsa competenza informatica degli utilizzatori del sistema potrebbe portare a un uso inefficiente di quest'ultimo.
                </li>
                <li>
                Il ridotto numero dei dipendenti di PunchCode potrebbe portare non essere sufficiente per affrontare il progetto nei tempi concordati.
                </li>
                <li>
                CSEN potrebbe modificare le modalità di gestione delle competizioni di Taekwondo in maniera significativa.
                </li>
                <li>
                CSEN potrebbe decidere di abortire il progetto.
                </li>
            </ul>
            <br/>
            <i>Ostacoli</i>
            <ul>
                <li>
                La versione massima di Android supportata dai tablet risulta essere 4.1.1 (Jelly Bean); questo potrebbe impedire l'utilizzo di API Android più recenti, rendendo più faticoso lo svilupo dell'app.
                </li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <b>Classificazione del progetto</b><br/><br/>
            In base alla <a href="../../project_classification/project_classification.md">classificazione</a> adottata dall'azienda, il progetto risulta essere di classe <b>B</b>.
        </td>
    </tr>
    <tr>
        <td>
            <b>Glossary</b><br/><br/>
            <ul>
                <li>
                    <b>Poomsae (o forma):</b>
                    serie di tecniche di braccia, calci e passi codificati. Rappresentano dei combattimanenti con avversari immaginari che attaccano da diverse direzioni.
                </li>
                <li>
                    <b>Categoria:</b>
                    è un raggruppamento per classe d'età assegnato a ogni atleta.
                </li>
                <li>
                    <b>Grado:</b>
                    è il grado rappresentato dalla cintura indossata dall'atleta.
                </li>
                <li>
                    <b>Competizione:</b>
                    insieme di tornei di poomsae previsti in occasione di un certo evento.
                </li>
                <li>
                    <b>Torneo:</b>
                    insieme di gare attraverso cui i partecipanti si contendono le medaglie sportive messe in palio. Ne esistono di tre tipologie: <i>individuali</i>, <i>coppie</i> e <i>team</i>. Le possibili gare sono <i>Eliminatorie</i>, <i>Semifinali</i> e <i>Finali</i>. La gara di partenza è determinata dal numero di atleti iscritti al torneo.
                </li>
                <li>
                    <b>Gara:</b>
                    confronto interno a un torneo tra più atleti che cercano di assicurarsi il passaggio alla gara successiva o l'assegnamento di una medaglia. 
                </li>
            </ul>
        </td>
    </tr>
</table>
