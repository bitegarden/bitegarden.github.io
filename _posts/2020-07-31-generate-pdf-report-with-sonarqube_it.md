---
layout: post_it
title: Come esportare un report in PDF sulla qualità del codice con SonarQube™
description: Diversi tipi di report per tenere sotto controllo la qualità del codice in SonarQube&trade;.

permalink: esportare-report-pdf-qualita-codice-sonarqube
english: generate-code-quality-pdf-report-sonarqube
spanish: genera-informe-pdf-calidad-codigo-sonarqube

cover: /img/thumbs/2020-07-31-generate-pdf-report-with-sonarqube.png
---

SonarQube™ è uno strumento creato dagli sviluppatori per gli sviluppatori. Fornisce tutto il necessario per scrivere codice pulito e per gestire il debito tecnico in modo che il tuo sviluppo sia sostenibile.

Ma cosa succede se vuoi estrarre i dati sulla qualità del codice e generare un rapporto sulla qualità per i tuoi progetti? 

SonarQube non offre di default alcuna semplice gestione dei report, sebbene tu possa utilizzare l'API web per sviluppare il tuo report personalizzato, la maggior parte delle volte ciò di cui si avrebbe bisogno è qualcosa di più veloce e più semplice.
 
# Come esportare facilmente un report in PDF?

Con il nostro [bitegarden Report Plugin for SonarQube&trade;](/it/sonarqube-report) questi report possono essere generati in modo semplice e rapido.

All'interno del progetto nell'opzione "**More ...**" troverai una sezione con tutti i report di cui puoi avere bisogno, da un sommario esecutivo a un report interamente personalizzabile. 

Ora non ti resterà altro che scegliere quale reprot scaricare facendo clic sul pulsante di download corrispondente.

![Gestione dei reports](/img/sonarqube-report/bitegarden-report-management.png){:width="100%" .center-image}

# Configurare un logo personalizzato

Per impostazione predefinita il plugin utilizzerà il logo di bitegarden nel piè di pagina di ogni pagina, ma è possibile cambiarlo
dalla configurazione del plugin in modo che venga utilizzato il logo della tua azienda o del tuo progetto.

Se vuoi cambiare il logo per tutti i reports SonarQube&trade; devi andare nel pannello di configurazione generale del plugin (**Administration -> General Settings –> bitegarden Report**) e utilizzare l'URL del logo che
vuoi che appaia nel piè di pagina.

---

![Gestione dei reports](/img/sonarqube-report/bitegarden-report-logo-global-settings.png){:width="100%" .center-image}

<p class="center-text">
    Impostazioni logo piè di pagina
</p>

--- 

![Esempio di un report con il logotipo personalizzato](/img/posts/2020-07-31-bitegarden-report-logo-sample.png){:width="100%" .center-image}

<p class="center-text">
    Report di esempio con logo personalizzato
</p>

---

# Report diversi, obiettivi diversi

Ogni persona del team ha bisogno di vedere dati diversi. 

Inizialmente pensavamo che alcuni membri del team/progetto sarebbero entrati direttamente in SonarQube&trade; per vedere i dettagli delle prove, ma l'esperienza ci insegna che non è così. Ci sono molti ruoli che non accedono a SonarQube ma hanno comunque bisogno di lavorare con i reports estratti.

Per questo motivo abbiamo deciso di generare diversi tipi di reports.

## Executive Summary Report (PDF)

---

**Obiettivo**: permette di determinare a colpo d'occhio se il progetto soddisfa o meno le condizioni di qualità e i principali
valori per ciascuna delle dimensioni di qualità analizzate.

---

Questo è un report di un'unica pagina con tutte le informazioni importanti sulla qualità del codice del progetto.

Include:

-- I tre fondamenti del modello di qualità del codice: **affidabilità, sicurezza e manutenibilità**

-- **Codice ripetuto** (o duplicato)

-- **Copertura del codice** e **test unitari**

-- **Blocco e prove critiche** suddivise per bug, vulnerabilità e code smells

Include sia i valori globali che le informazioni sul periodo di perdita (codice nuovo o modificato).

<a href="http://sonarqube.bitegarden.com/api/bitegarden/report/pdf?resource=apache:airflow&branch=master" target="_blank" class="btn btn-primary btn-call-to-action fancybox">GUARDA L'ESEMPIO ></a>

## Issues Breakdown Summary Report (PDF)

---

**Obiettivo**: fornire un riassunto delle evidenze del progetto (più comuni e per severità) e un riassunto per regole, con le principali evidenze rilevate (file, riga, messaggio).

---

Questo report è disponibile dalla versione 2.1 ed include la pagina di riepilogo esecutivo e nuove sezioni:

-- **Most common issuess**: un elenco con i problemi più comuni. Le regole con più problemi verranno visualizzate per prime.

-- **Issues by severity**: elenco delle prove per gravità. Appariranno prima le regole con maggiore severità, indipendentemente dal fatto che non siano le più frequenti.

-- **Issues Breakdown by rule**: una pagina per ogni regola con una piccola descrizione e l'elenco dei problemi riscontrati per la regola.

Il report permette di avere un maggior livello di dettaglio ed è ottimo per confrontarsi con un team esterno o come report di audit di un progetto, dove si vogliono mostrare le principali evidenze.

<a href="http://sonarqube.bitegarden.com/api/bitegarden/report/pdf_issues_breakdown?resource=apache:airflow&branch=master" target="_blank" class="btn btn-primary btn-call-to-action fancybox">GUARDA L'ESEMPIO ></a>

## Issues Breakdown Full Report (PDF)

---

**Obiettivo**: conoscere il dettaglio completo delle evidenze del progetto.

---
  
Questo report è il più completo (e il più grande in termini di dimensioni) in quanto include tutte le informazioni dei rapporti precedenti ma, invece di un riepilogo di una pagina per regola, vengono visualizzate tutte le prove rilevate. 

Se una regola ha 50 issues, il rapporto includerà tutte le 50 issues (file, riga e messaggio di errore).

Questo report permette di avere TUTTE le informazioni sulla qualità del codice di progetto da consegnare a chi deve fare la revisione del rispetto della qualità del codice.

<a href="http://sonarqube.bitegarden.com/api/bitegarden/report/pdf_full_issues_breakdown?resource=apache:airflow&branch=master" target="_blank" class="btn btn-primary btn-call-to-action fancybox">GUARDA L'ESEMPIO ></a>

## Custom Metrics Report with Open Document (ODT)

---

**Obiettivo**: csreare un report completamente personalizzato che possa anche essere modificato in seguito per includere ulteriori informazioni aggiuntive.

---
  
Questo tipo di report viene creato a partire da un modello ODT (documento aperto).

E' possibile creare reports con diverse sezioni completamente personalizzate e con testi, paragrafi, stili e tabelle configurate dal modello.

La definizione del template si basa sull'utilizzo di FreeMarker come variabili inserite nel documento ODT. Il nostro plugin
sostituirà le variabili con i valori effettivi del progetto in base alle metriche SonarQube&trade;. 

Maggiori informazioni su come utilizzarlo [qui](/it/sonarqube-report-documentation).

<a href="http://sonarqube.bitegarden.com/api/bitegarden/report/odt?resource=apache:airflow&branch=master" target="_blank" class="btn btn-primary btn-call-to-action fancybox">GUARDA L'ESEMPIO ></a>

--- 

### Scopri altri esempi...

Se vuoi vedere come funziona la creazione di report su SonarQube&trade; puoi
scaricare la **versione di prova di 14 giorni** del [Report Plugin per SonarQube](/it/sonarqube-report-trial-form) o accedere alla nostra istanza demo
di uno dei progetti disponibili, come [Apache Airflow](http://sonarqube.bitegarden.com/project/extension/bitegardenReport/report_page?id=apache%3Aairflow&qualifier=TRK).

Cosa aspetti a generare rapporti sulla qualità del codice del tuo progetto? 

<a class="btn btn-primary btn-call-to-action fancybox" href="/it/sonarqube-report-trial-form">**PROVA GRATUITAMENTE IL REPORT PLUGIN** ></a>

