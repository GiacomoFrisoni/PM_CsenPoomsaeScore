# Piano di qualità

## Indicatori di qualità di obiettivo

### Indicatori di qualità applicabili a tutti gli obiettivi

#### IQ01 - Slittamento nell'esecuzione dell'obiettivo

L'indicatore vuole valutare se la durata effettiva dell'obiettivo è maggiore rispetto a quella concordata nell'ultima pianificazione approvata da CSEN, considerando la data di attivazione come la data di partenza (comune alle due durate) per il calcolo della metrica.  
Si valuta quindi lo slittamento della data di accettazione effettiva rispetto a quella di fine obiettivo riportata nell'ultima pianificazione.

<table>
  <tr>
    <th align="left">Caratteristica</th>
    <td align="left">Efficienza</th>
    <th align="left">Sottocaratteristica</th>
    <td align="left">Efficienza temporale</th>
  </tr>
  <tr>
    <th align="left">Aspetto da valutare</th>
    <td align="left" colspan="3">Slittamento della fine effettiva dell'obiettivo (data di accettazione) rispetto a quella concordata nell'ultima pianificazione, partendo dalla data di attivazione, per cause imputabili al fornitore</td>
  </tr>
  <tr>
    <th align="left">Unità di misura</th>
    <td align="left">Giorni lavorativi</th>
    <th align="left">Fonte dati</th>
    <td align="left">Piano di lavoro<br/>Lettera di accettazione</th>
  </tr>
  <tr>
    <th align="left">Periodo di riferimento</th>
    <td align="left">Durata dell'obiettivo</th>
    <th align="left">Frequenza di misurazione</th>
    <td align="left">Dopo il termine dell'obiettivo</th>
  </tr>
  <tr>
    <th align="left">Dati da rilevare</th>
    <td align="left" colspan="3">
        <ul>
            <li>Data di accettazione (<i>Data_accett</i>)</li>
            <li>Data di accettazione prevista dall'ultimo Piano di lavoro approvato (<i>Data_pian_accett</i>)</li>
            <li>Data di attivazione dell'obiettivo (<i>Data_attiv</i>)</li>
        </ul>
    </td>
  </tr>
  <tr>
    <th align="left">Regole di campionamento</th>
    <td align="left" colspan="3">Nessuna</td>
  </tr>
  <tr>
    <th align="left">Formula</th>
    <td align="left" colspan="3"><i>IQ01 = (Data_accett - Data_attiv) - (Data_pian - Data_attiv)</i></td>
  </tr>
  <tr>
    <th align="left">Regole di arrotondamento</th>
    <td align="left" colspan="3">Nessuna</td>
  </tr>
  <tr>
    <th align="left">Valore di soglia</th>
    <td align="left" colspan="3">IQ01 <= 0</td>
  </tr>
  <tr>
    <th align="left">Azioni contrattuali</th>
    <td align="left" colspan="3">Penale <i>"Slittamento nell'esecuzione dell'obiettivo"</i> qualora non sia rispettato il valore di soglia</td>
  </tr>
  <tr>
    <th align="left">Eccezioni</th>
    <td align="left" colspan="3">Nessuna</td>
  </tr>
</table>

<br/>

------------

<br/>

#### IQ02 - Slittamento della consegna di un incremento dell'obiettivo

L'indicatore si applica ad ogni macro incremento previsto per l'obiettivo.

<table>
  <tr>
    <th align="left">Caratteristica</th>
    <td align="left">Efficienza</th>
    <th align="left">Sottocaratteristica</th>
    <td align="left">Efficienza temporale</th>
  </tr>
  <tr>
    <th align="left">Aspetto da valutare</th>
    <td align="left" colspan="3">Puntualità nella consegna di un macro incremento dell'obiettivo rispetto alla data prevista nel Piano di lavoro</td>
  </tr>
  <tr>
    <th align="left">Unità di misura</th>
    <td align="left">Giorni lavorativi</th>
    <th align="left">Fonte dati</th>
    <td align="left">Piano di lavoro<br/>Lettera di accettazione</th>
  </tr>
  <tr>
    <th align="left">Periodo di riferimento</th>
    <td align="left">Durata dell'obiettivo</th>
    <th align="left">Frequenza di misurazione</th>
    <td align="left">Ad ogni consegna di incremento</th>
  </tr>
  <tr>
    <th align="left">Dati da rilevare</th>
    <td align="left" colspan="3">
        <ul>
            <li>Data prevista di consegna di un incremento (<i>Data_prev</i>)</li>
            <li>Data effettiva di consegna di un incremento (<i>Data_eff</i>)</li>
        </ul>
    </td>
  </tr>
  <tr>
    <th align="left">Regole di campionamento</th>
    <td align="left" colspan="3">Vanno considerate tutte le consegne di incremento eseguite nel periodo di riferimento</td>
  </tr>
  <tr>
    <th align="left">Formula</th>
    <td align="left" colspan="3"><i>IQ02 = Data_eff - Data_prev</i></td>
  </tr>
  <tr>
    <th align="left">Regole di arrotondamento</th>
    <td align="left" colspan="3">Nessuna</td>
  </tr>
  <tr>
    <th align="left">Valore di soglia</th>
    <td align="left" colspan="3">IQ02 <= 0</td>
  </tr>
  <tr>
    <th align="left">Azioni contrattuali</th>
    <td align="left" colspan="3">Rilievo sull'obiettivo per ogni ritardo di 5 giorni lavorativi o frazione rispetto al valore di soglia (<i>es. un ritardo rispetto al piano di 11 gg lavorativi comporterà 3 rilievi sull'obiettivo</i>)</td>
    <!--In realtà immagino che se non riusciamo a consegnare un incremento per gare davvero importanti il rilievo venga sollevato anche con meno di 5 giorni o addirittura una penale-->
  </tr>
  <tr>
    <th align="left">Eccezioni</th>
    <td align="left" colspan="3">Nessuna</td>
  </tr>
</table>

<br/>

------------

<br/>

#### IQ03 - Rilievi sull'obiettivo

I rilievi conteggiati nella metrica sono quelli notificati al fornitore tramite comunicazione formale emessa da CSEN. Si precisa che ciascuna comunicazione potrà contenere più rilievi.  
Il numero di rilievi tollerati dall'obiettivo è in relazione alla [classe](project_docs/csen_poomsae_score/project_classification/project_classification.md) del progetto.

<table>
  <tr>
    <th align="left">Caratteristica</th>
    <td align="left">Efficacia</th>
    <th align="left">Sottocaratteristica</th>
    <td align="left">Efficacia</th>
  </tr>
  <tr>
    <th align="left">Aspetto da valutare</th>
    <td align="left" colspan="3">Numero di rilievi emessi sull'obiettivo</td>
  </tr>
  <tr>
    <th align="left">Unità di misura</th>
    <td align="left">Rilievo</th>
    <th align="left">Fonte dati</th>
    <td align="left">Rilievo</th>
  </tr>
  <tr>
    <th align="left">Periodo di riferimento</th>
    <td align="left">Durata dell'obiettivo</th>
    <th align="left">Frequenza di misurazione</th>
    <td align="left">Al termine dell'obiettivo</th>
  </tr>
  <tr>
    <th align="left">Dati da rilevare</th>
    <td align="left" colspan="3">
        <ul>
            <li>Numero di rilievi emessi sull'obiettivo (<i>Nrilievi_obiettivo</i>)</li>
        </ul>
    </td>
  </tr>
  <tr>
    <th align="left">Regole di campionamento</th>
    <td align="left" colspan="3">Vanno considerati tutti i rilievi emessi nel periodo di riferimento sull'obiettivo</td>
  </tr>
  <tr>
    <th align="left">Formula</th>
    <td align="left" colspan="3"><i>IQ03 = Nrilievi_obiettivo</i></td>
  </tr>
  <tr>
    <th align="left">Regole di arrotondamento</th>
    <td align="left" colspan="3">Nessuna</td>
  </tr>
  <tr>
    <th align="left">Valore di soglia</th>
    <td align="left" colspan="3">
        IQ03 <= 4&emsp;Classe = A<br/>
        IQ03 <= 3&emsp;Classe = B<br/>
        IQ03 <= 2&emsp;Classe = C o Classe = D<br/>
    </td>
  </tr>
  <tr>
    <th align="left">Azioni contrattuali</th>
    <td align="left" colspan="3">Penale <i>"Eccesso di rilievi tollerati per obiettivo"</i> qualora non sia rispettato il valore di soglia</td>
  </tr>
  <tr>
    <th align="left">Eccezioni</th>
    <td align="left" colspan="3">Nessuna</td>
  </tr>
</table>

<br/>

------------

<br/>

### Indicatori di qualità applicabili agli obiettivi di sviluppo, mev e mad

#### IQ04 - Test negativi in collaudo

Con questo indicatore si vogliono individuare i casi di test eseguiti (sia in modalità manuale che automatica) dal fornitore con successo prima del rilascio e che, se rieseguiti durante il collaudo, danno esito negativo.

<table>
  <tr>
    <th align="left">Caratteristica</th>
    <td align="left">Affidabilità</th>
    <th align="left">Sottocaratteristica</th>
    <td align="left">Maturità</th>
  </tr>
  <tr>
    <th align="left">Aspetto da valutare</th>
    <td align="left" colspan="3">Casi di test eseguiti con esito negativo in collaudo</td>
  </tr>
  <tr>
    <th align="left">Unità di misura</th>
    <td align="left">Casi di test eseguiti in collaudo con esito negativo</th>
    <th align="left">Fonte dati</th>
    <td align="left">Piano di Test<br/>Verbale di collaudo</th>
  </tr>
  <tr>
    <th align="left">Periodo di riferimento</th>
    <td align="left">Durata della fase di collaudo dell'obiettivo</th>
    <th align="left">Frequenza di misurazione</th>
    <td align="left">Al termine del collaudo</th>
  </tr>
  <tr>
    <th align="left">Dati da rilevare</th>
    <td align="left" colspan="3">
        <ul>
            <li>Numero di casi di test dichiarati come eseguiti con successo dal fornitore e che in collaudo hanno dato esito negativo (<i>Ntest_notok</i>)</li>
        </ul>
    </td>
  </tr>
  <tr>
    <th align="left">Regole di campionamento</th>
    <td align="left" colspan="3">Nessuna</td>
  </tr>
  <tr>
    <th align="left">Formula</th>
    <td align="left" colspan="3"><i>IQ04 = Ntest_notok</i></td>
  </tr>
  <tr>
    <th align="left">Regole di arrotondamento</th>
    <td align="left" colspan="3">Nessuna</td>
  </tr>
  <tr>
    <th align="left">Valore di soglia</th>
    <td align="left" colspan="3">IQ04 = 0</td>
  </tr>
  <tr>
    <th align="left">Azioni contrattuali</th>
    <td align="left" colspan="3">Rilievo sull'obiettivo per ogni caso di test eseguito in collaudo con esito negativo</td>
  </tr>
  <tr>
    <th align="left">Eccezioni</th>
    <td align="left" colspan="3">Nessuna</td>
  </tr>
</table>

<br/>

------------

<br/>

#### IQ05 - Difettosità in collaudo

Per "*Difetto*" si intende un errore presente nel software da collaudare, latente finchè non rilevato.  
Per "*Difettosità in collaudo*" si intende il rapporto tra il numero di difetti (relativi a tutte le categorie di malfunzionamento) emersi in fase di collaudo dell'obiettivo, e <!--TODO-->

<table>
  <tr>
    <th align="left">Caratteristica</th>
    <td align="left">Affidabilità</th>
    <th align="left">Sottocaratteristica</th>
    <td align="left">Maturità</th>
  </tr>
  <tr>
    <th align="left">Aspetto da valutare</th>
    <td align="left" colspan="3">Difettosità in collaudo</td>
  </tr>
  <tr>
    <th align="left">Unità di misura</th>
    <td align="left">Difetti / <!--TODO--></th>
    <th align="left">Fonte dati</th>
    <td align="left"><!--TODO--></th>
  </tr>
  <tr>
    <th align="left">Periodo di riferimento</th>
    <td align="left">La fase di collaudo dell'obiettivo</th>
    <th align="left">Frequenza di misurazione</th>
    <td align="left">Al termine del collaudo</th>
  </tr>
  <tr>
    <th align="left">Dati da rilevare</th>
    <td align="left" colspan="3">
        <ul>
            <li>Numero totale di elementi difettosi emersi durante il collaudo (<i>N_difetti</i>)</li>
            <li><!--TODO--></li>
        </ul>
    </td>
  </tr>
  <tr>
    <th align="left">Regole di campionamento</th>
    <td align="left" colspan="3">Vanno considerati tutti gli elementi difettosi rilevati durante il collaudo</td>
  </tr>
  <tr>
    <th align="left">Formula</th>
    <td align="left" colspan="3">
      <img src="https://latex.codecogs.com/gif.latex?\inline&space;\dpi{150}&space;IQ05&space;=&space;\frac{N\_difetti}{TODO}" title="IQ05 = \frac{N\_difetti}{TODO}" />
    </td>
  </tr>
  <tr>
    <th align="left">Regole di arrotondamento</th>
    <td align="left" colspan="3">
      Il risultato della misura va arrotondato:<br/>
      - per difetto se la parte decimale è <= 0,0005<br/>
      - per eccesso se la parte decimale è > 0,0005
    </td>
  </tr>
  <tr>
    <th align="left">Valore di soglia</th>
    <td align="left" colspan="3">IQ05 <= 0,040</td>
  </tr>
  <tr>
    <th align="left">Azioni contrattuali</th>
    <td align="left" colspan="3">Rilievo sull'obiettivo nel caso di mancato rispetto del valore di soglia</td>
  </tr>
  <tr>
    <th align="left">Eccezioni</th>
    <td align="left" colspan="3">Nessuna</td>
  </tr>
</table>

<br/>

------------

<br/>

#### IQ06 - Giorni di sospensione del collaudo

<table>
  <tr>
    <th align="left">Caratteristica</th>
    <td align="left">Affidabilità</th>
    <th align="left">Sottocaratteristica</th>
    <td align="left">Maturità</th>
  </tr>
  <tr>
    <th align="left">Aspetto da valutare</th>
    <td align="left" colspan="3">Numero complessivo di giorni in cui è stato sospeso il collaudo di un obiettivo per cause imputabili al fornitore</td>
  </tr>
  <tr>
    <th align="left">Unità di misura</th>
    <td align="left">Giorni lavorativi</th>
    <th align="left">Fonte dati</th>
    <td align="left">Comunicazione formale di sospensione del collaudo<br/>Comunicazione formale di ripresa del collaudo</th>
  </tr>
  <tr>
    <th align="left">Periodo di riferimento</th>
    <td align="left">La fase di collaudo dell'obiettivo</th>
    <th align="left">Frequenza di misurazione</th>
    <td align="left">Al termine del collaudo</th>
  </tr>
  <tr>
    <th align="left">Dati da rilevare</th>
    <td align="left" colspan="3">
        <ul>
            <li>Data e ora di sospensione del collaudo (<i>Data_sospensione<sub>j</sub></i>)</li>
            <li>Data e ora di ripresa del collaudo (<i>Data_ripresa<sub>j</sub></i>)</li>
            <li>Numero di giorni non lavorativi tra la sospensione e la ripresa del collaudo (<i>Ngiorni_nolav<sub>j</sub></i>)</li>
            <li>Numero di sospensioni del collaudo (<i>Nsosp_collaudo</i>)</li>
        </ul>
    </td>
  </tr>
  <tr>
    <th align="left">Regole di campionamento</th>
    <td align="left" colspan="3">Si applica a tutte le sospensioni di collaudo (<i>sia la prima che, qualora capiti, le successive</i>)</td>
  </tr>
  <tr>
    <th align="left">Formula</th>
    <td align="left" colspan="3">
      <img src="https://latex.codecogs.com/gif.latex?\inline&space;\dpi{150}&space;IQ06&space;=&space;\sum_{j=1}^{Nsosp\_collaudo}(Data\_ripresa_j&space;-&space;Data\_sospensione_j&space;-&space;Ngiorni\_nolav_j)" title="IQ06 = \sum_{j=1}^{Nsosp\_collaudo}(Data\_ripresa_j - Data\_sospensione_j - Ngiorni\_nolav_j)" />
    </td>
  </tr>
  <tr>
    <th align="left">Regole di arrotondamento</th>
    <td align="left" colspan="3">Nessuna</td>
  </tr>
  <tr>
    <th align="left">Valore di soglia</th>
    <td align="left" colspan="3">IQ06 = 0</td>
  </tr>
  <tr>
    <th align="left">Azioni contrattuali</th>
    <td align="left" colspan="3">Rilievo sull'obiettivo nel caso di mancato rispetto del valore di soglia</td>
  </tr>
  <tr>
    <th align="left">Eccezioni</th>
    <td align="left" colspan="3">Nessuna</td>
  </tr>
</table>

<br/>

------------

<br/>

#### IQ07 - Slittamento della risoluzione dei malfunzionamenti del collaudo

Durante il collaudo di ogni obiettivo gli interventi effettuati a fronte di malfunzionamenti del software applicativo avranno un livello di ripristino della piena operatività in funzione della categoria di malfunzionamento, così definito:

<table>
  <tr>
    <th align="left">Caratteristica</th>
    <td align="left">Efficienza</th>
    <th align="left">Sottocaratteristica</th>
    <td align="left">Efficienza temporale</th>
  </tr>
  <tr>
    <th align="left">Aspetto da valutare</th>
    <td align="left" colspan="3">Tempestività di ripristino in collaudo a seguito di malfunzionamenti, valutata rispetto alla durata prevista</td>
  </tr>
  <tr>
    <th align="left">Unità di misura</th>
    <td align="left">Giorni lavorativi</th>
    <th align="left">Fonte dati</th>
    <td align="left"><!--TODO--></th>
  </tr>
  <tr>
    <th align="left">Periodo di riferimento</th>
    <td align="left">Fase di collaudo</th>
    <th align="left">Frequenza di misurazione</th>
    <td align="left">Al termine del collaudo</th>
  </tr>
  <tr>
    <th align="left">Dati da rilevare</th>
    <td align="left" colspan="3">
        <ul>
            <li>Avvio del processo di risoluzione del malfunzionamento: data, ora e minuti comunicati dal fornitore <i>(inizio<sub>i</sub>)</i></li>
            <li>Termine della risoluzione del malfunzionamento: data, ora e minuti <i>(fine<sub>i</sub>)</i></li>
            <li>Tempo di sospensione della risoluzione del malfunzionamento (<i>sospensione</i>) a causa dell'indisponibilità dell'ambiente di correzione, o per ragioni non imputabili al fornitore (<i>TRO<sub>i</sub></i>)</li>
            <li>Numero totale di segnalazioni chiuse a fronte di malfunzionamenti rilevati in collaudo (<i>Ntotale_malf_coll</i>)</li>
        </ul>
    </td>
  </tr>
  <tr>
    <th align="left">Regole di campionamento</th>
    <td align="left" colspan="3">Nessuna</td>
  </tr>
  <tr>
    <th align="left">Formula</th>
    <td align="left" colspan="3">
      <img src="https://latex.codecogs.com/gif.latex?\inline&space;\dpi{150}&space;IQ07&space;=&space;\sum_{i=1}^{Ntotale\_malf\_coll}ritardo\_risol_i" title="IQ07 = \sum_{i=1}^{Ntotale\_malf\_coll}ritardo\_risol_i" />
      <br/>
      Dove:
      <br/>
      <ul>
        <li><i>durata_risol<sub>i</sub> = termine<sub>i</sub> - inizio<sub>i</sub> - TRO<sub>i</sub></i></li>
        <li>
          <i>valore_limite = </i>
          <table>
            <tr>
              <td><i>categoria A</i></td>
              <td><i>categoria B</i></td>
              <td><i>categoria C</i></td>
            </tr>
            <tr>
              <td><i>2 giorni lavorativi</i></td>
              <td><i>3 giorni lavorativi</i></td>
              <td><i>5 giorni lavorativi</i></td>
            </tr>
          </table>
        </li>
        <li>
          <i>ritardo_risol<sub>i</sub> = </i>
          <table>
            <tr>
              <td><i>0</i></td>
              <td><i>durata_risol<sub>i</sub> - valore_limite</i></td>
            </tr>
            <tr>
              <td><i>(se durata_risol<sub>i</sub> <= valore_limite)</i></td>
              <td><i>(se durata_risol<sub>i</sub> > valore_limite)</i></td>
            </tr>
          </table>
        </li>
      </ul>
    </td>
  </tr>
  <tr>
    <th align="left">Regole di arrotondamento</th>
    <td align="left" colspan="3">Nessuna</td>
  </tr>
  <tr>
    <th align="left">Valore di soglia</th>
    <td align="left" colspan="3">IQ07 = 0</td>
  </tr>
  <tr>
    <th align="left">Azioni contrattuali</th>
    <td align="left" colspan="3">Il mancato rispetto del valore di soglia comporterà un rilievo sull'obiettivo per ogni giorno lavorativo o frazione eccedente la soglia</td>
  </tr>
  <tr>
    <th align="left">Eccezioni</th>
    <td align="left" colspan="3">Nessuna</td>
  </tr>
</table>

<br/>

------------

<br/>

#### IQ08 - Difettosità in esercizio (per applicazione)

<table>
  <tr>
    <th align="left">Caratteristica</th>
    <td align="left">Affidabilità</th>
    <th align="left">Sottocaratteristica</th>
    <td align="left">Maturità</th>
  </tr>
  <tr>
    <th align="left">Aspetto da valutare</th>
    <td align="left" colspan="3">Difettosità in esercizio di un'applicazione</td>
  </tr>
  <tr>
    <th align="left">Unità di misura</th>
    <td align="left">Difetti / <!--TODO--></th>
    <th align="left">Fonte dati</th>
    <td align="left"><!--TODO--></th>
  </tr>
  <tr>
    <th align="left">Periodo di riferimento</th>
    <td align="left">Tremestre precedente la rilevazione</th>
    <th align="left">Frequenza di misurazione</th>
    <td align="left">Trimestrale</th>
  </tr>
  <tr>
    <th align="left">Dati da rilevare</th>
    <td align="left" colspan="3">
        <ul>
            <li>Numero totale di difetti dell'applicazione rilevati durante il periodo di riferimento (<i>N_difetti_appl</i>)</li>
            <li><!--TODO--></li>
        </ul>
    </td>
  </tr>
  <tr>
    <th align="left">Regole di campionamento</th>
    <td align="left" colspan="3">Vanno considerati tutti i difetti rilevati durante il periodo di riferimento</td>
  </tr>
  <tr>
    <th align="left">Formula</th>
    <td align="left" colspan="3">
      <img src="https://latex.codecogs.com/gif.latex?\inline&space;\dpi{150}&space;IQ08&space;=&space;\frac{N\_difetti\_appl}{TODO}" title="IQ08 = \frac{N\_difetti\_appl}{TODO}" />
    </td>
  </tr>
  <tr>
    <th align="left">Regole di arrotondamento</th>
    <td align="left" colspan="3">
      Il risultato della misura va arrotondato:
      - per difetto se la parte decimale è <= 0,00005
      - per eccesso se la parte decimale è > 0,00005
    </td>
  </tr>
  <tr>
    <th align="left">Valore di soglia</th>
    <td align="left" colspan="3"><!--TODO--></td>
  </tr>
  <tr>
    <th align="left">Azioni contrattuali</th>
    <td align="left" colspan="3"><!--TODO--></td>
  </tr>
  <tr>
    <th align="left">Eccezioni</th>
    <td align="left" colspan="3">Nessuna</td>
  </tr>
</table>