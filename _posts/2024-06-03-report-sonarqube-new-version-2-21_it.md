---
layout: post_it
title: 'Nuova versione! Plugin Report per SonarQube 2.21'
description: Nuovi campi di report e nuovo endpoint!

permalink: report-sonarqube-nuova-versione-2-21
spanish: report-sonarqube-nueva-version-2-21
english: report-sonarqube-new-version-2-21

cover: /img/posts/2024-06-03-bitegarden-report-new-version-2-21_IT.png
---

Abbiamo una nuova versione del [Plugin Report per SonarQube](/sonarqube-report). Si tratta della **versione 2.21** che apporta diverse novità!
Questa versione aggiunge alcuni nuovi campi ai report, come richiesto. D'ora in poi, sarà possibile vedere:

- **Linee di Codice**: Ora è possibile visualizzare il numero totale di linee di codice analizzate.
- **Data di Download**: È stata aggiunta la data in cui il report è stato scaricato.
- **Versione di SonarQube**: I report ora includono la versione di SonarQube utilizzata per l'analisi.

<br/>

## Miglioramento nelle Notifiche Email

In precedenza, il plugin permetteva di configurare una lista di email da notificare dopo ogni analisi. Tuttavia, questo stava causando problemi per alcuni clienti e influenzava i tempi di analisi aggiungendo più lavoro al compute engine.

#### Soluzione Implementata

In questa versione, è stato incluso un endpoint che permette di notificare gli utenti desiderati inviando la lista di email. In questo modo, le notifiche email non vengono più eseguite nel compute engine, migliorando così le prestazioni e riducendo i problemi segnalati.

<img src="/img/sonarqube-report/bitegarden-report-sonarqube-email-endpoint.png" width="100%" alt="endpoint">

## Patch Applicata

È stata implementata una piccola patch per risolvere il problema della sovrapposizione delle email tra diversi progetti quando c'erano più di un worker configurato nel compute engine. Questo miglioramento garantisce che le notifiche vengano inviate correttamente senza mescolare i destinatari tra diversi progetti.

#### Avviso

Pertanto, dato che abbiamo un endpoint per questo, la funzionalità precedente è stata contrassegnata come “deprecata” per mantenere solo il nuovo endpoint. Verrà rimossa nelle versioni future.

<br />

## Scarica la nuova versione

Il plugin per la sicurezza è ora disponibile per il download tramite [Universal Plugin Manager](/it/sonarqube-upm) o dalla pagina [download del prodotto](/it/sonarqube-report-trial-form).

Ricorda, se non hai ancora questo plugin puoi **scaricarlo e provarlo gratuitamente**. 

<a href = "/it/sonarqube-report#product-block-center" class = "btn btn-primary btn-call-to-action fancybox" style = "font-weight: bold; font-size: 16px; text-transform : mayúsculas; "> Iniziare la prova gratuita > </a>

---
**<span style="color: green">bitegarden</span> team**

_Helping companies to develop better software_