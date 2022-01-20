---
layout: post_it
title: Come trovare le vulnerabilità nel codice
description: SonarQube è lo strumento di analisi statica del codice per eccellenza. Ha l'obiettivo di identificare vulnerabilità, code smell, bug e permetterti di scrivere un codice sempre più sicuro.

permalink: come-trovare-vulnerabilita-nel-codice
english: how-to-detect-vulnerabilities-in-your-code
spanish: como-detectar-vulnerabilidades-en-el-codigo


cover: /img/thumbs/Thumb-how-to-detect-vulnerabilities-in-your-code.jpg
---

![Come trovare le vulnerabilità nel codice](/img/posts/bitegarden-how_to_detect_vulnerabilities_in_your_code.jpg){:width="100%" .center-image}

[SonarQube](https://www.sonarqube.org) è diventato lo strumento di analisi statica e ispezione continua per eccellenza.

Per un paio d'anni il loro team di sviluppo si è concentrato sul miglioramento di tutte quelle funzionalità di analisi associati al rilevamento di vulnerabilità e ai diversi standard di sicurezza, tra cui OWASP, SANS, CWE, ecc, così che al momento possiamo già dire che [SonarQube è uno strumento **SAST**](https://www.sonarqube.org/features/security/) (= Test di sicurezza statica delle applicazioni).

Inoltre, integrandolo con altri componenti Open Source come
[OWASP Dependency Check](https://owasp.org/www-project-dependency-check/), o con il nostro [Security Plugin](/it/sonarqube-security) possiamo aumentare ulteriormente le sue capacità di analisi della vulnerabilità (Software Composition Analysis, SCA) o creare nuovi report di conformità. 

Possiamo inoltre aumentare l'insieme delle regole di sicurezza disponibili tramite strumenti come [Find Security Bugs](https://find-sec-bugs.github.io) o
utilizzare il plugin [sonar-findbugs](https://github.com/spotbugs/sonar-findbugs).

Ma al di là di tutto questo, come facciamo a trovare le vulnerabilità nel codice con SonarQube?

## Prove di sicurezza: Hotspot vs Vulnerabilità

SonarQube distingue tra due tipi di prove relative alla sicurezza, e la principale differenza sta nella necessità di **revisione**, ovvero se è necessario o meno trovare una soluzione.

![Vulnerabilità vs Hotspot](/img/posts/hotspots-vulnerabilities.png){:width="100%" .center-image}

- Nel caso di un **Hotspot** viene rilevata una parte di codice sensibile alla sicurezza, ma la sicurezza dell'applicazione potrebbe anche non esserne influenzata. È responsabilità dello sviluppatore rivedere il codice per determinare se è necessaria, o meno, una modifica.

- Nel caso di una **vulnerabilità**, viene rilevato un problema che influisce sulla sicurezza dell'applicazione e deve essere riparato immediatamente.

## Come trovare le vulnerabilità nel codice

#### 1. Attiva le regole di sicurezza

Se vuoi fare una prima revisione della sicurezza del tuo codice, la prima cosa da fare sarà configurare il tuo profilo di qualità per rilevare il maggior numero possibile di problemi.

Questo è il profilo di qualità predefinito:

![Regole predefinite](/img/posts/default-security-rules.png){:width ="300px".center-image}

Ci sono poi 45 regole di tipo **vulnerabilità** e altre 31 regole di tipo **hotspot**.

Ma puoi anche attivare altre 20 regole associate alla sicurezza. 

Il profilo predefinito è generalmente sufficiente ma se vuoi puoi provare con tutto attivo.

---
> **Suggerimento:** ci sono anche alcune regole sui code smells e codice
> classificati in standard di sicurezza. Trovali e attivali per migliorare l'analisi della sicurezza del tuo codice.
>

Ecco un esempio di regola di tipo **bug** che interessa lo standard OWASP (categoria A6).

![Bug che colpisce la sicurezza](/img/posts/bug-security-rule.png){:width ="30%".center-image}

Ecco perché è importante non solo conservare le vulnerabilità e le prove degli hotspot, ma anche andare un po' oltre, poiché alcuni bug o code smell potrebbero essere correlati a futuri problemi di sicurezza.

---

#### 2. Controlla il livello di sicurezza

Una volta che il tuo progetto è stato analizzato, puoi vedere il punteggio della sicurezza nella pagina principale:


![classificazione di sicurezza](/img/posts/overall-security-rating.png){:width="100%" .center-image}

Esiste una valutazione per le vulnerabilità e un'altra per gli hotspot.

- In caso di vulnerabilità, è calcolato tenendo conto della gravità delle vulnerabilità rilevate.
 
- Nel caso di hotspot, viene calcolato in base al numero di hotspot in attesa di revisione.

Da qui puoi iniziare a risolvere i problemi di sicurezza del codice sfogliando tutte le prove rilevate. 

Questo va bene per uno sviluppatore, ma per quanto riguarda un responsabile o un responsabile della sicurezza che non cambia il codice? In tal caso, le informazioni che interessano sono più esecutive.

#### 3. Verificare la conformità agli standard

Oltre alla valutazione globale, se hai installato il [Security Plugin](/it/sonarqube-security) di bitegarden, puoi verificare la conformità agli standard più importanti e alcune metriche aggiuntive in una sezione dedicata all'interno del progetto.

Questa sezione è più "friendly" rispetto a dover sfogliare tutte le prove e ti permette di analizzare la sicurezza del tuo codice da un punto di vista meno tecnico:

![rapporto di conformità](/img/posts/bitegarden-security-owasp-page.png){:width="60%" .center-image}


Con queste informazioni non solo puoi conoscere meglio quali aspetti della sicurezza sono migliori o peggiori nel progetto, ma anche decidere quali vulnerabilità del codice risolvere per prime in base alle categorie e criticità.

Ad esempio, potresti essere più interessato a iniziare a risolvere i problemi di iniezione di codice piuttosto che a problemi di installazione.

#### 4. Genera un rapporto PDF sulla sicurezza del tuo codice

Infine, se hai bisogno di pubblicare le informazioni o farle raggiungere ad altre persone che non fanno parte del team, puoi semplicemente esportare tutte le informazioni in PDF, sempre attraverso [il Security Plugin](/it/sonarqube-security), in modo che tutti possano vedere i risultati sulla sicurezza del codice:

![report-owasp-pagina-1](/img/posts/owasp-report-page-1.png){:width="45%"} ![report-owasp-pagina-2](/img/posts/owasp-report-page-2.png){:width="45%"}

---

## Conclusione

SonarQube ha migliorato molto il suo [motore di sicurezza](https://blog.sonarsource.com/what-is-taint-analysis) e gioca nella stessa
league di altri strumenti più specializzati. 

Controlla tutti i problemi di sicurezza nel tuo codice con questi 4 semplici passaggi:

1. Attiva delle regole che rilevano vulnerabilità e hotspot
2. Rivedi la valutazione complessiva della sicurezza del tuo progetto
3. Verifica il rispetto degli standard di sicurezza
4. Condividi le informazioni con altri team tramite i report in PDF

Prova il [Security Plugin](/it/sonarqube-security) e inizia subito a migliorare il modo in cui trovi e risolvi le vulnerabilità del tuo codice.

<a href="/it/sonarqube-security-trial-form" class="btn btn-primary btn-call-to-action fancybox">SCARICA IL SECURITY PLUGIN ></a>

---
**<span style="color: green">bitegarden</span> team**

_Helping companies to develop better software_





