---
layout: post_it
title: Gestione della qualità del codice con SonarQube
description: Come migliorare il controllo della qualità dei progetti con SonarQube

permalink: gestione-qualita-codice-con-sonarqube
english: static-code-analysis-with-sonarqube
spanish: analisis-estatico-del-codigo-con-sonarqube

cover: /img/thumbs/2020-07-13-static-code-analysis-using-sonarqube-thumb.png
---
Investire nel **controllo della qualità dei progetti** significa analizzare il codice durante tutto il processo. Ciò si traduce nell'inclusione delle revisioni del codice nei flussi di lavoro così da mantenere la qualità elevata.

Per raggiungere questo obiettivo è necessario includere un analizzatore di codice statico, come [**SonarQube&trade;**](https://www.sonarqube.org/).

![SonarQube](/img/posts/2020-07-13-static-code-analysis-using-sonarqube-logo-300x93.jpg){: .center-image}

---

## Che cos'è SonarQube&trade;?


**SonarQube&trade;** è un software **open source** che effettua l'**analisi statica** del codice e genera metriche che permettono di tenere sotto controllo  e migliorare la qualità del codice del tuo progetto.

**SonarQube&trade;** recupera le metriche dal codice sorgente, mentre le metriche relative al debito tecnico si basano su
[**SQALE**](https://www.bitegarden.com/sonarqube-sqale), che potremmo definire come un algoritmo in grado di definire se le aspettative che erano state fissate durante il ciclo di vita dello sviluppo sono state soddisfatte e/o quanto tempo ci vorrà per farlo.

Il primo cambio da effettuare nel flusso di lavoro è adottare **SonarQube&trade;** fin dal primo giorno, questo proprio perché si tratta di software **evolutivo** che analizzando il codice giorno per giorno è in grado di monitorare l'evoluzione del progetto. 

Il flusso di lavoro cambierà per sempre (ed in bene) perchè non si tratterà più di codifica, codifica e codifica, ma codifica, analizza e correggi. Questa nuova pratica eviterà la generazione grosso debito tecnico e ti permetterà di migliorare la qualità dell'intero progetto.

Tra le metriche troverai: codice duplicato, copertura, code smells, bugs, vulnerabilità dei fattori di rischio, densità di violazioni della sicurezza e molto altro.

**SonarQube&trade;** è diviso in due parti: il **server**, dove si trova il motore di calcolo che esegue l'analisi, memorizza i risultati ed è dove è possibile definire i progetti, i parametri di qualità, i risultati dell'analisi e sarà responsabile di ogni compito. Mentre l'altra parte è l'analizzatore in sè, **SonarQube Scanner**.

**SonarQube&trade;** è uno strumento multilingue ed è possibile analizzare diversi codici e repository.

Attualmente, l'ultima versione è la **8.4** e supporta più di **27 linguaggi di programmazione**.

![Sonarqube - Linguaggi di programmazione](/img/posts/2020-07-13-static-code-analysis-using-sonarqube-programming-languages.jpg)

## Differenza tra analisi statica o dinamica del codice sorgente

L'**Analisi statica** del codice esegue il processo di valutazione del software senza dover eseguire il codice, in questo modo è possibile prima trovare bug, errori e metriche.

D'altra parte, l'**analisi dinamica** prevede l'esecuzione del software per vederne il comportamento e il tempo di esecuzione. Il problema con questo approccio è che avrai bisogno di più test per definire la correttezza del tuo codice.


## Le caratteristiche più importanti di SonarQube&trade;

-- **Vulnerabilità**: SonarQube&trade ha un ottimo set di regole per rilevare bug, code smells, vulnerabilità e conoscere nel dettaglio il livello di sicurezza e qualità del progetto.

-- **Codice duplicato**: rileva il codice duplicato e consente di prendere decisioni di refactoring o disaccoppiare i componenti.

- **Programming Standard**: consente di sapere se gli standard vengono violati e rileva le cattive pratiche (code smells).

- **Coverage (copertura)** : monitora se la copertura dei test è sufficiente per gli standard di qualità e se è necessario aumentarne l'investimento.

- **Quality profiles (profili di qualità)** : per ogni lingua esiste un profilo di qualità predefinito ma c'è anche la possibilità di creare un profilo personalizzato È un pacchetto di regole che vengono applicate durante l'analisi statica del codice.

## Funzionalità di reporting

Visto che il **ciclo di vita dello sviluppo del software** coinvolge anche altri ruoli, non solo quello degli sviluppatori, abbiamo creato diversi [**plugins per SonarQube&trade;**](https://www.bitegarden.com/it/products/) in grado di ampliare le sue funzionalità e fornire features di reporting
che mancano ma risultano indispensabili per **Responsabili di progetto**, **Product Owners**.

## Monitora la qualità del codice e migliora i tuoi standard

[SonarQube&trade;](https://www.sonarqube.org/) è uno strumento molto potente - e per di più **gratuito** e
**open source** - che grazie alle sue funzionalità ti permetterà di controllare **costantemente** la qualità del codice con pochissimo sforzo. Inoltre,  se ti occupi di gestire numerosi progetti, con SonarQube riuscirai ad avere finalmente tutto sotto controllo.

<a href="/it/products/" class="btn btn-primary btn-call-to-action fancybox">SCOPRI TUTTI I PLUGINS ></a>

Siamo sicuri che ti piacerà!

---
**<span style="color: green">bitegarden</span> team**

_Helping companies to develop better software_