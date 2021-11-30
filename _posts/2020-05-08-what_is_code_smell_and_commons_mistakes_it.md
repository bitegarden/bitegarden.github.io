---
layout: post_it
title: Che cosa sono i code smells e gli errori comuni
description: Un 'code smell', noto anche come "cattiva pratica", nel campo della programmazione si riferisce a un sintomo nel codice sorgente che probabilmente ci sta dicendo che qualcosa non va

permalink: cosa-sono-code-smell-e-errori-comuni-nel-codice
english: what-is-code-smell-and-common-mistakes
spanish: que-es-un-code-smell-y-errores-comunes

cover: /img/thumbs/Thumb-what-is-code-smell-mistakes.jpg
---

Hai cambiato lavoro o sei semplicemente appena entrato a lavorare su un progetto già iniziato, ti siamo vicini, non è semplice. 

Se sei fortunato ti sarà capitato di trovare nel codice delle annotazioni come queste:
  
`//TO DO` o `//FIX ME`  
  
Questi testi non aggiungono nessuna funzionalità, ma evidenziano una possibile implementazione sbagliata nel codice o qualcosa in pending da verificare. In ogni modo si tratta di qualcosa "puzza" nel codice.

Diciamo che ti piacerebbe iniziare col piede giusto e vorresti ripulire il codice che hai ereditato, ma il problema, con questo tipo di cattive pratiche, sta proprio nel trovarle. Ogni sviluppatore ha il suo "metodo" per lavorare e così anche il suo metodo per inserire i commenti sulle cose da fare (e che puntualmente non farà).

![cosa sono i code smells - bitegarden](/img/posts/2020-05-08-what_is_code_smell_and_commons_mistakes.png){:width="100%" .center-image}
  
## Cosa sono i *code smells*?
  
>“Un *code smell*, noto anche come negligenza, nello sviluppo del software, si riferisce a qualsiasi sintomo nel codice sorgente di un programma che potrebbe indicare un problema più profondo. (...)
>  
>I *code smells* di solito non sono bug di programmazione (errori) - non sono tecnicamente errati e in realtà non impediscono al programma di funzionare correttamente.
>  
>Indicano invece cattive pratiche nella progettazione del software che possono rallentare lo sviluppo o aumentare il rischio di errori o guasti in futuro." 
>  
>**Fonte:** *[Wikipedia](https://es.wikipedia.org/wiki/Hediondez_del_código)*  
  
## Gli errori più comuni
  
-- **Bloatware**: si tratta di parti del codice (classi, metodi, ...) che sono aumentate in modo sproporzionato e
diventano difficili da mantenere poichè stanno facendo troppe cose invece di avere una chiara responsabilità.
Questo tipo di errore può diventare un grosso problema, soprattutto se nessuno se ne occupa.
  
-- **Codice ripetuto (duplicato)**: si verifica quando uno sviluppatore non può rispettare le scadenze (o semplicemente uno sviluppatore troppo pigro) e inziare a fare copia e incolla parti del codice invece di creare del codice ad hoc. Altre volte capita quando più programmatori stanno lavorando sulla stessa porzione di codice.
In futuro, questo errore comporterà un grande sforzo, visto che dovrà essere cambiato in più di luogo o, peggio, se uno di questi venisse dimenticato, il codice finirà per comportarsi in maniera inaspettata.
  
-- **Classi pigre (*lazy*)**, come sai, mantenere il codice costa tempo e denaro, quindi se una classe è stata creata solo per anticipare una funzionalità futura e non sta facendo molto nella situazione attuale, dovrebbe essere rimossa.

Sfortunatamente, questi elementi non sono facili da risolvere e richiedono un grande sforzo, tempo o una modifica importante nel codice.
  
## Come evitare i *code smells*?  
  
[SonarQube](https://www.sonarqube.org/) è uno strumento straordinario per monitorare lo stato del codice e aiutarti a migliorare la revisioni delle cattive pratiche presenti nel tuo progetto.
  
Noi consigliamo ai teams di iniziare a fare un'analisi continua del codice, in questo modo sarà possibile correggere le cattive pratiche, errori (*bug*) e vulnerabilità del codice invece di creare o aprire ogni volta nuovi tasks per risolverli.
  
Se invece il tuo team sta già utilizzando SonarQube e stai cercando di migliorare la gestione del debito tecnico del tuo progetto e/o vorresti tenerlo
sotto controllo, prova lo [SQALE Plugin](https://www.bitegarden.com/it/sonarqube-sqale) che estendendo le funzionalità di SonarQube ti permetterà di gestire il tuo debito in maniera semplice e veloce.

Happy coding!
