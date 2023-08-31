---
layout: post_it
title:  Come valutare il debito tecnico con SonarQube
description: Cos'è il debito tecnico, come misurarlo e controllarlo con SonarQube.

permalink: come-valutare-debito-tecnico-sonarqube
english: how-to-evaluate-technical-debt-sonarqube
spanish: como-evaluar-deuda-tecnica-sonarqube

cover: /img/posts/2021-04-15-how-to-evaluate-technical-debt-sonarqube-1.png
---

Forse non sai cosa intendiamo quando parliamo di **debito tecnico**, ma sicuramente leggendo la parola "debito" puoi immaginare che non sia una buona cosa, e che è qualcosa che se non viene gestito, influenzerà in qualche modo i nostri progetti.

Ebbene, oggi voglio parlarti del **debito tecnico**, di come influisce sui tuoi progetti, e di come potete evitare i problemi che causerebbe.

## Che cos'è il debito tecnico?

In primo luogo, vedremo in cosa consiste il **debito tecnico** e, per questo, niente di meglio che confrontarlo come fosse un debito più conosciuto, il debito economico.

Nelle occasioni in cui si ha bisogno di una grande quantità di denaro (acquisto di una casa, nuova impresa, ecc ...) è necessario chiedere un prestito che, successivamente, dovrà essere restituito in piccole rate per un determinato periodo di tempo.

Ebbene, il termine **debito tecnico** si riferisce a quando abbiamo bisogno, in questo caso, di una quantità di tempo (sì, che è sostanzialmente denaro) per poter consegnare il lavoro concordato entro la data concordata.

## Come si genera debito tecnico?

Accade, ad esempio, quando **copiamo il codice** invece di creare una nuova classe che esegua la funzione di cui abbiamo bisogno, o quando **duplichiamo** invece di usare delle costanti.

In quei casi, chiediamo del tempo per poter consegnare prima, ma come nel debito tecnico, quel tempo dovrà essere restituirto, poiché se non lo facciamo, avremo solo problemi (sotto forma di errori nel progetto).

E poi, un'altra cosa in cui il debito tecnico è simile a quello economico, è che deve essere **pagato con gli interessi**. 

Se nel debito economico si paga una cifra aggiuntiva oltre alla quantità richiesta per estinguere il prestito, nel debito tecnico, si traduce in un tempo maggiore per risolvere una mala praxis, come ad esempio un code smell, cosa che non sarebbe accaduta se si fosse risolto il problema fin dall'inizio.

Quindi, il debito tecnico non è direttamente correlato all'affidabilità o alla sicurezza del nostro progetto, poiché si tratta principalmente di errori che si verificano nel nostro codice, ma è dovuto alle cattive pratiche e alla mancanza di lungimiranza. Possiamo perciò dire che è legato alla **manutenibilità**, ovvero alla facilità (o meno) di poter aggiornare o far evolvere i progetti.

## Come misurare il debito tecnico?

Ora che sai cos'è, passiamo a vedere **come viene misurato il debito tecnico, come capire quanto se ne ha e se è molto o poco**.

Come ti dicevo all'inizio, nel debito tecnico ciò che viene preso in prestito è il tempo; quindi, quello che **dovresti restituire è il tempo**. Ma questo debito tecnico influisce anche sulla **manutenibilità del codice**, come si calcola quanto debito tecnico ho? 

Tutte queste informazioni sono facilmente reperibili attraverso l'open-source per l'analisi statica del codice, [**SonarQube**](/6-ragioni-utilizzare-sonarqube) 

SonarQube, infatti, quando rileva un code smell, ti informa sul **tempo stimato per risolverlo**.

<img src="img/posts/2021-04-15-how-to-evaluate-technical-debt-sonarqube-1.png" width="100%" alt="Come misurare il debito tecnico con SonarQube">

## Gravità del debito tecnico

È importante essere consapevoli che questa valutazione dipende in gran parte dall'esperienza dello sviluppatore e può essere influenzata dalle particolarità del progetto, dell'organizzazione o persino della sua infrastruttura. Quindi, anche se non è un'informazione esatta, può servire come prima approssimazione.

Infatti conoscere il tempo che "a debito" non è sufficiente per conoscere il livello di gravità del debito tecnico di un progetto.

Non è lo stesso chiedere € 5.000 in prestito per acquistare un'auto che costa € 10.000, e chiedere € 5.000 in prestito per acquistare degli uffici che costano € 500.000.

Nel primo caso il debito è la metà del bene (l'auto) e in alcuni casi, se si verifica un imprevisto (ad esempio, nel caso in cui il debitore diventi disoccupato), il debito residuo costituirebbe un problema. Mentre nel secondo caso, il debito è una quota minima del totale e non dovrebbe causare problemi di liquidità all'organizzazione.

Per questo motivo **il debito tecnico deve essere rapportato al tempo totale di sviluppo del progetto** (che sarebbe equivalente al prezzo totale del bene), ed è per questo motivo che viene mostrato in percentuale.

Ad esempio, se si parla di un debito tecnico del 10%, significa che, se il progetto è stato sviluppato in circa 1.000 ore, il tempo per correggere le evidenze relative alla manutenibilità (code smells) è di circa 100 ore.

## Controllare il debito tecnico con SonarQube

[SonarQube](https://www.sonarsource.com/products/sonarqube/) attribuisce grande importanza al monitoraggio del debito tecnico.

Tanto che lo utilizza come uno dei suoi tre indicatori principali che sono: **affidabilità, sicurezza e manutenibilità**.

## Debito tecnico nel rating di manutenibilità globale

<img src="img/posts/2021-04-15-how-to-evaluate-technical-debt-sonarqube-2.png" width="100%" alt="Debito tecnico nel rating di manutenibilità globale in SonarQube">

Nel caso del rating di manutenibilità globale, SonarQube mostrerà il risultato in base al debito tecnico ottenuto.

Le valutazioni globali vanno da A (miglior valutazione) a E (peggiore valutazione) e sulla manutenibilità, SonarQube può mostrare i seguenti risultati:

 - A: Debito tecnico inferiore al 5%
 - B: Debito tecnico tra il 6% e il 10%
 - C: Debito tecnico compreso tra 11% e 20%
 - D: Debito tecnico tra il 21% e il 50%
 - E: Debito tecnico superiore al 50%


## Tempo necessario per risolvere il debito tecnico

D'altra parte, SonarQube mostra il tempo totale dei code smells nel progetto. Quindi, nell'immagine precedente, puoi vedere che nel nuovo codice (negli ultimi 30 giorni) c'è 1 code smells, il cui tempo approssimativo di soluzione è di 30 minuti, quindi il debito tecnico del nuovo codice sarà esattamente di 30 minuti.

Mentre nel progetto completo, ci sono più di 6.900 code smells e il tempo totale per risolverli sarà di circa 164 giorni.

Tieni presente che Sonarqube memorizza il debito tecnico in minuti, ma può mostrarlo in ore o giorni (1 giorno = 8 ore di lavoro).


## Monitoraggio del debito tecnico

Per tenere traccia del debito tecnico in SonarQube, abbiamo diverse opzioni.
Da un lato, nella sezione Misure, si può vedere il debito tecnico dell'intero codice, o solo quello del nuovo codice.

<img src="img/posts/2021-04-15-how-to-evaluate-technical-debt-sonarqube-3.png" width="100%" alt="Monitorare il debito tecnico in SonarQube">

Mentre nella Sezione **Activity**, possiamo vedere la storia del debito tecnico durante tutta la vita del progetto.

<img src="img/posts/2021-04-15-how-to-evaluate-technical-debt-sonarqube-4.png" width="100%" alt="Monitoraggio in SonarQube">

In questo modo, puoi vedere l'evoluzione del tuo debito tecnico anche se come abbiamo detto prima, solo in giorni.

Se vuoi davvero vedere cosa significa per il progetto, dovresti controllare il rapporto di indebitamento tecnico, e in questo modo puoi vedere meglio la sua evoluzione, indipendentemente dal fatto che il progetto sia cresciuto in numero di righe.

<img src="img/posts/2021-04-15-how-to-evaluate-technical-debt-sonarqube-5.png" width="100%" alt="Come tenere sotto controllo il debito tecnico con SonarQube">

E così hai imparato cos'è il debito tecnico e come tenerlo sotto controllo grazie a SonarQube.

Quindi, cerca di non prendere troppo in prestito, che in futuro dovrai pagarlo... e con gli interessi!


E se hai bisogno di mantenere sotto controllo il tuo codice o di avere dei report dettagliati sul suo andamento, dai un'occhiata ai nostri **Plugins per SonarQube**, ti aiuteranno a mantenere sotto controllo e migliorare la qualità del tuo codice.
<br>
<br>
<a href="/it/products" class="btn btn-primary btn-call-to-action fancybox" style="font-weight:bold;font-size:15px; text-transform: uppercase;">SCOPRI I PLUGINS PER SONARQUBE > </a>
<br>
<br/>

Happy coding!

---
**<span style="color: green">bitegarden</span> team**

_Helping companies to develop better software_
