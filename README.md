# MPB 23/24 proejct

## [Note generali]

Leggere attentamente il testo del progetto e consegnare una breve relazione (max. 7 pagine di testo, figure escluse) in formato elettronico che
illustri le soluzioni proposte e le analisi condotte.
Progettare le reti a partire da modelli più astratti (EPC, BPMN), utilizzando le tecniche di trasformazione viste nel corso indicando quali tecniche
sono state impiegate e perchè.
Nel presentare una workflow net, illustrarne le caratteristiche (invarianti,
s-components, se è free-choice, se è well-handled, se è safe,...) e descrivere
le caratteristiche del grafo di raggiungibilità (quanti vertici, quanti archi, se
contiene cicli,...).
Per lo sviluppo di workflow module, verificare preventivamente che togliendo le piazze di input / output dell’interfaccia (e gli archi incidenti su
esse) la rete sia sound.
Qualora non sia possibile progettare processi sound, chiarirne i motivi e
studiarne le proprietà di weak soundness.
Se ritenuto utile, compilare la checklist di analisi disponibile sul canale
Teams del corso per ogni rete analizzata.
Spedire al docente la versione elettronica della relazione in formato .pdf,
i file .pnml di tutte le reti analizzate, i file .bpmn di tutti i diagrammi BPMN
progettati e, opzionalmente, le checklist di analisi.

## [P44: Vettore]

Si consideri lo scenario della gestione delle consegne di un vettore di un’azienda di trasporti. Il processo inizia quando il vettore riceve un ordine di
trasporto con data, luogo e contatto di origine, e data, luogo e contatto di
destinazione. Se il vettore non è in grado di effettuare il trasporto il processo termina. Altrimenti il vettore inserisce l’ordine nel piano delle consegne
ed effettua il prelievo, il trasporto e la consegna nei tempi indicati. Se il
mittente o il destinatario non sono presenti al momento del prelievo o della
consegna il vettore li contatta per negoziare una nuova data di prelievo e
consegna. Durante le negoziazioni vengono proposte a turno nuove date fino
a quando l’ultima data proposta viene accettata. Al momento del prelievo e
della consegna vengono fatti firmare i documenti di trasporto al mittente e
al destinatario, rispettivamente. Il processo termina quando il destinatario
restituisce il modulo firmato.
Progettare opportuni processi che rispecchino fedelmente lo scenario sopra
descritto e siano compatibili.
Modificare i processi in modo che, in caso di un ritardo imprevisto, il
vettore contatti preventivamente il destinatario per negoziare una nuova data
di consegna