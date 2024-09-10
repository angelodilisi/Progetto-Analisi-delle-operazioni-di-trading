# Progetto-Analisi-delle-operazioni-di-trading

**Modifica foglio di calcolo sulle revenue
ottenute dal trading di azioni finanziarie**


Questo progetto consiste nel modificare il foglio di calcolo allegato in modo da soddisfare alcuni
requisiti.


**Il dataset**

I dati presenti nel foglio di calcolo allegato rappresentano le operazioni finanziarie effettuate da
Bob dal 1 gennaio 2021.
Nello specifico, le colonne sono denominate come segue:
● TradeID: identificativo dell'azione scambiata - numero a 8 cifre
● Stock exchange: mercato sul quale è stata scambiata l'azione
● Region: nazione o confederazione a cui appartiene il mercato
● Date added: data di acquisto dell'azione in formato YYYY-MM-DD
● Quantity: numero di azioni acquistate/vendute nella transazione
● Buy Price: prezzo di acquisto per azione
● Date sold: data di vendita dell'azione in formato YYYY-MM-DD
● Sell Price: prezzo di vendita per azione


**Cosa devi fare**

Per realizzare il progetto, dovrai modificare il foglio di calcolo allegato, con lo scopo di avere
una più profonda comprensione dei dati in esso contenuti.
In particolare, il foglio avrà la seguente struttura:

Primo tab o scheda

● Nome: "My trades"

● Stile:

○ La prima riga di intestazione ha carattere Comics Sans MS, dimensione 12pt e
colore blu, riquadrata su 4 lati con bordo doppio

○ Ogni cella non del titolo è riquadrata su 4 lati in nero con il bordo sottile

○ Al di fuori della tabella non sono presenti celle vuote (vengono colorate di bianco
senza bordi righe e colonne a contorno dei veri e propri dati)

○ Le date presenti nelle colonne Date added e Date sold hanno il formato
DD/MM/YY

Secondo tab o scheda

● Nome: "Stock exchanges"

● Stile:
○ La prima riga di intestazione ha carattere Comics Sans MS, di dimensione 12pt e
colore blu, riquadrata su 4 lati con bordo doppio

○ Ogni cella non del titolo è riquadrata su 4 lati in nero con il bordo sottile

○ Al di fuori della tabella non sono presenti celle vuote (vengono colorate di bianco
senza bordi righe e colonne a contorno dei veri e propri dati)

○ La riga di intestazione contiene i seguenti titoli:
■ Region
■ Stock exchange
■ Num of trades
■ Mandatory to pay taxes

● Contenuto:
○ Una pivot table che raggruppi i mercati finanziari a seconda dello stato al quale
appartengono (hint: inserire i campi per riga). Tale tabella contiene anche il
numero di azioni scambiate per ogni stato
○ Sapendo che è necessario pagare tasse anche nel paese di acquisto quando si
scambiano azioni per un totale maggiore o uguale a 67 (per semplicità usiamo il
numero di azioni e non l'importo), la colonna D conterrà "yes" oppure "no" in
base al totale di azioni scambiate in quello stato (hint: usa il costrutto
condizionale SE). Notare che il valore è da associarsi soltanto al totale per stato

Terzo tab o scheda

● Nome: "Profit insights"

● Stile:
○ La prima riga di intestazione ha carattere Comics Sans MS, dimensione 12pt e
colore blu, riquadrata su 4 lati con bordo doppio

○ Ogni cella non del titolo è riquadrata su 4 lati in nero con il bordo sottile

○ La riga di intestazione contiene i seguenti titoli:
■ TradeID
■ Duration
■ Profit

● Contenuto:

○ Nella colonna A sono riportati i riferimenti a tutti i trade del primo tab (hint: usare
il carattere "=" e il riferimento alle celle)

○ Nella colonna B è calcolata la durata del possesso del trade in giorni

○ Nella colonna C è calcolato il profitto (eventualmente negativo) fatto. Tale profitto
si calcola come differenza fra prezzo di vendita e acquisto, il tutto moltiplicato per
il numero di azioni scambiate. Il profitto sarà in formato valuta dollaro americano,
con 5 cifre decimali

○ Al centro del foglio è mostrato a video un diagramma a barre che rappresenta le
frequenze del tempo (Duration) per cui le azioni sono state mantenute

○ Sotto a tale diagramma si scriva una casella di testo che commenti tale
diagramma e spieghi se la durata assume una distribuzione normale o no

Quarto tab o scheda

● Nome: "Number of trades exchanged"

● Stile:

○ Riga e colonna di intestazione hanno carattere Comics Sans MS, dimensione
12pt e colore blu, riquadrata su 4 lati con bordo doppio

○ Ogni cella della tabella di contingenza è riquadrata su 4 lati in nero con il bordo
sottile

○ Al di fuori della tabella non sono presenti celle vuote (vengono colorate di bianco
senza bordi righe e colonne a contorno dei veri e propri dati)

○ La tabella di contingenza contiene i seguenti titoli:

■ Region
■ Number of trades
● Contenuto:
○ La tabella di contingenza è utilizzata per calcolare la probabilità che in un dato
stato vengano scambiate un certo numero di azioni

○ Nello specifico, si realizzi per prima cosa una tabella che contiene come righe
tutti i possibili stati e nelle colonne il numero di trade scambiati (hint. COUNTIFS)

○ Una volta calcolata la tabella di contingenza, aggiungere le due distribuzioni
marginali (per stato e per numero di azioni) e inserire nell’angolo a destra il totale
calcolato

○ Calcolare la probabilità che, sorteggiata una qualunque azione (tradeID) essa sia
stata acquistata esattamente 7 volte nel Regno Unito e riportare tale valore in un
punto scelto dalla colonna M in poi

○ Calcolare la probabilità che, sorteggiata una qualunque azione (tradeID) essa sia
stata acquistata in un qualunque stato asiatico in quantità non superiore (!!<=!!!)
a 8 unità. Riportare tale valore (con rispettivo titolo) in un punto scelto dalla
colonna M in poi

**NOTE**

In questo progetto si assume che, quando le azioni vengono vendute, quest'ultime siano
vendute in quantità uguale a quella acquistat
