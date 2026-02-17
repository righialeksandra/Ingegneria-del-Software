### Introduzione
==1. Quali sono le principali differenze nelle esigenze che intercorrono quando si programma un software di piccole dimensioni realizzato per soddisfare un'esigenza limitata e un software complesso ?==

Un ==SW di piccole dimensioni== è più facile capire meglio i ==requisiti==, che siano funzionali o non, perché le caratteristiche devono essere minori e per questo l'==effort estimation== risulta più accurato e lo ==scheduling== è relativamente semplice.
Quando si parla di SW di piccole dimensioni, progettato per risolvere un problema specifico, con funzionalità limitate e molto focalizzate, si ha un ==design== semplice e diretto, senza un'architettura troppo articolata.
In SW di piccole dimensioni la ==sicurezza== è meno critica e generalmente, questo SW, non richiede una ==gestione dei dati== complessa. La ==manutenibilità== è ridotta, con pochi interventi successivi e pochi aggiornamenti, testing limitato a scenari principali, spesso manuali e limitati a pochi casi d'uso. Questo SW non richiede grande ==coordinamento==, essendo realizzato da poche persone.

In un ==SW di grandi dimensioni== capire i ==requisiti== può risultare eccessivamente complicato e sovrastante, per questo l'==estimation effort== risulta meno accurato.
Oltre al ==designing== e al ==coding==, sono richieste altre persone per il ==testing==, ==integration== e ==tool support== e tanto più è grande il SW, tante più persone serviranno e saranno coinvolte, quindi aumenta la complessità della comunicazione e con essa gli errori.
Un grande SW richiede anche una ==progettazione modulare== e un'==architettura robusta e scalabile==, per poter gestire i diversi componenti. 
In un SW di grandi dimensioni posso avere un'architettura basata su ==servizi== e ==micro-servizi==, per supportare un'espansione futura e una distribuzione su più server. 
In SW di grandi dimensioni la ==sicurezza== è una priorità alta e deve gestire ==grandi volumi di dati==.


==2. Che cosa si intende per Ingegneria del Software e quali sono i problemi che questa disciplina si propone di affrontare ?==

L'==Ingegneria del Software== è una disciplina dell'Ingegneria Informatica, che si occupa dello ==sviluppo==, della ==progettazione==, della ==manutenzione==, della ==documentazione== e della ==gestione dei sistemi SW==, in modo sistematico, disciplinato e quantificabile.
L'Ingegneria del SW deve garantire che i SW siano di ==alta qualità==, ==a basso costo== e si basa su tecniche, strumenti e principi specifici per sviluppare e gestire il ciclo di vita di un SW.

La produzione di un SW è un processo composto di ==6 fasi== :
1) ==Analisi dei Requisiti== : comprendere i bisogni degli utenti e tradurli in requisiti funzionali e non funzionali.
2) ==Progettazione== : definire l'architettura del sistema, i componenti e l'interfaccia.
3) ==Sviluppo== : scrittura e implementazione del codice.
4) ==Test e Verifica== : il SW deve funzionare correttamente e soddisfare i requisiti.
5) ==Manutenzione== : miglioramenti, aggiornamenti e correzione di bug.
6) ==Gestione== : monitoraggio del progetto, coordinamento e pianificazione.

I ==problemi che affronta l'Ingegneria del Software== sono :
1) ==Complessità del SW== : suddividere un SW complesso in parti più piccole e semplici da gestire, attraverso decomposizione funzionale e modularizzazione.
2) ==Scalabilità== : il SW deve adattarsi ad un numero crescente di utenti o dati senza perdita di prestazioni.
3) ==Qualità== : prodotti affidabili, sicuri e performanti.
4) ==Gestione Tempi e Costi==.
5) ==Cambiamenti nei Requisiti== : deve garantire SW che sia flessibile e facile da cambiare, piuttosto che il SW funzioni correttamente.
6) ==Manutenzione== : il SW deve essere mantenuto rilevante e funzionante a lungo termine, tramite aggiornamenti.
7) ==Collaborazione e Coordinazione all'interno dei Team==.


==3. Che cosa implica la produzione di un software e qual è l'output generalmente atteso da questo processo ?==

La ==produzione di un software== è un ==processo complesso e iterativo==, che implica tutte le attività necessarie per progettare, sviluppare, testare, distribuire e mantenere un sistema SW : 
1) ==Analisi dei Requisiti== : raccogliere e documentare i bisogni degli utenti e degli stakeholder. Identificare sia i ==requisiti funzionali== (cosa deve fare il SW), sia quelli ==non funzionali== (usabilità, performance e sicurezza).
2) ==Progettazione (Design)== : definire componenti, moduli, interfacce e flussi dati. ==L'architettura del sistema deve essere manutenibile e scalabile==.
3) ==Sviluppo o Coding== : usare ==specifici linguaggi di programmazione, che garantiscono leggibilità==.
4) ==Test e Verifica== : verificare che il ==SW funzioni correttamente rispetto ai requisiti iniziali==. Eseguire test unitari, di integrazione, di sistema e di accettazione.
5) ==Documentazione== : creare ==documenti tecnici, manuali utente e guide di installazione per facilitare l'uso e la manutenzione del SW==.
6) ==Distribuzione e Rilascio== : garantire ==disponibilità per utenti e implementare il SW nell'ambiente di produzione==.
7) ==Manutenzione e Aggiornamento==.

L'==output==, generalmente, atteso è un ==SW funzionante==, che implementi correttamente tutte le funzionalità richieste dagli utenti, che sia affidabile e di qualità, senza bug critici, che sia capace di gestire una crescita delle richieste, o dei dati, senza perdita di prestazioni. Ossia, SW scalabile, che sia ben documentato, facile da utilizzare e accessibile, progettato in modo modulare e manutenibile, per consentire future estensioni e miglioramenti.


### Requirements Engineering
==1. Quali sono le principali fasi in cui il processo di specifica dei requisiti può essere suddiviso ?==

Le principali fasi in cui il processo di specifica dei requisiti può essere suddiviso sono :
1) ==Elicitazione (raccolta)== : in questa fase vengono ==identificati e raccolti i requisiti dagli stakeholders==, attraverso interviste, workshop, questionari, studio di documentazione esistente e da osservazione diretta. L'elicitazione può essere sia ==verbale==, che ==scritta==, che ==online==, ma si preferisce quella verbale. In questa fase devo ==comprendere le esigenze dell'utente==, i ==problemi== e gli ==obiettivi del progetto==, di conseguenza, può essere utile il ==prototyping==. Il prototyping viene utilizzato per comprendere meglio i requisiti degli stakeholders, aiutare gli utenti a visualizzare funzionalità, o interfacce, soprattutto se non riescono ad esprimere bene le loro esigenze. Il prototyping, quindi, ==aiuta ad identificare i requisiti impliciti e difficili da esplicitare, generando un feedback immediato sulle idee proposte==. Spesso, il prototipo in questo caso è ==low-fidelity== (schizzi, wireframe) e serve per stimolare discussioni.
2) ==Analisi dei Requisiti== : I requisiti raccolti vengono ==analizzati per identificare eventuali conflitti, o ambiguità, prioritizzarli e valutare i vincoli e la fattibilità tecnica==. Si include anche la ==modellazione== e la ==rappresentazione dei requisiti==, con diagrammi, casi d'uso, o scenari.
3) ==Specificazione dei Requisiti== : ==Documentazione dei requisiti in un documento chiamato "Specifiche dei requisiti SW" (SRS)==. I requisiti devono essere ==chiari== e ==non ambigui==, ==tracciabili==, ==completi== e ==consistenti==.
4) ==Validazione e Verifica== : Si verifica che i ==requisiti soddisfino le necessità degli stakeholders==, che siano ==completi==, ==corretti== e ==coerenti==, che siano ==comprensibili== per tutte le parti coinvolte. La validazione può avvenire ==attraverso revisioni, prototipi e simulazioni==. In questa fase, il ==prototyping== viene usato ==per verificare che i requisiti raccolti siano stati compresi correttamente==, ==per validare le aspettative degli stakeholders==, confrontandole con un prototipo più avanzato (high-fidelity), che simula in modo realistico il sistema e ==per ridurre il rischio di malintesi==, permettendo agli utenti di testare le funzionalità chiave.
5) ==Gestione dei Requisiti (Requirement Management)== : I requisiti possono cambiare e quindi ==eventuali modifiche devono essere controllate==. I requisiti devono essere ==tracciati== e ci deve essere un ==aggiornamento continuo della documentazione==.
6) ==Accettazione==.


==2. Qual è la differenza tra l’operazione di elicitation eseguita a alto livello e l'elicitation eseguita a livello di dettaglio ?==

L'elicitazione dei requisiti deve essere suddivisa in ==due livelli principali== :
1) ==Elicitazione ad Alto Livello== : ==si concentra sul livello generale di business e sugli obiettivi strategici del sistema, o del progetto==. L'==obiettivo== è ==identificare i requisiti generali e i bisogni principali degli stakeholders==. Il focus è sugli obiettivi del sistema e sul suo scopo, sulle funzionalità principali non dettagliate, sull'identificazione degli stakeholders coinvolti e sui vincoli globali (budget, tempistiche e tecnologie utilizzabili). 
	Come ==output== ci si aspetta una ==comprensione globale del contesto del progetto, più un elenco preliminare di requisiti o caratteristiche macro==.
	Le ==tecniche== utilizzate per eseguire un'elicitazione ad alto livello sono un'==analisi dei documenti esistenti==, unito a ==brainstorming==, ==riunioni iniziali con i team di progetto==, ==benchmarking rispetto a sistemi simili== e ==interviste generali con gli stakeholders chiave==.
2) ==Elicitazione a livello di dettaglio== : ==comprensione approfondita e specifica di ogni requisito==. Si devono ==dettagliare i requisiti identificati ad alto livello, per renderli implementabili==. Nell'elicitazione a livello di dettaglio ci si concentra sul ==dettaglio delle funzionalità== (requisiti funzionali), sulle ==specifiche tecniche== e sui ==requisiti non funzionali== (prestazioni, sicurezza, usabilità...), ==requisiti espliciti== e ==impliciti== e ==regole di business== e ==flussi operativi==.
	Come ==output== ci si aspetta ==documenti dettagliati dei requisiti== (SRS), insieme a ==diagrammi== (casi d'uso, modelli di processo...) e la ==tracciabilità dei requisiti==.
	Le ==tecniche== utilizzate per eseguire un'elicitazione a basso livello sono ==workshop con stakeholders specifici==, ==prototyping per chiarire dettagli==, ==analisi di casi d'uso==, ==osservazione diretta dei processi operativi== e ==questionari==. 

L'elicitazione ad alto livello è il punto di partenza per stabilire una base comune e definire i contorni del progetto. Da lì si passa al livello di dettaglio per garantire che ogni requisito sia chiaro e pronto per la progettazione e l'implementazione.


==3. Indicare le principali caratteristiche dell'analisi dei requisiti di alto livello e di dettaglio.==

1) ==Analisi dei Requisiti di Alto Livello== : richiede una ==comprensione generale del progetto, o sistema, favorendo una panoramica alta e poco dettagliata==. I requisiti di alto livello definiscono lo scopo generale del sistema, identificano gli obiettivi principali del progetto e i problemi che il sistema deve risolvere. I requisiti di alto livello devono determinare chi sono gli stakeholders principali (utenti, clienti, sponsor) e deve raccogliere le loro aspettative generali. L'analisi dei requisiti di alto livello si concentra su requisiti business o di sistema, evitando di entrare in dettagli tecnici, o operativi, analizza l'ambiente in cui il sistema opererà e stabilisce i vincoli globali, come tempo, budget e tecnologia.
	Come ==output== ci si aspetta un ==documento preliminare dei requisiti==, una ==lista di funzionalità principali e obiettivi== e ==priorità iniziali==.
	Le ==tecniche== utilizzate per un'analisi dei requisiti di alto livello sono ==brainstorming e workshop==, ==analisi dei documenti esistenti== e ==interviste a stakeholders==.
2) ==Analisi dei Requisiti di Dettaglio== : si tratta dell'==analisi dei requisiti identificati in precedenza e resi chiari, completi e implementabili==. L'analisi dei requisiti di dettaglio traduce i requisiti di alto livello in specifiche dettagliate e ==comprende sia i requisiti funzionali, che non funzionali, specificando cosa deve fare il sistema e come deve comportarsi==. L'analisi dei requisiti di dettaglio include vincoli tecnici, prestazioni richieste, sicurezza e usabilità e si assicura che i requisiti siano completi, coerenti e non ambigui, individuando incongruenze e conflitti nei requisiti. Per gestire eventuali modifiche future, si crea una matrice di tracciabilità. Ogni requisito viene collegato agli obiettivi aziendali e alle necessità degli stakeholders. 
	Come ==output== ci si aspetta ==documenti dettagliati dei requisiti (SRS)==, insieme a ==diagrammi== (casi d'uso, modelli di processo...), ==prototipi==, per confermare la validità dei requisiti.
	Le ==tecniche== utilizzate per un'analisi dei requisiti di basso livello sono ==prototyping==, ==workshop dettagliati==, ==analisi di casi d'uso==, ==simulazioni==.


==4. Cosa si intende per analisi dei requisiti e in che modo si differisce dall'operazione di elicitation ?==

==L'elicitazione è la fase iniziale di raccolta dei requisiti==.
==Nell'analisi, invece, vado a lavorare sui dati raccolti per elaborarli, interpretarli e affinarli==. Nell'analisi dei requisiti i ==dati== devono essere resi ==chiari==, per eliminare ambiguità e incomprensioni, ==completi== (comprendere tutte le esigenze e funzionalità richieste), ==coerenti== (evitare conflitti tra i requisiti) e ==implementabili== (pronti per la progettazione e sviluppo del sistema).

Ci sono ==5 fasi dell'analisi dei requisiti== :
1) ==Classificazione dei requisiti== : suddividere i requisiti in categorie, funzionali e non funzionali e in vincoli.
2) ==Prioritizzazione== : stabilire requisiti importanti e urgenti.
3) ==Conflitti e risoluzione== : identificazione delle contraddizioni.
4) ==Modellazione e Rappresentazione== : usare diagrammi, prototipi e casi d'uso.
5) ==Validazione== : verificare con stakeholders che i requisiti definiti siano corretti e completi.


==5. La prototipazione dei requisiti include anche la realizzazione di diagrammi UML di tipo Use Case. Che cosa si vuole rappresentare con questo tipo di diagrammi ? Quali sono le informazioni che rappresentano questo tipo di diagrammi.==

Gli ==Use Case Diagrams== sono una ==rappresentazione grafica in UML (Unified Modelling Language) utilizzata per descrivere il comportamento di un sistema dal punto di vista degli utenti e degli stakeholders==. Il diagramma Use Case si concentra su ==cosa fa il sistema==. 

Con il diagramma Use Case ==si vuole rappresentare== :
- ==Le funzionalità del sistema== : le funzioni e i servizi offerti agli utenti;
- ==Le interazioni tra attori e sistema==;
- ==Cos'è incluso ed escluso dal sistema==;
- ==Relazioni tra casi d'uso== : dipendenze, inclusioni, estensioni, generalizzazioni tra casi d'uso.

Come vengono rappresentate le informazioni con il diagramma Use Case :
- ==Attori== : entità esterne, che interagiscono con il sistema e possono essere primari (iniziano un'interazione per ottenere un obiettivo) e secondari (assisitono o collaborano);
- ==Casi d'Uso== : sono le funzionalità e i servizi, che il sistema offre agli attori e creano un flusso di eventi;
- ==Relazioni== : 
	- ==Associazioni== : collegamenti, tra attori e casi d'uso, che indicano chi utilizza una determinata funzione;
	- ==Include== : un caso d'uso include un altro caso d'uso come parte del suo flusso;
	- ==Extend==;
	- ==Generalizzazione== : gerarchia tra attori o casi d'uso.

I ==vantaggi== del diagramma Use Case sono una ==riduzione del rischio di scope creep== (rischio di aggiungere funzionalità non necessarie) e una ==rappresentazione facile e chiara da capire==.


==6. Introduzione di un problema che deve essere descritto dallo studente  con un diagramma UML di tipo Use Case.==

All'università, il sistema ESSE3 viene utilizzato dagli studenti, dai professori e dal personale di segreteria per gestire l'intera carriera accademica.
Uno studente può iscriversi agli esami; durante l'iscrizione il sistema mostra gli appelli disponibili, così lo studente può scegliere quello più adatto alle proprie esigenze. 
In alcuni casi, lo studente annulla un'iscrizione già effettuata, modificando così la propria situazione agli esami.

Durante il percorso di studi, lo studente organizza il proprio piano, di studio selezionando gli insegnamenti da seguire, mentre la segreteria verifica che le scelte siano corrette e conformi al regolamento. Ogni modifica del piano comprende la selezione degli insegnamenti, un'operazione che viene sempre eseguita come parte della gestione del piano di studio.

Quando lo studente si avvicina alla laurea, presenta la domanda alla segreteria, che controlla il completamento di tutti i requisiti e conferma la regolarità della carriera. In alcune situazioni, lo studente invia la tesi al professore per la valutazione; solo dopo l'approvazione del docente la segreteria può completare la pratica di laurea.
![[Pasted image 20251230161206.png]]


==7. Quali sono gli standard con cui si rappresentano i requisiti ?==

La rappresentazione dei requisiti è un processo fondamentale nell'ingegneria del software e dei sistemi, poiché garantisce che tutti gli stakeholder abbiano una visione condivisa del progetto.

1. ==Lo Standard Internazionale : ISO/IEC/IEEE 29148:2018== :
L'ISO/IEC/IEEE 29148:2018 è il principale standard internazionale per l'ingegneria dei requisiti. Esso ==definisce i processi e i prodotti necessari per documentare e gestire i requisiti lungo l'intero ciclo di vita del sistema==.
Caratteristiche principali dello standard :
- Classificazione : Distingue tra requisiti funzionali (cosa fa il sistema) e non funzionali (come lo fa : prestazioni, sicurezza, ecc.).
- Criteri di Qualità : Stabilisce che ogni requisito deve possedere sei caratteristiche fondamentali : chiarezza, concisione, verificabilità, completezza, consistenza (assenza di contraddizioni) e tracciabilità.
- Struttura dei documenti : Fornisce i template standard per i principali documenti di specifica (SRS, SyRS, ecc.).

2. ==La gerarchia di documentazione specifica== :
La documentazione dei requisiti segue una gerarchia che va dagli obiettivi di business ai dettagli tecnici.
A. Business Requirement Specification (BRS) :
È il documento di alto livello che spiega il perché del progetto.
- Obiettivo : Definire i traguardi strategici dell'organizzazione e i benefici attesi.
- Contenuto : Contesto aziendale, descrizione del problema, metriche di successo e vincoli di business.
B. Stakeholder Requirements Specification (StRS) :
Funge da "ponte" tra il business e la tecnica.
- Obiettivo : Raccogliere le esigenze e le aspettative di tutte le parti interessate (utenti, clienti, enti regolatori).
- Contenuto : Scenari di utilizzo e vincoli, espressi in un linguaggio comprensibile ai non tecnici ma strutturato.
C. System Requirements Specification (SyRS) :
Si utilizza per sistemi complessi che integrano sia hardware che software (es. sistemi automotive o aerospaziali).
- Obiettivo : Descrivere il funzionamento complessivo e l'integrazione tra le componenti.
- Contenuto : Architettura generale, interfacce tra componenti e requisiti di sistema totali.
D. Software Requirements Specification (SRS) :
È il documento tecnico di dettaglio focalizzato esclusivamente sul software.
- Obiettivo : Fornire agli sviluppatori una guida precisa su cosa deve essere implementato.
- Contenuto : Funzionalità dettagliate, specifiche tecniche, requisiti non funzionali (sicurezza, scalabilità) e diagrammi di modellazione.

2. ==Tecniche di Rappresentazione e Modellazione== :
Esistono diversi modi per descrivere i requisiti, combinando testo e modelli grafici.
Linguaggio Naturale :
È la forma più comune, ma per essere efficace deve seguire regole rigide :
- Utilizzo di frasi brevi e attive.
- Eliminazione di termini ambigui o soggettivi (es. "veloce", "intuitivo").
- Strutturazione tramite elenchi numerati per favorire la tracciabilità.
UML (Unified Modeling Language) :
UML fornisce un set di diagrammi standard per visualizzare i requisiti :
- Use Case Diagram (Diagramma dei Casi d'Uso) : Rappresenta le interazioni tra gli attori (utenti o altri sistemi) e le funzionalità del sistema, definendo il perimetro del progetto.
- Activity Diagram (Diagramma di Attività) : Descrive il flusso logico e operativo di un processo o di un caso d'uso.
- Nota : Sebbene i Data Flow Diagram (DFD) siano spesso associati all'analisi, essi appartengono tecnicamente alla metodologia Structured Analysis, ma vengono frequentemente integrati per mostrare il movimento dei dati.
Scenario-Based Modeling :
Questa tecnica utilizza narrazioni per descrivere l'interazione utente-sistema:
- User Stories : Brevi descrizioni (tipiche delle metodologie Agile) nel formato: _"Come [utente], voglio [azione], affinché [beneficio]"_.
- Scenari : Descrizioni dettagliate dei flussi principali (main flow) e dei flussi alternativi (eccezioni) che si verificano durante l'uso del sistema.


## Design Pattern
==1. Quali sono i principi di programmazione che motivano la realizzazione e l’uso di design pattern ?==

I i principi di programmazione, che motivano la realizzazione e l’uso di design pattern, servono per ==progettare un SW robusto==, ==riusabile== e ==manutenibile==. Questi principi guidano gli sviluppatori verso ==soluzioni standardizzate ed efficienti per affrontare problemi ricorrenti nel design del SW==. 
Alla base della creazione dei design pattern troviamo i ==principi di progettazione orientata agli oggetti== :
- ==Incapsulamento== : separare i dettagli dell’implementazione dall’uso del componente, per favorire la modularità e ridurre il rischio di errori (Façade + Decorator).
- ==Ereditarietà e Polimorfismo== : per evitare duplicazioni creiamo strutture gerarchiche e riutilizziamo il codice (Template Method).
- ==Composizione piuttosto che Ereditarietà==.


==2. Viene fornito uno scenario e viene richiesto di selezionare il pattern opportuno (giustificando la scelta) e di descrivere le classi principali anche attraverso il codice.==

    
==3. NON è richiesta la descrizione estratta dal libro della GoF (in alcuni design pattern è presente nelle slide).==


==4. Per ogni pattern introdotto a lezione (Strategy, Observer, Decorator, Factory, Singleton, Command, Adapter, Facade, Template, Iterator, Composite, State, Proxy, Builder, Bridge, Chain of Responsibility)   può essere chiesto :
	- Motivazione/ Uso/ Funzionamento/ Esempio rilevante/ PseudoCodice/ Applicazione a un determinato ambito;
	- Class Diagram; 
	- In che modo il diagramma soddisfa un principio di programmazione.==

==Strategy==.
Il ==principio== del pattern Strategy è ==identificare gli aspetti dell'applicazione che variano e separarli da ciò che rimane invariante==. 
Nello strategy ==si programma attraverso le interfacce== e non con le implementazioni, perché questo permette alle classi di variare dinamicamente il loro comportamento, rendendo così gli algoritmi intercambiabili a runtime. 
Quando una classe “Context” esegue delle operazioni che richiedono l’implementazione di un algoritmo, è facile pensare di ==includere l’algoritmo direttamente nella definizione dell’oggetto, che ne dovrà fare utilizzo==, ma ciò ==violerebbe il principio di Singola Responsabilità e il principio di Aperto/Chiuso==. Tuttavia, gli algoritmi necessari allo svolgimento di una determinata operazione potrebbero variare nel tempo, rendendo necessaria la modifica della classe “Context” (e delle sottoclassi che ereditano da essa). 
Questo Design Pattern consiste nell’==incapsulare un algoritmo all’interno di una classe, mantenendo un’interfaccia generica==. Il tutto si traduce nel seguente diagramma delle classi :
![[Pasted image 20251231053532.png]]
==Strategy== dichiara l’interfaccia della nostra classe di algoritmi, che viene utilizzata da ==Context==, per invocare un algoritmo concreto. 
==ConcreteStrategy== sono i nostri algoritmi concreti, ovvero implementano uno specifico algoritmo, che espone l’interfaccia Strategy. 
==Context== è la classe di contesto, che invoca la ConcreteStrategy.

Se ti trovi davanti a un problema, chiediti queste tre cose. Se la risposta è sì, allora serve il Pattern Strategy :
1. **C'è un'azione principale che rimane sempre la stessa ?** (Es: Zog deve sempre "Muoversi", o un sito deve sempre "Pagare").
2. **Ci sono tanti modi diversi per fare quell'azione ?** (Es: Camminare/Volare, oppure Carta di Credito/PayPal/Bitcoin).
3. **Voglio poter cambiare il "modo" velocemente senza smontare tutto il sistema ?** (Es: Cambiare scheda a Zog mentre sta già correndo).

==Observer==.
Il pattern Observer (noto anche col nome Publish-Subscribe) permette di ==definire una dipendenza "uno a molti" fra oggetti==, in modo tale che ==se un oggetto cambia il suo stato interno, ciascuno degli oggetti dipendenti da esso viene notificato e aggiornato automaticamente==. 
L’Observer nasce dall’esigenza di ==mantenere un alto livello di consistenza fra classi correlate, senza produrre situazioni di forte dipendenza e di accoppiamento elevato==. 
Trova applicazione nei casi in cui diversi oggetti (Observer) devono conoscere lo stato di un oggetto (Subject). In poche parole, abbiamo un oggetto che viene “osservato” (il subject) e tanti oggetti che “osservano” i cambiamenti di quest’ultimo (gli observer).
![[Pasted image 20251231054726.png]]
==Subject== (interfaccia Observable) ha conoscenza dei propri Observer, i quali possono essere in numero illimitato, fornisce operazioni per l’aggiunta e la cancellazione di Observer e fornisce operazioni per la notifica agli Observer. 
==Observer== (interfaccia Observer) specifica un’interfaccia per la notifica di eventi agli oggetti interessati in un Subject.
==Concrete Subject== (ObservedSubject) mantiene lo stato del soggetto osservato e notifica gli observer in caso di un cambio di stato, invoca le operazioni di notifica ereditate dal Subject, quando devono essere informati i ConcreteObserver. 
==ConcreteObserver== implementa l’interfaccia dell’Observer, definendo il comportamento in caso di cambio di stato del soggetto osservato. 
Ci sono due modi in cui il Subject notifica gli Observer : ==push==, in cui l’Observer ottiene esattamente i dati che vuole (ha senso utilizzarlo quando si hanno massimo 2-3 Observer) e ==pull== in cui l’Observer ottiene i dati racchiusi in un oggetto estraendo quelli di cui ha bisogno (più di 2-3 Observer).

Chiediti queste cose. Se la risposta è sì, allora corri a usare l'Observer :
1. **C'è un oggetto "importante" che cambia stato ?** (Es: Arriva un'email, il prezzo di un'azione in borsa sale, il personaggio di un gioco perde vita).
2. **Ci sono altri oggetti che devono "reagire" a questo cambiamento ?** (Es: Il computer deve suonare, il grafico della borsa deve aggiornarsi, la barra della vita sullo schermo deve accorciarsi).
3. **L'oggetto importante non sa (e non gli interessa) quanti sono quelli che lo guardano ?** (A Super-Pippo non importa se i fan sono 10 o 1 milione, lui manda lo stesso messaggio a tutta la lista).

==Decorator==.
Il design pattern Decorator fornisce un’==alternativa flessibile all’ereditarietà, per estendere la funzionalità degli oggetti==. Tale pattern consente di ==arricchire dinamicamente, a run-time, un oggetto con nuove funzionalità== : è possibile impilare uno o più decorator uno sopra l’altro, ciascuno aggiungendo nuove funzionalità.
![[Pasted image 20251231055604.png]]
La struttura del decorator pattern si compone di quattro elementi principali : 
==Component== rappresenta l’interfaccia dell’oggetto che dovrà essere decorato dinamicamente.
==ConcreteComponent== rappresenta l’oggetto a cui andranno aggiunte le nuove funzionalità.
==Decorator== rappresenta l’interfaccia tra il Component e i ConcreteDecorator, possiede un riferimento al Component e un’interfaccia ad esso conforme.
==ConcreteDecorator== rappresentano gli oggetti che aggiungono le funzionalità ai ConcreteComponent.

Fatti queste domande. Se la risposta è sì, allora usa il Decorator :
1. **Ho un oggetto base a cui voglio aggiungere "abilità" o "caratteristiche" extra?** (Es: Un'arma che può diventare "infuocata" o "ghiacciata").
2. **Queste aggiunte possono essere combinate tra loro in mille modi diversi ?** (Es: Posso volere l'arma infuocata E ghiacciata contemporaneamente).
3. **Voglio poter aggiungere o togliere questi pezzi "al volo" mentre il programma gira ?** (Es: Il personaggio beve una pozione e ottiene un potere temporaneo).

==Factory==.
==Factory method== : 
==Definisce un’interfaccia per creare oggetti, ma lascia alle sottoclassi la decisione del tipo di classe da istanziare==. 
Il pattern può rivelarsi utile quando una classe non è in grado di conoscere a priori il tipo di oggetti da creare, o quando si vuole delegare la creazione di un oggetto alle sottoclassi. 
L’applicazione del pattern consente di eliminare le dipendenze dai tipi concreti utilizzati. 
È molto utile quando : una classe non è in grado di sapere in anticipo le classi di oggetti che deve creare, la creazione di un oggetto preclude il suo riuso, senza una significativa duplicazione di codice, la creazione di un oggetto richiede l’accesso ad informazioni, o risorse che non dovrebbero essere contenute nella classe di composizione, la gestione del ciclo di vita degli oggetti gestiti deve essere centralizzata, in modo da assicurare un comportamento coerente all’interno dell’applicazione, o le classi delegano le responsabilità di creazione.
![[Pasted image 20251231061002.png]]
Possiamo individuare i seguenti componenti : 
==Creator== dichiara la Factory che avrà il compito di ritornare l’oggetto appropriato.
==ConcreteCreator== effettua l’override del metodo della Factory, al fine di ritornare l’implementazione dell’oggetto.
==Product== definisce l’interfaccia dell’oggetto che deve essere creato dalla Factory.
==ConcreteProduct== implementa l’oggetto in base ai metodi definiti dall’interfaccia Product.
![[Pasted image 20251231061146.png]]

Fatti queste domande. Se la risposta è sì, allora ti serve una Factory :
1. **Il mio programma deve creare degli oggetti, ma non so ancora di che tipo preciso saranno ?** (Es: Un gioco di mostri dove i mostri nascono a caso: a volte un Drago, a volte un Goblin).
2. **Voglio che chi usa l'oggetto non sappia come è stato costruito ?** (Es: Voglio usare un "Database", ma non voglio sapere se è di tipo MySQL o Oracle).
3. **Voglio poter aggiungere nuovi tipi di oggetti senza cambiare tutto il codice principale ?** (Es: Domani voglio aggiungere il "Robot-Ninja" al mio negozio senza dover spiegare a tutti i clienti come si monta).

==Abstract factory== :
Questo pattern fornisce un’==interfaccia per la creazione di famiglie di oggetti correlati o dipendenti, senza specificarne le loro classi concrete==.
![[Pasted image 20251231061733.png]]
È composta da : 
==AbstractFactory== definisce l’interfaccia di riferimento per gli oggetti che creano le istanze.
==ConcreteFactory== implementa in modo concreto l’interfaccia definita da AbstractFactory e crea effettivamente una tipologia specifica di oggetti appartenenti ad una famiglia.
==AbstractProduct== definisce l’interfaccia di riferimento per una famiglia di oggetti da creare tramite il factory corrispondente.
==ConcreteProduct== implementa in modo concreto l’oggetto appartenente alla famiglia, per cui vale l’interfaccia AbstractProduct e che viene creato dall’oggetto factory corrispondente.
==Client== utilizza unicamente le classi astratte del factory e dell’oggetto da creare, senza conoscerne gli aspetti implementativi. 
==L’annullamento dell’accoppiamento tra il client e gli oggetti concreti è ottenuto tramite l’inversione delle dipendenze==. 
Una differenza tra l’Abstract Factory e il Factory Method è che, con il primo una classe delega la responsabilità di istanziare un oggetto ad un altro oggetto tramite la composizione, mentre il secondo utilizza l’ereditarietà e si basa su una sottoclasse per gestire l’istanza dell’oggetto desiderato.

Chiediti queste cose. Se la risposta è sì, allora ti serve questa "Super-Fabbrica" :
1. **Devo creare tanti oggetti diversi che però devono stare bene insieme ?** (Es: In un gioco, il set di armi, armature e scudi di un "Cavaliere" contro quelli di un "Alieno").
2. **Ho diverse "famiglie" o "stili" tra cui scegliere ?** (Es: Il mio programma deve girare su Windows e su Mac. Se gira su Windows, tutti i bottoni e le finestre devono avere lo stile Windows. Se gira su Mac, devono avere tutti lo stile Mac).
3. **Voglio evitare che l'utente mescoli pezzi di famiglie diverse ?** (Es: Non voglio che il mio programma usi un bottone di Windows dentro una finestra di Mac).

Questa è la parte dove molti si confondono, ma per te sarà semplicissimo :
- **Factory Method :** Crea **un solo tipo** di oggetto (es. solo la Pizza). È una singola ricetta.
- **Abstract Factory :** Crea **un'intera famiglia** di oggetti diversi ma correlati (es. Sedia + Tavolo + Divano). È un catalogo intero.

==Template Method==.
Si tratta di un ==pattern comportamentale basato su classi e viene utilizzato per definire la struttura di un algoritmo, delegando alcuni passi di dettaglio alle sottoclassi==. 
Questo pattern nasce dall’==esigenza di specificare l’ordine delle operazioni da effettuare, ma di delegare alle sottoclassi l’implementazione di alcune operazioni==. Pertanto, il metodo che definisce l’algoritmo viene implementato nella superclasse, mentre i metodi che definiscono i comportamenti di dettaglio vengono dichiarati astratti nella superclasse ed implementati nelle sottoclassi. 
L’utilizzo di questo pattern permette di : implementare una sola volta la parte “immutata” dell’algoritmo e di consentire alle sottoclassi di implementare il comportamento delle parti “variabili”, individuare comportamenti comuni delle sottoclassi e “promuoverli” a comportamenti della superclasse, in modo da evitare la duplicazione di codice, individuare comportamenti NON comuni delle sottoclassi e definire un metodo di gancio hook per consentire alle sottoclassi di implementare uno specifico comportamento. 
L’utilizzo di questo pattern si presenta con una serie di variazioni, anche se per una completa aderenza alle intenzioni occorrerebbe che rispettasse alcune caratteristiche : ==la superclasse venga dichiarata "abstract" in modo da non poter essere instanziata dal Client==, ==il metodo template venga dichiarato "final", in modo tale che le sottoclassi non siano in grado di modificarlo e cambiare il suo comportamento==, ==i metodi primitivi vengano dichiarati abstract nella superclasse e vengano implementati nelle sottoclassi==, ==le sottoclassi non invochino direttamente il metodo concreto della superclasse ma lascino che sia la superclasse ad invocarli all’occorrenza==, ==Principio di Hollywood== : “non chiamarci, ti chiameremo noi”, ==minimizzare il numero di metodi primitivi per evitare che lo sviluppatore delle sottoclassi debba implementare troppi metodi per poter usare questo pattern==, ==creare un metodo concreto hook vuoto tra le fasi dell’algoritmo, per permettere agli sviluppatori di sovrascriverlo ed implementare un passaggio logico da loro richiesto==. 
Questo pattern è composto dai seguenti partecipanti : 
==AbstractClass== definisce il metodo concreto ed i metodi primitivi astratti. Il metodo concreto richiama i metodi primitivi implementati nelle sottoclassi.
==ConcreteClass== implementa i metodi primitivi per svolgere i passi specifici dell’algoritmo ed eventualmente i metodi hook.
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

==Composite==.
Si tratta di un ==pattern strutturale basato su oggetti, che viene utilizzato quando si ha la necessità di realizzare una gerarchia di oggetti, in cui l’oggetto contenitore può detenere oggetti elementari e/o oggetti contenitori==. 
L’obiettivo è di ==permettere al Client, che deve navigare la gerarchia, di comportarsi sempre nello stesso modo, sia verso gli oggetti elementari e sia verso gli oggetti contenitori==. 
Questo pattern è composto dai seguenti partecipanti : 
==Client== colui che effettua l’invocazione all’operazione di interesse.
==Component== definisce l’interfaccia degli oggetti della composizione.
==Leaf== rappresenta l’oggetto foglia della composizione, non ha figli e definisce il comportamento “primitivo” dell’oggetto della composizione. 
==Composite== definisce il comportamento degli oggetti usati come contenitori e detiene il riferimento ai componenti “figli”.
![[Pasted image 20251231063733.png]]
Tale pattern presenta i seguenti vantaggi/svantaggi : gli oggetti della gerarchia possono essere composti da oggetti semplici e/o da oggetti contenitori, che a loro volta sono composti ricorsivamente da altri oggetti semplici e/o da oggetti contenitori, il Client tratta gli oggetti semplici e gli oggetti contenitori nello stesso modo. Questo semplifica il suo lavoro, il quale astrae dalla specifica implementazione, l’alberatura è facilmente modificabile aggiungendo/rimuovendo foglie e contenitori.

Fatti queste tre domande. Se la risposta è sì, allora serve il Composite :
1. **I miei oggetti formano una struttura a "albero" ?** (Cioè ci sono rami che hanno foglie o altri rami).
2. **Voglio poter ignorare la differenza tra un oggetto singolo e un gruppo di oggetti ?** (Es: Voglio poter dire "Sposta" sia a un file che a una cartella intera senza cambiare comando).
3. **Un contenitore può contenere altri contenitori dello stesso tipo ?** (Scatole dentro scatole).

==5. Indicare le principali differenze/ somiglianze tra due pattern di design==.


==6. Factory :
	- Differenza tra simple factory e static factory.==


==7. Composite :
	- [NON Richiesto] implementazione CompositeIterator.==


### Design : Architecture and Methodology
==1. Che cosa si intende per design di alto livello di dettaglio ?==

I progetti grandi hanno ==due fasi progettuali== : 
1) ==Architetturale== : vengono elencati i componenti principali e le loro relazioni e sono i requisiti funzionali e non funzionali a guidare questa fase.
2) ==Dettagliata== : i componenti sono scomposti a un livello di dettaglio molto fine e sono l’architettura e i requisiti funzionali a guidare questa fase. 
Tutti i requisiti funzionali devono essere trasformati in un design dettagliato.

==2. Quali sono i principi di programmazione SOLID ? Fornire esempi dei principi di programmazione.==

I principi di programmazione SOLID sono 5 :
1) ==Single Responsibility Principle (SRP) - Principio di responsabilità unica== : 
	==Una classe dovrebbe avere una, ed una sola, ragione per cambiare==. 
	Responsabilità diverse implicano classi separate. Una classe dovrebbe svolgere un unico compito ben definito e non essere sovraccaricata da diverse funzionalità. 
	Serve per ==mantenere il codice più modulare, leggibile e manutenibile== (se una classe ha una sola responsabilità è più facile localizzare e modificare il codice associato a quella specifica funzionalità). Inoltre, serve per ==ridurre il rischio di bug== (modificare una funzionalità non dovrebbe influenzare un’altra). 
	Si tratta di ==classi piccole e con un solo scopo, che possono essere riutilizzate in contesti diversi==.
	
	Esempio :
	![[Pasted image 20251231095313.png]]
	Se in questo caso CFO decidesse di modificare un algoritmo condiviso anche da COO, come RegularHours, queste modifiche se le ritroverebbe anche COO che magari non le vuole !
	![[Pasted image 20251231095435.png]]
	Soluzione :
	![[Pasted image 20251231095510.png]]

1) ==Open Closed Principle (OCP) - Principio aperto e chiuso== :
	==Dovresti essere in grado di estendere il comportamento di una classe, senza modificarla==.
	 Si dice che ==il codice è aperto alle estensioni e chiuso alle modifiche==, perché il codice esistente non dovrebbe essere modificato ogni volta che aggiungiamo una nuova funzionalità, ma dovrebbe essere progettato in modo da consentire l’estensione del comportamento tramite l’aggiunta di nuovo codice. 
	 ==Il codice è più stabile, manutenibile, flessibile di fronte ai cambiamenti dei requisiti==. 
	 ==La struttura è modulare e riutilizzabile==.

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

3) ==Liskov Substitution Principle (LSP) - Principio di sostituzione di Liskov== :
	==Le classi derivate devono essere sostituibili con le rispettive classi base==. 
	Il principio di sostituzione di Liskov è importante nel contesto dell’ereditarietà. 
	Le classi derivate devono essere pienamente compatibili con la classe base e comportarsi come ci si aspetta dalla classe base. 
	Caratteristiche fondamentali di questo principio di programmazione sono la ==flessibilità==, la ==robustezza== e la ==modularità==. 
	Importante è ==non utilizzare l’ereditarietà==. 
	Bisogna progettare con interfacce, per definire comportamenti comuni.
	![[Pasted image 20251231100756.png]]
	![[Pasted image 20251231100813.png]]

4) ==Interface Segregation Principle (ISP) - Principio di segregazione dell'interfaccia== :
	==Realizzare interfacce a grana fine specifiche per il cliente==. 
	Un’interfaccia dovrebbe essere progettata in modo che ogni classe che la implementa debba fornire solo ciò di cui ha effettivamente bisogno, senza obblighi di implementare metodi inutili. 
	Questo principio di programmazione riduce le dipendenze inutili (non implementare metodi che non verranno mai usati).

	Esempio :
	![[Pasted image 20251231101544.png]]
	Anziché implementare un’unica grande interfaccia, implementiamo delle interfacce più piccole e specifiche.

5) ==Dependency Inversion Principle (DIP) - Principio di inversione delle dipendenze== :
	==Dipendere dalle classi astratte, non dalle concrete==. 
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


==3. Principi per il design di componenti : principi relativi alla coesione e all’accoppiamento. Misurare la qualità del design dei componenti.== 

Il design dei componenti si concentra sull'organizzazione delle classi in unità più grandi (pacchetti o moduli) e sulla gestione delle relazioni tra di esse. La qualità di un design si misura attraverso due concetti chiave : la coesione (cosa mettere dentro un componente) e l'accoppiamento (come far interagire i componenti).
Ecco una sintesi completa e strutturata dei principi di Robert C. Martin (Uncle Bob) per il design dei componenti.

1. ==Principi di Coesione== : Quali classi raggruppare ?
Questi tre principi aiutano a decidere la granularità dei componenti, bilanciando le esigenze di chi sviluppa e di chi riutilizza il codice.
==REP (Reuse/Release Equivalence Principle)== :
> _"La granularità del riutilizzo è la granularità del rilascio."_
- **Il concetto :** Non puoi riutilizzare un pezzo di software se non viene rilasciato con un sistema di versioning (es. v1.0.1, v1.1.0).
- **Regola :** Un componente deve essere un'entità coerente, documentata e tracciabile. Chi lo usa deve poter decidere se e quando aggiornare alla nuova versione. Se le classi dentro un componente non hanno un obiettivo comune, non possono essere rilasciate insieme.

==CCP (Common Closure Principle)== :
> _"Le classi che cambiano insieme, vanno insieme."_
- **Il concetto :** È la versione "componente" del _Single Responsibility Principle_.
- **Regola :** Se dobbiamo fare una modifica, vogliamo che questa colpisca il minor numero possibile di componenti. Raggruppando le classi che tendono a cambiare per lo stesso motivo, limitiamo la manutenzione a un solo pacchetto, riducendo l'impatto sul resto del sistema.

==CRP (Common Reuse Principle)== :
> _"Non forzare gli utenti a dipendere da ciò che non usano."_
- **Il concetto :** È la versione "componente" dell'_Interface Segregation Principle_.
- **Regola :** Le classi che vengono riutilizzate insieme devono stare nello stesso componente. Se un utente ha bisogno di una sola classe di un componente, ma quel componente ne contiene altre dieci che non gli servono, l'utente sarà comunque influenzato dai cambiamenti di quelle dieci classi. **In sintesi : separa le classi che non vengono usate insieme.**
![[Pasted image 20251231104653.png]]

2. ==Principi di Accoppiamento: Come gestire le dipendenze ?==
Questi principi governano le relazioni tra i componenti e la stabilità dell'architettura.
==ADP (Acyclic Dependencies Principle)== :
> _"Niente cicli nelle dipendenze tra componenti."_
- **Il problema :** Se il componente A dipende da B, B dipende da C, e C dipende da A, abbiamo un **ciclo**. Questo crea un unico enorme blocco : non puoi testare o rilasciare A senza coinvolgere anche B e C.
- **Soluzione :** Per rompere un ciclo si può :
    1. Utilizzare il **Dependency Inversion Principle (DIP)** (creare un'interfaccia).
    2. Creare un nuovo componente che contenga le classi comuni da cui entrambi dipendono.

==SDP (Stable Dependencies Principle)== :
> _"Dipendi nella direzione della stabilità."_
- **Il concetto :** Un componente è "stabile" non perché è vecchio, ma perché **molti altri dipendono da lui**. Se molti dipendono da me, cambiare è difficile perché rischierei di rompere tutto.
- **Regola :** I componenti che cambiano spesso (instabili) devono dipendere da componenti difficili da cambiare (stabili). Non vogliamo mai che un componente stabile dipenda da uno instabile.

==SAP (Stable Abstractions Principle)== :
> _"La stabilità di un componente deve essere proporzionale alla sua astrazione."_
- **Il concetto :** Se un componente è molto stabile (difficile da cambiare), come facciamo a estenderlo ?
- **Regola :** Un componente stabile dovrebbe essere **astratto** (pieno di interfacce), in modo che il suo comportamento possa essere esteso senza modificare il codice sorgente. Al contrario, i componenti instabili (che cambiano spesso) dovrebbero essere **concreti**.
![[Pasted image 20251231104735.png]]

 3. ==Misurare la Qualità: Le Metriche== 
Per capire se stiamo rispettando questi principi, utilizziamo dei calcoli matematici.
==A. Misurare l'Instabilità ($I$)== :
==L'instabilità si calcola guardando i collegamenti (fan-in e fan-out)== :
- **Fan-in :** Numero di classi esterne che dipendono dalle classi dentro il mio componente (chi mi "guarda").
- **Fan-out :** Numero di classi esterne da cui il mio componente dipende (chi "guardo").
==$$I = \frac{\text{Fan-out}}{\text{Fan-in} + \text{Fan-out}}$$==
- **$I = 0$ :** Massima stabilità (molti mi guardano, io non guardo nessuno).
- **$I = 1$ :** Massima instabilità (io guardo molti, nessuno mi guarda).

==B. Misurare l'Astrazione ($A$)== :
==Rappresenta il rapporto tra classi astratte/interfacce e il totale delle classi==.
==$$A = \frac{N_a}{N_c}$$==
- $N_a$ : Numero di classi astratte o interfacce.
- $N_c$ : Numero totale di classi nel componente.
- **$A = 0$ :** Componente completamente concreto.
- **$A = 1$ :** Componente completamente astratto.

> **La Regola d'Oro :** Un design sano dovrebbe avere componenti che sono o **Molto Stabili e Astratti** ($I=0, A=1$) o **Molto Instabili e Concreti** ($I=1, A=0$).


==4. Che cosa è una architettura del software ? In che modo può essere caratterizzata ?==

L'==architettura del software== rappresenta la ==struttura organizzativa di un sistema==, ovvero la "forma" che gli sviluppatori conferiscono al software per permettergli di soddisfare i suoi obiettivi. 
Citando definizioni celebri, l'architettura riguarda "le cose importanti, qualunque esse siano", ovvero ==tutte quelle decisioni che hanno un impatto significativo a lungo termine e che sono difficili e costose da cambiare in seguito==.

1. Lo Scopo dell'Architettura :
L'obiettivo primario non è solo far "funzionare" il software, ma ==supportare l'intero ciclo di vita del sistema==. ==Un'architettura ben progettata deve facilitare== :
- ==Sviluppo== :Rendere il sistema facile da costruire per i team di programmatori.
- ==Distribuzione (Deployment)== : Permettere di installare e aggiornare il sistema con rischi minimi.
- ==Funzionamento== : Garantire che il sistema risponda in modo efficiente alle richieste degli utenti.
- ==Manutenzione== : Ridurre i costi e la complessità necessari per correggere errori o aggiungere nuove funzionalità.

2. Caratterizzazione dell'Architettura :
L'architettura può essere caratterizzata attraverso ==diverse dimensioni che ne definiscono la qualità e la struttura==.

==A. I Componenti Logici e le Interazioni== :
==L'architettura definisce i Logical Components, ovvero le parti principali del sistema, le loro responsabilità e i modi in cui comunicano tra loro==. 
All'aumentare della complessità del sistema, cresce l'importanza di decisioni come il tipo di database (SQL vs NoSQL), il numero di servizi e i protocolli di comunicazione.
==B. Proprietà Fondamentali (Qualità del Design)== :
==Un'architettura solida si basa su principi cardine che ne guidano la progettazione== :
- ==Modularità== : Suddividere il sistema in moduli isolati per facilitare test e comprensione.
- ==Separazione delle Responsabilità (SoC)== : Ogni modulo deve avere uno scopo distinto. Un esempio classico è la separazione tra interfaccia utente (UI), logica di business e persistenza dei dati.
- ==Gestione delle Dipendenze== : Evitare che componenti critici dipendano da parti instabili, seguendo spesso principi di inversione delle dipendenze per proteggere il nucleo del sistema.
==C. Requisiti Non Funzionali (Le "-ità")== :
Mentre i requisiti funzionali dicono _cosa_ il sistema deve fare, ==l'architettura determina _come_ il sistema si comporta==. Queste caratteristiche includono :
- ==Scalabilità== : Capacità di gestire carichi crescenti, sia **verticale** (più potenza allo stesso server) che **orizzontale** (aggiunta di nuovi server).
- ==Testabilità e Manutenibilità== : La facilità con cui il sistema può essere verificato e modificato senza introdurre regressioni.
- ==Resilienza e Affidabilità== : La capacità di resistere ai guasti e di recuperare il corretto funzionamento.
- ==Sicurezza e Prestazioni== : L'efficienza nel rispondere ai carichi di lavoro e la robustezza contro attacchi esterni.
 
 3. Stili Architetturali :
==In base ai requisiti, gli architetti scelgono uno "stile" o un modello di riferimento==. Alcuni dei più comuni includono :

| **Stile**              | **Descrizione**                                                                                |
| ---------------------- | ---------------------------------------------------------------------------------------------- |
| **Layered (A Strati)** | Organizza i componenti in strati orizzontali (es. Presentation, Business, Data).               |
| **Client-Server**      | Distribuisce il carico tra un fornitore di risorse (Server) e un richiedente (Client).         |
| **Microservices**      | Scompone l'applicazione in piccoli servizi indipendenti che comunicano tramite rete.           |
| **Event-Driven**       | Il sistema reagisce a eventi che scatenano azioni tra i componenti.                            |
| **Clean Architecture** | Pone la logica di business al centro, rendendola indipendente da database e framework esterni. |

==5. Cosa si intende per caratteristiche architetturali (e quali sono le principali), decisioni architetturali, componenti logici e stili ?==

Per comprendere l'architettura del software, è necessario distinguere tra le sue componenti strutturali, le decisioni che la guidano e gli stili che ne definiscono la forma. Ecco una sintesi fluida e completa dei concetti principali.

==Caratteristiche Architetturali== :
==Le caratteristiche architetturali sono gli attributi del sistema che ne definiscono la qualità e il comportamento, derivando principalmente dai requisiti non funzionali==.
Esse rispondono alla domanda : =="Come si comporta il sistema ?"==. Tra le principali troviamo :
- ==Scalabilità== : Capacità di gestire un aumento del carico. 
- ==Manutenibilità== : Facilità di aggiornamento e correzione.
- ==Resilienza e Affidabilità== : Capacità di resistere ai guasti.
- ==Sicurezza e Prestazioni== : Protezione dei dati e velocità di risposta.

==Decisioni Architetturali e ADR== :
==Le decisioni architetturali sono le scelte fondamentali che stabiliscono come il sistema sarà costruito== (tecnologie, metodologie, approcci). Poiché queste scelte hanno un impatto a lungo termine, vengono ==documentate tramite gli ADR== (Architectural Decision Records).
==Un ADR garantisce trasparenza e tracciabilità attraverso 7 sezioni standard== :
1. ==Title== : Nome breve e identificativo.
2. ==Status== : Stato della decisione (Proposta, Accettata, Superata).
3. ==Context== : Il motivo e le circostanze che hanno portato alla scelta.
4. Decision : La strategia scelta.
5. ==Consequences== : Effetti positivi e negativi della decisione.
6. ==Governance== : Come garantire che l'organizzazione rispetti la scelta.
7. ==Notes== : Informazioni aggiuntive.

![[Pasted image 20251231113453.png]]
==Componenti Logici vs Architettura Fisica== :
==I Componenti Logici sono unità astratte che definiscono cosa fa il sistema== (es. "Processore di Pagamento"). Rappresentano la logica pura, indipendentemente dalla tecnologia.
Esiste una distinzione netta tra :
- ==Architettura Logica== : Mostra come i componenti interagiscono e le loro responsabilità.
- ==Architettura Fisica== : Definisce come il software è distribuito su server, database utilizzati e protocolli di rete.

![[Pasted image 20251231113525.png]]
==Partizionamento e Struttura== :
Il sistema può essere diviso (partizionato) in due modi :
- ==Technical Partitioning (Orizzontale)== : Il codice è diviso per strati tecnici (es. Layered Architecture: UI, Business, DB). È semplice da standardizzare ma meno flessibile per cambiamenti di dominio.
- ==Domain Partitioning (Verticale)== : Il sistema è diviso per funzionalità di business (es. Ordini, Catalogo, Utenti). Ogni parte è un "silo" completo.
![[Pasted image 20251231113931.png]]

==Stili Architetturali Principali== :
==Gli stili definiscono la "forma" complessiva del sistema==.

==A. Architetture Monolitiche== :
- ==Monolite Classico== : Tutti i componenti sono in un'unica unità. Semplice da avviare e testare, ma difficile da scalare e mantenere nel tempo.
- ==Monolite Modulare== : L'applicazione è un'unica entità ma internamente è divisa in moduli indipendenti basati sul dominio. È un ottimo compromesso che riduce l'accoppiamento tecnico.
![[Pasted image 20251231114044.png]]
==B. Architetture Distribuite== :
- ==Layered (A Strati)== : Organizzata in livelli (es. Presentation, Business, Persistence). Ogni strato è isolato (architettura "chiusa"), favorendo la manutenibilità e la specializzazione dei team.
![[Pasted image 20251231114011.png]]
- ==Microkernel (Plug-in)== : Composta da un Core minimale (funzioni base) e diversi Plug-in per le funzioni extra. I plug-in comunicano con il core tramite un "contratto" (interfaccia). È estremamente estensibile (es. Sistemi Operativi, IDE come VS Code).    
- ==Microservices== : Suddivide l'app in piccoli servizi autonomi, ognuno con il proprio database. Offre massima scalabilità e isolamento dei guasti, ma è complessa da gestire (richiede orchestrazione o coreografia).
- ==Event-Driven== : Basata su messaggi asincroni (eventi). È estremamente veloce e scalabile perché i componenti non aspettano risposte (disaccoppiamento temporale), ma è più difficile da debuggare.

==Modelli di Integrazione e Pattern== :
- ==MVC (Model-View-Controller)== : Pattern per separare la logica (Model), l'interfaccia (View) e il flusso di dati (Controller).
- ==Orchestrator vs Choreography== : Nei sistemi distribuiti, si può avere un servizio centrale che comanda gli altri (Orchestratore) o lasciare che i servizi reagiscano autonomamente agli eventi (Coreografia).
- ==Database-per-service== : Caratteristica dei micro-servizi dove ogni servizio possiede i suoi dati, aumentando la _fault tolerance_ ma introducendo la necessità di chiamate tra servizi per recuperare informazioni mancanti.


==6. Qual è la differenza tra architettura e design ?==

La distinzione tra architettura e design è uno dei temi più dibattuti nell'ingegneria del software. Sebbene i due concetti si sovrappongano spesso, possono essere distinti analizzando il loro scopo, il livello di astrazione e l'impatto delle decisioni.

Definizioni Generali :
- ==Architettura== : È la ==visione d'insieme del sistema==. Si concentra sulla struttura organizzativa, sui componenti principali e su come questi interagiscono tra loro. ==L'architettura definisce i vincoli entro i quali il software deve essere costruito per soddisfare i requisiti non funzionali== (scalabilità, sicurezza, ecc.).
- ==Design (Progettazione)== : Si occupa dei ==dettagli implementativi all'interno dei componenti definiti dall'architettura==. Riguarda il "come" risolvere problemi specifici a livello di codice, classi e funzioni, assicurando che i singoli moduli siano ben strutturati e manutenibili.
> **Citazione celebre:** _"L'architettura è design, ma non tutto il design è architettura."_ – Grady Booch.

Differenze Chiave :
 ==A. Livello di Astrazione== :
- ==Architettura (Alto Livello)== : Si occupa di moduli, sottosistemi, database, server e protocolli di comunicazione. È la "scheletro" del sistema.
- ==Design (Basso Livello)== : Si occupa di pattern (es. i Design Pattern di GoF), interfacce, algoritmi e gerarchie di classi. È il "dettaglio interno" di ogni stanza dello scheletro.
==B. Costo del Cambiamento== :
- ==Architettura== : Le decisioni architetturali sono difficili e costose da cambiare una volta che lo sviluppo è avviato (es. passare da un Monolite ai Microservizi). Riguarda le scelte che devono essere "giuste" fin dall'inizio.
- ==Design== : Le decisioni di design sono più localizzate e più facili da rifattorizzare (es. cambiare un pattern Strategy con un Template Method all'interno di una classe).
==C. Obiettivi (Cosa vs Come)== :
- ==Architettura== : Risponde principalmente ai Requisiti Non Funzionali (Efficienza, Robustezza, Scalabilità). Serve a garantire che il sistema possa sostenere il business nel tempo.
- ==Design== : Risponde principalmente ai Requisiti Funzionali (cosa deve fare l'app per l'utente) e alla manutenibilità del codice (leggibilità, testabilità).

==Dove si incontrano ?==
Il confine è spesso sfumato. Un pattern architetturale (come il _Layered Style_) determina la struttura di tutto il progetto, mentre un design pattern (come l'_Observer_) risolve un problema di comunicazione tra due oggetti.
Tuttavia, entrambi condividono lo stesso obiettivo finale : gestire la complessità.
- L'architettura gestisce la complessità esterna (tra i moduli).
- Il design gestisce la complessità interna (dentro i moduli).

Sintesi Comparativa :

|**Caratteristica**|**Architettura**|**Design**|
|---|---|---|
|**Focus**|Struttura globale e sistema totale|Dettagli locali e componenti|
|**Principali preoccupazioni**|Scalabilità, Sicurezza, Distribuzione|Logica, Algoritmi, Pattern di classi|
|**Facilità di modifica**|Bassa (Costi elevati)|Alta (Refactoring possibile)|
|**Esempio**|Scelta tra REST o GraphQL|Scelta tra Factory o Singleton|


==7. Quali sono le principali caratteristiche architetturali ?==

Le ==caratteristiche architetturali== (spesso chiamate "requisiti non funzionali" o "-ility" in inglese) ==rappresentano il modo in cui l'architettura soddisfa le necessità del sistema al di là delle semplici funzioni di business==.
Si tratta di considerazioni di design non legate al dominio : non riguardano _cosa_ fa il software (es. calcolare un mutuo), ma _come_ lo fa (es. quanto velocemente lo calcola). Possono essere ==esplicite==, se chiaramente documentate nei requisiti, o ==implicite==, se date per scontate, ma fondamentali per il successo del progetto (come la sicurezza).
==Le caratteristiche possono essere raggruppate in quattro categorie principali== :
1) ==Caratteristiche Operative (Operational)== : riguardano il comportamento del sistema durante il suo funzionamento in ambiente di produzione.
	- ==Disponibilità (Availability)== : Il tempo in cui il sistema è effettivamente operativo (es. uptime del 99,9%).
	- ==Scalabilità (Scalability)== : La capacità di gestire un aumento del carico (utenti o dati) mantenendo le prestazioni costanti.
	- ==Performance== : Il rispetto dei tempi di risposta e dei limiti di latenza previsti.
	- ==Affidabilità e Robustezza== : La capacità di operare correttamente anche in condizioni estreme o in presenza di errori imprevisti.
	- ==Recupero (Recoverability)== : La velocità con cui il sistema torna operativo dopo un guasto (disaster recovery).
2) ==Caratteristiche Strutturali (Structural)== : definiscono il modo in cui il sistema è costruito internamente e la qualità del suo codice.
	- ==Manutenibilità (Maintainability)== : Quanto è semplice e poco costoso modificare il codice o correggere errori.
	- ==Estensibilità (Extensibility)== : La facilità con cui si possono aggiungere nuove funzionalità senza compromettere la struttura esistente.
	- ==Portabilità (Portability)== : La capacità del software di girare su diverse piattaforme (es. Windows, Linux, Cloud).
	- ==Localizzazione (Localization)== : Il supporto per diverse lingue, valute e formati regionali.
	- ==Accoppiamento (Coupling)== : Il grado di dipendenza tra i vari componenti (un basso accoppiamento è preferibile).
3) ==Caratteristiche di Processo (Process)== : si trovano all'intersezione tra l'architettura e la gestione del ciclo di vita dello sviluppo.
	- ==Modularità (Modularity)== : Il grado di suddivisione del sistema in componenti indipendenti e isolati.
	- ==Testabilità (Testability)== : Quanto è facile sottoporre il software a test automatici per verificarne la correttezza.
	- ==Impiego (Deployability)== : La facilità e la velocità con cui il software può essere distribuito e aggiornato negli ambienti di destinazione.
	- ==Disaccoppiamento== : Favorisce la possibilità che team diversi lavorino su parti diverse del sistema senza pestarsi i piedi.
4) ==Caratteristiche Trasversali (Cross-Cutting)== : sono proprietà che non appartengono a un singolo modulo, ma permeano l'intero sistema.
	- Sicurezza (Security) : Include crittografia, autenticazione e protezione dei dati.
	- Usabilità (Usability) : Quanto è intuitivo e facile da usare per l'utente finale.
	- Accessibilità : La capacità di essere utilizzato da persone con disabilità.
	- Legalità e Privacy : Il rispetto delle normative (es. GDPR) e dei vincoli legali sulla gestione dei dati.


==8. Stili architetturali :  layered, microkernel, event driven, micro-servizi, ... principali caratteristiche, pro e contro di ogni architettura.== 

==Gli stili architetturali definiscono la struttura fondamentale e il modello di comunicazione di un sistema==. Ogni stile è ottimizzato per specifiche caratteristiche architetturali (le "-ility" viste in precedenza) e comporta inevitabili compromessi (trade-off).

1. ==Layered Architecture (N-Tier)==
È lo ==stile più comune, basato sul partizionamento tecnico orizzontale==. Il sistema è diviso in strati (tipicamente: Presentation, Business, Persistence, Database).
- Caratteristiche : ==Ogni layer ha una responsabilità specifica==. È un'==architettura "chiusa"== : una richiesta deve passare per ogni strato (es. la UI non può saltare la Business logic per andare al DB).
- ==Pro== :   
    - ==Semplicità== : Facile da capire, sviluppare e testare.
    - ==Isolamento== : Le modifiche a un layer non influenzano gli altri (se le interfacce rimangono stabili).
    - ==Standardizzazione== : Molto diffusa e ben documentata.
- ==Contro== :
    - ==Scalabilità limitata== : È solitamente un monolite; per scalare bisogna replicare l'intera app.
    - ==Affidabilità== : Se un layer fallisce, l'intero sistema può bloccarsi.
    - ==Performance== : Il passaggio forzato tra strati (sinkhole effect) può creare overhead.
    
2. ==Microkernel Architecture (Plug-in)==
==Si basa su un Core System minimale, che contiene solo la logica essenziale, estendibile tramite moduli esterni chiamati Plug-in==.
- Caratteristiche : ==Il core espone un'interfaccia (contract) a cui i plug-in si collegano==. ==Un "registro" tiene traccia dei plug-in attivi==.
- Pro :
    - ==Estensibilità== : Permette di aggiungere funzionalità senza modificare il core.
    - ==Isolamento== : Un errore in un plug-in solitamente non abbatte il core.
    - ==Portabilità== : Il core può essere adattato a diversi contesti cambiando i plug-in.
- Contro :
    - ==Complessità di design== : Definire un contract stabile per il core è difficile.
    - ==Scalabilità== : Spesso implementato come sistema a singola istanza.

3. ==Event-Driven Architecture (EDA)==
==Uno stile distribuito e asincrono, basato sulla produzione e ricezione di eventi (notifiche di qualcosa che è accaduto)==.
- Caratteristiche : Si compone di _Event Producers_, _Event Channels_ (code) e _Event Consumers_. La comunicazione è spesso non bloccante.
- ==Pro== :
    - ==Performance e Reattività== : Tempi di risposta bassi grazie all'asincronia.
    - ==Scalabilità== : Altissima, i componenti possono scalare indipendentemente.
    - ==Disaccoppiamento== : I produttori non sanno chi consumerà l'evento.
- ==Contro== :
    - ==Difficoltà di test e debug== : Difficile tracciare il flusso di un'operazione tra molti servizi.
    - ==Gestione degli errori== : Cosa succede se un evento va perso o fallisce a metà catena ?

4. ==Microservices Architecture==
==Scompone l'applicazione in piccoli servizi indipendenti, ognuno con il proprio dominio di business e il proprio database== (**Database-per-service**).
- Caratteristiche : ==Partizionamento verticale basato sul dominio==. ==Ogni servizio è un'unità di deployment separata==.
- ==Pro== :
    - ==Scalabilità e Deployment== : Ogni servizio può essere aggiornato e scalato autonomamente.
    - ==Diversità tecnologica== : Ogni team può usare il linguaggio/DB più adatto al problema.
    - ==Resilienza== : Un guasto a un servizio non ferma l'intera piattaforma (fault isolation).
- ==Contro== :
    - ==Complessità operativa== : Richiede automazione estrema, monitoraggio avanzato e orchestrazione.
    - ==Integrità dei dati== : Gestire transazioni tra database diversi è molto complesso (Saga Pattern).
    - ==Latenza== : Le chiamate di rete tra servizi sono più lente delle chiamate interne a un monolite.

4. ==Serverless Architecture==
==Un'evoluzione dei microservizi dove lo sviluppatore scrive solo la logica (funzioni) e il cloud provider gestisce interamente l'infrastruttura==.
- Caratteristiche : "Pay-as-you-go" (paghi solo quando la funzione gira) e auto-scaling infinito.
- ==Pro== :
    - ==Costi ridotti== : Zero costi per server inattivi.
    - ==Manutenzione nulla== : Nessun server da patchare o gestire.
- Contro :    
    - ==Cold Start== : Latenza iniziale al primo avvio della funzione.
    - Vendor Lock-in : Difficile migrare da un provider cloud all'altro.-

### Tabella Comparativa di Sintesi

|**Stile**|**Agilità**|**Scalabilità**|**Semplicità**|**Costo Iniziale**|
|---|---|---|---|---|
|**Layered**|Bassa|Bassa|Alta|Molto Basso|
|**Microkernel**|Alta|Bassa|Media|Medio|
|**Event-Driven**|Alta|Altissima|Bassa|Alto|
|**Microservices**|Altissima|Altissima|Molto Bassa|Molto Alto|

==9. Principi clean dell’architettura del software : Indipendenza, disaccoppiamento dei layer/ disaccoppiamento degli use case.==

I ==Principi Clean== (o Clean Architecture), resi celebri da Robert C. Martin, ==hanno l'obiettivo principale di separare la logica di business dai dettagli tecnici (database, framework, interfacce utente)==. ==Questa separazione permette di creare sistemi facili da mantenere, testare e pronti al cambiamento==.

 1. ==Il Principio di Indipendenza== : un'architettura "pulita" deve garantire l'indipendenza da tutto ciò che è esterno alla logica di business. Questo si traduce in:
	- ==Indipendenza dai Framework== : L'architettura non deve dipendere dall'esistenza di librerie software cariche di funzioni. I framework devono essere usati come strumenti, non come fondamenta su cui poggiare l'intero sistema.
	- ==Indipendenza dalla UI== : L'interfaccia utente deve poter cambiare facilmente (es. passare da una console a un'interfaccia web) senza che la logica del sistema ne risenta.
	- ==Indipendenza dal Database== : Il sistema non deve sapere se i dati sono salvati in SQL, NoSQL o in un semplice file di testo. La logica di business non deve essere "inquinata" da query o schemi del DB.
 2. ==Disaccoppiamento dei Layer (La Regola della Dipendenza)== : l'architettura pulita è rappresentata solitamente da cerchi concentrici. La regola d'oro è : l==e dipendenze del codice possono puntare solo verso l'interno==.
	- ==Entità (Il cuore)== : Rappresentano gli oggetti di business della tua impresa e le regole più generali. Non dipendono da nulla all'esterno.
	- ==Use Cases (Casi d'uso)== : Contengono la logica specifica dell'applicazione. Sanno _come_ orchestrare le entità per raggiungere un obiettivo, ma non sanno chi le chiama o come i dati vengono salvati.
	- ==Interface Adapters== : Convertono i dati dal formato più comodo per i casi d'uso a quello necessario per il DB o la UI. Qui risiedono i Controller e i Presenter.
	- ==Frameworks & Drivers (Strato esterno)== : Qui troviamo i dettagli : il DB specifico, i web framework, i dispositivi. È lo strato più instabile e può essere sostituito senza toccare i cerchi interni.
3. ==Disaccoppiamento degli Use Case== : un errore comune è raggruppare tutti i casi d'uso in un unico grande blocco. Il disaccoppiamento degli Use Case suggerisce invece di separarli in base al dominio di business.
	- ==Il Concetto== : Se la funzione "Aggiungi al carrello" cambia, non dovrebbe esserci alcun rischio di rompere la funzione "Genera fattura".
	- ==Vantaggio nello Sviluppo== : Team diversi possono lavorare su Use Case diversi senza conflitti, poiché ogni caso d'uso è isolato e indipendente.
	- ==Vantaggio nel Deployment== : Questo disaccoppiamento facilita la transizione verso architetture distribuite (come i Microservizi). Se gli Use Case sono ben separati, è facile estrarli dal monolite e trasformarli in servizi autonomi.
4. ==Perché è importante il Disaccoppiamento ?==
	Il disaccoppiamento trasforma il software in un sistema modulare e testabile :
	- ==Testabilità Estrema== : Poiché i cerchi interni non sanno nulla del mondo esterno, puoi testare la logica di business (Entità e Use Case) senza dover avviare un database o un server web.
	- ==Agilità nel Cambiamento== : Se un domani volessi sostituire il tuo database Oracle con MongoDB, dovresti modificare solo i dettagli nello strato più esterno, lasciando intatto il cuore del sistema.


==10. Principi clean dell’architettura del software : policy e livelli/ entità==.

La ==Clean Architecture==, teorizzata da Robert C. Martin, ==si basa su un principio cardine== : la distinzione netta tra le Policy (le regole del business) e i Dettagli (i mezzi tecnici per attuarle).

==L'obiettivo dell'architettura è creare una struttura in cui le policy siano l'elemento centrale e stabile, mentre i dettagli (database, UI, framework) siano considerati irrilevanti e intercambiabili==.

==Policy vs Dettagli== :
Un sistema software è composto da due anime :
- ==Policy== : rappresentano le regole aziendali e le procedure. Sono il cuore del sistema e devono essere protette dai cambiamenti esterni. Secondo Martin, "l'architettura deve parlare del dominio", non delle tecnologie usate.
- ==Dettagli== : Sono gli elementi necessari affinché gli umani o altri sistemi comunichino con le policy (I/O, database, sistemi web, server). Questi devono essere considerati come "plugin" del sistema: la loro scelta dovrebbe essere ritardata il più possibile per evitare che condizionino la logica di business.

==Le Entità : Il cuore del sistema== :
Le Entità r==appresentano il livello più alto di astrazione==. Esse ==incapsulano le Business Rules critiche==, ovvero quelle regole che esisterebbero anche se l'azienda non avesse un sistema informatico (es. "un ordine deve avere almeno un prodotto").
- ==Dati e Regole== : Le entità legano strettamente i dati aziendali critici alle regole che li governano.
- ==Indipendenza== : Sono completamente autonome; non sanno nulla di database, interfacce grafiche o framework. Questo le rende riutilizzabili in contesti e progetti diversi.

==La Struttura a Livelli e la Regola della Dipendenza== :
==L'architettura è rappresentata da cerchi concentrici==. Il concetto di livello esprime la "distanza" di una policy dall'input/output : ==più una regola è generale e astratta, più è ad "alto livello" (vicina al centro); più è legata ai dettagli tecnici, più è a "basso livello" (periferia)==.
==La Regola della Dipendenza stabilisce che le dipendenze del codice possono puntare solo verso l'interno, verso l'alto livello. I cerchi interni non possono sapere nulla di ciò che accade nei cerchi esterni==.
I Quattro Livelli :
1. ==Entità (Inner Circle)== : Contengono le regole di business universali e indipendenti. Sono il livello più stabile e astratto.
2. ==Use Cases== : Contengono le Policy Applicative. Coordinano il flusso di dati verso e dalle entità, specificando cosa deve fare il sistema per soddisfare un requisito (es. "prima di salvare l'ordine, verifica la disponibilità").
3. ==Adattatori dell'Interfaccia (Interface Adapters)== : Traduttori che convertono i dati dal formato dei casi d'uso a quello dei dispositivi esterni (e viceversa). Qui risiedono Controller, Presenter e Gateway.
4. ==Frameworks & Drivers (Outer Circle)== : Il livello dei dettagli tecnici. Qui si trovano il database specifico, il web server e le librerie. È il livello più volatile.

==Tipologie di Policy== :
Il sistema governa il comportamento attraverso ==due tipi di regole== :
- ==Business Rules (in Entità)== : Regole fondamentali e costanti (es. calcolo dell'IVA).    
- ==Policy Applicative (in Use Cases)== : Regole che definiscono i flussi operativi specifici di quell'applicazione (es. l'invio di una notifica email dopo un acquisto).

==Vantaggi dell'Approccio Clean== :
Seguire questa separazione garantisce che il sistema sia :
- ==Indipendente dai Framework== : Non si è schiavi di una tecnologia.
- ==Testabile== : Si può testare la logica di business senza bisogno di database o UI.
- ==Mantenibile== : Le decisioni sui dettagli possono essere prese (o cambiate) in un secondo momento senza riscrivere il cuore del software.


==11. Principi clean dell’architettura del software : principali componenti dell’architettura.==

==Per descrivere i componenti principali della Clean Architecture dobbiamo guardare al software non come a un blocco unico, ma come a un insieme di moduli organizzati secondo la loro "distanza" dall'utente e dai dettagli tecnici==.

Ecco una sintesi fluida e completa dei componenti che formano la struttura di un sistema "Clean" :

==La Struttura a Componenti e la Legge di Conway== :
==L'architettura deve essere suddivisa in componenti ben isolati==. Spesso questa suddivisione riflette la ==Legge di Conway==, la quale suggerisce che ==le organizzazioni progettano sistemi che sono la copia della loro struttura di comunicazione== (ad esempio, se un'azienda ha tre team separati, è molto probabile che il sistema finisca per avere tre moduli principali).
In un'architettura "Clean", i componenti sono organizzati in modo che il cambiamento in uno non obblighi a riscrivere gli altri.

==Le Policy (Regole di Business)== :
Le Policy sono il cuore pulsante dell'architettura. ==Rappresentano le regole aziendali e i processi che governano il sistema==. Si dividono in due grandi gruppi :
- ==Policy di Business (Regole Critiche)== : Sono le regole fondamentali che esistono indipendentemente dal computer (es. come si calcola lo sconto per un cliente fedele).
- ==Policy Applicative== : Sono le regole che definiscono il comportamento specifico del software (es. "quando l'utente preme invio, salva i dati e manda una mail").

==Le Entità (Il Cuore stabile)== :
==Le Entità incapsulano le Business Rules più generali e di alto livello==.
- Possono essere ==oggetti con metodi o semplici strutture dati==.
- ==Indipendenza== : Sono la parte più protetta del sistema. Non devono essere influenzate da cambiamenti nella UI, nel database o nei framework.
- ==Stabilità== : Rappresentano il concetto più stabile dell'azienda; cambiano solo se cambiano le regole fondamentali del business.

==I Casi d’Uso (Use Cases)== :
==I Casi d'Uso sono la descrizione del modo in cui il sistema automatizzato viene utilizzato==. Rappresentano la ==logica applicativa specifica che orchestra il flusso di dati==.
- Cosa contengono : Descrivono l'input ricevuto dall'utente, le fasi di elaborazione necessarie e l'output risultante.
- Orchestrazione : Non contengono le regole aziendali universali (che stanno nelle Entità), ma sanno come usare le Entità per raggiungere un obiettivo specifico dell'applicazione.
- Dettaglio tecnico : Pur essendo specifici dell'app, non sanno ancora _come_ l'utente interagisce (se via web o app mobile) né _dove_ i dati vengono salvati fisicamente.

==Adattatori e Componenti di Frontiera== :
Oltre al nucleo (Entità e Casi d'Uso), ==l'architettura include componenti che fungono da ponte verso il mondo esterno== :
- ==Interface Adapters== : Componenti che trasformano i dati dal formato dei Casi d'Uso a quello più comodo per i database o le interfacce grafiche (Controller, Presenter, Gateway).
- ==Frameworks & Drivers== : I dettagli "sporchi" come il tipo di database (SQL/NoSQL) o il framework web (Spring, Express, ecc.).


### Design : Characteristics and Metrics
==1. In che modo può essere descritta e caratterizzata la progettazione di un software ?==

La progettazione del software può essere analizzata e perfezionata attraverso l'==uso delle metriche software==, strumenti che permettono di valutare in modo oggettivo la qualità del sistema. Tuttavia, sebbene i dati forniscano una base analitica solida, il ==giudizio umano== rimane insostituibile per interpretare correttamente i risultati e guidare le scelte progettuali finali.


==2. Cosa si intende per metrica del software, quali sono i limiti nell’utilizzare metriche per caratterizzare i software e quali tipi di metriche possono essere utilizzate ?==

==Una metrica software è una misura quantitativa del grado in cui un sistema, un componente o un processo possiede una determinata proprietà==. In altre parole, è uno strumento oggettivo utilizzato per valutare la qualità, la complessità e l'efficienza del software e del suo ciclo di vita.

Tipologie di Metriche :
==Le metriche si dividono generalmente in tre grandi categorie, che analizzano il software da diverse prospettive== (dalla struttura del codice alla gestione economica) :
- ==Metriche di Prodotto== : Si concentrano sulle caratteristiche del risultato intermedio o finale (il software stesso). Includono la dimensione del codice (Linee di Codice - LOC), la complessità logica (come la _Complessità Ciclotomatica_), la manutenibilità e il grado di soddisfazione del cliente.
- ==Metriche di Processo== : Misurano l'efficacia dei metodi, delle tecniche e degli strumenti utilizzati per sviluppare il software. L'obiettivo è analizzare "come" il codice è stato costruito per migliorare la produttività e la qualità dei futuri cicli di sviluppo.
- ==Metriche di Progetto== : Riguardano la gestione operativa e le risorse. Misurano variabili come il rispetto del budget, i tempi di consegna, il numero di sviluppatori coinvolti, i costi e la produttività complessiva del team.

Esempi e Criticità :
==La metrica più semplice è il conteggio delle Linee di Codice (LOC)==. Tuttavia, questa misura è spesso considerata poco valida o addirittura fuorviante : un codice con molte righe non è necessariamente migliore o più complesso di uno sintetico; al contrario, potrebbe essere scritto male o essere ridondante.

Limiti nell'uso delle Metriche :
Nonostante l'utilità, ==l'applicazione delle metriche presenta limiti significativi che richiedono sempre l'intervento del giudizio umano== :
- ==Assenza di standard universali== : È difficile stabilire range di valori "ottimali" validi per ogni tipo di software; spesso i parametri di riferimento devono essere determinati empiricamente per ogni specifico progetto.
- ==Inaccuratezza e Non Linearità== : Le metriche tradizionali possono essere imprecise. Ad esempio, la complessità non cresce in modo lineare con la dimensione del codice.
- ==Effetto sul comportamento (Legge di Goodhart)== : Quando una metrica diventa un obiettivo (es. "premiamo chi scrive più linee di codice"), i professionisti tendono ad adeguare il proprio comportamento per soddisfare il parametro, a discapito della qualità reale. Questo può portare a risultati disastrosi, come codice inutilmente lungo o frammentato.
- ==Stima imprecisa== : Le metriche forniscono indicazioni, ma raramente possono essere considerate misure assolute della qualità o dello sforzo necessario.


==3. Cosa si intende per analisi statica e dinamica del software ?==

L'analisi del software si divide in due grandi categorie che si differenziano principalmente per il momento in cui vengono eseguite e per l'oggetto della loro osservazione : ==la struttura del codice o il suo comportamento in esecuzione==.

Analisi Statica :
==L'analisi statica viene eseguita sul codice sorgente senza che il programma venga effettivamente avviato==. È una forma di revisione automatizzata o manuale che mira a identificare difetti strutturali, violazioni di standard o potenziali vulnerabilità nelle prime fasi dello sviluppo.
==Metriche e aspetti principal==i :
- ==Linee di Codice (LOC)== : Misura la dimensione fisica del software.
- ==Complessità Ciclotomatica (McCabe)== : Misura il numero di percorsi linearmente indipendenti attraverso il codice, indicando quanto sia difficile da testare o mantenere.
- ==Complessità di Halstead== : Valuta la complessità basandosi sul numero di operatori e operandi.
- ==Livello di nidificazione== : Controlla quanti cicli o istruzioni condizionali sono inseriti l'uno dentro l'altro.
- ==Accoppiamento e Coesione== : Valutano rispettivamente quanto i moduli dipendano l'uno dall'altro e quanto siano focalizzati su una singola responsabilità.
- ==Duplicazione di Codice== : Identifica porzioni di codice ripetute che dovrebbero essere rifattorizzate.
- ==Punti Funzione (Function Points)== : Misura le funzionalità offerte dal software dal punto di vista dell'utente.

Analisi Dinamica :
==L'analisi dinamica viene effettuata mentre il programma è in esecuzione==. Si concentra sul comportamento reale del sistema, sulle prestazioni e sull'interazione con l'ambiente (memoria, rete, processore).
==Metriche e aspetti principali== :
- ==Copertura del codice (Code Coverage)== : Percentuale di codice sorgente effettivamente eseguita durante i test (unitari, d'integrazione, ecc.).
- ==Densità di Bug== : Numero di difetti rilevati per riga di codice durante l'esecuzione.
- ==Utilizzo delle funzionalità== : Monitoraggio di quali parti del software vengono effettivamente utilizzate dagli utenti finali.
- ==Analisi delle prestazioni== : Monitoraggio dell'uso della CPU e dei leak (perdite) di memoria.
- ==Analisi dei tempi di risposta== : Valutazione della velocità del sistema sotto diversi carichi di lavoro.


==4. Caratteristiche delle misure basate : ==
	==- Sul conteggio delle linee di codice;==
	==- Sul livello di innestamento del codice;==
	==- Sulla complessità del codice (Halstead e complessità ciclomatica di Mc Cabe)==

Le metriche software sono strumenti quantitativi utilizzati per valutare la dimensione, la complessità e la qualità del codice sorgente. Si dividono principalmente in tre categorie : basate sul conteggio delle linee, sulla struttura di annidamento e sulla complessità logica.

==Metriche basate sul conteggio delle linee di codice (LOC)== :
Servono per misurare la dimensione del software e valutare a posteriori lo sforzo produttivo o stimare i costi generali.
- ==LOC (Lines of Code)== : Numero totale di linee. Monitora l'evoluzione del codice nel tempo.
- Varianti principali :
    - NLOC : Linee senza commenti.
    - SLOC (Source LOC) : Esclude commenti e righe vuote.
    - CLOC : Numero di linee di commento. Il rapporto CLOC/LOC indica il grado di documentazione del codice.
    - LLOC (Logical LOC) : Numero di istruzioni logiche effettive (indipendente dalla formattazione).
- Svantaggi : ==Non considera la complessità logica==; il codice può risultare prolisso e i valori variano drasticamente in base al linguaggio di programmazione usato.
![[Pasted image 20260101124630.png]]
> Nota sulla Duplicazione : Il "Code Duplication" aumenta i costi di manutenzione e testing. Le tecniche di ricerca possono essere sintattiche (stesse parole), token-based (blocchi di caratteri) o basate su Alberi AST (Abstract Syntax Tree) per individuare duplicazioni logiche.

==Metriche sul livello di annidamento (Nesting Level - NL)== :
Misurano la profondità delle strutture di controllo (if, while, chiamate di funzione, classi nidificate). Un codice troppo profondo è difficile da leggere e mantenere.
- ==NL (Nesting Level)== : Livello di innestamento medio o massimo.
- ==LoopNL== : Livello di nidificazione specifico all'interno dei cicli.
- ==NL#+ (es. NL4+, NL8+)== : Conteggio delle righe che superano una determinata soglia di profondità.
- Utilizzo : Oltre una certa soglia (es. NL 8), il codice è considerato eccessivamente complesso e richiede obbligatoriamente un intervento di refactoring (riscrittura).

Metriche sulla complessità del codice.
==Halstead Complexity Metric== :
Si basa sull'analisi statica degli operatori (comandi, parole chiave) e degli operandi (variabili, costanti).
- ==Parametri base== : $n_1$ (operatori distinti), $n_2$ (operandi distinti), $N_1$ (totale operatori), $N_2$ (totale operandi).
- ==Vocabolario== : $n = n_1 + n_2$
- ==Volume ($V$)== : Rappresenta la dimensione informativa del programma ($V = N \times \log_2 n$).
- ==Difficoltà ($D$)== : Legata all'errore potenziale ($D = \frac{n_1}{2} \times \frac{N_2}{n_2}$).
- ==Sforzo ($E$)== : Il lavoro mentale richiesto ($E = V \times D$).
- Svantaggi : ==Ignora la struttura logica e il design complessivo, concentrandosi solo sul testo==.

==Complessità Ciclotomatica di McCabe== :
È una delle metriche più importanti per il testing. Misura il numero di percorsi linearmente indipendenti attraverso il codice sorgente.
- Concetto : ==Ogni clausola di decisione (es. IF) crea un nuovo percorso. Maggiore è il numero, più test logici saranno necessari per verificare il software==.
- ==Formule di calcolo== :
    1. $V(G) = \text{Numero di regioni chiuse} + 1$
    2. $V(G) = \text{Archi} - \text{Nodi} + 2$
- Importanza : ==Aiuta a identificare i punti decisionali critici e garantisce che ogni possibile ramificazione venga testata almeno una volta==.
![[Pasted image 20260101124738.png]]


==5. Quali sono i problemi generati dalla duplicazione del codice ?==

==La duplicazione del codice==, spesso definita come pratica del "copia e incolla", ==si verifica quando porzioni di codice identiche o molto simili appaiono in più punti del sistema==. Questo fenomeno ==viola il principio fondamentale DRY== (Don't Repeat Yourself), secondo cui ==ogni pezzo di conoscenza deve avere una rappresentazione unica e non ambigua all'interno di un sistema==.

Problemi Generati dalla Duplicazione :
==La presenza di codice duplicato comporta gravi svantaggi tecnici ed economici== :
- ==Manutenzione Difficile== : Se si riscontra un errore in una porzione di codice duplicata, la correzione deve essere replicata manualmente in tutti i punti in cui quel codice appare. Se un punto viene dimenticato, l'errore (bug) rimarrà nel sistema.
- ==Aumento del Debito Tecnico== : Il codice diventa inutilmente più lungo e complesso da leggere e comprendere, rendendo più oneroso l'inserimento di nuovi sviluppatori nel progetto.
- ==Inconsistenza== : Nel tempo, le varie copie possono iniziare a divergere leggermente a causa di modifiche parziali, creando comportamenti del software incoerenti e difficili da diagnosticare.
- ==Costi di Testing Elevati== : Ogni blocco duplicato richiede i propri test unitari, raddoppiando (o triplicando) lo sforzo necessario per garantire la copertura del codice.

Tipologie di Duplicazione (Cloni) :
==La duplicazione non è sempre identica parola per parola; si divide generalmente in quattro livelli== :
1. ==Cloni di Tipo 1== : Pezzi di codice esattamente uguali (salvo spazi bianchi e commenti).
2. ==Cloni di Tipo 2== : Pezzi sintatticamente uguali (stessa struttura, ma cambiano i nomi delle variabili o dei tipi).
3. ==Cloni di Tipo 3== : Pezzi simili con alcune modifiche (aggiunte, rimozioni o istruzioni riordinate).
4. ==Cloni di Tipo 4== : Pezzi di codice che eseguono lo stesso calcolo logico ma sono scritti in modi completamente diversi.

Tecniche di Ricerca dei Duplicati :
==Per rintracciare i duplicati, si utilizzano diversi approcci di analisi== :
- ==Corrispondenze Sintattiche== : Confronto testuale riga per riga (efficace solo per il Tipo 1).
- ==Analisi basata su Token== : Il codice viene trasformato in una sequenza di simboli (token), permettendo di ignorare nomi di variabili e formattazione.
- ==Abstract Syntax Tree (AST)== : Il codice viene trasformato in una struttura ad albero che rappresenta la gerarchia logica delle istruzioni. Questa tecnica è la più potente perché permette di individuare duplicazioni logiche anche se il testo appare differente.

Consiglio per il refactoring : La soluzione standard per eliminare la duplicazione è la tecnica Extract Method : si estrae il codice comune, lo si inserisce in una singola funzione e la si richiama ovunque sia necessario.


==6. Come si possono misurare le relazioni tra i moduli del software ?==

==Le relazioni tra i moduli (classi o pacchetti) determinano la manutenibilità e la stabilità di un sistema==. Queste relazioni si manifestano principalmente attraverso legami di dipendenza, come quando una classe A chiama un metodo di B, usa una variabile di tipo B o eredita da B.

Concetti Fondamentali : ==Accoppiamento e Coesione== :
Per valutare la qualità del design, si analizzano due forze contrapposte:
- ==Coesione== : Misura quanto un modulo sia focalizzato su una singola responsabilità. Una **coesione alta** è un obiettivo primario (principio SRP), poiché indica che il modulo fa "una sola cosa fatta bene".
- ==Accoppiamento== : Misura il grado di dipendenza tra i moduli. L'obiettivo è ottenere un **accoppiamento basso** per garantire che le modifiche a un modulo non si propaghino a catena su tutto il sistema.

> Relazione : In sistemi complessi, è fisiologico che un aumento della coesione porti a un aumento del numero di moduli e, potenzialmente, delle loro interazioni. La sfida dell'architetto è bilanciare questi due aspetti.

==Metrica di Henry-Kafura (Information Flow==) :
==Questa metrica valuta la complessità basandosi sul flusso di informazioni che entra ed esce da un modulo, misurando l'interazione del modulo con il resto del sistema e con l'ambiente==.
Si basa su ==due parametri principali== :
- ==FAN-IN== : Rappresenta le informazioni che fluiscono verso il modulo. Indica quanti altri moduli chiamano il modulo in esame o gli passano dati.
- ==FAN-OUT== : Rappresenta le informazioni che escono dal modulo. Indica il numero di moduli chiamati dal componente o il numero di variabili globali di cui ha bisogno per funzionare.
==Formula della Complessità ($C_p$)== :
$$C_p = (\text{fan-in} \times \text{fan-out})^2$$
Interpretazione dei valori :
- ==Classi di Alto Livello== : Dovrebbero avere un alto Fan-in (molte parti del sistema le usano) e un basso Fan-out (non devono dipendere da dettagli tecnici o moduli instabili).
- ==Un valore di $C_p$ molto elevato indica un potenziale punto critico del sistema che potrebbe richiedere un refactoring per ridurre le dipendenze o dividere le responsabilità==.

==Metrica di Card e Glass== :
==Questa metrica scompone la complessità di un modulo in due componenti== :
1. ==Complessità Strutturale ($S$)== : Basata sul fan-out del modulo ($S = f^2_{out}$).
2. ==Complessità dei Dati ($D$)== : Basata sul numero di variabili di input/output che passano attraverso l'interfaccia.
==La complessità totale del sistema è data dalla somma delle complessità medie dei singoli moduli==. Anche in questo caso, l'obiettivo è minimizzare l'impatto delle dipendenze esterne per mantenere il sistema flessibile.
![[Pasted image 20260101130157.png]]


==7. Cosa si intende e come si descrive la coesione e l’accoppiamento dei moduli di un software ?==

Un buon design software ha l'obiettivo di rendere il sistema facile da comprendere, modificare, testare e riutilizzare. Questo obiettivo si raggiunge ottimizzando due parametri fondamentali : Alta Coesione e Basso Accoppiamento.

==La Coesione (Intra-modulare)== :
==La coesione misura il grado di connessione tra gli elementi interni a un singolo modulo (classe o pacchetto)==. Indica quanto le responsabilità interne siano focalizzate verso un ==unico scopo funzionale==.
Livelli di Coesione (dal più basso al più alto) :
- ==Coincidental (Coincidenziale)== : Elementi messi insieme senza una logica (violazione totale dell'SRP).
- ==Logical (Logica)== : Il modulo esegue operazioni simili ma distinte (es. un modulo che gestisce tutti i tipi di input/output).
- ==Temporal (Temporale)== : Gli elementi sono raggruppati perché vengono eseguiti nello stesso momento (es. una funzione di inizializzazione).
- ==Procedural (Procedurale)== : Gli elementi seguono una specifica sequenza di controllo.
- ==Communicational (Comunicativa)== : Gli elementi operano sugli stessi dati di input/output.
- ==Functional (Funzionale)== : Il livello massimo. Il modulo esegue una sola operazione o funzione logica coerente.
Metriche di Misura (Slice & Tokens) :
==Per misurare la coesione si analizzano i Data Token (variabili e costanti) e gli Slice (porzioni di codice che influenzano una variabile)== :
- ==Glue Token== : Token utilizzati in più di uno slice (indicano coesione).
- ==Superglue Token== : Token presenti in tutti gli slice del modulo (massima coesione).
![[Pasted image 20260101131026.png]]

==L'Accoppiamento (Inter-modulare)== :
==L'accoppiamento misura il grado di interdipendenza tra due o più moduli==. ==Un accoppiamento alto è negativo perché rende il codice fragile== (una modifica a un modulo rompe l'altro) ==e difficile da riutilizzare==.
Tipologie di Accoppiamento (dal peggiore al migliore) :
- ==Content (Di Contenuto)== : Un modulo modifica direttamente i dati interni di un altro.
- ==Common (Comune)== : Più moduli condividono le stesse variabili globali.
- ==Control (Di Controllo)== : Un modulo passa informazioni a un altro per influenzarne la logica interna (es. flag di controllo).
- ==Stamp (Di Struttura)== : I moduli si scambiano intere strutture dati, anche se ne usano solo una parte.
- ==Data (Di Dati)== : I moduli si scambiano solo i dati strettamente necessari.
Metrica di Fenton e Melton :
==Valuta l'accoppiamento tramite una formula $C(x, y) = i + \frac{n}{n+1}$, dove $i$ è il livello di accoppiamento e $n$ è il numero di collegamenti tra i moduli==.
![[Pasted image 20260101131055.png]]

==Analisi Afferente ed Efferente== :
==Per misurare l'impatto di un modulo nell'architettura, si utilizzano le metriche di dipendenza== :
- ==Accoppiamento Afferente ($Ca$)== : Numero di dipendenze in entrata. Indica quanti altri moduli dipendono da questo. Un valore alto indica grande responsabilità : modificare questo modulo è rischioso perché l'impatto è vasto.
- ==Accoppiamento Efferente ($Ce$)== : Numero di dipendenze in uscita. Indica quanto questo modulo dipende dagli altri. Un valore alto indica fragilità : se uno qualsiasi dei moduli esterni cambia, questo modulo potrebbe rompersi.


==8. Quali sono le principali misure che caratterizzano un software costruito con un linguaggio Object Oriented (CK metrics) ?==

==Nella programmazione orientata agli oggetti (OOP), la qualità del design dipende da come le classi interagiscono e da quanto sono focalizzate==. ==Le metriche CK==, introdotte da Chidamber e Kemerer nel 1994, ==rappresentano lo standard per valutare oggettivamente la complessità, la manutenibilità e la riusabilità di un software basato su classi==.
L'obiettivo ideale è sempre ottenere classi con alta coesione e basso accoppiamento.

==WMC (Weighted Methods per Class) - Metodi Ponderati per Classe== :
==Misura la complessità complessiva di una classe sommando la complessità di tutti i suoi metodi==.
- Significato : Se tutti i metodi hanno complessità unitaria, WMC è semplicemente il numero totale di metodi.
- Impatto : Un valore WMC elevato indica che la classe è difficile da mantenere, testare e riutilizzare, poiché accentra troppe funzionalità.

==DIT (Depth of Inheritance Tree) - Profondità dell'Albero di Ereditarietà== :
==Indica la lunghezza massima del percorso gerarchico dalla classe radice fino alla classe in esame==.
- Significato : Quanto è profonda la gerarchia di ereditarietà.
- Impatto : Più l'albero è profondo, maggiore è la complessità, poiché una classe eredita comportamenti da molti livelli superiori. Questo rende più difficile prevedere il comportamento della classe e aumenta il rischio di errori.

==NOC (Number of Children) - Numero di Sottoclassi== :
==Conta il numero di discendenti diretti (sottoclassi) di una classe==.
- Significato : Misura quanto una classe è "padre" nella gerarchia.
- Impatto : Un NOC alto indica un elevato riutilizzo del codice tramite ereditarietà, ma suggerisce anche che un errore nella classe base influenzerà moltissime sottoclassi, richiedendo test molto estesi.

==CBO (Coupling Between Object Classes) - Accoppiamento tra Classi== :
==Rappresenta il numero di altre classi a cui una classe è legata== (tramite chiamate a metodi, variabili istanza, ereditarietà, ecc.).
- Significato : Misura l'interdipendenza tra i moduli.
- Impatto : Per un buon design, il CBO deve essere basso. Un accoppiamento eccessivo rende il sistema rigido: cambiare una classe obbliga a modificare tutte le classi accoppiate.

==RFC (Response For a Class) - Risposta per una Classe== :
==Rappresenta l'insieme di tutti i metodi che possono essere eseguiti in risposta a un messaggio ricevuto da un oggetto di quella classe==. Include i metodi interni della classe e quelli chiamati su altri oggetti.
- Significato : Misura la potenziale comunicazione della classe con il resto del sistema.
- Impatto : Un RFC alto aumenta la complessità dei test e del debugging, poiché il flusso di esecuzione si sposta frequentemente fuori dalla classe stessa.

==LCOM (Lack of Cohesion in Methods) - Mancanza di Coesione nei Metodi== :
==È la metrica più importante per valutare la coesione. Misura quanto i metodi di una classe condividono gli stessi attributi (variabili istanza)==.
- Valutazione :    
    - ==LCOM = 0== : Massima coesione (tutti i metodi usano gli stessi attributi).
    - ==LCOM = 1 (o valori alti)== : Scarsa coesione (i metodi operano su dati diversi).
- Impatto : Una classe con LCOM alto dovrebbe essere scomposta in due o più classi più piccole, seguendo il _Single Responsibility Principle_ (SRP).
![[Pasted image 20260101131841.png]]


### Implementation
==1. Che cosa si intende per fase di implementazione e quali sono le caratteristiche di questa fase ? In che modo le caratteristiche si influenzano e quando assumono una particolare importanza ? Che importanza è opportuno dare all’ottimizzazione del codice ?==

La ==fase di implementazione== è il ==processo di trasformazione del progetto dettagliato (design) in un programma eseguibile, scritto in uno specifico linguaggio di programmazione==.
- Nei ==progetti piccoli==, il design dettagliato è spesso considerato parte integrante dell'implementazione stessa.
- Nei ==progetti grandi==, le figure professionali sono distinte : i progettisti definiscono le specifiche e i programmatori le traducono in codice.

==Caratteristiche Fondamentali== :
Durante questa fase, ==il codice deve rispettare alcune proprietà essenziali per garantire la qualità del prodotto== :
- ==Leggibilità== : Il codice deve essere chiaro per facilitare la manutenibilità e la verifica della correttezza.
- ==Tracciabilità== : Deve essere possibile collegare ogni porzione di codice a uno specifico requisito (fondamentale per verifica e validazione).
- ==Completezza== : Il codice deve implementare tutte le funzionalità previste, garantendo il comportamento corretto del sistema.
- ==Manutenibilità== : La struttura del codice deve permettere adeguamenti futuri ai cambiamenti senza costi eccessivi.
- ==Prestazioni== : Capacità del codice di rispettare i vincoli di tempo e risorse (critica nei sistemi real-time).

==Interdipendenza e Conflitti tra Caratteristiche== :
==Le caratteristiche del software non sono isolate, ma si influenzano reciprocamente, spesso entrando in conflitto==.
L'esempio classico è il rapporto tra Ottimizzazione e Leggibilità : un codice estremamente ottimizzato per le prestazioni (es. uso di trucchi a basso livello o assembly) tende a diventare oscuro, compromettendo la leggibilità e, di conseguenza, la manutenibilità.
==L'obiettivo dell'ingegneria del software è trovare un equilibrio== (trade-off) ==basato sulle priorità del progetto== : un sistema bancario privilegerà la correttezza e la tracciabilità, mentre un driver video darà priorità alle prestazioni.

==L'Importanza dell'Ottimizzazione del Codice== :
L'ottimizzazione non deve essere un fine in sé, ma uno strumento mirato.
- Regola d'oro : ==L'ottimizzazione ha generalmente una bassa importanza relativa==, a meno che non sia necessaria per soddisfare specifici requisiti non funzionali (es. limiti di memoria o tempi di risposta minimi).
- Approccio corretto : ==L'ottimizzazione deve essere eseguita solo dopo aver misurato le prestazioni reali del sistema (profiling)==. Ottimizzare prematuramente porta spesso a un codice inutilmente complesso e difficile da gestire ("Premature optimization is the root of all evil").


==2. Nozione dello standard ISO/EIC 25010==

==Lo standard ISO/IEC 25010 è il riferimento internazionale che definisce i criteri per valutare la qualità di un prodotto software==. Sostituisce il precedente ISO 9126 e si articola in ==due modelli principali== : il ==modello della Qualità del Prodotto (statica)== e il ==modello della Qualità in Uso (dinamica)==.

==Modello della Qualità del Prodotto (8 Caratteristiche)== :
==Questo modello analizza le proprietà intrinseche del software==. È utile ==durante la progettazione e lo sviluppo== per ==misurare quanto il sistema sia ben costruito==.
- ==Idoneità Funzionale (Functional Suitability)== : Il grado in cui il software fornisce funzioni che soddisfano le esigenze dichiarate (completezza e correttezza funzionale).
- ==Efficienza delle Prestazioni (Performance Efficiency)== : Capacità del sistema di rispondere entro tempi adeguati e con un uso ottimale delle risorse.
- ==Compatibilità (Compatibility)== : Grado in cui il prodotto può scambiare informazioni con altri sistemi o condividere lo stesso ambiente hardware/software.
- ==Usabilità (Usability)== : Facilità con cui gli utenti possono imparare a usare il sistema e quanto sia soddisfacente l'interazione.
- ==Affidabilità (Reliability)== : Capacità del sistema di mantenere un livello specificato di prestazioni in condizioni definite per un periodo di tempo.
- ==Sicurezza (Security)== : Capacità di proteggere le informazioni e i dati, garantendo che solo le persone autorizzate vi abbiano accesso.
- ==Manutenibilità (Maintainability)== : Facilità con cui il software può essere modificato, corretto o migliorato (include modularità e riusabilità).
- ==Portabilità (Portability)== : Facilità con cui il software può essere trasferito da un ambiente hardware o software a un altro.

==Modello della Qualità in Uso (5 Caratteristiche)== :
==Questo modello si focalizza sull'impatto che il software ha sull'utente finale e sul business quando viene effettivamente utilizzato nel suo contesto reale==.
- ==Efficacia (Effectiveness)== : Accuratezza e completezza con cui gli utenti raggiungono i propri obiettivi.
- ==Efficienza (Efficiency)== : Rapporto tra le risorse impiegate e l'accuratezza/completezza dei risultati ottenuti.
- ==Soddisfazione (Satisfaction)== : Grado in cui le esigenze dell'utente sono soddisfatte durante l'uso del prodotto.
- ==Libertà dal Rischio (Freedom from Risk)== : Capacità del sistema di mitigare i rischi potenziali per l'economia, la salute, la sicurezza o l'ambiente.
- ==Copertura del Contesto (Context Coverage)== : Il grado in cui il software può essere utilizzato con efficacia, efficienza e soddisfazione in contesti d'uso specifici e differenti.


==3. Cosa si intende per stile di programmazione ?==

L'==implementazione== non è una semplice attività di scrittura, ma ==un processo ingegneristico che mira a produrre codice di alta qualità==. Questo obiettivo si raggiunge attraverso l'==adozione di uno stile di programmazione rigoroso== e l'==attenzione a diverse caratteristiche fondamentali==.

Definizione di Stile di Programmazione :
Con ==stile di programmazione== si intende l'==insieme di convenzioni, regole e buone pratiche adottate per scrivere codice in modo organizzato, coerente e leggibile==. Lo stile non riguarda il linguaggio scelto, ma il modo in cui il programmatore lo utilizza.

I pilastri di un ==buon stile== sono :
- ==Leggibilità== : Uso di un'identazione chiara, spaziature adeguate e nomi di variabili/funzioni descrittivi (es. `calcolaTotaleOrdine()` invece di `func1()`).
- ==Modularità== : Organizzare il codice in componenti piccoli e indipendenti per ridurre la complessità cognitiva.
- ==Coerenza== : Applicare le stesse convenzioni in tutto il progetto per facilitare il lavoro di squadra.
- ==Commenti== : Utilizzarli per spiegare il "perché" di una scelta complessa, evitando di commentare l'ovvio.

Caratteristiche di Qualità del Codice :
Mentre gli sviluppatori tendono spesso a focalizzarsi solo su Correttezza (il codice fa ciò che deve) e Performance (efficienza), ==un'implementazione professionale deve garantire anche== :
- ==Manutenibilità== : Il codice deve essere facilmente modificabile per correggere bug o aggiungere funzioni senza rompere le parti esistenti.
- ==Tracciabilità== : Ogni riga di codice deve essere riconducibile a un elemento del design o a un requisito specifico.
- ==Completezza== : Garanzia che tutti i requisiti funzionali siano stati effettivamente implementati.

Attività Fondamentali dell'Implementazione :
Oltre alla scrittura della sorgente, l==a fase di implementazione comprende attività critiche== :
- ==Testing== : Sottoporre il codice a verifiche approfondite (Unit Test, Integration Test) per identificare e correggere gli errori precocemente.
- Version Control (Gestione delle versioni) : Utilizzare strumenti come Git per tracciare la storia del codice, gestire le modifiche nel tempo e permettere la collaborazione tra più programmatori.


==4. Come possono essere classificati i commenti ?==

==I commenti sono uno strumento fondamentale per la leggibilità e la manutenibilità del software, ma il loro abuso o un uso errato possono paradossalmente rendere il codice più difficile da leggere==. L'obiettivo deve essere scrivere codice "auto-esplicativo", utilizzando i commenti solo dove necessario per aggiungere valore non espresso dal codice stesso.

Classificazione dei Commenti :
==I commenti possono essere suddivisi in sei categorie principali== :
- ==Ripetizioni del codice== : Commenti che dicono esattamente ciò che fa la riga di codice successiva (es. `i = i + 1 // incrementa i`). Vanno evitati assolutamente perché non aggiungono informazioni, appesantiscono la lettura e rischiano di diventare obsoleti se il codice cambia.
- ==Spiegazioni del codice== : Traduzioni in lingua naturale di logiche particolarmente complesse o algoritmi non immediati.
- ==Marker nel codice== : Utilizzati per tracciare cambiamenti, versioni o per segnalare punti che richiedono attenzione futura (es. `// TODO: ottimizzare questo ciclo`).
- ==Riassuntivi== : Sintetizzano lo scopo di un intero blocco di codice o di un modulo, permettendo al programmatore di capire la funzione generale senza leggere ogni singola riga.
- ==Descrittivi dell'intento== : Spiegano perché il codice è stato scritto in un certo modo e quale risultato si intende ottenere, piuttosto che descrivere l'operazione tecnica. Sono tra i commenti più preziosi.
- ==Riferimenti esterni (External References)== : Commenti che rimandano a documentazione esterna, specifiche di progetto, bug tracker o link a librerie utilizzate.

Buone Pratiche e Trade-off :
==L'uso dei commenti richiede una ricerca costante di equilibrio (_trade-off_)== :
- ==Evitare i "commenti di scusa"== : Non utilizzare mai i commenti per giustificare o spiegare un codice scritto male. Se il codice è confuso, la soluzione corretta è il refactoring (riscrittura), non l'aggiunta di una spiegazione.
- ==Mantenimento== : Un commento errato o non aggiornato è peggiore di nessun commento, poiché fornisce informazioni fuorvianti che possono causare bug durante la manutenzione.
- ==Codice come documentazione== : Prima di scrivere un commento, chiediti se puoi rendere il codice più chiaro cambiando il nome di una variabile o estraendo una funzione.
  

==5. Cosa si intende per debugging e quali sono le fasi di quel processo ?==

==Il debugging è l'attività sistematica volta a individuare, analizzare e rimuovere le cause dei malfunzionamenti (bug) rilevati durante le fasi di test o di esercizio del software==. A differenza del testing, che ha lo scopo di _trovare_ gli errori, il debugging ha lo scopo di _risolverli_.

Le Fasi del Processo di Debugging :
==Per correggere un errore in modo efficace, è necessario seguire un percorso strutturato in quattro fasi== :
- ==Stabilizzazione== : Consiste nel rendere l'errore riproducibile in modo costante. In questa fase si cerca di isolare la configurazione specifica o l'input che scatena il bug per comprenderne le cause scatenanti (spesso con un approccio _black-box_).
- ==Localizzazione== : Una volta riprodotto l'errore, si analizza il codice per individuare l'esatta sezione, funzione o riga di comando che genera il comportamento anomalo.
- ==Correzione== : Si interviene sul codice sorgente modificando la logica o la struttura per risolvere definitivamente il problema identificato.
- ==Verifica== : È l'atto di assicurarsi che la correzione sia efficace. In questa fase è fondamentale eseguire il Regression Test (test di regressione) per garantire che la modifica non abbia introdotto nuovi errori in parti del sistema precedentemente funzionanti.

Classificazione degli Errori :
==Non tutti gli errori hanno la stessa gravità o difficoltà di risoluzione== :
- ==Errori Sintattici== : Sono violazioni delle regole grammaticali del linguaggio di programmazione. Sono i più semplici da correggere poiché vengono solitamente segnalati dal compilatore o dall'IDE durante la scrittura del codice.
- ==Errori Logici== : Sono i più insidiosi e gravi. Il programma viene eseguito senza crash, ma produce risultati errati o non soddisfa i requisiti del cliente. Indicano una mancata validazione del software o un difetto nel design della soluzione.


==6. Che cosa si intende per programmare per asserzioni ? In che modo Java supporta quel processo ? Quali sono le funzionalità offerte da junit per il debugging del software ? ==

==La programmazione per asserzioni è una tecnica di progettazione legata al concetto di Design by Contract==. Si basa sull'uso di ==speciali istruzioni (asserzioni) per verificare che la logica interna del programma sia corretta durante l'esecuzione==.
Vengono utilizzate principalmente ==per validare== :
- ==Precondizioni== : Condizioni che devono essere vere affinché un modulo produca risultati corretti.
- ==Postcondizioni== : Condizioni che devono essere vere al termine dell'esecuzione di un modulo.
- ==Invarianti== : Condizioni che devono rimanere costanti durante l'esecuzione di un blocco di codice.

==Se un'asserzione fallisce, il programma si arresta immediatamente lanciando un errore==. Questo permette di individuare bug logici già in fase di sviluppo e testing. Nota : Le asserzioni non devono essere usate per la gestione degli errori a runtime in ambiente di produzione, ma solo per il controllo della correttezza logica del codice.

Supporto alle Asserzioni in Java :
==Java supporta nativamente questa tecnica tramite la parola chiave `assert`==. Per impostazione predefinita, ==le asserzioni sono disabilitate per non influire sulle prestazioni==; devono essere attivate a runtime usando l'opzione `-ea` (enable assertions).
Esistono due forme sintattiche :
1. ==`assert EspressioneBooleana;`== : Se l'espressione è falsa, viene lanciato un `AssertionError` senza messaggi di dettaglio.
2. ==`assert EspressioneBooleana : EspressioneValore;`== : Se l'espressione è falsa, viene lanciato un `AssertionError` che include il valore dell'espressione (utile per fornire dettagli sull'errore).

JUnit e il Debugging del Software :
==JUnit è il framework standard per il testing unitario in Java==. Pur essendo uno strumento di test, offre funzionalità fondamentali che supportano il processo di debugging semplificando la localizzazione degli errori :
- ==Annotazioni per il ciclo di vita== :
    - ==`@Test`== : Identifica un metodo come caso di test.
    - ==`@BeforeEach` / `@BeforeAll`== : Preparano l'ambiente prima dei test (setup).
    - ==`@AfterEach` / `@AfterAll`== : Puliscono l'ambiente dopo i test (teardown).
- ==Metodi di Asserzione (`Assertions`)== : JUnit fornisce metodi come `assertEquals()`, `assertTrue()` o `assertNotNull()` per verificare che i risultati ottenuti corrispondano alle aspettative. Se un test fallisce, JUnit indica esattamente quale valore è stato ricevuto rispetto a quello atteso.
- ==Automazione e Isolamento== : Permette di eseguire test in modo automatico e isolato. Se un test fallisce dopo una modifica al codice, lo sviluppatore può localizzare immediatamente il bug (Regression Testing).
- ==Integrazione con IDE== : Gli strumenti di sviluppo (come IntelliJ o Eclipse) integrano JUnit consentendo di avviare i test con un clic e visualizzare graficamente quali parti del codice non rispondono correttamente ai requisiti.

   
==7. Cosa si intende per defensive programming ?==

==La programmazione difensiva è una pratica di sviluppo software il cui obiettivo primario è garantire la continuità operativa di un programma, anche di fronte a condizioni impreviste==. Si basa sull'assunto che "se qualcosa può andare storto, lo farà", e mira a rendere il codice robusto, sicuro e resistente agli errori.

==Obiettivi Principali== :
- ==Prevenire potenziali errori== : Anticipare situazioni anomale prima che causino il crash del sistema.
- ==Proteggere da input non validi== : Assicurarsi che i dati provenienti dall'esterno (utenti, file, API) non corrompano lo stato interno dell'applicazione.
- ==Migliorare la robustezza== : Fare in modo che il software sia in grado di gestire i problemi in modo "grazioso" (graceful degradation), fornendo messaggi di errore chiari invece di interrompersi bruscamente.

Tecniche Comuni di Programmazione Difensiva :
==Per implementare questo approccio, gli sviluppatori utilizzano diverse strategie pratiche== :
- ==Controllo degli Input== : Non fidarsi mai dei dati in ingresso. Ogni parametro deve essere validato prima di essere elaborato (controllo di tipo, range e formato).
- ==Gestione dei Valori Null (Evitare NullPointerException)== :  Utilizzare i Literal per i confronti : ad esempio, scrivere `"COSTANTE".equals(variabile)` invece di `variabile.equals("COSTANTE")`. Nel primo caso, se la variabile è null, il risultato è semplicemente `false`; nel secondo caso verrebbe lanciata un'eccezione.
    - Utilizzare classi contenitore come `Optional` (in Java) per gestire esplicitamente l'assenza di un valore.
- ==Uso delle Asserzioni== : Inserire `assert` per verificare che le condizioni interne (invarianti) siano rispettate durante lo sviluppo.
- ==Gestione delle Eccezioni== : Utilizzare blocchi `try-catch-finally` in modo oculato per catturare gli errori prevedibili e garantire che le risorse (come i file aperti) vengano sempre rilasciate.
- ==Principio del Privilegio Minimo== : Limitare l'accesso ai dati e alle funzioni solo a ciò che è strettamente necessario per ridurre la superficie di attacco e l'impatto di eventuali bug.

==Mentre la gestione degli errori si occupa di cosa fare dopo che un problema è stato rilevato, la programmazione difensiva cerca di evitare che il problema si presenti o di intercettarlo non appena si manifesta alla "frontiera" del modulo, impedendo che si propaghi nel resto del sistema==.


==8. Cosa si intende per refactoring del codice ?== 

==Il refactoring è una tecnica disciplinata che consiste nel modificare la struttura interna di un programma per renderlo più facile da comprendere e più economico da modificare, senza però alterarne il comportamento osservabile dall'esterno==.

Obiettivi del Refactoring :
==Non si tratta di aggiungere nuove funzionalità o correggere bug, ma di migliorare la qualità del design del codice esistente==. I principali obiettivi sono :
- ==Ridurre la complessità== : Semplificare logiche intricate e frammentare componenti troppo grandi.
- ==Eliminare il "Code Smell"== : Rimuovere segnali di cattiva progettazione come il codice duplicato o classi eccessivamente lunghe.
- ==Migliorare la leggibilità== : Rendere il codice auto-esplicativo per facilitare il lavoro di squadra e la manutenzione futura.

 Caratteristiche della Pratica :
- ==Processo Continuo== : Il refactoring non è un evento isolato, ma una pratica costante che accompagna lo sviluppo (spesso integrata nel ciclo _Test-Driven Development_).
- ==Sicurezza tramite i Test== : Prima di procedere, è fondamentale avere una solida suite di test automatizzati. Solo i test possono garantire che le modifiche strutturali non abbiano rotto le funzionalità esistenti.
- ==Strumenti di supporto== : Si utilizzano spesso _Profiler_ (per monitorare le prestazioni) e strumenti integrati negli IDE per automatizzare le operazioni di spostamento o rinomina.

Tecniche Principali di Refactoring :
==Esistono diversi "pattern" di refactoring, tra cui i più comuni sono== :
- ==Estrazione di Metodo (Extract Method)== : Quando un metodo è troppo lungo o complesso, si estrae una parte del suo codice e la si sposta in un nuovo metodo con un nome descrittivo. Questo migliora la modularità e la riusabilità.
- ==Introduzione di un Oggetto Parametro (Introduce Parameter Object)== : Se un metodo accetta troppi parametri (es. `x1, y1, x2, y2`), conviene raggrupparli in una nuova classe o oggetto (es. un oggetto `Point` o `Rectangle`). Questo riduce la complessità della firma del metodo e facilita il passaggio dei dati.
- ==Sostituzione dell'Algoritmo== : Sostituire un algoritmo complesso e poco efficiente con uno più semplice o performante, mantenendo invariato l'input e l'output.


==9. Indicare le principali linee guida per lo sviluppo del codice==

==Lo sviluppo del software moderno non punta solo alla "correttezza" immediata, ma alla capacità del sistema di evolvere nel tempo==. Le linee guida principali si concentrano su ==due pilastri== : ==la gestione oculata delle prestazioni e la massimizzazione della manutenibilità==.

Gestione delle Performance :
==Le prestazioni non devono essere l'unico obiettivo dello sviluppatore, poiché un'ottimizzazione prematura spesso danneggia la leggibilità e la manutenibilità del codice==.
- ==Ottimizzazione come ultimo step== : Si interviene sulle performance solo se strettamente necessario per soddisfare i requisiti. A volte, aumentare la potenza hardware (scaling verticale) è più economico che riscrivere codice complesso.
- ==Approccio sistematico== : Se si decide di ottimizzare, bisogna farlo tramite profiling (misurazione), intervenendo solo sui colli di bottiglia e verificando con i dati che i miglioramenti siano reali.

La Manutenibilità :
==La manutenibilità è la capacità del software di essere modificato==. Si divide in ==quattro tipologie== :
- ==Correttiva== : Interventi per rimuovere bug scoperti dopo il rilascio.
- ==Adattiva== : Modifiche necessarie per far funzionare il software in un nuovo ambiente (es. cambio sistema operativo o database).
- ==Perfettiva== : Implementazione di nuove funzionalità o miglioramenti richiesti dall'utente.
- ==Preventiva== : Rifattorizzazione (refactoring) di parti del codice per evitare problemi futuri, anche se al momento non ci sono errori.

Le 10 Regole di Fowler per la Qualità del Codice :
==Per garantire un codice leggibile e manutenibile, si possono seguire queste dieci regole fondamentali, ispirate ai principi di Martin Fowler== :
1. ==Unità di codice corte== : Ogni funzione o metodo dovrebbe idealmente non superare le **15 linee**. Questo facilita il rispetto del _Single Responsibility Principle_ (SRP).
2. ==Semplicità strutturale (No Nesting)== : Evitare strutture annidate complesse.
    - Sostituire gli `if` complessi con il polimorfismo (es. ogni sottoclasse gestisce il proprio comportamento specifico).
    - Usare le Guard Clauses (clausole di guardia): gestire subito i casi d'errore o particolari con un `return` anticipato, evitando blocchi `if-else` profondi.
3. ==Scrivi il codice una sola volta (DRY - Don't Repeat Yourself)== : Estrarre le parti comuni in una superclasse o in metodi condivisi.
4. ==Interfacce piccole== : Rispettare l'Interface Segregation Principle, creando interfacce specifiche per i client invece di un'unica interfaccia generica e ingombrante.
5. ==Modularità== : Suddividere il software in moduli logici indipendenti.
6. ==Basso Accoppiamento== : Progettare componenti che dipendano il meno possibile l'uno dall'altro per facilitare le modifiche isolate.
7. ==Bilanciamento dei Pacchetti== : Organizzare il codice in modo che i pacchetti abbiano dimensioni equilibrate e responsabilità chiare.
8. ==Codice Snello== : Mantenere la base di codice il più piccola possibile, rimuovendo parti morte o ridondanti.
9. ==Automazione dei Test== : Scrivere test automatizzati per garantire che le modifiche non introducano regressioni.
10. ==Codice Pulito (Clean Code)== : Rimuovere commenti obsoleti, mantenere una formattazione coerente e nomi auto-esplicativi.


==10. Indicare alcune tecniche di refactoring con possibili esempi (ad esempio estrazione di un metodo, estrazione di una superclasse, …)==

Il refactoring mira a trasformare il codice esistente in un design più pulito senza alterarne le funzionalità. Di seguito sono elencate le tecniche più comuni utilizzate per eliminare il "code smell" e migliorare la manutenibilità.

Estrazione di Metodo (Extract Method) :
Si applica quando un metodo è troppo lungo o contiene frammenti di codice che hanno uno scopo logico isolato.
- Problema : Un metodo esegue troppe operazioni, diventando difficile da leggere.
- Soluzione : Si estrae il frammento di codice in un nuovo metodo con un nome descrittivo.

Esempio :
- _Prima:_
    Java
```
    void stampaDettagli() {
        // Logica per calcolare il prezzo
        double totale = quantita * prezzoUnitario;
        // Logica per la stampa (estratta)
        System.out.println("Nome: " + nome);
        System.out.println("Totale: " + totale);
    }
```
- _Dopo:_
    Java
```
    void stampaDettagli() {
        double totale = calcolaTotale();
        stampaBanner(totale);
    }
    
    void stampaBanner(double totale) {
        System.out.println("Nome: " + nome);
        System.out.println("Totale: " + totale);
    }
```

Estrazione di Superclasse (Extract Superclass) :
Si applica quando due o più classi hanno metodi o campi in comune.
- Problema : Duplicazione di codice tra classi simili.
- Soluzione : Si crea una superclasse comune e si spostano (push-up) i membri comuni in essa.

Esempio :
- _Scenario:_ Hai una classe `Impiegato` e una classe `Dirigente` che hanno entrambe i campi `nome` e `stipendio`.
- _Dopo il Refactoring:_ Si crea la classe `Persona` (Superclasse) che contiene `nome` e `stipendio`, mentre le classi specifiche ereditano da essa.

Sostituzione di Condizionali con Polimorfismo :
Si applica quando si hanno istruzioni `switch` o `if-else` che scelgono comportamenti diversi in base al tipo di oggetto.
- Problema : Ogni volta che si aggiunge un nuovo tipo, bisogna modificare tutti i blocchi condizionali nel sistema.
- Soluzione : Si creano sottoclassi per ogni tipo e si implementa un metodo comune.

Introduzione di Clausole di Guardia (Guard Clauses) :
Si applica per eliminare l'annidamento eccessivo di `if`.
- Problema : Il codice è difficile da seguire a causa di molti livelli di indentazione (codice "a freccia").
- Soluzione : Gestire i casi d'errore o i casi particolari subito con un `return` anticipato.

**Esempio:**
- _Prima:_
    Java
```
    double getPrezzo() {
        if (isDisponibile) {
            if (isInSconto) {
                return prezzoScontato;
            } else {
                return prezzoNormale;
            }
        }
        return 0;
    }
```
- _Dopo (con Guard Clauses):_
    Java
 ```
    double getPrezzo() {
        if (!isDisponibile) return 0;
        if (isInSconto) return prezzoScontato;
        return prezzoNormale;
    }
```

Introduzione di Oggetto Parametro (Introduce Parameter Object) :
Si applica quando un metodo accetta un numero eccessivo di parametri correlati.
- Problema : Una firma del metodo come `calcolaDistanza(x1, y1, x2, y2)` è difficile da leggere e soggetta a errori di ordine.
- Soluzione : Raggruppare i parametri in un oggetto logico (es. una classe `Punto`).

Spostamento di Metodo (Move Method) :
Si applica quando un metodo viene usato più da un'altra classe rispetto a quella in cui è definito.
- Problema : Un modulo ha troppe dipendenze verso l'esterno (alto accoppiamento).
- Soluzione : Spostare il metodo nella classe che lo utilizza più frequentemente per aumentare la coesione.


### Testing and Quality Assurance
==1. Cosa si intende per qualità del software e come si ottiene un software di qualità ? In che modo/ attraverso quali prospettive si può valutare la qualità (cosa si intende per verifica e per validazione) ?==

==La qualità del software rappresenta il grado di conformità di un prodotto rispetto ai suoi requisiti funzionali (cosa deve fare) e non funzionali (come deve farlo, es. sicurezza, performance)==. Un software di qualità soddisfa le aspettative dell'utente finale, è affidabile e privo di errori critici che possano comprometterne l'utilizzo.

Verifica e Validazione (V&V) :
==La qualità si valuta attraverso due prospettive complementari== :
- ==Verifica== : Risponde alla domanda _"Stiamo costruendo il prodotto correttamente ?"_. Si accerta che il software sia conforme alle specifiche tecniche e di progettazione definite nelle fasi precedenti. Include analisi statica del codice e test unitari.
- ==Validazione== : Risponde alla domanda _"Stiamo costruendo il prodotto giusto ?"_. Si accerta che il software soddisfi i bisogni reali e le aspettative dell'utente finale. È un processo spesso soggettivo che coinvolge l'utente e valuta il software nel suo contesto d'uso.
![Image of verification vs validation in software testing](https://encrypted-tbn2.gstatic.com/licensed-image?q=tbn:ANd9GcRwBpraySvDc0xXYgLTIzVIzLxbU3VtpViGGsj1mfltBDeFrppR462o5zh8-NbgxK0xOhDwmZLhdzAwbtpPzzlGd8o3S9afgEhIhsXpK45ODWnq2LI)

Metodi per garantire la Qualità :
==Esistono due approcci principali, spesso confusi tra loro, ma con scopi diversi== :
- ==Quality Assurance (QA)== : Si concentra sul processo. È un insieme di attività preventive volte a garantire che le metodologie di sviluppo siano eseguite correttamente per evitare la nascita di difetti (include training del team e definizione di standard).
- ==Quality Control (QC)== : Si concentra sul prodotto. Sono le attività operative (come il testing) volte a individuare i difetti nel software già costruito prima che venga rilasciato.

Il Ruolo del Testing :
==Il testing è lo strumento principale per il controllo della qualità==. È un'attività sistematica (pianificata) e metodica (basata su checklist e procedure) che non termina finché il software è in esercizio.
==Tipologie di Testing== :
- ==Funzionale== : Verifica che ogni funzione risponda ai requisiti specificati.
- ==Non Funzionale== : Valuta performance, usabilità, sicurezza e scalabilità.
- ==Manuale== : Essenziale per valutazioni soggettive (UX) o scenari esplorativi.
- ==Automatizzato== : Fondamentale per test ripetitivi, veloci e regressioni su larga scala.
==Fasi del processo di testing== :
1. ==Pianificazione== : Definizione di obiettivi, strategie e casi di test (Test Cases).
2. ==Esecuzione== : Avvio dei test per identificare difetti (failures).
3. ==Documentazione== : Registrazione dei risultati per valutare oggettivamente la qualità.
4. ==Risoluzione dei difetti== : Correzione tramite debugging e successiva riverifica.

==Principi Fondamentali== :
- ==Early Testing== : Il testing deve iniziare il prima possibile. Errori individuati durante l'analisi dei requisiti costano molto meno rispetto a quelli trovati dopo il rilascio.
- ==Ambiente Reale== : I test devono essere eseguiti in condizioni che simulino l'ambiente esterno reale per gestire variabili impreviste.
- ==Rilevazione vs Correzione== : Il testing osserva i fallimenti (failures), mentre il debugging corregge i difetti (faults) sottostanti.


==2. Come si possono individuare gli errori in un software o in un artefatto a esso connesso ?==

==L'individuazione dei difetti è un processo multicriterio che coinvolge sia l'analisi del codice eseguibile che la revisione degli artefatti prodotti durante il ciclo di vita del software==.

==Il Testing (Analisi Dinamica)== :
==Il testing è il metodo principale per rilevare errori==. È una ==componente della Quality Assurance che riporta i difetti affinché vengano rimossi, riducendo il rischio di fallimenti critici==.
- ==Gravità vs Priorità== : Un errore viene valutato per la sua gravità (impatto tecnico e conseguenze) e per la sua priorità (urgenza della risoluzione in base alle condizioni di accadimento).
==Livelli di Testing== :
- ==Unit Testing== : Verifica delle singole unità di codice (metodi/classi), solitamente eseguito dallo sviluppatore.
- ==Integration Testing== : Verifica dell'interazione tra moduli e pacchetti diversi.
- ==System Testing== : Valutazione dell'intero sistema rispetto ai requisiti funzionali e tecnici.
- ==Acceptance Testing== : Fase di validazione finale eseguita dal cliente per confermare che il software risponda alle aspettative di business.
- ==Regression Testing== : Esecuzione di test dopo ogni modifica per garantire che il nuovo codice non abbia compromesso le funzionalità esistenti.

==Analisi Statica e Revisioni== :
==Queste tecniche permettono di trovare errori senza eseguire il programma (Testing Statico)== :
- ==Analisi Statica del Codice== : Uso di tool automatici per individuare vulnerabilità di sicurezza, violazioni di stile e potenziali bug sintattici.
- ==Code Review (Revisione del Codice)== : Controllo manuale tra pari (peer review) per identificare errori logici e migliorare la qualità del design.
- ==Ispezione degli Artefatti== : Revisione di documentazione, diagrammi UML, specifiche e requisiti. Individuare un errore nei requisiti prima dell'implementazione riduce drasticamente i costi di correzione.

==Analisi Dinamica e Debugging== :
- ==Debugging== : Processo sistematico per localizzare e correggere la causa radice di un errore emerso durante l'esecuzione.
- ==Analisi Dinamica== : Monitoraggio del software in tempo reale (uso memoria, CPU, tempi di risposta) per individuare anomalie comportamentali.
- ==Stress Testing e Simulazione== : Sottoporre il sistema a carichi di lavoro estremi per far emergere difetti che si manifestano solo in condizioni critiche di traffico o dati.

==Monitoraggio, Sicurezza e Nuove Tecnologie== :
- ==Security Testing== : Ricerca attiva di falle di sicurezza e vulnerabilità (es. penetration testing).
- ==Monitoraggio e Feedback== : Raccolta di log e segnalazioni dagli utenti finali in ambiente di produzione per identificare errori non emersi in fase di test.
- ==Testing basato su AI== : Utilizzo di algoritmi di intelligenza artificiale per generare casi di test complessi o prevedere le aree del codice più soggette a bug.


==3. Differenza tra fallimento, difetto e errore.==

Nel software engineering, ==esiste una precisa relazione causale tra le azioni umane, le anomalie nel codice e il comportamento del sistema durante l'esecuzione==. Questa catena è definita dallo standard internazionale come segue :
1. ==Errore (Error)== :
==L'Errore è un'azione umana che produce un risultato errato==. Si verifica durante le fasi di analisi, progettazione o scrittura del codice.
- Causa : Malintesi dei requisiti, distrazioni, mancanza di conoscenza tecnica o logica errata.
- Soggetto : È commesso dal programmatore, dall'analista o dal progettista.
- Esempio : Un programmatore scrive `>` invece di `>=` in una condizione di ciclo.
2. ==Difetto o Bug (Fault / Bug)== :
==Il Difetto è la manifestazione fisica dell'errore all'interno di un artefatto== (codice sorgente, diagramma di progettazione o documentazione).
- Natura : È un'anomalia statica presente nel software. Un difetto può rimanere latente nel codice per anni senza mai essere scoperto se la riga di codice specifica non viene eseguita.
- Relazione : L'Errore umano introduce un Difetto nel sistema.
- Esempio : La riga di codice con l'operatore relazionale errato scritta nell'esempio precedente.
3. ==Fallimento (Failure)== :
==Il Fallimento si verifica quando il sistema non esegue la funzione richiesta o si comporta in modo inatteso rispetto ai requisiti==.
- Natura : È un evento dinamico che accade esclusivamente durante l'esecuzione (runtime) del software in un ambiente specifico.
- Relazione : Un Difetto, se eseguito in determinate condizioni, causa un Fallimento.
- Esempio : Il programma si arresta improvvisamente (crash) o produce un calcolo errato nella fattura finale dell'utente perché il ciclo non ha incluso l'ultimo elemento.

La sequenza logica può essere riassunta come segue :
1. Un **ERRORE** (azione umana) genera...
2. Un **DIFETTO** (anomalia nel codice), che se eseguito porta a...
3. Un **FALLIMENTO** (comportamento esterno errato).

> **Nota importante:** Non tutti i difetti portano necessariamente a un fallimento. Se una porzione di codice contenente un difetto non viene mai raggiunta dal flusso di esecuzione, l'utente non percepirà mai alcun fallimento.

![[Pasted image 20260101192245.png]]


==4. Cosa si intende per testing del software ? Quali sono gli scopi del testing ? In che modo è possibile fare del test ? Esistono delle procedure automatizzate per supportare il testing ?==

==Il Testing è un processo fondamentale dell'Ingegneria del Software che consiste nella verifica e nella validazione di un sistema o di un'applicazione==. Il suo obiettivo è assicurarsi che il prodotto funzioni come previsto, soddisfi i requisiti specificati (funzionali e non funzionali) e sia privo di difetti significativi che potrebbero compromettere l'esperienza dell'utente o la sicurezza del sistema.

Gli Scopi del Testing :
==Contrariamente a quanto si possa pensare, il testing non serve a dimostrare che un programma è "perfetto"==. I suoi ==scopi principali== sono :
- ==Individuazione dei difetti== : Trovare il maggior numero possibile di errori (bug) affinché possano essere mitigati e corretti dal debugging.
- ==Valutazione della qualità== : Fornire una misura oggettiva dell'affidabilità, della sicurezza e dell'usabilità del software.
- ==Prevenzione dei fallimenti== : Ridurre il rischio che si verifichino comportamenti inattesi in ambiente di produzione.
- ==Verifica dei limiti== : Il testing può dimostrare la presenza di errori, ma, come affermato da Edsger Dijkstra, non può mai dimostrare l'assenza totale di essi.

Livelli di Testing (da Unit ad Acceptance) :
==Il processo di test è strutturato in livelli incrementali per isolare i problemi in diverse fasi dello sviluppo== :
1. ==Unit Testing== : Verifica delle singole unità di codice (classi o metodi) in isolamento.
2. ==Integration Testing== : Verifica dell'interazione tra moduli che sono stati già testati singolarmente.
3. ==System Testing== : Test dell'intero sistema integrato per verificarne la conformità ai requisiti complessivi.
4. ==Acceptance Testing== : Test finale condotto dall'utente o dal cliente per validare se il software è pronto per il rilascio.

Procedure Automatizzate per il Testing :
==L'automazione del testing è diventata una pratica essenziale per gestire la complessità dei software moderni==. Consiste nell'uso di strumenti software per eseguire test che altrimenti richiederebbero un intervento umano costante.
==Vantaggi dell'automazione== :
- ==Ripetibilità== : I test possono essere eseguiti migliaia di volte (ad esempio a ogni modifica del codice) senza sforzo aggiuntivo (Regression Testing).
- ==Precisione== : Elimina l'errore umano dovuto alla stanchezza o alla distrazione durante l'esecuzione di procedure ripetitive.
- ==Scalabilità== : Permette di gestire grandi volumi di dati o scenari complessi (come il caricamento simultaneo di migliaia di utenti).
==Strumenti principali== :
- ==JUnit== : Lo standard per il testing unitario in ambiente Java.
- ==Selenium== : Utilizzato per l'automazione dei test su browser e interfacce web.
- ==Postman== : Strumento leader per il testing e la documentazione delle API.

![Image of continuous integration and continuous testing workflow](https://encrypted-tbn3.gstatic.com/licensed-image?q=tbn:ANd9GcQvndlwyzQXDX8lj2Qf7ruI91jqtsywZeVp_12w14ViXmMvdRPA36Vis2sRwZS1sP2F5I8CdIbMNdL3TiB58TrijZXHIRSkomRISsEGyuVYzWU9Z4g)


==5. Chi esegue il testing ? Quando si fa il testing ? Cosa si intende per testing funzionale e non funzionale ?==

1. Chi esegue il testing ?
==Il testing è un'attività collaborativa che coinvolge diverse figure professionali e gli utenti finali== :
- ==Programmatori== : Eseguono principalmente lo Unit Testing per verificare la correttezza dei singoli moduli durante lo sviluppo.
- ==Tester Professionisti (QA Specialists)== : Esperti che pianificano ed eseguono strategie di test complesse per valutare oggettivamente la qualità, l'integrità e la sicurezza del prodotto.
- ==Utenti Finali== : Valutano l'usabilità e la rispondenza ai bisogni di business. Si distinguono due fasi cruciali :
    - ==Alpha Testing== : Condotto da utenti selezionati che fanno parte dell'organizzazione di sviluppo (ambiente controllato).
    - ==Beta Testing== : Condotto da utenti esterni all'organizzazione nel loro ambiente reale, prima del rilascio definitivo.

2. Quando si esegue il testing ?
==Il testing deve iniziare il prima possibile (Early Testing) e continuare per tutto il ciclo di vita del software== :
- ==Fase di Analisi== : La revisione e la verifica dei requisiti sono già forme di test (statico). Individuare un errore qui riduce drasticamente costi e tempi.
- ==Fase di Design== : Rivisitare il design per migliorarne la struttura è considerato testing preventivo.
- ==Fase di Sviluppo e Manutenzione== : Il testing prosegue durante l'implementazione e non termina finché il software è in uso, includendo aggiornamenti e bug fixing.
![Image of software testing life cycle phases](https://encrypted-tbn1.gstatic.com/licensed-image?q=tbn:ANd9GcQp8SLtaEsOLcMhIQKFbR1eQdP4-U_tFBWl5Oo0E_S0Qv0w7CWGoBaCgBOR1ju3q64pfLEsMsHZRiNJy-A13QYA5RXSm73ukJthfxse4b2-ImMXxI0)

3. Testing Funzionale (Black Box Testing) 
==Si concentra su cosa il sistema fa. Verifica che il software soddisfi i requisiti specificati e fornisca i risultati attesi per input determinati==.
- Obiettivo : Controllare correttezza, appropriatezza e completezza delle funzioni.
- Caratteristiche : Simula l'interazione dell'utente senza conoscere la struttura interna del codice (approccio a "scatola nera"). Include livelli che vanno dallo Unit testing fino all'Acceptance testing.
- Focus : Requisiti aziendali e tecnici, flusso dei dati e operazioni dell'interfaccia.

4. Testing Non Funzionale
==Si concentra su come il sistema si comporta. Valuta la qualità, le prestazioni e l'esperienza d'uso sotto diverse condizioni==.
- Obiettivi : Garantire che il sistema sia scalabile, veloce, stabile e sicuro.
- ==Principali tipologie== :
    - ==Performance Testing== : Valuta i tempi di risposta sotto carichi normali e pesanti.
    - ==Load Testing== : Verifica il comportamento del sistema con carichi di lavoro crescenti.
    - ==Stress Testing== : Testa il sistema sotto carichi estremi per identificarne i punti di rottura.
    - ==Usability Testing== : Valuta quanto il sistema sia intuitivo e facile da usare per l'utente.
    - ==Security Testing== : Ricerca vulnerabilità contro attacchi o accessi non autorizzati.
    - ==Compatibility Testing== : Verifica il corretto funzionamento su diversi dispositivi, browser e sistemi operativi.


==6. Che differenza c’è tra testing a livello di requisito (acceptance test), a livello funzionale (System test), a livello di specifica (Integration test), a livello di codice (Unit test) ?==

Il testing del software è organizzato in modo gerarchico. Ogni livello ha un obiettivo diverso, un diverso oggetto di analisi e viene eseguito da attori differenti.

1. ==Unit Test (Livello di Codice)== :
==È il livello più basso e granulare. Si concentra sulla verifica della singola unità logica (metodo, funzione o classe) in totale isolamento==.
- Cosa si testa : La logica interna del codice sorgente.
- Obiettivo : Verificare che ogni singolo componente sia corretto e gestisca bene gli input/output.
- Chi lo esegue : Lo sviluppatore che scrive il codice.

2. ==Integration Test (Livello di Specifica)== :
==Verifica l'interazione tra i diversi moduli o componenti del sistema che sono già stati testati singolarmente==.
- Cosa si testa : Le interfacce e il passaggio di dati tra i moduli (es. chiamata a un database, comunicazione tra due classi).
- Obiettivo : Identificare errori derivanti dall'integrazione di componenti sviluppati separatamente (incongruenze di dati o protocolli).
- Chi lo esegue : Sviluppatori o tester specializzati.

3. ==System Test (Livello Funzionale) ==:
==Valuta il sistema nel suo complesso per verificare che soddisfi i requisiti funzionali e tecnici definiti nel progetto==.
- Cosa si testa : L'intero software completamente integrato (approccio _Black-Box_).
- Obiettivo : Assicurarsi che il sistema funzioni correttamente da un punto di vista tecnico e operativo, includendo anche aspetti non funzionali (es. performance).
- Chi lo esegue : Team di testing professionisti (QA).

4. ==Acceptance Test (Livello di Requisito)== :
==È la fase finale del processo di test, condotta per validare se il sistema risponde ai bisogni di business e ai requisiti originali del cliente==.
- Cosa si testa : La rispondenza ai requisiti di alto livello e ai casi d'uso dell'utente.
- Obiettivo : Determinare se il sistema è pronto per il rilascio ("Go/No-Go"). Serve a ottenere l'accettazione ufficiale da parte del cliente.
- Chi lo esegue : Il cliente o l'utente finale (spesso attraverso le fasi di Alpha e Beta testing).

Tabella Comparativa di Sintesi :

|**Livello**|**Ambito di analisi**|**Focus**|**Documento di riferimento**|
|---|---|---|---|
|**Unit Test**|Codice|Logica interna|Design dettagliato|
|**Integration Test**|Interfacce|Flusso dati tra moduli|Specifiche tecniche|
|**System Test**|Funzionalità|Intero sistema|Requisiti di sistema|
|**Acceptance Test**|Requisiti|Bisogno dell'utente|Analisi dei requisiti|


==7. Come si scelgono i casi da testare ?==

==Esistono due approcci principali per determinare cosa testare, basati rispettivamente sulla struttura interna del codice o sui requisiti funzionali==.

1. ==Black-Box Testing (Basato sui Requisiti)== :
==In questo approccio si scelgono i casi di test basandosi solo sulle specifiche, senza conoscere il codice interno==. Le tecniche principali sono :
- ==Partizionamento in Classi di Equivalenza== : Si suddivide l'input in gruppi (classi) che il sistema dovrebbe trattare allo stesso modo. Si testa un solo valore per ogni classe (es. per un campo "età" tra 18 e 99, si testa un valore valido come 25 e uno non valido come 10).
- ==Analisi dei Valori Limite (Boundary Value Analysis)== : Molti errori si concentrano ai bordi degli intervalli. Si scelgono valori esattamente sul limite, appena sopra e appena sotto (es. per il range 18-99, si testano 17, 18, 19 e 98, 99, 100).
- ==Tabelle di Decisione== : Utili quando diverse combinazioni di input generano azioni diverse.

2. ==White-Box Testing (Basato sulla Struttura)== :
==Qui i casi di test sono scelti guardando la logica del codice sorgente==. L'obiettivo è massimizzare la copertura (coverage) :
- ==Statement Coverage== : Garantire che ogni riga di codice venga eseguita almeno una volta.
- ==Decision/Branch Coverage== : Garantire che ogni ramo di una struttura decisionale (ogni `if` e ogni `else`) venga percorso.
- ==Path Coverage== : Testare tutti i possibili percorsi logici all'interno di una funzione (tecnica più complessa e rigorosa).

 3. ==Criteri di Priorità e Rischio== :
Quando il tempo è limitato, i casi di test vengono scelti in base a :
- ==Analisi del Rischio== : Si testano prioritariamente le funzionalità critiche (es. il modulo pagamenti in un e-commerce).
- ==Frequenza d'uso== : Si scelgono i percorsi che l'utente compie più spesso (Happy Path).
- ==Cronologia dei difetti== : Si insiste sulle aree del codice che storicamente hanno presentato più bug (principio di "clusterizzazione" dei difetti).

4. ==Error Guessing== :
==Una tecnica basata sull'esperienza del tester, che consiste nello scegliere casi di test mirati a scenari "particolari" o tipici errori comuni che i programmatori tendono a fare== (es. inserire una stringa vuota, caratteri speciali o valori nulli).


==8. Come avviene il processo di testing ?==

==Il processo di testing non è un'attività isolata che avviene alla fine dello sviluppo, ma un vero e proprio ciclo di vita (STLC - Software Testing Life Cycle) che si svolge parallelamente allo sviluppo del software==.

Il Ciclo di Vita del Testing (STLC) :
==Il processo di testing moderno è articolato in diverse fasi sequenziali e iterative, ognuna con obiettivi e artefatti specifici== :

1. ==Analisi dei Requisiti== :
In questa fase, ==il team di test studia i requisiti (funzionali e non funzionali) per capire cosa deve essere testato==.
- Obiettivo : Identificare se i requisiti sono testabili e rilevare eventuali ambiguità o lacune già in questa fase (Testing Statico).

2. ==Pianificazione dei Test (Test Planning)== :
==Viene definito il Test Plan, il documento strategico che guida l'intero processo==.
- Attività : Definizione dell'ambito (scope), degli obiettivi, delle risorse necessarie, dei tempi e dei criteri di accettazione (quando un test può considerarsi superato).

3. ==Progettazione dei Test (Test Design)== :
==Si passa dalla strategia alla pratica, creando i dettagli operativi==.
- Attività : Creazione dei Test Cases (Casi di Test) e degli script di automazione. Un caso di test include : precondizioni, passi da eseguire, dati di input e risultati attesi.

4. ==Preparazione dell'Ambiente (Environment Setup)== :
==Viene allestito l'ambiente hardware e software in cui verranno eseguiti i test==.
- Obiettivo : Replicare il più fedelmente possibile l'ambiente di produzione dell'utente finale (database, server, dispositivi).

5. ==Esecuzione dei Test (Test Execution)== :
==I tester eseguono i casi di test pianificati==.
- Attività : I risultati reali vengono confrontati con i risultati attesi. Se un test fallisce, viene aperto un Bug Report per segnalare il difetto agli sviluppatori.
- Regression Testing : Dopo che gli sviluppatori hanno corretto i bug, si rieseguono i test per garantire che le modifiche non abbiano introdotto nuovi errori.

6. ==Chiusura del Ciclo di Test (Test Closure)== :
==Fase finale in cui si analizzano i risultati ottenuti==.
- Attività : Valutazione della copertura dei test, analisi delle metriche (quanti bug trovati, quanti risolti) e redazione del rapporto finale di test. Se i criteri di qualità sono soddisfatti, il software è pronto per il rilascio.


==9. Cosa si intende per review ? Come si progettano le review ? Quali sono i tipi di review ?==

==Le Review (o revisioni) rappresentano una forma di testing statico==. A differenza del testing dinamico, non richiedono l'esecuzione del codice, ma ==si basano sull'esame visivo e analitico degli artefatti (documenti, diagrammi o codice sorgente) per individuare errori, omissioni o violazioni degli standard nelle fasi iniziali dello sviluppo==.

1. Cosa si intende per Review ?
==La Review è un processo disciplinato in cui uno o più revisori esaminano un artefatto software (requisiti, design, codice, piani di test) con l'obiettivo di identificare difetti prima che vengano propagati alle fasi successive==. È una delle tecniche più efficaci per il controllo della qualità, poiché permette di correggere gli errori quando il costo di riparazione è ancora minimo.

2. Come si progettano le Review (Il Processo) ?
==Una review efficace non è una discussione informale, ma segue un processo strutturato in fasi== :
-  ==Pianificazione== : Definizione dell'obiettivo della review, selezione del team (revisori) e assegnazione dei ruoli.
- ==Preparazione== : Ogni revisore studia l'artefatto individualmente per identificare potenziali problemi o punti poco chiari.
- ==Riunione di Review (Meeting)== : Discussione collettiva dei rilievi emersi. L'obiettivo è registrare i difetti, non risolverli sul momento.
- ==Rilavorazione (Rework)== : L'autore dell'artefatto corregge i difetti identificati.
- ==Follow-up== : Verifica che tutte le correzioni siano state apportate correttamente e chiusura della procedura.

3. Tipi di Review.
==Esistono diversi livelli di formalità, scelti in base alla criticità del progetto== :
- ==Walkthrough (Meno formale)== : L'autore dell'artefatto guida gli altri membri del team attraverso il documento o il codice, spiegandone la logica. Lo scopo è principalmente didattico o di condivisione della conoscenza.
- ==Technical Review (Formale)== : Un incontro tra esperti tecnici volto a valutare l'idoneità del prodotto rispetto agli standard e alle specifiche. Si focalizza sulla correttezza tecnica e sulla qualità del design.
- ==Inspection (Molto formale)== : È la forma più rigorosa di revisione (spesso chiamata _Fagan Inspection_). È guidata da un moderatore addestrato e utilizza checklist specifiche e metriche per misurare la densità dei difetti. Prevede ruoli precisi (Moderatore, Lettore, Segretario, Autore).
- ==Peer Review== : Revisione effettuata da colleghi di pari livello. Nel codice viene spesso chiamata Code Review ed è fondamentale per mantenere uno stile coerente e ridurre il debito tecnico.

Ruoli principali in una Review formale :
- Moderatore (Facilitatore) : Gestisce la riunione e garantisce che il processo venga rispettato.
- Autore : Chi ha creato l'artefatto (ascolta i feedback per apportare correzioni).
- Lettore : Espone l'artefatto durante la riunione.
- Segretario (Scribe) : Registra ogni difetto o suggerimento emerso.


==10. Che cosa si intende per black/white box testing (equivalence partitioning, boundary value analysis)==

Le metodologie di testing si dividono principalmente in due approcci, a seconda che il tester abbia o meno visibilità sulla struttura interna del codice sorgente.

==Black Box Testing (Test Funzionale==) :
==In questo approccio, il tester verifica il comportamento del software senza conoscere la struttura interna o l'implementazione del codice==. Il test si basa esclusivamente sui requisiti e sulle specifiche funzionali, concentrandosi sulla relazione tra input e output.
Tecniche principali :
- ==Equivalence Partitioning (Partizionamento in classi di equivalenza)== : Gli input vengono suddivisi in "classi equivalenti", ovvero gruppi di valori che il sistema dovrebbe trattare allo stesso modo. Si testa un solo valore per ogni classe, riducendo il numero di test necessari.
- ==Boundary Value Analysis (Analisi dei valori limite)== : Poiché statisticamente la maggior parte degli errori si verifica ai margini degli intervalli di input, questa tecnica si concentra sul testare i valori ai limiti minimi e massimi delle classi di equivalenza.

==White Box Testing (Test Strutturale)== :
==Il tester ha pieno accesso al codice sorgente e verifica il funzionamento interno del sistema (percorsi logici, flussi di controllo e strutture dati)==. È tipicamente eseguito dagli sviluppatori durante le fasi di Unit e Integration testing.
Tecniche principali :
- ==Path Testing== : Analizza tutti i possibili percorsi logici che il programma può eseguire, garantendo che ogni ramificazione sia stata percorsa almeno una volta.
- ==Condition Testing== : Verifica che tutte le condizioni logiche (booleane) all'interno del codice siano valutate correttamente sia come `true` che come `false`.
- ==Loop Testing== : Si focalizza sui cicli (for, while), verificando il comportamento con zero iterazioni, una sola iterazione e il numero massimo previsto di ripetizioni.

Differenza tra Testing e Debugging :
Sebbene siano attività correlate, hanno scopi e responsabilità differenti :
- ==Testing== : È l'esplorazione sistematica del sistema per individuare e riportare i difetti. Il suo scopo è mostrare che il software non si comporta come previsto (identificazione delle _failures_).
- ==Debugging== : È il processo condotto dagli sviluppatori per localizzare la causa radice di un difetto e correggerlo nel codice sorgente.

Sintesi Comparativa

|**Caratteristica**|**Black Box Testing**|**White Box Testing**|
|---|---|---|
|**Conoscenza del codice**|Nessuna (Scatola nera)|Totale (Scatola trasparente)|
|**Focus**|Cosa fa il sistema (Requisiti)|Come è costruito (Logica interna)|
|**Eseguito da**|Tester, Utenti finali|Programmatori|
|**Obiettivo**|Validazione delle funzionalità|Verifica della struttura e copertura|


==11. Che cosa sono e a cosa servono le decision table ?==

==La Decision Table è una tecnica di progettazione dei test di tipo Black-Box utilizzata per modellare logiche di business complesse==. È particolarmente efficace quando il comportamento di un sistema dipende dalla combinazione di molteplici fattori o condizioni di input.

A cosa servono ?
==A differenza di tecniche più semplici (come il partizionamento in classi di equivalenza), le tabelle di decisione servono a== :
- ==Rappresentare in modo strutturato e visivo regole decisionali complesse==.
- ==Garantire la completezza del testing, assicurandosi che ogni possibile combinazione di condizioni sia stata considerata==.
- ==Identificare contraddizioni o lacune nei requisiti logici del software==.
- ==Essere utilizzate in contesti di sistema o di busines==s (non sono solitamente usate per lo Unit Testing, dove la logica è più atomica).

Struttura della Tabella.
==Una Decision Table è una matrice organizzata in quattro aree principali== :
- ==Condition Stub (Sinistra-Alto)== : L'elenco delle condizioni o degli input (variabili booleane o stati).
- ==Action Stub (Sinistra-Basso)== : L'elenco delle possibili azioni o output che il sistema può generare.
- ==Condition Entry (Destra-Alto)== : Le combinazioni di valori (Vero/Falso o SI/NO) per ogni condizione. Ogni colonna rappresenta una Regola.
- ==Action Entry (Destra-Basso)== : Indica quali azioni vengono eseguite per ogni specifica combinazione (regola).

Il concetto di "Regole" e "Collasso".
- ==Regole== : Ogni colonna della tabella definisce uno scenario di test unico. Se si hanno $n$ condizioni booleane, la tabella completa avrà $2^n$ regole.
- ==Collasso delle regole (Regole Combinate)== : Se il valore di una determinata condizione non influenza l'output finale in una specifica combinazione, quella riga può essere segnata come "irrilevante" (spesso indicata con un trattino `-`). Ciò permette di accorpare più colonne, semplificando la tabella senza perdere copertura.
![[Pasted image 20260101220557.png]]
![[Pasted image 20260101220620.png]]


==12. Che cosa sono e a che cosa servono i grafici causa/effetto ?==

==I grafici causa-effetto sono una tecnica di progettazione dei test di tipo Black-Box che permette di rappresentare visivamente le relazioni logiche tra le condizioni di input (cause) e i risultati attesi (effetti)==.

Cosa sono e a cosa servono ?
==Questi grafici fungono da ponte tra il linguaggio naturale dei requisiti e la logica formale necessaria per il testing==. Il loro scopo principale è :
- ==Visualizzare la logica di business== : Rappresentare graficamente le dipendenze tra input e output che altrimenti sarebbero descritte in testi complessi.
- ==Identificare combinazioni di test== : Aiutare il tester a selezionare il set minimo di casi di test necessario per coprire tutte le regole decisionali.
- ==Analizzare i vincoli== : Permettono di inserire vincoli (es. due input che non possono verificarsi contemporaneamente) che non sempre sono evidenti in una tabella.

Relazione con le Tabelle Decisionali.
==I grafici causa-effetto e le tabelle decisionali sono strettamente legati== :
- ==Intercambiabilità== : Entrambi rappresentano la stessa logica di business. È sempre possibile convertire un grafico causa-effetto in una tabella decisionale e viceversa.
- ==Processo di analisi== : Spesso il grafico viene disegnato per primo per comprendere meglio la logica, e successivamente viene trasformato in una tabella decisionale per definire rigorosamente i singoli casi di test.
- ==Contesti di applicazione== : Si applicano negli stessi contesti, ovvero sistemi con logiche decisionali complesse in cui l'output non dipende da un singolo valore ma da una combinazione di eventi.

Componenti del Grafico.
==Un grafico causa-effetto utilizza una simbologia simile alle porte logiche dell'elettronica== :
- ==Cause : Nodi di input== (es. "L'utente è loggato").
- ==Effetti : Nodi di output== (es. "Accesso consentito").
- ==Operatori Logici : Connettori che definiscono la relazione, come AND (tutte le cause devono essere vere), OR (almeno una causa vera), e NOT (negazione)==.
![[Pasted image 20260101221129.png]]


==13. E’ possibile generare test a partire da Use Case ?==

==Il testing basato sui casi d'uso è una tecnica fondamentale per il Black-Box testing a livello di sistema==. 

Generazione di Test a partire dagli Use Case.
Sì, ==è assolutamente possibile (e consigliato) generare casi di test a partire dagli Use Case (Casi d'Uso)==. ==Questa tecnica permette di validare il sistema dal punto di vista dell'utente finale, assicurandosi che il software supporti i processi di business reali==.

Fondamenti del Testing basato su Use Case.
==L'obiettivo principale è la copertura dei flussi operativi e dei requisiti funzionali e non funzionali, analizzati secondo le diverse prospettive degli Attori (utenti o sistemi esterni) che interagiscono con l'applicazione==.
- ==Simulazione dell'utilizzo reale== : Il test non verifica solo singole funzioni isolate, ma simula scenari completi di interazione per evitare lacune nella logica di processo.
- ==Focus sull'utente== : Il test viene progettato pensando a come l'utente utilizzerà concretamente il sistema per raggiungere un obiettivo specifico.

Elementi da Testare.
==Per trasformare un Use Case in casi di test efficaci, è necessario coprire tutti i percorsi descritti nella specifica== :
- ==Main Success Scenario (Flusso Principale)== : Il percorso "felice" (happy path) in cui tutto procede correttamente e l'obiettivo viene raggiunto senza errori.
- ==Alternative Paths (Percorsi Alternativi)== : Varianti del flusso principale che portano comunque al successo (es. diversi metodi di pagamento).
- ==Exception Paths (Percorsi di Eccezione)== : Gestione degli errori o situazioni in cui l'obiettivo non può essere raggiunto (es. credenziali errate, timeout del server).

Vantaggi di questo approccio.
- ==Rilevazione di difetti di integrazione== : Identifica problemi che emergono solo durante una sequenza di operazioni.
- ==Validazione dei requisiti== : Garantisce che il sistema faccia esattamente ciò che l'utente si aspetta.
- ==Facilità di Acceptance Testing== : Gli Use Case sono scritti in un linguaggio comprensibile al business, facilitando la creazione dei test di accettazione finale.


==14. Cosa si intende per control flow graph ?==

==Il Control Flow Graph (Grafo del Flusso di Controllo) è uno strumento fondamentale del White-Box Testing (o test strutturale)==. Viene utilizzato per ==rappresentare graficamente tutte le possibili strade che l'esecuzione di un programma può percorrere==.

Definizione e Struttura :
==Il CFG è un diagramma astratto che modella il comportamento logico di un frammento di codice o di un intero programma==. È composto da due elementi principali :
- ==Nodi== : Rappresentano istruzioni atomiche o blocchi sequenziali di codice (Basic Blocks) che non contengono salti o decisioni al loro interno.
- ==Archi (Edge)== : Rappresentano le transizioni di controllo tra i nodi, ovvero il passaggio da un'istruzione a quella successiva, basato su flussi sequenziali, salti condizionali (`if`, `switch`) o iterativi (`for`, `while`).

Utilizzo nel White-Box Testing :
==L'obiettivo principale dell'analisi del CFG è verificare la struttura interna del codice per garantire una copertura completa dei test. In particolare, permette di analizzare== :
- ==Copertura dei percorsi (Path Coverage)== : Assicurarsi che ogni ramificazione e ogni possibile combinazione di percorsi sia stata testata.
- ==Raggiungibilità== : Identificare "codice morto" (nodi che non possono mai essere raggiunti da alcun flusso di esecuzione).
- ==Presenza di cicli== : Individuare cammini infiniti o anomalie nella logica dei loop.

La Complessità Ciclomatica :
==Il CFG è la base per il calcolo della Complessità Ciclomatica di McCabe, una metrica software utilizzata per misurare la complessità logica di un programma==. ==Essa indica il numero di percorsi linearmente indipendenti attraverso il codice e aiuta a stabilire il numero minimo di casi di test necessari per coprire tutte le decisioni==.

   
==15. Che cosa si intende per  statement coverage, decision coverage, loop coverage, condition coverage e modified condition/decision coverage ?==

==Nel contesto del White-Box Testing, le metriche di copertura servono a misurare quanto accuratamente i casi di test "esercitano" la struttura logica del codice sorgente==, solitamente rappresentata tramite il _Control Flow Graph_.

1. ==Statement Coverage (Copertura delle Istruzioni)== :
==È il livello base di copertura. Assicura che ogni singola riga di codice eseguibile venga percorsa almeno una volta==.
- Obiettivo : Identificare "codice morto" o rami mai testati.
- Calcolo : $\frac{\text{Numero di istruzioni eseguite}}{\text{Totale istruzioni eseguibili}} \times 100$.
- Nota : Una copertura del 100% è considerata il requisito minimo ("morale") per lo sviluppo professionale, ma non garantisce l'assenza di bug logici.

2. ==Decision Coverage / Branch Coverage (Copertura delle Decisioni)== :
==Garantisce che ogni punto decisionale (come `if`, `while`, `for`) sia valutato almeno una volta come Vero e almeno una volta come Falso==.
- Proprietà : La Decision Coverage include sempre lo Statement Coverage (se copro tutti i rami, copro anche tutte le istruzioni), ma non è vero il contrario.
- Obiettivo : Verificare i percorsi alternativi generati dalle ramificazioni.

 3. ==Condition Coverage (Copertura delle Condizioni)== :
==Si focalizza sulle decisioni composte (es. `if (A or B)`). Richiede che ogni singola sub-condizione booleana (`A` e `B` individualmente) venga testata sia come vera che come falsa==.
- Differenza dalla Decision Coverage : La Decision Coverage guarda il risultato totale della parentesi; la Condition Coverage guarda i singoli componenti atomici.

4. ==Modified Condition/Decision Coverage (MC/DC)== :
==È un criterio molto rigoroso richiesto in sistemi critici (avionica, automotive). Richiede che== :
- ==Ogni condizione atomica influenzi il risultato della decisione finale in modo indipendente==.
- ==Si dimostri che cambiando una sola condizione (mentre le altre restano costanti), il risultato della decisione cambia==.
- ==Scopo : Ottenere un'alta affidabilità con un numero di test inferiore rispetto alla copertura di tutte le combinazioni possibili ($2^n$)==.

 5. ==Loop Coverage (Copertura dei Cicli)== :
==Si focalizza sulla correttezza delle iterazioni. Un test completo dei cicli dovrebbe verificare almeno tre scenari== :
-  ==Zero iterazioni== : Il ciclo viene saltato (condizione falsa all'inizio).
- ==Una iterazione== : Il corpo del ciclo viene eseguito una sola volta.
- ==Molte iterazioni== : Verifica del comportamento a regime e, se possibile, al numero massimo di iterazioni consentite.
![[Pasted image 20260101222749.png]]
![[Pasted image 20260101222809.png]]
![[Pasted image 20260101222831.png]]


==16. Semplici esercizi sul white testing : può essere richiesta l’individuazione di test da fare per raggiungere la massima copertura di statement o decision.==


==17. Che cosa è il path testing ?==

==Il Path Testing è una tecnica di White-Box Testing estremamente analitica che si basa sulla struttura logica del codice. Il suo obiettivo è garantire che ogni possibile "cammino" o rotta di esecuzione all'interno di un programma venga identificato ed esercitato attraverso casi di test specifici==.

Definizione e Metodologia :
==Questa tecnica utilizza il Control Flow Graph (CFG) per mappare visivamente il codice==. ==Un "percorso" (path) è una sequenza di nodi (istruzioni) e archi (transizioni) che inizia dal punto di ingresso del programma e termina nel punto di uscita==.
- ==Analisi dei flussi== : Il tester seleziona percorsi considerati "interessanti" o critici (flussi funzionali principali, percorsi più brevi, percorsi con logiche complesse).
- ==Rilevazione dei difetti== : È particolarmente efficace per individuare errori nelle interfacce tra moduli, bug nella logica decisionale e problemi legati all'ordine di esecuzione delle istruzioni.

Livelli di Copertura dei Percorsi :
==Dato che in programmi con molti cicli e condizioni il numero di percorsi totali può essere infinito, il Path Testing si focalizza su criteri specifici== :
- ==All-Paths Coverage== : Il test di ogni singolo percorso possibile (spesso impossibile per motivi di tempo e complessità).
- ==Basis Path Testing (Metodo di McCabe)== : Una tecnica che identifica un set di percorsi "linearmente indipendenti". Testando questi percorsi base, si ha la garanzia di aver esercitato ogni arco (decisione) e ogni nodo (istruzione) del grafo almeno una volta.

==Fasi operative== :
1. ==Costruzione del Grafo== : Si trasforma il codice sorgente in un Control Flow Graph.
2. ==Calcolo della Complessità== : Si determina la Complessità Ciclomatica per sapere quanti percorsi indipendenti esistono.
3. ==Definizione dei Percorsi== : Si elencano i cammini logici da seguire.
4. ==Creazione dei Casi di Test== : Si definiscono i dati di input necessari per forzare l'esecuzione di ciascuno dei percorsi identificati.

==Vantaggi del Path Testing== :
- ==Qualità Strutturale== : Assicura che nessuna parte del codice rimanga "oscura" o non testata.
- ==Efficienza== : Permette di concentrare le risorse sui percorsi logici più complessi, riducendo la ridondanza dei test.
- ==Prevedibilità== : Aiuta a stimare lo sforzo necessario per il testing in base alla complessità del grafo.


==18. Altre tecniche di test : ispezioni e review.== 

==Oltre al testing dinamico (esecuzione del codice), esistono tecniche di testing statico che permettono di individuare difetti negli artefatti (codice, requisiti, design) senza eseguirli. Le due metodologie principali sono le Ispezioni e le Review==.

==Ispezioni (Formali)== :
==L'ispezione è la forma più rigorosa e strutturata di analisi statica==.
- ==Processo formale== : Prevede ruoli ben definiti (Moderatore, Autore, Lettore, Segretario) e fasi precise (pianificazione, preparazione individuale, riunione, rilavorazione).
- ==Obiettivo== : Identificare difetti, violazioni di standard o condizioni errate basandosi su checklist (liste di controllo) obbligatorie.
- ==Caratteristiche== : È una tecnica molto efficace ma costosa in termini di tempo, motivo per cui viene spesso applicata solo su componenti critiche del sistema. Sebbene esistano strumenti per automatizzare parte dell'analisi (Analisi Statica Automatica), l'ispezione classica rimane un'attività di gruppo.

==Review (Informali o Tecniche)== :
==La Review è una tecnica meno rigida e più flessibile rispetto all'ispezione==.
- ==Flessibilità== : Può essere eseguita da un collega (Peer Review) o da un piccolo gruppo. Non richiede necessariamente una riunione formale; può avvenire anche tramite strumenti di commento asincrono.
- Obiettivo : Non serve solo a trovare bug, ma anche a condividere conoscenze, generare nuove idee o trovare soluzioni rapide a problemi di design.
- Caratteristiche : La lista di controllo è facoltativa e il processo non è strettamente regolamentato. È la tecnica più diffusa nelle aziende moderne (es. le _Pull Request_ nello sviluppo Agile) per la sua capacità di migliorare la qualità del codice in modo rapido e collaborativo.

Sintesi delle differenze :

|**Caratteristica**|**Ispezione**|**Review**|
|---|---|---|
|**Formalità**|Molto Alta|Media / Bassa|
|**Ruoli definiti**|Sì (Moderatore, Segretario, ecc.)|No (solitamente Autore e Revisore)|
|**Checklist**|Obbligatoria|Facoltativa|
|**Scopo primario**|Identificazione rigorosa dei difetti|Miglioramento qualità e condivisione idee|
|**Documentazione**|Report formale dei difetti|Commenti o note di revisione|


==19. Tecniche automatizzate : perché sono importanti ?==

==L'automazione del testing è diventata una pratica indispensabile nel moderno ciclo di sviluppo del software (specialmente in contesti Agile e DevOps). Consiste nell'uso di strumenti software per gestire l'esecuzione dei test, il confronto dei risultati e il reporting==.

Efficienza e Riduzione dei Costi :
==L'automazione permette di eseguire una vasta suite di test in una frazione del tempo richiesto per il testing manuale==.
- ==Velocità== : Una volta creato lo script, l'esecuzione è quasi istantanea.
- ==Risparmio a lungo termine== : Sebbene la creazione iniziale degli script richieda un investimento, il costo per ogni esecuzione successiva è quasi nullo, riducendo drasticamente le spese operative nel tempo.

Ampia Copertura dei Test :
==Consente di sottoporre l'applicazione a una quantità di verifiche impossibile da gestire manualmente==.
- ==Test di Regressione== : Ad ogni minima modifica del codice, è possibile rieseguire l'intera suite di test per garantire che non siano stati introdotti nuovi difetti.
- ==Test complessi== : Gestisce facilmente scenari multi-utente, grandi volumi di dati o stress test che sarebbero logisticamente impossibili per un operatore umano.

Consistenza e Affidabilità :
==A differenza degli esseri umani, gli strumenti automatizzati non soffrono di stanchezza o distrazione==.
- ==Precisione== : Ogni test viene eseguito esattamente nello stesso modo, garantendo risultati oggettivi e riproducibili.
- ==Eliminazione dell'errore umano== : Si evita il rischio di saltare passaggi critici o interpretare erroneamente i risultati durante procedure ripetitive e monotone.

Ottimizzazione delle Risorse Umane :
==L'automazione non sostituisce il tester, ma ne potenzia il ruolo==.
- ==Focus sul valore aggiunto== : Liberando le persone dai compiti ripetitivi (come i test di routine), queste possono dedicarsi ad attività a più alto valore, come il testing esplorativo, l'analisi dell'usabilità (UX) e la progettazione di strategie di qualità più sofisticate.


### Configuration Management, Integration, and Builds
==1. Cosa si intende per Software configuration management ? Da che cosa dipendono gli strumenti software utilizzati a supporto di questa fase ?==

==La Software Configuration Management è un processo sistematico di ingegneria del software dedicato alla gestione, al controllo e al tracciamento di tutti gli artefatti prodotti durante l'intero ciclo di vita del software==.

Cosa si intende per SCM ?
==Si tratta di un sistema integrato che funge da "memoria storica" del progetto==. Il suo obiettivo non è solo conservare i file, ma ==garantire che ogni modifica sia tracciata, gestita e integrata correttamente, evitando perdite di dati o conflitti tra i membri del team==.
==Gli artefatti gestiti includono== :
- ==Codice sorgente== : Tutte le versioni dei file di programmazione.
- ==Documentazione== : Requisiti, manuali utente, specifiche tecniche e piani di test.
- ==Risorse e librerie== : File di configurazione, icone, file multimediali e dipendenze esterne.

La sfida della complessità : Versioni e Relazioni :
==Gestire le singole versioni di un file (versioning) è un compito relativamente semplice==. ==La vera complessità risiede nella gestione delle relazioni tra gli artefatti==.
Per ogni versione del software, ==il sistema deve tenere traccia di legami complessi== : ad esempio, quale specifica di requisito corrisponde a quale versione della classe e quale versione del manuale in una lingua specifica (es. italiano vs inglese) è compatibile con quel rilascio.

Fattori che influenzano la scelta degli strumenti di supporto :
==Gli strumenti software utilizzati per la SCM (come Git, SVN, Jira o Jenkins) non sono scelti a caso, ma la loro selezione dipende da tre fattori critici== :
1. ==Comprensione delle attività e degli output== : È necessario analizzare quali processi aziendali devono essere supportati e quali tipologie di file (artefatti) il team produrrà.
2. ==Definizione degli output e delle relazioni== : Lo strumento deve essere in grado di gestire la forma specifica degli artefatti e, soprattutto, la rete di collegamenti che li unisce.
3. ==Definizione del framework di gestione== : La scelta dipende dalle metodologie adottate (es. Waterfall, dove il controllo è rigoroso e lineare, o Agile, dove è necessario gestire rami di sviluppo paralleli e frequenti integrazioni).
 

==2. Quali sono le funzioni fondamentali che supportano lo storage e la fase di integrazione e build ?==

==Nella gestione della configurazione del software, le fasi di archiviazione (Storage) e di costruzione del prodotto (Build & Integration) sono supportate da funzioni specifiche che garantiscono l'integrità e la coerenza del sistema==.

Storage e Modello di Accesso :
==Lo storage definisce le strutture necessarie per immagazzinare e controllare l'accesso a tutti gli artefatti. Questo sistema si basa su un Naming Model, ovvero una convenzione di denominazione univoca (che può includere versione, paese, lingua o modulo) per identificare ogni componente==.
Funzioni fondamentali di gestione (tipiche di sistemi come Git) :
- ==Create/Delete== : Creazione o rimozione di un artefatto nel repository.
- ==View/Modify== : Visualizzazione e modifica controllata degli artefatti.
- ==Return (Check-out/Check-in)== : Recupero di una versione specifica e riconsegna della versione modificata.
- ==Merge== : Unione di modifiche provenienti da rami di sviluppo diversi, gestendo i conflitti tramite notifiche e database unificati.
- ==Versione Stabile== : Il sistema identifica una versione "ufficiale" stabile, proteggendola da modifiche concorrenti non autorizzate.

Il Processo di Build :
==La Build è il processo di trasformazione del codice sorgente in un artefatto finale eseguibile (come file `.exe`, `.jar` o `.war`). Strumenti come Maven o Gradle automatizzano queste fasi==:
1. ==Compilazione== : Traduzione del codice sorgente in codice binario (eseguibile dalla macchina), identificando errori sintattici o semantici.
2. ==Linking (Collegamento)== : Risoluzione delle dipendenze e collegamento delle librerie esterne necessarie al funzionamento dell'applicazione.
3. ==Ottimizzazione== : Rimozione del codice superfluo per migliorare le prestazioni e ridurre la dimensione del pacchetto finale.
4. ==Packaging== : Creazione dell'artefatto finale pronto per la distribuzione.

Integrazione :
==L'Integrazione consiste nell'unire i vari moduli o componenti software sviluppati separatamente per verificare che funzionino correttamente come un unico sistema coeso==.
- Scopo : Identificare problemi di comunicazione tra le interfacce dei moduli.
- Automazione : Spesso integrata nel processo di Build (Continuous Integration), dove ogni modifica viene compilata e testata automaticamente insieme al resto del sistema.


### Software Support and Maintenance
==1. Perché la fase di supporto del software e manutenzione è importante ? Quali sono le operazioni che vengono svolte in questa fase ?==

==La fase di supporto e manutenzione inizia dopo il rilascio del software (post-vendita) e l'entrata in produzione==. È spesso la fase più lunga e costosa dell'intero ciclo di vita del software, arrivando talvolta a superare i costi dello sviluppo iniziale.

Perché è fondamentale ?
==Nessun software di grandi dimensioni è perfetto al momento del rilascio. La manutenzione è necessaria per diversi motivi== :
- ==Correzione dei difetti== : Gestire i bug che emergono solo quando il software viene utilizzato in contesti reali da un gran numero di utenti.
- ==Adattamento== : Il mondo esterno cambia (nuove leggi, nuovi sistemi operativi, nuovi hardware) e il software deve evolversi per restare funzionale.
- ==Soddisfazione del cliente== : Il supporto post-vendita serve a educare l'utente, monitorare l'utilizzo del sistema e fornire assistenza tempestiva, garantendo il valore dell'investimento fatto dal cliente.

Operazioni svolte in questa fase :
==Le attività di manutenzione si dividono solitamente in quattro categorie principali== :
1. ==Manutenzione Correttiva== : Identificazione e risoluzione dei bug segnalati dagli utenti dopo il rilascio.
2. ==Manutenzione Adattativa== : Modifiche apportate per far funzionare il software in un nuovo ambiente (es. migrazione su cloud o aggiornamento del database).
3. ==Manutenzione Perfettiva (Estensione)== : Aggiunta di nuove funzionalità o miglioramento delle prestazioni su richiesta dell'utente.
4. ==Manutenzione Preventiva== : Revisione del codice per prevenire problemi futuri e migliorarne la manutenibilità (rifattorizzazione).

Il dilemma : Manutenzione o Riprogettazione ?
==Quando le richieste di estensione diventano troppo complesse o costose perché il software ha "cambiato natura", sorge un bivio critico== :
- ==Continuare la manutenzione== : Può diventare insostenibile se il codice originale è troppo degradato.
- ==Riprogettazione (Re-engineering)== : Spesso si preferisce creare un nuovo sistema da zero se il costo dell'estensione supera quello dello sviluppo. Tuttavia, la riprogettazione comporta costi elevati non solo di programmazione, ma anche di training del personale e rischi di migrazione dati.


==2. E’ importante stimare il tasso di notifica di problemi ?==

Sì, ==stimare e monitorare accuratamente il tasso di arrivo (o di notifica) dei problemi è un'attività fondamentale per il successo di un progetto software nel post-vendita==.

Monitoraggio della "Fase Critica" (Post-Rilascio) :
==Dopo il rilascio in produzione, è fisiologico attendersi un picco di segnalazioni== (la cosiddetta "prima chiamata" per la correzione dei bug). Queste notifiche derivano dall'impatto del software con scenari d'uso reali che non potevano essere completamente previsti durante i test in laboratorio.

Il Paradosso dell'Assenza di Segnalazioni :
==Un basso tasso di notifica subito dopo il rilascio non è necessariamente un indicatore di qualità. Al contrario, può nascondere un rischio critico== :
- ==Mancato utilizzo== : Se non arrivano segnalazioni, spesso significa che il cliente non sta utilizzando il sistema.
- ==Mancato testing reale== : Se il software non viene usato attivamente, non viene "testato" sul campo. Di conseguenza, i bug rimangono latenti e pronti a emergere in modo massiccio non appena il carico di lavoro aumenterà.

Pianificazione delle Risorse :
==Stimare il tasso di notifica permette all'azienda di== :
- ==Dimensionare il team di supporto== : Sapere quanti tecnici servono per gestire il flusso di ticket nei primi mesi.
- ==Valutare la stabilità== : Se il tasso di notifica non accenna a diminuire nel tempo, significa che il software ha problemi strutturali che richiedono una manutenzione più profonda o una riprogettazione.
![[Pasted image 20260101230408.png]]


==3. In che modo può essere strutturato il centro di supporto ? Quali sono i ruoli che svolge ?==

==Il centro di supporto (o Service Desk) è tipicamente organizzato in un modello a tre livelli, ognuno con competenze specifiche==. ==Il funzionamento è regolato dagli SLA (Service Level Agreement), contratti che definiscono i tempi massimi di risposta e di risoluzione garantiti al cliente==.

==1° Livello : Supporto Clienti (Customer Service)== :
==È il punto di contatto diretto con l'utente finale==.
- Ruoli : Rappresentanti dell'assistenza clienti.
- Obiettivi : Ricevere le segnalazioni, registrare i ticket e fornire risposte immediate se la soluzione è già presente nel database (FAQ).
- Attività tecniche : Raccolgono tutti gli elementi necessari per riprodurre il difetto (screenshot, log, passi eseguiti) e interagiscono con la parte tecnica. Se non possono risolvere il problema, scalano la richiesta al livello superiore.

==2° Livello : Analisi Tecnica (Technical Support)== :
==Entra in gioco quando il problema richiede competenze specialistiche sul software==.
- Ruoli : Analisti del problema e ingegneri qualificati.
- Obiettivi : Analizzare la causa radice (_root cause analysis_) del difetto tecnico.
- Attività tecniche : Intervengono direttamente sul codice o sulla configurazione del sistema per creare la correzione (bug fix). Gestiscono le FAQ tecniche aggiornate per supportare il primo livello.

==3° Livello : Controllo delle Modifiche (Change Management)== :
==È il livello di governance che supervisiona l'intero ciclo di vita delle modifiche al software==.
- Ruoli : Gruppo di controllo delle modifiche (Change Control Board).
- Obiettivi : Gestire il flusso di approvazione, tracciamento e chiusura delle modifiche per garantire che non introducano nuovi rischi.
- Attività tecniche : Si occupa della pianificazione dei rilasci, della documentazione delle correzioni e delle procedure di installazione (deployment) presso il cliente.

Gestione delle Priorità :
==Un aspetto fondamentale del centro di supporto è lo stabilire i livelli di priorità per ogni segnalazione (es. Bloccante, Alta, Media, Bassa)==. ==La priorità determina l'ordine di intervento e assicura che le risorse si concentrino prima sui problemi che causano il maggior impatto al business del cliente==.


==4. Quali sono i problemi connessi con la distribuzione e l’installazione delle patch di manutenzione / miglioria del software ?==

==La gestione delle modifiche (manutentive o migliorative) e la loro distribuzione tramite patch o fix release comportano diverse sfide logistiche e tecniche che possono impattare sulla stabilità del sistema==.

Complessità del Processo di Modifica :
==Ogni intervento deve essere gestito tramite un Change Request Form (CRF), che include la stima dell'impegno, l'analisi degli impatti sui moduli DB e sugli altri componenti==.
- ==Rallentamenti== : L'eccessiva complessità dei moduli burocratici può rallentare il processo di risoluzione.
- ==Tracciabilità== : È fondamentale che ogni campo e ogni modifica siano documentati con rigore. Una documentazione incompleta è una delle cause principali di errori di implementazione o di conflitti tra versioni differenti del software.

Il Rischio delle "Correzioni di Emergenza" :
==Spesso, per sistemi critici inattivi (down), vengono applicate correzioni rapide ("Hotfix") al di fuori del normale ciclo di rilascio==.
- ==Sovrascrittura== : Esiste il rischio concreto che le future _fix releases_ cumulative non includano la correzione d'emergenza, sovrascrivendola e facendo ricomparire il bug originario (regressione).
- ==Incompatibilità== : Le patch spesso richiedono aggiornamenti simultanei di più componenti, aumentando il rischio di instabilità nei sistemi connessi.

Gestione della Distribuzione e Disallineamento dei Clienti :
==Un problema rilevante è legato al comportamento degli utenti finali e alla logistica di installazione== :
- ==Mancata installazione== : Non tutti i clienti applicano le patch immediatamente. Questo crea un parco macchine frammentato dove diversi clienti utilizzano versioni differenti del software, rendendo il supporto tecnico estremamente complesso.
- ==Sospensione dell'attività== : L'installazione di una patch può richiedere il fermo del sistema. Se il cliente ha un'attività critica sospesa, la pressione sul team di supporto aumenta, rendendo più probabili errori durante il deployment.

Strategie di Mitigazione :
==Per gestire correttamente queste criticità, è necessario== :
- ==Validazione preventiva== : Garantire che tutte le patch siano testate per la compatibilità con l'intero ecosistema prima del rilascio.
- ==Cadenze regolari== : Stabilire finestre di manutenzione e rilasci periodici per abituare il cliente all'aggiornamento costante.
- ==Tracciabilità totale== : Utilizzare sistemi di _Configuration Management_ per assicurarsi che ogni modifica d'emergenza venga poi integrata formalmente nel ramo principale del codice (_Mainline_).