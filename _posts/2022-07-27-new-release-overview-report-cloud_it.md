---
layout: post_it
title: 'Overview Report per SonarCloud 1.2'
description: Questa nuova versione include nuove funzionalità per migliorare i report generati

english: new-release-overview-report-sonarcloud-1-2
spanish: nueva-version-overview-report-sonarcloud-1-2
permalink: nuova-versione-overview-report-sonarcloud-1-2

cover: /img/posts/2022-07-27-new-release-overview-report-cloud.png
---

Abbiamo appena rilasciato una nuova versione di *[bitegarden Overview Report for SonarCloud&trade;](/it/sonarcloud-overview)*, versione 1.2, che include diverse interessanti novità:

### Health Rating

Da un lato, il report include una nuova sezione "Health Rating" che consente di conoscere lo stato di salute dell'organizzazione SonarCloud in termini di se il codice è pronto per essere caricato in produzione (rispetto dei controlli di qualità).

Lo stato di salute è la percentuale di progetti che soddisfano la soglia di qualità (*quality gate*):

-- A: > 80%

-- B: > 60%

-- C: > 40%

-- D: > 20%

-- E: <= 20%

<br>
<img src="/img/posts/2022-07-27-overview-health-rating.png" alt="health rating" width="100%">
<br><br>

### Valori differenziali

È inclusa la possibilità di visualizzare le differenze rispetto ai periodi precedenti.
Per impostazione predefinita, sono stati inclusi 3 periodi (dalla prima analisi, da sei mesi fa e nell'ultimo mese),
ma la cosa interessante è che include anche la possibilità di specificare una data precisa a partire dalla quale vedere
differenze ed evoluzione.

Queste informazioni sono mostrate sia nella sezione "executive" della prima pagina che nell'elenco dei progetti.

<br>
<img src="/img/posts/2022-07-27-overview-differential-values.png" alt="differential values" width="100%">
<br><br>

### Quality gates

Inoltre, l'elenco con il dettaglio dei progetti includeva anche lo stato del quality gate per ciascun progetto.

<br>
<img src="/img/posts/2022-07-27-overview-quality-gates.png" alt="quality gates" width="100%">
<br><br>

### Scarica l'ultima versione

Ci auguriamo che questa nuova versione ti piaccia, aggiornaci per goderti tutte le novità.

Puoi scaricare la versione dalla [pagina del prodotto](/it/sonarcloud-overview-trial-form).

E ricorda che il feedback è sempre molto apprezzato, quindi sentiti libero di aprire un ticket sul nostro 
[portale di supporto](http://support.bitegarden.com/) per aiutarci a continuare a migliorare il prodotto.

<a href = "/es/sonarcloud-overview-trial-form" class = "btn btn-primary btn-call-to-action fancybox" style = "font-weight: bold; font-size: 16px; text-transform : mayúsculas; "> Scarica > </a>

<br/>

---
**<span style="color: green">bitegarden</span> team**

_Helping companies to develop better software_