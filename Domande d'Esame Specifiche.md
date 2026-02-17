### Introduzione
==1. Che cosa studia l'Ingegneria del Software ?==
L'Ingegneria del Software è una disciplina dell'Ingegneria Informatica, che si occupa dello sviluppo, della progettazione, della manutenzione, della documentazione e della gestione dei sistemi SW, in modo sistematico, disciplinato e quantificabile.
L'Ingegneria del Software deve garantire che i SW siano di alta qualità, a basso costo e si basa su tecniche, strumenti e principi specifici per sviluppare e gestire il ciclo di vita di un SW.

La produzione di un SW è un processo composto di 6 fasi :
1) Analisi dei Requisiti : comprendere i bisogni degli utenti e tradurli in requisiti funzionali e non funzionali.
2) Progettazione : definire l'architettura del sistema, i componenti e l'interfaccia.
3) Sviluppo : scrittura e implementazione del codice.
4) Test e Verifica : il SW deve funzionare correttamente e soddisfare i requisiti.
5) Manutenzione : miglioramenti, aggiornamenti e correzione di bug.
6) Gestione : monitoraggio del progetto, coordinamento e pianificazione.

I problemi che affronta l'Ingegneria del Software sono :
1) Complessità del SW : suddividere un SW complesso in parti più piccole e semplici da gestire, attraverso decomposizione funzionale e modularizzazione.
2) Scalabilità : il SW deve adattarsi ad un numero crescente di utenti o dati senza perdita di prestazioni.
3) Qualità : prodotti affidabili, sicuri e performanti.
4) Gestione Tempi e Costi.
5) Cambiamenti nei Requisiti : deve garantire SW che sia flessibile e facile da cambiare, piuttosto che il SW funzioni correttamente.
6) Manutenzione : il SW deve essere mantenuto rilevante e funzionante a lungo termine, tramite aggiornamenti.
7) Collaborazione e Coordinazione all'interno dei Team.

### Requirements Engineering
==2. Descrivere come può essere suddiviso il processo di specifica dei requisiti.== 
Le principali fasi in cui il processo di specifica dei requisiti può essere suddiviso sono :
1) Elicitazione (raccolta) : in questa fase vengono identificati e raccolti i requisiti dagli stakeholders, attraverso interviste, workshop, questionari, studio di documentazione esistente e da osservazione diretta. L'elicitazione può essere sia verbale, che scritta, che online, ma si preferisce quella verbale. In questa fase devo comprendere le esigenze dell'utente, i problemi e gli obiettivi del progetto, di conseguenza, può essere utile il prototyping. Il prototyping viene utilizzato per comprendere meglio i requisiti degli stakeholders, aiutare gli utenti a visualizzare funzionalità, o interfacce, soprattutto se non riescono ad esprimere bene le loro esigenze. Il prototyping, quindi, aiuta ad identificare i requisiti impliciti e difficili da esplicitare, generando un feedback immediato sulle idee proposte. Spesso, il prototipo in questo caso è low-fidelity (schizzi, wireframe) e serve per stimolare discussioni.
2) Analisi dei Requisiti : I requisiti raccolti vengono analizzati per identificare eventuali conflitti, o ambiguità, prioritizzarli e valutare i vincoli e la fattibilità tecnica. Si include anche la modellazione e la rappresentazione dei requisiti, con diagrammi, casi d'uso, o scenari.
3) Specificazione dei Requisiti : Documentazione dei requisiti in un documento chiamato "Specifiche dei requisiti SW" (SRS). I requisiti devono essere chiari e non ambigui, tracciabili, completi e consistenti.
4) Validazione e Verifica : Si verifica che i requisiti soddisfino le necessità degli stakeholders, che siano completi, corretti e coerenti, che siano comprensibili per tutte le parti coinvolte. La validazione può avvenire attraverso revisioni, prototipi e simulazioni. In questa fase, il prototyping viene usato per verificare che i requisiti raccolti siano stati compresi correttamente, per validare le aspettative degli stakeholders, confrontandole con un prototipo più avanzato (high-fidelity), che simula in modo realistico il sistema e per ridurre il rischio di malintesi, permettendo agli utenti di testare le funzionalità chiave.
5) Gestione dei Requisiti (Requirement Management) : I requisiti possono cambiare e quindi eventuali modifiche devono essere controllate. I requisiti devono essere tracciati e ci deve essere un aggiornamento continuo della documentazione.
6) Accettazione.

==3. Che cosa si intende per SRS ? A cosa serve ? In che fase del ciclo della produzione del SW si colloca ? Quali sono le caratteristiche che rendono un SRS di qualità ?==
L'SRS è un documento formale che funge da punto di incontro tra gli stakeholder (clienti, utenti) e il team di sviluppo.
Serve a :
- Definire l'ambito : Stabilisce i confini del progetto (cosa è incluso e cosa no).
- Ridurre i rischi : Evita malintesi tra cliente e sviluppatori. Se una funzione non è nell'SRS, non deve essere sviluppata.
- Base per la stima : Permette di calcolare costi, tempi e risorse necessarie.
- Guidare il Testing : I tester usano l'SRS per scrivere i casi di test (se il requisito dice "X", il test deve verificare "X").
 
 L'SRS si colloca nella fase di Analisi dei Requisiti (Requirement Engineering), che è la seconda fase del ciclo di vita del software (SDLC), subito dopo lo Studio di Fattibilità e prima della Progettazione (Design).

Un buon SRS divide sempre i requisiti in due grandi categorie :
- Requisiti Funzionali : Descrivono cosa il sistema deve fare (es: "Il sistema deve permettere l'ingresso tramite badge").
- Requisiti Non Funzionali : Descrivono come il sistema deve essere (es: "Il sistema deve rispondere in meno di 2 secondi", "Il sistema deve essere sicuro").

Secondo lo standard IEEE 830, un SRS per essere considerato di qualità deve essere :
1. Corretto : Ogni requisito deve riflettere una reale necessità del cliente.
2. Non ambiguo : Ogni frase deve avere una sola interpretazione possibile (evitare termini come "veloce", "facile", "spesso").
3. Completo : Deve contenere tutti i requisiti significativi (funzioni, prestazioni, vincoli).
4. Coerente : Non devono esserci requisiti in contrasto tra loro (es. un punto dice "schermo blu" e un altro "schermo rosso").
5. Verificabile (Testabile) : Deve esistere un modo per controllare se il requisito è stato soddisfatto (es. misurando i tempi di risposta).
6. Tracciabile : Ogni requisito deve avere un identificativo unico (es. REQ-01) per poterlo seguire durante il design e il testing.
7. Modificabile : La struttura deve permettere aggiornamenti senza compromettere l'intero documento.

==4. Quali sono le fasi in cui si suddivide il processo di analisi dei requisiti ?==
Durante l'analisi dei requisiti, invece, vado a lavorare sui dati raccolti per elaborarli, interpretarli e affinarli. Nell'analisi dei requisiti i dati devono essere resi chiari, per eliminare ambiguità e incomprensioni, completi (comprendere tutte le esigenze e funzionalità richieste), coerenti (evitare conflitti tra i requisiti) e implementabili (pronti per la progettazione e sviluppo del sistema).

Ci sono 5 fasi dell'analisi dei requisiti :
1) Classificazione dei requisiti : suddividere i requisiti in categorie, funzionali e non funzionali e in vincoli.
2) Prioritizzazione : stabilire requisiti importanti e urgenti.
3) Conflitti e risoluzione : identificazione delle contraddizioni.
4) Modellazione e Rappresentazione : usare diagrammi, prototipi e casi d'uso.
5) Validazione : verificare con stakeholders che i requisiti definiti siano corretti e completi.

==5. E' possibile commettere degli errori nella fase dell'analisi dei requisiti ? Si tratta di errori facili da correggere o la cui correzione è rilevante nello sviluppo del Software ? In che modo possono essere corretti ?==
Sì, è estremamente comune commettere errori durante la fase di analisi. Spesso questi errori non sono di natura tecnica, ma comunicativa e logica.

Tipologie di errori comuni :
Gli errori si dividono solitamente in tre categorie :
- Omissione : Dimenticare un requisito fondamentale (es. non prevedere il recupero password in un sistema di login).
- Ambiguità : Scrivere un requisito che può essere interpretato in modi diversi dallo sviluppatore e dal cliente.
- Inconsistenza : Avere due requisiti che si contraddicono tra loro (es. "il sistema deve essere accessibile senza login" e "tutti i dati utente devono essere protetti da credenziali").

La gravità dell'errore : Facile o Rilevante ?
Gli errori nei requisiti sono i più difficili e costosi da correggere se scoperti in ritardo.
Secondo la celebre curva di Boehm, il costo di correzione di un errore cresce in modo esponenziale con il progredire delle fasi di sviluppo :
- Fase Requisiti : Se l'errore è trovato qui, il costo è quasi nullo (basta cancellare e riscrivere una riga sul documento SRS).
- Fase Implementation : Il costo aumenta (bisogna buttare via il codice già scritto).
- Fase Support/Maintenance : Il costo è massimo. Correggere un requisito sbagliato quando il software è già in produzione può costare fino a **100-200 volte di più** rispetto alla fase iniziale, poiché richiede di rifare design, codice e test.

In che modo possono essere corretti ?
Per correggere e, soprattutto, prevenire questi errori, si utilizzano diverse tecniche di Validation & Verification (V&V) :
- Requirement Reviews (Ispezioni) : Un gruppo di esperti e stakeholder legge il documento SRS per trovare errori, ambiguità o mancanze prima che inizi il design.
- Prototipazione rapida : Creare una versione "bozza" dell'interfaccia (mockup) per farla vedere al cliente. Spesso l'utente capisce cosa vuole solo quando vede qualcosa di concreto, permettendo di correggere i requisiti subito.
- Traceability Matrix (Matrice di Tracciabilità) : Uno strumento che collega ogni requisito a un caso di test. Se un requisito non ha un test, probabilmente è mal definito o incompleto.
- Formalizzazione : Tradurre i requisiti dal linguaggio naturale a modelli grafici (come gli Use Case Diagram di UML) per eliminare le ambiguità del linguaggio parlato.

### Design Pattern
==6. Java propone una specifica libreria per utilizzare il design pattern Observer. Spiegare il pattern e indicare in che modo e con quali varianti questa libreria implementa il pattern.==
Observer.
Il pattern Observer (o Publish-Subscribe) definisce una dipendenza uno-a-molti : quando un oggetto, detto Subject (Soggetto), cambia il suo stato, tutti gli oggetti dipendenti, detti Observer (Osservatori), vengono notificati e aggiornati automaticamente.
Questo pattern risolve il problema della consistenza dei dati tra classi correlate mantenendo un basso accoppiamento : il Subject non ha bisogno di conoscere i dettagli concreti degli Observer, sa solo che implementano una determinata interfaccia.

Componenti del Pattern : 
- Subject (Interfaccia/Classe astratta) : Gestisce l'elenco degli osservatori e i metodi per iscriverli (`attach`), rimuoverli (`detach`) e avvisarli (`notify`).
- Observer (Interfaccia) : Definisce il metodo di aggiornamento (es. `update()`) che verrà richiamato dal Subject.
- ConcreteSubject : L'oggetto reale che viene osservato. Quando il suo stato cambia, invoca il metodo di notifica.
- ConcreteObserver : L'oggetto che reagisce al cambiamento, implementando la logica specifica nel metodo `update()`.
![[Pasted image 20251231054726.png]]
Chiediti queste cose. Se la risposta è sì, allora corri a usare l'Observer :
1. **C'è un oggetto "importante" che cambia stato ?** (Es: Arriva un'email, il prezzo di un'azione in borsa sale, il personaggio di un gioco perde vita).
2. **Ci sono altri oggetti che devono "reagire" a questo cambiamento ?** (Es: Il computer deve suonare, il grafico della borsa deve aggiornarsi, la barra della vita sullo schermo deve accorciarsi).
3. **L'oggetto importante non sa (e non gli interessa) quanti sono quelli che lo guardano ?** (A Super-Pippo non importa se i fan sono 10 o 1 milione, lui manda lo stesso messaggio a tutta la lista).

La Libreria Java : `java.util.Observable` e `java.util.Observer`
Java ha fornito storicamente una implementazione pronta all'uso nel pacchetto `java.util`. Ecco come funziona e quali sono le sue particolarità :

Implementazione tramite Classe e Interfaccia :
A differenza del pattern "puro", Java utilizza una combinazione di classe e interfaccia :
- `java.util.Observable` (Classe) : Il Subject non è un'interfaccia, ma una Classe da estendere. Fornisce metodi come `addObserver()`, `deleteObserver()` e `notifyObservers()`.
- `java.util.Observer` (Interfaccia) : Gli osservatori devono implementare questa interfaccia che contiene l'unico metodo : `void update(Observable o, Object arg)`.

Il meccanismo del "Changed State" :
Una variante specifica della libreria Java è l'uso di un flag interno booleano chiamato `changed`. Prima di chiamare `notifyObservers()`, il ConcreteSubject deve obbligatoriamente chiamare il metodo `setChanged()`. Se non lo fa, la notifica non viene inviata. Questo serve a ottimizzare le prestazioni, evitando notifiche inutili se il cambiamento di stato è irrilevante.

Modalità Push e Pull in Java :
Java supporta entrambe le varianti tramite i parametri del metodo `update(Observable o, Object arg)` :
- Pull : Se il parametro `arg` è `null`, l'Observer riceve solo il riferimento al Subject (`o`) e deve "estrarre" i dati usando i metodi getter del Subject.
- Push : Se il Subject passa un oggetto specifico tramite `arg` (es. `notifyObservers(datiNuovi)`), l'Observer riceve direttamente i dati aggiornati.

==7. Un principio di Design del SW indica di favorire architetture che usano composizione, rispetto a quelle che usano ereditarietà. Per quale motivo ? Utilizzare qualche esempio per descrivere il concetto.==
Questo principio, spesso riassunto nella frase "Favor Composition over Inheritance", è un pilastro della programmazione a oggetti moderna. Sebbene l'ereditarietà sia uno dei concetti base del paradigma OOP, un suo uso eccessivo può rendere il codice rigido e difficile da mantenere.

L'Ereditarietà è una relazione rigida (is-a) :
L'ereditarietà crea un legame fortissimo tra classe padre e classe figlia (accoppiamento forte). Se la classe padre cambia, tutte le classi figlie potrebbero "rompersi".
- Problema : È una relazione statica, definita a tempo di compilazione. Non puoi cambiare il comportamento di un oggetto una volta creato.

B. La Composizione è una relazione flessibile (has-a) :
La composizione consiste nel costruire un oggetto inserendo al suo interno riferimenti ad altri oggetti.
- Vantaggio : È una relazione dinamica. Puoi cambiare il comportamento di un oggetto a tempo di esecuzione (Runtime) semplicemente sostituendo l'oggetto contenuto con un altro.

Il problema della "Fragile Base Class" :
Con l'ereditarietà, la sottoclasse dipende dai dettagli implementativi del padre. Se il padre viene modificato per correggere un bug, potrebbe inavvertitamente alterare il comportamento della sottoclasse che faceva affidamento su quella specifica logica. La composizione incapsula il comportamento, rendendo ogni pezzo indipendente.

Esempio Pratico : La gestione dei Robot
Immaginiamo di voler creare diversi tipi di Robot.

Approccio con Ereditarietà (Rigido) :
Creiamo una classe base `Robot` e poi sottoclassi come `RobotVolante` e `RobotCingolato`.
- Il problema : Cosa succede se voglio un robot che sia sia volante che cingolato ? In Java (e in molti altri linguaggi) non esiste l'ereditarietà multipla. Dovrei creare una terza classe `RobotVolanteCingolato` duplicando il codice, portando a una "esplosione" di classi.

Approccio con Composizione (Flessibile) :
Creiamo una classe `Robot` che **possiede** un oggetto `Movimento`.
Java
```
public class Robot {
    private Movimento tipoMovimento; // COMPOSIZIONE

    public Robot(Movimento m) {
        this.tipoMovimento = m;
    }

    public void muoviti() {
        tipoMovimento.esegui();
    }
}
```
- Il vantaggio : Ora posso creare un solo oggetto `Robot` e decidere al momento se deve volare o camminare passandogli l'oggetto `Volo` o `Camminata`. Se in futuro voglio aggiungere il movimento "Sott'acqua", creo solo la piccola classe `Nuoto` senza toccare la classe `Robot`.

==8. Per ogni pattern introdotto a lezione (Strategy, Observer, Decorator, Factory,  Template, Composite)   può essere chiesto :
	- Motivazione/ Uso/ Funzionamento/ Esempio rilevante/ PseudoCodice/ Applicazione a un determinato ambito;
	- Class Diagram; 
	- In che modo il diagramma soddisfa un principio di programmazione.==
Strategy.
Il principio del pattern Strategy è identificare gli aspetti dell'applicazione che variano e separarli da ciò che rimane invariante. 
Nello strategy si programma attraverso le interfacce e non con le implementazioni, perché questo permette alle classi di variare dinamicamente il loro comportamento, rendendo così gli algoritmi intercambiabili a runtime. 
Quando una classe “Context” esegue delle operazioni che richiedono l’implementazione di un algoritmo, è facile pensare di includere l’algoritmo direttamente nella definizione dell’oggetto, che ne dovrà fare utilizzo, ma ciò violerebbe il principio di Singola Responsabilità e il principio di Aperto/Chiuso. Tuttavia, gli algoritmi necessari allo svolgimento di una determinata operazione potrebbero variare nel tempo, rendendo necessaria la modifica della classe “Context” (e delle sottoclassi che ereditano da essa). 
Questo Design Pattern consiste nell’incapsulare un algoritmo all’interno di una classe, mantenendo un’interfaccia generica. Il tutto si traduce nel seguente diagramma delle classi :
![[Pasted image 20251231053532.png]]
Strategy dichiara l’interfaccia della nostra classe di algoritmi, che viene utilizzata da Context, per invocare un algoritmo concreto. 
ConcreteStrategy sono i nostri algoritmi concreti, ovvero implementano uno specifico algoritmo, che espone l’interfaccia Strategy. 
Context è la classe di contesto, che invoca la ConcreteStrategy.

Se ti trovi davanti a un problema, chiediti queste tre cose. Se la risposta è sì, allora serve il Pattern Strategy :
1. **C'è un'azione principale che rimane sempre la stessa ?** (Es: Zog deve sempre "Muoversi", o un sito deve sempre "Pagare").
2. **Ci sono tanti modi diversi per fare quell'azione ?** (Es: Camminare/Volare, oppure Carta di Credito/PayPal/Bitcoin).
3. **Voglio poter cambiare il "modo" velocemente senza smontare tutto il sistema ?** (Es: Cambiare scheda a Zog mentre sta già correndo).

Observer.
Il pattern Observer (o Publish-Subscribe) definisce una dipendenza uno-a-molti : quando un oggetto, detto Subject (Soggetto), cambia il suo stato, tutti gli oggetti dipendenti, detti Observer (Osservatori), vengono notificati e aggiornati automaticamente.
Questo pattern risolve il problema della consistenza dei dati tra classi correlate mantenendo un basso accoppiamento : il Subject non ha bisogno di conoscere i dettagli concreti degli Observer, sa solo che implementano una determinata interfaccia.

Componenti del Pattern : 
- Subject (Interfaccia/Classe astratta) : Gestisce l'elenco degli osservatori e i metodi per iscriverli (`attach`), rimuoverli (`detach`) e avvisarli (`notify`).
- Observer (Interfaccia) : Definisce il metodo di aggiornamento (es. `update()`) che verrà richiamato dal Subject.
- ConcreteSubject : L'oggetto reale che viene osservato. Quando il suo stato cambia, invoca il metodo di notifica.
- ConcreteObserver : L'oggetto che reagisce al cambiamento, implementando la logica specifica nel metodo `update()`.
![[Pasted image 20251231054726.png]]
Chiediti queste cose. Se la risposta è sì, allora corri a usare l'Observer :
1. **C'è un oggetto "importante" che cambia stato ?** (Es: Arriva un'email, il prezzo di un'azione in borsa sale, il personaggio di un gioco perde vita).
2. **Ci sono altri oggetti che devono "reagire" a questo cambiamento ?** (Es: Il computer deve suonare, il grafico della borsa deve aggiornarsi, la barra della vita sullo schermo deve accorciarsi).
3. **L'oggetto importante non sa (e non gli interessa) quanti sono quelli che lo guardano ?** (A Super-Pippo non importa se i fan sono 10 o 1 milione, lui manda lo stesso messaggio a tutta la lista).

Decorator.
Il design pattern Decorator fornisce un’alternativa flessibile all’ereditarietà, per estendere la funzionalità degli oggetti. Tale pattern consente di arricchire dinamicamente, a run-time, un oggetto con nuove funzionalità : è possibile impilare uno o più decorator uno sopra l’altro, ciascuno aggiungendo nuove funzionalità.
![[Pasted image 20251231055604.png]]
La struttura del decorator pattern si compone di quattro elementi principali : 
Component rappresenta l’interfaccia dell’oggetto che dovrà essere decorato dinamicamente.
ConcreteComponent rappresenta l’oggetto a cui andranno aggiunte le nuove funzionalità.
Decorator rappresenta l’interfaccia tra il Component e i ConcreteDecorator, possiede un riferimento al Component e un’interfaccia ad esso conforme.
ConcreteDecorator rappresentano gli oggetti che aggiungono le funzionalità ai ConcreteComponent.

Fatti queste domande. Se la risposta è sì, allora usa il Decorator :
1. **Ho un oggetto base a cui voglio aggiungere "abilità" o "caratteristiche" extra?** (Es: Un'arma che può diventare "infuocata" o "ghiacciata").
2. **Queste aggiunte possono essere combinate tra loro in mille modi diversi ?** (Es: Posso volere l'arma infuocata E ghiacciata contemporaneamente).
3. **Voglio poter aggiungere o togliere questi pezzi "al volo" mentre il programma gira ?** (Es: Il personaggio beve una pozione e ottiene un potere temporaneo).

Factory.
Factory method : 
Definisce un’interfaccia per creare oggetti, ma lascia alle sottoclassi la decisione del tipo di classe da istanziare. 
Il pattern può rivelarsi utile quando una classe non è in grado di conoscere a priori il tipo di oggetti da creare, o quando si vuole delegare la creazione di un oggetto alle sottoclassi. 
L’applicazione del pattern consente di eliminare le dipendenze dai tipi concreti utilizzati. 
È molto utile quando : una classe non è in grado di sapere in anticipo le classi di oggetti che deve creare, la creazione di un oggetto preclude il suo riuso, senza una significativa duplicazione di codice, la creazione di un oggetto richiede l’accesso ad informazioni, o risorse che non dovrebbero essere contenute nella classe di composizione, la gestione del ciclo di vita degli oggetti gestiti deve essere centralizzata, in modo da assicurare un comportamento coerente all’interno dell’applicazione, o le classi delegano le responsabilità di creazione.
![[Pasted image 20251231061002.png]]
Possiamo individuare i seguenti componenti : 
Creator dichiara la Factory che avrà il compito di ritornare l’oggetto appropriato.
ConcreteCreator effettua l’override del metodo della Factory, al fine di ritornare l’implementazione dell’oggetto.
Product definisce l’interfaccia dell’oggetto che deve essere creato dalla Factory.
ConcreteProduct implementa l’oggetto in base ai metodi definiti dall’interfaccia Product.
![[Pasted image 20251231061146.png]]

Fatti queste domande. Se la risposta è sì, allora ti serve una Factory :
1. **Il mio programma deve creare degli oggetti, ma non so ancora di che tipo preciso saranno ?** (Es: Un gioco di mostri dove i mostri nascono a caso: a volte un Drago, a volte un Goblin).
2. **Voglio che chi usa l'oggetto non sappia come è stato costruito ?** (Es: Voglio usare un "Database", ma non voglio sapere se è di tipo MySQL o Oracle).
3. **Voglio poter aggiungere nuovi tipi di oggetti senza cambiare tutto il codice principale ?** (Es: Domani voglio aggiungere il "Robot-Ninja" al mio negozio senza dover spiegare a tutti i clienti come si monta).

Abstract factory :
Questo pattern fornisce un’interfaccia per la creazione di famiglie di oggetti correlati o dipendenti, senza specificarne le loro classi concrete.
![[Pasted image 20251231061733.png]]
È composta da : 
AbstractFactory definisce l’interfaccia di riferimento per gli oggetti che creano le istanze.
ConcreteFactory implementa in modo concreto l’interfaccia definita da AbstractFactory e crea effettivamente una tipologia specifica di oggetti appartenenti ad una famiglia.
AbstractProduct definisce l’interfaccia di riferimento per una famiglia di oggetti da creare tramite il factory corrispondente.
ConcreteProduct implementa in modo concreto l’oggetto appartenente alla famiglia, per cui vale l’interfaccia AbstractProduct e che viene creato dall’oggetto factory corrispondente.
Client utilizza unicamente le classi astratte del factory e dell’oggetto da creare, senza conoscerne gli aspetti implementativi. 
L’annullamento dell’accoppiamento tra il client e gli oggetti concreti è ottenuto tramite l’inversione delle dipendenze. 
Una differenza tra l’Abstract Factory e il Factory Method è che, con il primo una classe delega la responsabilità di istanziare un oggetto ad un altro oggetto tramite la composizione, mentre il secondo utilizza l’ereditarietà e si basa su una sottoclasse per gestire l’istanza dell’oggetto desiderato.

Chiediti queste cose. Se la risposta è sì, allora ti serve questa "Super-Fabbrica" :
1. **Devo creare tanti oggetti diversi che però devono stare bene insieme ?** (Es: In un gioco, il set di armi, armature e scudi di un "Cavaliere" contro quelli di un "Alieno").
2. **Ho diverse "famiglie" o "stili" tra cui scegliere ?** (Es: Il mio programma deve girare su Windows e su Mac. Se gira su Windows, tutti i bottoni e le finestre devono avere lo stile Windows. Se gira su Mac, devono avere tutti lo stile Mac).
3. **Voglio evitare che l'utente mescoli pezzi di famiglie diverse ?** (Es: Non voglio che il mio programma usi un bottone di Windows dentro una finestra di Mac).

Questa è la parte dove molti si confondono, ma per te sarà semplicissimo :
- **Factory Method :** Crea **un solo tipo** di oggetto (es. solo la Pizza). È una singola ricetta.
- **Abstract Factory :** Crea **un'intera famiglia** di oggetti diversi ma correlati (es. Sedia + Tavolo + Divano). È un catalogo intero.

Template Method.
Si tratta di un pattern comportamentale basato su classi e viene utilizzato per definire la struttura di un algoritmo, delegando alcuni passi di dettaglio alle sottoclassi. 
Questo pattern nasce dall’esigenza di specificare l’ordine delle operazioni da effettuare, ma di delegare alle sottoclassi l’implementazione di alcune operazioni. Pertanto, il metodo che definisce l’algoritmo viene implementato nella superclasse, mentre i metodi che definiscono i comportamenti di dettaglio vengono dichiarati astratti nella superclasse ed implementati nelle sottoclassi. 
L’utilizzo di questo pattern permette di : implementare una sola volta la parte “immutata” dell’algoritmo e di consentire alle sottoclassi di implementare il comportamento delle parti “variabili”, individuare comportamenti comuni delle sottoclassi e “promuoverli” a comportamenti della superclasse, in modo da evitare la duplicazione di codice, individuare comportamenti NON comuni delle sottoclassi e definire un metodo di gancio hook per consentire alle sottoclassi di implementare uno specifico comportamento. 
L’utilizzo di questo pattern si presenta con una serie di variazioni, anche se per una completa aderenza alle intenzioni occorrerebbe che rispettasse alcune caratteristiche : la superclasse venga dichiarata "abstract" in modo da non poter essere instanziata dal Client, il metodo template venga dichiarato "final", in modo tale che le sottoclassi non siano in grado di modificarlo e cambiare il suo comportamento, i metodi primitivi vengano dichiarati abstract nella superclasse e vengano implementati nelle sottoclassi, le sottoclassi non invochino direttamente il metodo concreto della superclasse ma lascino che sia la superclasse ad invocarli all’occorrenza, Principio di Hollywood : “non chiamarci, ti chiameremo noi”, minimizzare il numero di metodi primitivi per evitare che lo sviluppatore delle sottoclassi debba implementare troppi metodi per poter usare questo pattern, creare un metodo concreto hook vuoto tra le fasi dell’algoritmo, per permettere agli sviluppatori di sovrascriverlo ed implementare un passaggio logico da loro richiesto. 
Questo pattern è composto dai seguenti partecipanti : 
AbstractClass definisce il metodo concreto ed i metodi primitivi astratti. Il metodo concreto richiama i metodi primitivi implementati nelle sottoclassi.
ConcreteClass implementa i metodi primitivi per svolgere i passi specifici dell’algoritmo ed eventualmente i metodi hook.
![[Pasted image 20251231063017.png]]
Tale pattern presenta i seguenti vantaggi/svantaggi : occorre comprendere quali sono i comportamenti comunemente implementati dalle sottoclassi e “promuoverli” come comportamenti della superclasse in modo da centralizzarli ed evitare la duplicazione del codice, occorre permettere alle sottoclassi di poter definire un comportamento durante l’esecuzione dell’algoritmo tramite l’introduzione di un metodo “hook” che possono ma non sono obbligate a ridefinire.

Fatti queste domande. Se la risposta è sì, allora usa il Template :
1. **Ho diversi processi che seguono quasi tutti la stessa sequenza di passi ?** (Es: Caricare un file: Apri -> Leggi -> Chiudi. Cambia solo _come_ leggi se è un PDF o un Excel).
2. **Voglio che la struttura generale sia protetta e non cambiata, ma voglio permettere di personalizzare i dettagli ?** (Es: In un gioco, tutti i mostri "Nascono", "Attaccano" e "Muoiono" nello stesso ordine, ma ognuno attacca in modo diverso).
3. **Ho molto codice duplicato tra classi simili ?**

La differenza sottile : Template vs Strategy
Questa è la domanda "tranello" tipica degli esami. Ecco come non sbagliare mai :
- **Strategy :** Tu cambi **tutto l'algoritmo** (cambi tutta la scheda). L'oggetto "contesto" non sa nulla di cosa farà la scheda. È una scelta di "cosa usare".
- **Template Method :** La struttura è **fissa**. Tu cambi solo **alcuni pezzetti** dentro una procedura più grande che rimane sempre quella. È una scelta di "come personalizzare un pezzo".

Composite.
Si tratta di un pattern strutturale basato su oggetti, che viene utilizzato quando si ha la necessità di realizzare una gerarchia di oggetti, in cui l’oggetto contenitore può detenere oggetti elementari e/o oggetti contenitori. 
L’obiettivo è di permettere al Client, che deve navigare la gerarchia, di comportarsi sempre nello stesso modo, sia verso gli oggetti elementari e sia verso gli oggetti contenitori. 
Questo pattern è composto dai seguenti partecipanti : 
Client colui che effettua l’invocazione all’operazione di interesse.
Component definisce l’interfaccia degli oggetti della composizione.
Leaf rappresenta l’oggetto foglia della composizione, non ha figli e definisce il comportamento “primitivo” dell’oggetto della composizione. 
Composite definisce il comportamento degli oggetti usati come contenitori e detiene il riferimento ai componenti “figli”.
![[Pasted image 20251231063733.png]]
Tale pattern presenta i seguenti vantaggi/svantaggi : gli oggetti della gerarchia possono essere composti da oggetti semplici e/o da oggetti contenitori, che a loro volta sono composti ricorsivamente da altri oggetti semplici e/o da oggetti contenitori, il Client tratta gli oggetti semplici e gli oggetti contenitori nello stesso modo. Questo semplifica il suo lavoro, il quale astrae dalla specifica implementazione, l’alberatura è facilmente modificabile aggiungendo/rimuovendo foglie e contenitori.

Fatti queste tre domande. Se la risposta è sì, allora serve il Composite :
1. **I miei oggetti formano una struttura a "albero" ?** (Cioè ci sono rami che hanno foglie o altri rami).
2. **Voglio poter ignorare la differenza tra un oggetto singolo e un gruppo di oggetti ?** (Es: Voglio poter dire "Sposta" sia a un file che a una cartella intera senza cambiare comando).
3. **Un contenitore può contenere altri contenitori dello stesso tipo ?** (Scatole dentro scatole).

### Design : Architecture and Methodology
==9. Che cosa indicano i principi di programmazione SOLID ?==
I principi di programmazione SOLID sono 5 :
1) Single Responsibility Principle (SRP) - Principio di responsabilità unica : 
	Una classe dovrebbe avere una, ed una sola, ragione per cambiare. 
	Responsabilità diverse implicano classi separate. Una classe dovrebbe svolgere un unico compito ben definito e non essere sovraccaricata da diverse funzionalità. 
	Serve per mantenere il codice più modulare, leggibile e manutenibile (se una classe ha una sola responsabilità è più facile localizzare e modificare il codice associato a quella specifica funzionalità). Inoltre, serve per ridurre il rischio di bug (modificare una funzionalità non dovrebbe influenzare un’altra). 
	Si tratta di classi piccole e con un solo scopo, che possono essere riutilizzate in contesti diversi.
	
	Esempio :
	![[Pasted image 20251231095313.png]]
	Se in questo caso CFO decidesse di modificare un algoritmo condiviso anche da COO, come RegularHours, queste modifiche se le ritroverebbe anche COO che magari non le vuole !
	![[Pasted image 20251231095435.png]]
	Soluzione :
	![[Pasted image 20251231095510.png]]

1) Open Closed Principle (OCP) - Principio aperto e chiuso :
	Dovresti essere in grado di estendere il comportamento di una classe, senza modificarla.
	 Si dice che il codice è aperto alle estensioni e chiuso alle modifiche, perché il codice esistente non dovrebbe essere modificato ogni volta che aggiungiamo una nuova funzionalità, ma dovrebbe essere progettato in modo da consentire l’estensione del comportamento tramite l’aggiunta di nuovo codice. 
	 Il codice è più stabile, manutenibile, flessibile di fronte ai cambiamenti dei requisiti. 
	 La struttura è modulare e riutilizzabile.

	Esempio :
	Abbiamo un sistema per calcolare il bonus per i dipendenti basato sul loro ruolo. 
```
	Public class BonusCalculator { 
		Public double calculateBonus(String role, double salary) { 
			If(role.equals(“developer”)) { 
				Return salary * 0.2; 
			} 
			Else if (role.equals(“manager”)) { 
				Return salay*0.3; 
			} 
			else { 
				return 0; 
			}
		}
	}
```
Se volessimo aggiungere un nuovo ruolo come “designer” dovremmo modificare il codice esistente aggiungendo un altro `if`, violando l’OCP, quindi usiamo il polimorfismo, per rispettare questo principio, estendendo il comportamento senza modificare il codice esistente.
Creo un’interfaccia per calcolare il bonus :
```
	Public interface BonusPolicy { 
		Double calculateBonus(double salary); 
	} 
```
Implemento in diverse classi adesso :
```
	Public class DeveloperBonusPolicy implements BonusPolicy { 
		Public double calculateBonus(double salary) {
			return salary *0.2; 
		}
	} 

	Public class ManagerBonusPolicy implements BonusPolicy { 
		Public double calculateBonus(double salary) {
			return salary * 0.3; 
		}
	} 

	Public class BonusCalculator { 
		Public double calculateBonus(BonusPolicy policy, double salary) { 
			Return policy.calculateBonus(salary);
		}
	}
```

3) Liskov Substitution Principle (LSP) - Principio di sostituzione di Liskov :
	Le classi derivate devono essere sostituibili con le rispettive classi base. 
	Il principio di sostituzione di Liskov è importante nel contesto dell’ereditarietà. 
	Le classi derivate devono essere pienamente compatibili con la classe base e comportarsi come ci si aspetta dalla classe base. 
	Caratteristiche fondamentali di questo principio di programmazione sono la flessibilità, la robustezza e la modularità. 
	Importante è non utilizzare l’ereditarietà. 
	Bisogna progettare con interfacce, per definire comportamenti comuni.
	![[Pasted image 20251231100756.png]]
	![[Pasted image 20251231100813.png]]

4) Interface Segregation Principle (ISP) - Principio di segregazione dell'interfaccia :
	Realizzare interfacce a grana fine specifiche per il cliente. 
	Un’interfaccia dovrebbe essere progettata in modo che ogni classe che la implementa debba fornire solo ciò di cui ha effettivamente bisogno, senza obblighi di implementare metodi inutili. 
	Questo principio di programmazione riduce le dipendenze inutili (non implementare metodi che non verranno mai usati).

	Esempio :
	![[Pasted image 20251231101544.png]]
	Anziché implementare un’unica grande interfaccia, implementiamo delle interfacce più piccole e specifiche.

5) Dependency Inversion Principle (DIP) - Principio di inversione delle dipendenze :
	Dipendere dalle classi astratte, non dalle concrete. 
	I moduli di alto livello non dovrebbero dipendere dai moduli di basso livello. Entrambi dovrebbero dipendere da astrazioni. 
	Le astrazioni non dovrebbero dipendere dai dettagli. 
	I dettagli dovrebbero dipendere dalle astrazioni. 
	Così il codice diventa meno rigido alle modifiche, più testabile e meno fragile.

	Esempio :
	Abstract Factory.
	Supponiamo di avere un sistema di creazione di oggetti per diverse famiglie di prodotti (database… o connessioni API). 
	Con DIP separiamo modulo di alto livello da dettagli di basso livello.
```
	//creiamo un'interfaccia comune per definire un comportamento comune per il DB 
	public interface Database { 
		void saveOrder(String order); 
	} 
	
	//Creiamo 2 implementazioni concrete di basso livello per rappresentare 2 DB diversi 
	public class MySQLDatabase implements Database { 
		@Override 
		void saveOrder(String order) { 
			System.out.println("Ordine ..."); 
		} 
	} 
	
	public class PostgreeSQLDatabase implements Database { 
		@Override 
		void saveOrder(String order) { 
			System.out.println("order...");
		} 
	} 
	
	//Creo abstract Factory per definire l'interfaccia che mi permette di creare i prodotti 
	public interface DatabaseFactory{ 
		Database createDatabase(); 
	} 
	
	public class MySQLFactory implements DatabaseFactory { 
		@Override 
		public Database createDatabase() { 
			return new MySQLDatabase(); 
		} 
	} 
	
	public class PostgreeFactory implements DatabaseFactory { 
		@Override 
		public Database createDatabase() { 
			return new PostgreeSQLDatabase(); 
		} 
	} 
	
	//Service --> modulo di alto livello che usa le implementazioni senza conoscere i dettagli 
	public class OrderService { 
		private Database database; 
		
		/*dependency injection 
		(pattern di progettazione, che consente di iniettare le dipendenze, cioè gli oggetti di cui una classe ha bisogno per funzionare dall’esterno, invece di crearle all’interno della classe stessa. 
		Si promuove la separazione delle responsabilità rendendo codice più modulare e testabile. 
		3 modi : 
		1) le dipendenze vengono fornite alla classe tramite il costruttore; 
		2) dipendenze fornite tramite metodo setter pubblico; 
		3) classe dipendente implementa interfaccia per avere dipendenza)*/ 
		
		public OrderService(DatabaseFactory factory) { 
			this.database = factory.createDatabase(); 
		} 
		
		public void processOrder(String order) { 
			System.out.println("Processo ordine" + order); 
			database.saveOrder(order); 
		}
	} 
	
	public class Main { 
		public static void main(String[] args) { 
			DatabaseFactory mySQLdatabse = new MySQLFactory(); 
			OrderService orderServiceMySQL= new OrderService(mySQLdatabse); 
			orderServiceMySQL.processOrder("ordine 123"); 
		}
	}
```
![[Pasted image 20251231102711.png]]
	Così button non dipende da un’implementazione concreta come lampada che è una cosa specifica.
	![[Pasted image 20251231102806.png]]

==10. Secondo i principi della clean architecture, in che modo si può valutare la coesione dei moduli del SW ? Si tratta di qualcosa di importante, o può essere trascurata ?==
Nella Clean Architecture, la coesione dei moduli non è un concetto astratto, ma un parametro tecnico misurabile che determina la manutenibilità di un sistema. La coesione risponde alla domanda : "In base a quale criterio decidiamo che queste classi devono stare nello stesso pacchetto/modulo ?"

Come valutare la Coesione : I tre principi (REP, CCP, CRP) :
La valutazione avviene bilanciando tre tensioni contrastanti, spesso rappresentate nel Diagramma di Tensione della Coesione dei Componenti.
- REP (Reuse/Release Equivalence Principle) : Valuta la coesione in ottica di rilascio. Se le classi di un modulo non possono essere rilasciate insieme sotto un unico numero di versione e una documentazione comune, il modulo non è coeso.
- CCP (Common Closure Principle) : Valuta la coesione in ottica di manutenzione. Si chiede : "Se cambio un requisito, devo aprire un solo modulo o dieci ?". Se una modifica forza il cambiamento di più moduli, la coesione è bassa. Le classi che cambiano per la stessa ragione devono essere raggruppate.
- CRP (Common Reuse Principle) : Valuta la coesione in ottica di dipendenza. Se un modulo contiene classi che non vengono usate insieme, gli utenti saranno costretti a ri-validare il loro codice anche per modifiche a parti che non utilizzano. È un segnale di coesione "forzata" che va evitata.

L'importanza della Coesione : Può essere trascurata ?
Assolutamente no. La coesione non può essere trascurata perché la sua assenza porta a due problemi catastrofici :
1. L'architettura a "Spaghetti" : Senza CCP, ogni piccola modifica si propaga a macchia d'olio su tutto il sistema.
2. L'esplosione delle dipendenze : Senza CRP, i moduli diventano pesanti e interdipendenti, rendendo impossibile il riutilizzo di singole funzionalità.
Tuttavia, Robert C. Martin sottolinea che la coesione è dinamica. Inizialmente, un team può favorire il CCP (sviluppo rapido), ma man mano che il progetto matura e altri team iniziano a riutilizzare i moduli, l'attenzione deve spostarsi verso il REP e il CRP.

Misurare la stabilità e l'astrazione (Le Metriche) :
Mentre la coesione si valuta con i principi sopra descritti, la qualità delle relazioni tra i moduli si misura matematicamente per evitare l'accoppiamento rigido.
- Instabilità ($I$) : Misura il rapporto tra le dipendenze in uscita (Fan-out) e il totale delle dipendenze.
	$$I = \frac{\text{Fan-out}}{\text{Fan-in} + \text{Fan-out}}$$
	Un modulo con $I=0$ è una "roccia" (molti dipendono da lui), un modulo con $I=1$ è "fragile" (dipende da tutti).
- Astrazione ($A$) : Misura quante interfacce/classi astratte sono presenti rispetto al totale delle classi ($N_c$).
	$$A = \frac{N_a}{N_c}$$
  

La Sequenza Principale (Main Sequence) :
La coesione e l'accoppiamento sono bilanciati correttamente quando i moduli si posizionano sulla "Sequenza Principale" : una linea ideale dove i moduli stabili sono astratti (per poter essere estesi senza modifiche) e i moduli instabili sono concreti (perché contengono la logica che cambia spesso).

> Conclusione : Valutare la coesione significa trovare il punto di equilibrio tra la facilità di sviluppo (CCP) e la facilità di riutilizzo (REP/CRP). Trascurarla significa condannare il software a diventare un "monolito inestensibile" nel giro di pochi cicli di rilascio.

### Design : Characteristics and Metrics

==11. Che cosa si intende per Software Metrics ? E' sempre vantaggioso definire e utilizzare delle misure quantitative che descrivono il Software ? Introdurre una misura che si trova particolarmente interessante./ E' importante utilizzare delle metriche per qualificare il codice di un Software ? A cosa servono le metriche ? Proporre esempi di metriche.==
Una Metrica Software è una misura quantitativa del grado in cui un sistema, un componente o un processo possiede una determinata proprietà. Si tratta di strumenti oggettivi essenziali per :
- Controllare : Monitorare lo stato di avanzamento di un progetto.
- Valutare : Misurare la qualità e la complessità del codice prodotto.
- Predire : Stimare costi, tempi e risorse per cicli di sviluppo futuri.

Le metriche si dividono in tre categorie principali :
1. Metriche di Prodotto : (es. LOC, complessità, manutenibilità) analizzano il software "finito".
2. Metriche di Processo : (es. tempo medio di rimozione dei bug) analizzano l'efficacia del metodo di lavoro.
3. Metriche di Progetto : (es. budget consumato, numero di sviluppatori) analizzano la gestione operativa.

Il valore delle misure quantitative : È sempre vantaggioso usarle ?
L'utilizzo delle metriche è fondamentale ma non sempre vantaggioso se fatto acriticamente.
- Perché sono importanti : Senza dati quantitativi, la qualità del codice rimane un'opinione soggettiva. Le metriche permettono di individuare "punti caldi" (hotspots) nel codice che potrebbero nascondere bug o essere difficili da manutenere.
- I rischi del "Numerismo" : Come giustamente osservato, l'uso improprio delle metriche può essere fuorviante.
    - Legge di Goodhart : Quando una metrica diventa un obiettivo (es. premiare chi scrive più righe di codice), perde il suo valore di misura perché gli sviluppatori inizieranno a scrivere codice ridondante pur di soddisfare il parametro.
    - Mancanza di contesto : Le metriche non dicono "perché" un valore è alto; forniscono solo un segnale che richiede il giudizio umano per essere interpretato correttamente.

Un esempio interessante : La Complessità Ciclotomatica ($v(G)$) :
Mentre le righe di codice (LOC) sono una misura puramente dimensionale, la Complessità Ciclotomatica di McCabe è una metrica di struttura molto più raffinata.
- Cos'è : Misura il numero di cammini linearmente indipendenti attraverso il grafo di controllo di un programma. In parole povere, conta il numero di decisioni (if, switch, cicli) presenti nel codice.
- Perché è interessante : Fornisce un limite superiore al numero di test necessari per coprire ogni ramo del codice.
    - Un valore tra 1 e 10 indica un codice semplice e ben testabile.
    - Un valore superiore a 20-30 indica un codice ad alto rischio, difficile da capire e con un'alta probabilità di contenere bug.
    - È una metrica che spinge verso il refactoring : se la complessità è troppo alta, la funzione deve essere spezzata in componenti più piccoli (favorendo la coesione).

Conclusioni sulla qualità del software :
Qualificare il codice tramite metriche è indispensabile per la moderna ingegneria del software. Tuttavia, la qualità non è data dal "vincere" contro un numero, ma dall'usare quel numero come bussola. Una metrica di qualità dovrebbe essere sempre :
1. Attendibile : Deve misurare ciò che si propone di misurare.
2. Facile da raccogliere : Idealmente tramite strumenti di analisi statica automatizzati (come SonarQube).
3. Orientata all'azione : Deve suggerire dove intervenire (es. "questa classe ha troppe dipendenze, bisogna disaccoppiarla").

==12. Indicare cosa si intende per analisi statica del Software e illustrarne i vantaggi.==
L’Analisi Statica è il processo di esame del software (codice sorgente, bytecode o documentazione) che viene eseguito senza mandare in esecuzione il programma. Si contrappone all'analisi dinamica, che invece richiede l'esecuzione del codice per osservarne il comportamento.

Aspetti analizzati (Cosa viene misurato ?) :
L'analisi statica si concentra sulla struttura e sulla qualità intrinseca del codice. Le metriche principali includono :
- Metriche Dimensionali : Linee di Codice (LOC) e Punti Funzione (FP).
- Metriche di Complessità : Complessità Ciclotomatica (McCabe) per la testabilità, e complessità di Halstead per lo sforzo cognitivo.
- Architettura e Design : Valutazione dell’Accoppiamento e della Coesione, identificazione di Codice Duplicato (Copy-Paste) e analisi del livello di nidificazione.
- Standard di Codifica : Verifica del rispetto di regole sintattiche, convenzioni di naming e identificazione di potenziali vulnerabilità di sicurezza (es. SQL Injection o Buffer Overflow rilevabili dal codice).

I Vantaggi dell'Analisi Statica :
L'adozione sistematica dell'analisi statica offre vantaggi cruciali per la qualità del progetto :
- Rilevamento Precoce dei Difetti (Early Bug Detection) : Permette di individuare errori logici o violazioni di sicurezza non appena il codice viene scritto. È noto che correggere un bug nella fase di codifica costa fino a 100 volte meno che correggerlo dopo il rilascio.
- Oggettività e Ripetibilità : A differenza della revisione manuale, l'analisi statica automatizzata fornisce dati numerici oggettivi (es. "questo metodo ha una complessità di 15"), rendendo le valutazioni indipendenti dal giudizio personale dello sviluppatore.
- Miglioramento della Manutenibilità : Identificando codice eccessivamente complesso o nidificato, l'analisi statica spinge il team verso il refactoring, garantendo che il software sia più facile da aggiornare ed evolvere nel tempo.
- Conformità agli Standard : Assicura che tutto il team di sviluppo segua le stesse regole stilistiche e di sicurezza, rendendo il codice uniforme e leggibile per chiunque subentri nel progetto.
- Riduzione del Debito Tecnico : Monitorando metriche come la duplicazione del codice o l'accoppiamento, si evita l'accumulo di scelte di design povere che rallenterebbero lo sviluppo futuro.

Strumenti e Automazione :
L'analisi statica viene raramente eseguita a mano. Si avvale di strumenti di Static Analysis Security Testing (SAST) o dashboard di qualità come SonarQube. Questi strumenti integrano l'analisi direttamente nella pipeline di sviluppo, bloccando ad esempio il caricamento di codice che non rispetta i parametri di qualità minimi prefissati.

Integrazione : Statica vs Dinamica (Sintesi) :
Mentre l'analisi statica è eccellente per prevenire errori strutturali e garantire la qualità del design, l'analisi dinamica rimane indispensabile per misurare la Code Coverage (copertura dei test) e le prestazioni reali (memoria e CPU), che sono invisibili al solo esame del codice sorgente.

Un software di alta qualità nasce dall'integrazione di entrambe le tecniche.

==13. Che cosa si intende per coesione e accoppiamento di moduli Software ? Indicare se questa caratteristica è importante per la progettazione del Software e come è possibile valutare il grado di accoppiamento e coesione di un Software.==
Nella progettazione del software, le relazioni tra i moduli (classi, package o componenti) definiscono la robustezza del sistema. Il design ideale mira a creare sistemi fortemente coesi e debolmente accoppiati.

Definizioni :
- Coesione (Forza interna) : Indica il grado di unità funzionale di un modulo. Un modulo ad alta coesione contiene elementi (metodi, variabili) che sono strettamente correlati tra loro e lavorano per un unico scopo (conforme al _Single Responsibility Principle_).
- Accoppiamento (Forza esterna) : Indica il grado di interdipendenza tra due o più moduli. Un basso accoppiamento significa che un modulo ha una conoscenza limitata degli altri, interagendo solo attraverso interfacce ben definite.

Perché queste caratteristiche sono importanti ?
Questi concetti non sono solo estetici, ma influenzano direttamente i costi e la vita del software :
- Manutenibilità : Se i moduli sono debolmente accoppiati, posso modificare il codice interno di uno senza "rompere" gli altri.
- Riutilizzabilità : Un modulo altamente coeso che fa una sola cosa è facilmente trasportabile in un altro progetto. Un modulo "accoppiato" si porta dietro troppe dipendenze, rendendone impossibile il riuso isolato.
- Testabilità : È più semplice scrivere test unitari per moduli isolati (basso accoppiamento) che per blocchi di codice intrecciati tra loro.
- Comprensibilità : Un modulo con un'unica responsabilità è più facile da leggere e comprendere per un nuovo sviluppatore.

Come valutare il grado di Coesione e Accoppiamento :
La valutazione può essere qualitativa (revisione del codice) o quantitativa, utilizzando metriche specifiche che analizzano i flussi di informazione.

Metrica di Henry-Kafura (Information Flow) :
Questa metrica valuta la complessità di un modulo analizzando come le informazioni entrano ed escono da esso.
- Fan-in : Numero di moduli che chiamano il modulo in esame (indica popolarità o responsabilità).
- Fan-out : Numero di moduli chiamati dal modulo in esame (indica dipendenza).

La formula della complessità del modulo ($C_p$) è :
$$C_p = (\text{fan-in} \times \text{fan-out})^2$$
Interpretazione : Un valore di $C_p$ anomalo suggerisce che il modulo sta facendo troppe cose (bassa coesione) o dipende da troppi elementi (alto accoppiamento), rendendolo un punto critico per il sistema.

Metrica di Card e Glass :
Si concentra sulla distinzione tra la struttura delle chiamate e lo scambio di dati :
1. Complessità Strutturale ($S$) : Legata al fan-out ($S = f_{out}^2$). Misura quanto il modulo è "ramificato" verso l'esterno.
2. Complessità dei Dati ($D$) : Misura il traffico di variabili attraverso l'interfaccia del modulo.

L'obiettivo è minimizzare la complessità totale per garantire che il sistema non diventi un "monolito fragile", dove ogni cambiamento genera effetti collaterali imprevedibili.

==14. Indicare, anche attraverso esempi, cosa si intende per coesione dei moduli Software.==
La Coesione è una metrica intra-modulare che misura quanto gli elementi interni a un modulo (metodi, variabili, istruzioni) siano strettamente correlati tra loro. Un modulo ad alta coesione è focalizzato su un'unica responsabilità (seguendo il Single Responsibility Principle), rendendo il software più semplice da testare, mantenere e riutilizzare.

 I Livelli di Coesione (Scala di Myers) :
La qualità della coesione viene valutata su una scala che va dal livello più debole (negativo) al più forte (ideale).

|**Livello**|**Descrizione**|**Esempio Pratico**|
|---|---|---|
|**Coincidenziale** (Minima)|Gli elementi sono raggruppati casualmente.|Una classe `Utility` che contiene sia il calcolo del codice fiscale che la formattazione di una stringa SQL.|
|**Logica**|Elementi raggruppati perché eseguono funzioni simili, ma diverse.|Una funzione `Stampa(tipo)` che gestisce sia la stampa su carta che l'invio via email tramite un `if/else`.|
|**Temporale**|Elementi raggruppati perché eseguiti nello stesso momento.|Un metodo `InizializzaSistema()` che apre il database, carica i file di log e resetta i contatori della UI.|
|**Procedurale**|Gli elementi seguono una specifica sequenza di esecuzione.|Una funzione che prima legge i dati da un file, poi ne controlla i permessi e infine li scrive nel DB.|
|**Comunicativa**|Gli elementi operano sugli stessi dati di input o output.|Una classe che ha vari metodi per calcolare statistiche diverse (media, mediana, varianza) sullo stesso array di dati.|
|**Funzionale** (Massima)|Il modulo esegue un'unica operazione logica ben definita.|Una classe `CalcolatoreIVA` che espone un unico metodo per calcolare l'imposta dato un importo.|

Metriche per la valutazione della Coesione :
Oltre alla valutazione qualitativa, esistono criteri quantitativi per misurare la coesione analizzando il flusso dei dati all'interno del modulo :
- Slice e Token : Si analizzano le porzioni di codice (Slice) che influenzano una specifica variabile (Token).
    - Glue Token : Sono variabili utilizzate in più di uno slice. Indicano che diverse parti del codice "parlano" degli stessi dati.
    - Superglue Token : Sono variabili comuni a tutti gli slice del modulo. La loro presenza è il segnale statistico della massima coesione funzionale.
- LCOM (Lack of Cohesion of Methods) : Una metrica orientata agli oggetti che misura quante coppie di metodi in una classe non condividono attributi comuni. Un alto valore di LCOM suggerisce che la classe dovrebbe essere divisa in due o più moduli più piccoli.

Importanza del bilanciamento con l'Accoppiamento :
Sebbene la coesione debba essere massimizzata, l'architetto software deve monitorare anche l'Accoppiamento (inter-modulare).:
- Accoppiamento Afferente ($Ca$) : Misura la responsabilità. Se un modulo altamente coeso ha molte dipendenze in entrata, diventa un pilastro del sistema.
- Accoppiamento Efferente ($Ce$) : Misura la dipendenza. Un modulo dovrebbe idealmente dipendere da pochi altri moduli stabili per evitare l'effetto "domino" in caso di modifiche.

### Implementation
==15. Indicare gli aspetti più importanti della fase di implementazione. E' considerata buona norma riscrivere più volte il codice ? E' ritenuta una buona norma spiegare con commenti dettagliati che operazioni compie una specifica linea di codice complessa ?==
La fase di implementazione (o codifica) non è solo la traduzione dei requisiti in linguaggio di programmazione, ma è il momento in cui si definisce la qualità interna del software.

Aspetti più importanti dell'implementazione :
I fattori critici che determinano il successo di questa fase sono :
- Rispetto degli standard di codifica : L'uso di convenzioni di naming e stili condivisi dal team per rendere il codice "collettivo".
- Modularità e Coesione : Scrivere codice seguendo i principi SOLID, garantendo che ogni componente abbia una sola responsabilità.
- Gestione degli Errori : Implementare una gestione delle eccezioni robusta che non faccia crashare il sistema e fornisca log significativi.
- Testabilità : Scrivere codice che sia facilmente verificabile tramite Unit Test.
- Utilizzo del Versioning : Gestire il codice tramite sistemi come Git, permettendo la tracciabilità delle modifiche e la collaborazione.

Riscrivere il codice : Refactoring o Spreco?
È considerata ottima norma riscrivere il codice, ma con una distinzione fondamentale : non parliamo di "buttare via tutto", ma di Refactoring.
- Il concetto di Refactoring : È il processo di ristrutturazione del codice esistente senza cambiarne il comportamento esterno. L'obiettivo è migliorare la leggibilità, ridurre la complessità e rimuovere il "debito tecnico".
- Perché è necessario : Spesso la prima versione di un codice serve a "risolvere il problema" (funzionalità). La seconda o terza revisione serve a "scriverlo bene" (manutenibilità).
- La regola del boy scout : "Lascia il codice sempre un po' più pulito di come lo hai trovato". Riscrivere piccole porzioni di codice per migliorarle è un segno di professionalità, non di indecisione.

 Commenti dettagliati : Aiuto o "Odore di Codice" ?
Contrariamente a quanto si possa pensare, commentare ogni singola linea di codice complessa non è considerata una buona norma. Ecco perché :
- Il Codice deve essere Auto-esplicativo : Il miglior commento è un codice scritto così bene da non averne bisogno. Se una linea è troppo complessa, la soluzione non è spiegarla con un commento, ma semplificarla (ad esempio estraendo una parte della logica in una funzione con un nome significativo).
- Il rischio del disallineamento : I commenti spesso "mentono". Quando il codice viene modificato durante la manutenzione, gli sviluppatori tendono a dimenticare di aggiornare i commenti. Un commento non aggiornato è più pericoloso di nessun commento.
- Quando usare i commenti :
    - Perché, non cosa : I commenti dovrebbero spiegare le motivazioni strategiche (il "perché" di una scelta insolita), non la sintassi (il "cosa" sta facendo il codice).
    - Documentazione API : Per interfacce pubbliche (es. Javadoc) destinate ad altri sviluppatori.
    - Warning : Per avvertire di effetti collaterali non ovvi.

> In sintesi : Se senti il bisogno di commentare una linea di codice perché è troppo complessa, quel codice ha probabilmente un basso livello di leggibilità. Invece di commentare, dovresti applicare il Refactoring.

==16. E' opportuno creare dei commenti al codice ? In che modo possono essere classificati i commenti ? ==
L'inserimento di commenti nel codice è un'operazione che richiede equilibrio. Sebbene siano nati per migliorare la comprensibilità, la moderna ingegneria del software promuove il concetto di "Self-Documenting Code" (codice auto-esplicativo) : l'idea che un codice ben scritto debba parlare da sé attraverso nomi di variabili e funzioni chiare, riducendo al minimo la necessità di spiegazioni esterne.

Quando è opportuno commentare ?
L'opportunità di inserire un commento dipende dal valore informativo che aggiunge.
- Sì : Quando spiegano il perché di una scelta progettuale insolita o vincoli di business non evidenti.
- No : Quando tentano di spiegare un codice scritto male (i cosiddetti "commenti di scusa"). In questo caso, la buona norma impone il refactoring della logica piuttosto che l'aggiunta di testo.

Classificazione dei Commenti :
I commenti possono essere classificati in sei categorie, ognuna con un diverso impatto sulla qualità del software :
1. Ripetizioni del codice (Rumore) : Commenti ridondanti che descrivono letteralmente la sintassi (es. `x++ // incrementa x`). Sono considerati dannosi perché appesantiscono il file senza aggiungere informazione.
2. Spiegazioni del codice : Tentano di tradurre algoritmi complessi. Spesso indicano che il codice potrebbe essere semplificato o spezzato in funzioni più piccole.
3. Marker (Segnaposto) : Etichette come `// TODO:` o `// FIXME:`. Sono utili per tracciare attività pendenti, ma non dovrebbero mai rimanere nel codice in fase di produzione a lungo termine.
4. Riassuntivi : Forniscono una panoramica di un intero modulo o classe. Sono utili per chi legge il codice per la prima volta per inquadrare il contesto macroscopico.
5. Descrittivi dell'intento : Descrivono il razionale dietro una scelta (es. "Utilizziamo questo algoritmo di ordinamento perché i dati in ingresso sono quasi sempre già ordinati"). Sono i commenti più preziosi perché l'intento non è quasi mai deducibile dalla sola sintassi.
6. Riferimenti esterni : Forniscono link a specifiche tecniche, normative legali o ticket del bug-tracker (es. `// Segue specifica ISO-9001 per il calcolo dei pesi`).

Rischi e Buone Pratiche (Trade-off) :
L'uso dei commenti comporta dei costi nascosti che vanno gestiti con attenzione :
- Il problema dell'obsolescenza : Il codice cambia, ma i commenti raramente vengono aggiornati con la stessa frequenza. Un commento disallineato dal codice è una delle principali fonti di errore durante la manutenzione, poiché fornisce informazioni fuorvianti.
- Refactoring vs Commento : Se una porzione di codice è difficile da capire, la prima strategia deve essere migliorare i nomi delle variabili o estrarre metodi (metodologia "Extract Method"). Il commento deve essere l'ultima risorsa.
- Documentazione API : Una distinzione importante va fatta per i commenti di documentazione (come Javadoc in Java o Doxygen in C++). Questi non sono destinati a chi legge il codice sorgente, ma a chi utilizza le librerie, e sono considerati fondamentali per le interfacce pubbliche.

==17. Che cos'è il debugging e di quali fasi si compone ?==
Il Debugging è l'attività sistematica e iterativa volta a individuare la causa primaria di un malfunzionamento e a rimuoverla. Mentre il testing è un'attività di controllo qualità che evidenzia la presenza di un errore (il "sintomo"), il debugging è un'attività di sviluppo che mira alla sua risoluzione definitiva.

Le Fasi del Processo di Debugging :
Per evitare di procedere per tentativi ("trial and error"), il processo deve seguire quattro fasi logiche :
1. Stabilizzazione (Riproduzione) : È la fase più importante. Un bug che non si può riprodurre non può essere corretto. Consiste nel trovare l'insieme minimo di condizioni (input, configurazione, stato del sistema) che scatenano sistematicamente il malfunzionamento.
2. Localizzazione : Si restringe il campo d'indagine dal sistema intero alla singola unità di codice responsabile. In questa fase si usano strumenti come il debugger (per l'esecuzione passo-passo) o l'inserimento di log.
3. Correzione : Si modifica il codice sorgente. Una buona correzione non deve essere una "patch" superficiale, ma deve risolvere la causa radice (root cause) del problema.
4. Verifica : Si controlla che il bug sia sparito. È fondamentale eseguire Test di Regressione : si verifica cioè che la modifica non abbia alterato il corretto funzionamento di altre parti del sistema (effetto domino).

Classificazione degli Errori :
Gli errori possono essere classificati in base al momento in cui emergono e alla loro natura :
- Errori Sintattici : Violazioni delle regole del linguaggio. Vengono rilevati durante l'analisi statica (compilatore o IDE).
- Errori di Runtime (Eccezioni) : Il codice è sintatticamente corretto ma fallisce durante l'esecuzione (es. divisione per zero, puntatore nullo). Portano spesso al crash del programma.
- Errori Logici : Il programma gira, ma il risultato è sbagliato (es. calcolo errato dell'IVA). Sono i più costosi da correggere perché richiedono una profonda comprensione del dominio del problema.

Terminologia Tecnica (Standard IEEE) :
Per una risposta eccellente, è utile distinguere tra :
- Error (Errore) : L'azione umana errata (es. il programmatore dimentica un `if`).
- Fault / Defect (Difetto) : La manifestazione dell'errore nel codice (la riga di codice sbagliata).
- Failure (Guasto) : L'incapacità del software di eseguire la funzione richiesta (l'utente vede un errore a schermo).

> Il debugging è il passaggio che va dalla Failure (guasto osservato) alla rimozione del Fault (difetto nel codice).

Strumenti di Supporto :
Il debugging moderno si avvale di :
- Debugger : Strumenti che permettono di inserire breakpoint (punti di interruzione), ispezionare il valore delle variabili in tempo reale e avanzare istruzione per istruzione.
- Print Debugging/Logging : Inserimento di messaggi di tracciamento per ricostruire il flusso di esecuzione in ambienti dove non è possibile usare un debugger (es. sistemi in produzione).

==18. Che cosa si intende per refactoring del codice ? A cosa serve ? Ci sono rischi connessi con questa operazione ?==
Il Refactoring è una tecnica disciplinata volta a modificare la struttura interna di un codice sorgente per migliorarne la qualità, la leggibilità e la manutenibilità, senza alterarne in alcun modo il comportamento esterno.

A cosa serve ? (Obiettivi) :
Il refactoring non serve a correggere errori o aggiungere funzioni, ma a combattere il debito tecnico. I suoi scopi principali sono :
- Migliorare il Design : Riorganizzare il codice per rispettare principi come SOLID, riducendo l'accoppiamento e aumentando la coesione.
- Eliminare i "Code Smells" : Rimuovere "odori" del codice come il Long Method (metodi troppo lunghi), la Duplicate Code (codice copiato) o la Large Class (classi con troppe responsabilità).
- Semplificare la Manutenzione : Un codice pulito è più facile da comprendere per i nuovi sviluppatori, riducendo drasticamente i tempi e i costi di evoluzione del software.

Tecniche Comuni (Pattern di Refactoring) :
Esistono pattern standardizzati per operare in sicurezza :
- Extract Method : Si scompone un metodo complesso in parti più piccole e auto-esplicative.
- Introduce Parameter Object : Si raggruppano parametri correlati in un unico oggetto per pulire le firme dei metodi.
- Rename Variable/Method : Sembra banale, ma dare nomi significativi è la forma più potente di refactoring per la leggibilità.

Quali sono i rischi connessi ?
Il refactoring è un'operazione intrinsecamente rischiosa perché interviene su codice già funzionante. I rischi principali sono :
- Introduzione di Regressioni : Modificando la struttura, si possono inavvertitamente rompere logiche esistenti o introdurre nuovi bug.
- Spreco di Tempo (Over-engineering) : Esiste il rischio di dedicare troppo tempo a pulire codice che non verrà mai più toccato, trasformando il refactoring in un esercizio estetico poco utile al business.
- Conflitti di Merge : Nello sviluppo in team, refactorizzare classi centrali può causare enormi conflitti con il lavoro dei colleghi se non coordinato.
- Perdita di Performance : A volte, rendere il codice più leggibile (es. aggiungendo chiamate a metodo o nuovi oggetti) può comportare un lieve overhead prestazionale.

Come mitigare i rischi ? (Le "Reti di Sicurezza") :
Per rendere il refactoring un'attività sicura, è necessario seguire due regole d'oro :
1. Suite di Test Automatizzati : Non si deve iniziare il refactoring se non si ha una solida copertura di Unit Test. I test fungono da "rete di sicurezza" : se dopo una modifica i test passano ancora (Green), abbiamo la certezza matematica che il comportamento esterno non è cambiato.
2. Piccoli Passi (Baby Steps) : Il refactoring va fatto a piccoli incrementi. Ogni piccola modifica deve essere seguita dall'esecuzione dei test. Se qualcosa si rompe, è facile tornare indietro.

> In sintesi : Il refactoring è un investimento sulla salute a lungo termine del software. Se fatto senza test, è un azzardo; se fatto con i test, è la pratica che distingue un programmatore professionista da un dilettante.

==19. Nell'implementazione del codice che importanza assume l'ottimizzazione del codice che massimizzi la velocità di esecuzione del Software ?==
Nel contesto professionale, l'importanza dell'ottimizzazione per la velocità di esecuzione deve essere bilanciata con altri attributi di qualità come la leggibilità, la manutenibilità e la correttezza.

Il principio della "Premature Optimization" :
Citando Donald Knuth : "L'ottimizzazione prematura è la radice di tutti i mali".
Durante la fase di implementazione, la priorità assoluta è scrivere codice chiaro e corretto. Ottimizzare la velocità troppo presto comporta dei rischi :
- Riduzione della leggibilità : Spesso, per rendere un codice più veloce, lo si rende più complesso e difficile da capire per altri programmatori.
- Aumento del debito tecnico : Codice "astuto" o troppo ottimizzato a basso livello è più difficile da manutenere e da sottoporre a refactoring.
- Spreco di risorse : In molti sistemi gestionali o web, il collo di bottiglia non è la velocità del codice (CPU), ma l'accesso al database o la velocità della rete.

Quando l'ottimizzazione è davvero importante ?
L'ottimizzazione diventa una priorità solo in scenari specifici :
- Sistemi Real-Time o Embedded : Dove ci sono vincoli hardware stretti o necessità di risposte in millisecondi (es. software per frenata ABS).
- High Performance Computing (HPC) : Software per simulazioni scientifiche o elaborazione di Big Data.
- Algoritmi critici : Se una funzione viene eseguita milioni di volte al secondo, un piccolo risparmio ha un impatto enorme.

L'approccio corretto : Misurare prima di agire :
L'ingegnere del software non ottimizza "a sensazione", ma segue una strategia basata sui dati :
1. Scrivere codice pulito : Focalizzarsi sulla logica e sulla manutenibilità.
2. Profiling (Analisi Dinamica) : Una volta che il codice funziona, si utilizzano strumenti chiamati Profiler per misurare dove il software spende effettivamente più tempo.
3. Regola dell'80/20 (Principio di Pareto) : Solitamente l'80% del tempo di esecuzione è consumato dal 20% del codice. L'ottimizzazione va concentrata solo su quel 20%, lasciando il resto del codice leggibile e semplice.

Alternative all'ottimizzazione manuale :
Oggi si preferisce spesso migliorare le prestazioni agendo su altri livelli :
- Efficienza Algoritmica : Sostituire un algoritmo $O(n^2)$ con uno $O(n \log n)$ è molto più efficace che cercare di ottimizzare le singole istruzioni.
- Caching : Memorizzare risultati già calcolati invece di ricalcolarli.
- Hardware : Spesso è più economico comprare un server più potente che pagare settimane di lavoro di uno sviluppatore per ottimizzare poche righe di codice.

### Testing and Quality Assurance
==20. Indicare che cosa si intende con "White Box" Test e in che modo/che cosa verificano le principali tecniche di White Box Testing.==
Il White Box Testing (noto anche come Glass Box o Structural Testing) è una metodologia di test in cui la scelta dei casi di prova si basa sulla conoscenza della struttura logica interna e del codice sorgente del software. A differenza del Black Box, il tester "vede" dentro la scatola e progetta input per forzare il software a percorrere specifici sentieri logici.

Cosa verificano i test White Box ?
Queste tecniche mirano a verificare la correttezza della costruzione interna del programma, assicurandosi che :
- Tutte le istruzioni siano state eseguite.
- Tutte le decisioni logiche siano state testate in entrambi i rami (Vero/Falso).
- I flussi di dati interni e le strutture dati siano gestiti correttamente.
- Non vi siano porzioni di codice "morto" (mai raggiungibile).

Principali Tecniche di White Box Testing :
Le tecniche si misurano in base al livello di Coverage (copertura) che riescono a garantire :
- Statement Coverage (Copertura delle istruzioni) :
    - Cosa verifica : Che ogni riga di codice venga eseguita almeno una volta.
    - Limite : È il criterio più debole; potrebbe non testare rami condizionali vuoti (es. un `if` senza il relativo `else`).
- Decision/Branch Coverage (Copertura dei rami) :
    - Cosa verifica : Che ogni punto di decisione (if, switch, cicli) sia stato percorso in ogni sua uscita possibile. Se un `if` viene valutato sia come `true` che come `false`, la branch coverage è soddisfatta.
    - Vantaggio : È più rigorosa della statement coverage.
- Condition Coverage (Copertura delle condizioni) :
    - Cosa verifica : In espressioni logiche complesse (es. `if (A || B)`), verifica che ogni singola sotto-condizione (`A` e `B` separatamente) venga valutata sia come vera che come falsa.
- Path Coverage (Copertura dei percorsi) :
    - Cosa verifica : Tutti i possibili percorsi logici dall'ingresso all'uscita di una funzione.
    - Limite : In programmi complessi con molti cicli, il numero di percorsi può diventare infinito (esplosione combinatoria), rendendo questa tecnica applicabile solo a unità di codice molto piccole.

Misurazione della qualità : La Complessità Ciclotomatica :
Per supportare il White Box Testing, si utilizza spesso la metrica della Complessità Ciclotomatica ($v(G)$) di McCabe. Questa misura indica il numero di cammini linearmente indipendenti nel grafo di controllo.
- Utilità : Indica al tester esattamente quanti casi di test sono necessari, come minimo, per ottenere una Branch Coverage completa.

Vantaggi e Svantaggi (Trade-off) :
Il White Box è fondamentale ma presenta delle sfide :
- Vantaggi :
    - Permette di trovare errori di implementazione, refusi e logiche ridondanti.
    - È estremamente preciso e permette l'automazione (Unit Test).
    - Identifica rami di codice che i requisiti funzionali (Black Box) potrebbero non attivare mai.
- Svantaggi :
    - Richiede competenze di programmazione elevate.
    - È costoso in termini di tempo e risorse.
    - Non rileva i requisiti mancanti : Se una funzione è stata dimenticata del tutto, il White Box non potrà mai trovarla, poiché testa solo ciò che è stato effettivamente scritto.

> In sintesi : Il White Box testing è lo strumento principe per gli sviluppatori durante i Unit Test, garantendo che la "meccanica" del codice sia priva di difetti strutturali prima di passare ai test funzionali di alto livello.

==21. Indicare le differenze tra "Black Box" Test e "White Box" Test. L'analisi degli Use Case Diagram è utile per scrivere dei White Box Test efficaci ?==
Il testing del software si basa su due prospettive complementari che analizzano il sistema da angolazioni opposte : l'esterno (comportamento) e l'interno (struttura).

Black Box Testing (Test Funzionale) :
Il sistema è visto come una "scatola nera" : non se ne conosce l'implementazione.
- Focus : Rispondenza ai requisiti funzionali (cosa fa il software).
- Input : Specifiche, requisiti, Use Case.
- Tecniche : Partizionamento in classi di equivalenza, analisi dei valori limite.

White Box Testing (Test Strutturale) :
Il sistema è visto come una "scatola di vetro" : il codice è visibile.
- Focus : Correttezza del flusso logico e delle strutture dati (come è costruito).
- Input : Codice sorgente, diagrammi di flusso, diagrammi di sequenza.
- Tecniche : Copertura delle istruzioni (Statement Coverage), copertura dei rami (Branch Coverage), Loop Testing.

La seconda parte della domanda chiede se l'analisi degli Use Case Diagram sia utile per scrivere dei White Box Test efficaci.
La risposta è : Generalmente No.
Ecco le motivazioni tecniche :
1. Diverso livello di astrazione : Gli Use Case Diagram descrivono chi (attori) fa cosa (funzionalità) nel sistema dal punto di vista dell'utente. Sono strumenti di analisi dei requisiti e appartengono tipicamente al dominio del Black Box Testing.
2. Mancanza di dettagli implementativi : Un Use Case non dice nulla su come il codice è scritto, su quali istruzioni `if` vengono usate o su come sono strutturati i cicli. Per scrivere un test White Box efficace, servono documenti che descrivano la struttura interna, come :
    - Il Codice Sorgente.
    - I Diagrammi di Sequenza (che mostrano le chiamate tra oggetti).
    - I Diagrammi di Stato (che mostrano la logica interna di una classe).

Esiste una eccezione ?
L'analisi degli Use Case può essere utile indirettamente solo se si considerano i "Flussi Alternativi" o i "Casi d'Errore" descritti nella specifica testuale dell'Use Case. Questi possono suggerire al programmatore quali rami logici (branch) del codice devono essere assolutamente coperti dal White Box Test, ma lo Use Case Diagram di per sé (la parte grafica) rimane uno strumento quasi esclusivamente per il testing funzionale.

Sintesi Comparativa

| **Caratteristica**         | **Black Box Testing**        | **White Box Testing**                         |
| -------------------------- | ---------------------------- | --------------------------------------------- |
| **Conoscenza del codice**  | Nessuna                      | Totale                                        |
| **Riferimento principale** | Use Case Diagram, Specifiche | Codice sorgente, Diagrammi di classe/sequenza |
| **Focus**                  | Validazione dei requisiti    | Verifica della logica e copertura             |
| **Eseguito da**            | Tester, Utenti finali        | Sviluppatori (Unit Test)                      |

In conclusione : Per scrivere White Box Test efficaci, dovresti guardare più alla Complessità Ciclotomatica e alla struttura delle classi piuttosto che agli Use Case Diagram, che sono invece i tuoi migliori alleati per il Black Box Testing.

==22. Descrivere il concetto di Modified Condition/Decision Coverage ?==
La MC/DC è una metrica di copertura del codice avanzata che si colloca tra la semplice Branch Coverage e la complessa Multiple Condition Coverage. È stata progettata per testare in modo esaustivo le logiche booleane complesse senza richiedere un numero esorbitante di casi di test.

Il problema : L'esplosione combinatoria :
Se abbiamo una decisione con $n$ condizioni atomiche (es. if (A and B and C)), per testare tutte le combinazioni possibili servirebbero $2^n$ test (nel nostro caso $2^3 = 8$). In sistemi reali con decine di condizioni, questo è impossibile.
La MC/DC risolve il problema richiedendo solo $n + 1$ casi di test, mantenendo però un'altissima efficacia nel trovare bug logici.

Requisiti della MC/DC :
Secondo gli standard (come il DO-178C in avionica), per soddisfare la MC/DC ogni condizione atomica deve :
1. Influenzare il risultato della decisione indipendentemente.
2. Essere testata come Vera e come Falsa.
3. Dimostrare che, variando solo quella condizione e mantenendo fisse le altre, il risultato finale della decisione cambia.

Esempio Pratico : `if (A or B)` :
Per testare questa decisione con MC/DC servono $n+1 = 3$ test. Dobbiamo isolare l'influenza di ogni variabile :

| **Caso** | **A** | **B** | **Risultato** | **Note**                                                            |
| -------- | ----- | ----- | ------------- | ------------------------------------------------------------------- |
| **1**    | **F** | F     | **F**         | -                                                                   |
| **2**    | **V** | F     | **V**         | Cambiando solo A (da 1 a 2), il risultato cambia. A è indipendente. |
| **3**    | F     | **V** | **V**         | Cambiando solo B (da 1 a 3), il risultato cambia. B è indipendente. |

Nota : La combinazione (V, V) non è necessaria per la MC/DC in questo caso, perché non aiuta a dimostrare l'indipendenza di una singola variabile rispetto al fallimento.

Confronto con le altre metriche (Riepilogo) :
La MC/DC si inserisce in una gerarchia di rigore crescente :
1. Statement Coverage : Ho eseguito tutte le righe ? (Minimo sindacale).
2. Decision (Branch) Coverage : Ho preso tutte le uscite dei rami `if/else` ? (Buona norma).
3. Condition Coverage : Ogni singola sottocondizione è stata V/F ? (Non garantisce la copertura della decisione totale).
4. MC/DC : Ogni condizione influenza il risultato in modo provato e indipendente ? (Richiesto per sistemi critici).
5. Multiple Condition Coverage : Ho provato tutte le combinazioni possibili della tavola della verità ? (Spesso impossibile/ridondante).

Perché è importante ?
La MC/DC è considerata il "punto di equilibrio" perfetto : è molto più potente della Branch Coverage (perché guarda dentro le parentesi tonde degli `if`), ma è molto più economica della Multiple Condition Coverage. Permette di trovare errori nei programmatori che sbagliano operatori logici (es. usare `OR` invece di `AND`) che i test normali potrebbero non rilevare.

### Software Support and Maintenance
==23. Ci sono attività che una Software House dovrebbe avere la necessità di pianificare dopo il rilascio del Software ? Oppure con il rilascio del Software si ritiene generalmente concluso un progetto di sviluppo  di un Software ?==
Il rilascio del software segna il passaggio dalla fase di sviluppo alla fase di Esercizio e Manutenzione. È ampiamente dimostrato che questa fase può occupare dal 60% all'80% dell'intero ciclo di vita del software in termini di costi e risorse.

Le quattro categorie di Manutenzione :
Una Software House deve pianificare le attività post-rilascio suddividendole in quattro aree d'intervento, come previsto dagli standard di Ingegneria del Software (ISO/IEC 14764) :
- Manutenzione Correttiva (Reactive) : Risoluzione dei bug (difetti) residui che emergono solo nell'ambiente reale. Nonostante i test intensivi, l'uso massivo da parte degli utenti finali scopre sempre scenari non previsti.
- Manutenzione Adattativa : Aggiornamento del software per renderlo compatibile con i cambiamenti dell'ecosistema (es. nuove versioni di Android/iOS, patch di sicurezza del sistema operativo, o modifiche nelle normative fiscali come la fatturazione elettronica).
- Manutenzione Perfettiva (Evolutiva) : È l'attività più comune e riguarda il miglioramento delle prestazioni o l'aggiunta di nuove funzionalità per rispondere ai nuovi bisogni del business del cliente.
- Manutenzione Preventiva : Interventi "proattivi" per migliorare la struttura interna del codice (Refactoring), riducendo la probabilità che si verifichino guasti futuri e facilitando le manutenzioni successive.

Il concetto di "Software Aging" (Invecchiamento del Software) :
È importante pianificare queste attività perché il software, a differenza dei beni fisici, non si "logora", ma subisce un processo di deterioramento logico.
Se una Software House non pianifica la manutenzione, il software diventa obsoleto rapidamente a causa del cambiamento delle tecnologie circostanti. Questo porta al fenomeno del Debito Tecnico, dove ogni piccola modifica futura diventa sempre più costosa e rischiosa.

Il Dilemma Strategico : Manutenere o Rifare ?
La pianificazione post-rilascio serve anche a monitorare la convenienza economica del sistema. Arriva un momento nel ciclo di vita in cui la manutenzione diventa meno conveniente della Riprogettazione (Re-engineering).

|**Caratteristica**|**Continuare la Manutenzione**|**Riprogettazione (Re-engineering)**|
|---|---|---|
|**Costi Immediati**|Bassi (operativi)|Molto alti (investimento)|
|**Rischi**|Degradazione costante della qualità|Errori di migrazione e costi di formazione|
|**Flessibilità**|Limitata dall'architettura originale|Massima (nuove tecnologie)|

Attività non tecniche : Supporto e Training
Oltre alla scrittura del codice, la Software House deve pianificare :
- Help Desk e Supporto : Gestione delle segnalazioni e assistenza diretta agli utenti.
- Monitoraggio : Raccolta di metriche sull'utilizzo per capire quali funzioni sono realmente utili (utili per la manutenzione perfettiva).
- Customer Success : Garantire che il cliente ottenga il valore sperato dal software, fattore chiave per il rinnovo di licenze o contratti di assistenza.

==24. E' vero che una volta rilasciato il Software al cliente termina anche l'interazione della Software House con il cliente ? E lo stesso cliente perde importanza ? Descrivere l'importanza del post-vendita.==
In un mercato moderno, il software non è un prodotto "chiuso" (come un libro), ma un servizio continuo. L'idea che il rapporto finisca alla consegna è un retaggio del passato che non tiene conto della natura dinamica del digitale.

Il cliente non perde importanza : diventa un Partner :
Dopo il rilascio, il cliente diventa la principale fonte di informazioni per il miglioramento del prodotto.
- Feedback Reale : Solo l'utente finale può indicare quali funzioni sono davvero utili e quali sono troppo complesse.
- Fidelizzazione (Retention) : È molto più economico mantenere un cliente esistente tramite un buon supporto post-vendita che acquisirne uno nuovo. Un cliente soddisfatto nel post-vendita genera nuovi contratti di evoluzione del software.

L'importanza strategica del Post-Vendita :
La fase di supporto e manutenzione è fondamentale per tre ragioni principali :
- Affidabilità (Manutenzione Correttiva) : Nessun software è perfetto. Il supporto serve a gestire i bug che emergono solo quando il sistema viene messo sotto stress nel mondo reale.
- Evoluzione (Manutenzione Perfettiva) : Il mercato del cliente cambia. Se la Software House non interagisce più con lui, il software diventerà obsoleto in pochi mesi. Il post-vendita serve a pianificare nuove funzionalità per mantenere il software competitivo.
- Conformità (Manutenzione Adattativa) : Leggi, sistemi operativi e hardware si aggiornano continuamente. Senza un'interazione costante, il software smetterebbe di funzionare (es. un aggiornamento di Windows che rompe la compatibilità con il programma).

Attività chiave della fase di Supporto :
Una Software House deve pianificare queste interazioni tramite :
1. SLA (Service Level Agreement) : Contratti che definiscono i tempi di risposta in caso di problemi.
2. Help Desk : Un canale diretto di comunicazione per risolvere dubbi e raccogliere segnalazioni.
3. Training : Sessioni di formazione per assicurarsi che il cliente usi il software al 100% del suo potenziale.

Il Rischio dell'Abbandono :
Se la Software House interrompe l'interazione :
- Si accumula Debito Tecnico (il codice degrada).
- Si verifica il Software Aging (il software "invecchia" rispetto all'ambiente esterno).
- Il cliente, sentendosi abbandonato, si rivolgerà alla concorrenza per il prossimo progetto.

> In sintesi : Il rilascio è solo l'inizio di un ciclo di vita. La manutenzione e il supporto non sono "costi accessori", ma l'attività che garantisce la sopravvivenza stessa del prodotto software sul mercato.