# Visual Devblog - #001

<div align="center"><img src="https://i.imgur.com/eWuJmqE.png" alt="Visual Roleplay logo"/></div>

Visual punta ad essere sinonimo di qualità, una garanzia per la community italiana roleplay di Grand Theft Auto V. Questo blog stabilirà un nuovo punto di dialogo per i tutti i giocatori appassionati di questa modalità.

Dall'apertura del discord ad oggi, le domande sono state molte. In molti credono che Visual sia solo una grande incognità. Molti altri non ricononosco il potenziale di Visual, o meglio, non hanno ancora visione di ciò che Visual sarà in grado di offrire. Riteniamo pertanto doveroso, con l'apertura di questo blog, dimostrare la tenacia e la professionalità con cui stiamo portando a termine questo progetto.

## Stato dello sviluppo 
Il mese di Dicembre è stato molto movimentato, sono state impletamentate numerose migliorie al codice sorgente per migliorare le prestazioni del server e del client. Uno dei punti cardini di questo progetto è infatti proprio l'accessibilità: stiamo lavorando duramente per offrire un prodotto longevolo e di qualità. Ciò è il motivo per cui crediamo che lo sviluppo di Visual non debba essere forzato. L'apertura di Visual arriverà ed è inevitabile. 

In riferimento alla lista riportata in basso, abbiamo concentrato i nostri sforzi mensili per risolvere problematiche comuni e molto frequenti tra i server di GTA5 che utilizzano piattaforme multiplayer come FiveM o RageMP.

**Problematiche frequenti riscontrate su altri server di GTA 5**:
> Eccessivo utilizzo di CPU da parte del client, problemi di desync, assenza di un appropiato sistema per gestire le entities di gioco (oggetti vicino al player, checkpoint, ecc), consumo insolito di RAM da parte delle interfacce di gioco non native (create attraverso un browser fornito dalla mod multiplayer), FPS troppo bassi. 

Riportiamo inoltre di seguito i punti chiavi dello sviluppo di questo mese. 

**Punti chiave dello sviluppo di questo mese:**
* Streamer server side in grado di supportare 4 milioni di entites (es: oggetti, checkpoint) in prossimità del player senza influire negativamente sulle prestazioni del gioco/client.

* Riduzione drastica del consumo di RAM e CPU da parte dei browser non nativi di gioco generalmente utilizzati per fornire informazioni al player o creare GUI. 

* Conversione a Typescript. Attualmente in corso una revisione del codice sorgente completa per migliorarne la qualità e per indirizzare bug di gioco. 

### Approfondimenti tecnici

###### Che cos'è lo streamer?
Una meccanica quasi sempre tralasciata in molti server di GTA 5 è la presenza di uno streamer in grado di fare da tramite tra il client e il server di gioco per aggiornare le entità presenti in prossimità del player con altri player. In altre parole, un elemento di gioco addizionale e non incluso originariamente nel gioco che deve essere syncato tra i giocatori, ovvero che deve essere visibile da tutti quando si è in prossimita con esso. Cerchiamo di capirci meglio con un esempio pratico: immaginiamo di voler rilevare la posizione di una proprietà in prossimità di un player. La scelta più opportuna è quella di indicarla con un checkpoint, quindi ci basterà crearne uno e il gioco sarà fatto, giusto? Non esattamente. Immaginate di avere 100 proprietà molto vicine tra di loro e di doverle rilevare ad un player nelle vicinanze con 100 checkpoint differenti. Oltre a risultare sgradevole, ciò comporterebbe ad un notevole calo delle prestazioni di gioco. Immaginiamo ora invece di aver uno streamer in grado di mostrare al player le proprietà al momento più opportuno, ovvero quando il player si troverà effettivamente in prossimità di esse e ad una distanza minima specificata anticipamente dal server. Ciò comporterebbe nell'avere 100 proprietà vicine in range ma solo un unico checkpoint.

###### Cosa sono i browser di gioco, a cosa servono?
Quando si parla di browser di gioco non si fa altro che riferimento ad un vero e proprio browser (come Firefox, Google Chrome) implementato all'interno del gioco in grado di fornire al player un'interfaccia di navigazione. HTML, stili in CSS e codice in Javascript può essere fornito al browser per creare interfacce grafiche o per fornire informazioni di vario tipo. Un utilizzo non corretto dei browser di gioco può incidere negativamente sulle prestazioni del client.

## Anteprima creazione personaggio
È arrivato il momento che tutti aspettavamo. Sono passati dei mesi da quando ci siamo annunciati la prima volta, mesi in cui ci siamo confrontati incessantemente. 
Per noi è molto importante dare una direzione efficace allo sviluppo, ma questo lo possiamo fare soltanto discutendo e valutando tutti i possibili sviluppi prima di creare un sistema. 
Abbiamo raccolto idee, pareri, proposte provenienti da uno staff ampio ed eterogeneo. 
C’era una cosa, però, che non volevamo fare: mostrarvi qualcosa e poi dover aspettare mesi per vederla realizzata male. Adesso, finalmente, abbiamo un’idea precisa di cosa fare e sappiamo come farlo.
Non possiamo far altro che partire dal primo sistema che troverete in game, cioè quello di creazione dei personaggi. Abbiamo scelto una caratterizzazione molto approfondita: sono stati infatti inclusi tutti i parametri di customizzazione presenti nel gioco nativamente. La creazione del personaggio, inoltre, come anche del resto tutti i sistemi presenti all'interno della nostra gamemode, non dipendono da piattaforme esterne di terze parti non associate con Visual.

<div align="center"><iframe width="560" height="315" src="https://www.youtube.com/embed/cXYDWlLhDwY" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>

## Sneak peek di chiusura
Manca sempre meno all’apertura, tra poco potrete toccare con mano la qualità di questo progetto. 
Nel frattempo, godetevi quest'ultimo sneak peek di chiusura. 

<div align="center"><blockquote class="imgur-embed-pub" lang="en" data-id="a/Wg3XOAA" data-context="false" ><a href="//imgur.com/a/Wg3XOAA"></a></blockquote><script async src="//s.imgur.com/min/embed.js" charset="utf-8"></script></div>
