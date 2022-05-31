---
layout: post_it
title: ¡OWASP Application Security Verification Standard per SonarQube&trade; a disposizione!
description: Il plug-in Security include il supporto per lo standard OWASP ASVS con un report completo con la conformità ai requisiti nella tua istanza SonarQube&trade;

english: support-for-owasp-asvs-standard-security-plugin-for-sonarqube
spanish: soporte-para-estandar-owasp-asvs-security-plugin-para-sonarqube
permalink: supporto-owasp-asvs-security-plugin-per-sonarqube

cover: /img/posts/2022-05-31-new-release-security-plugin-owasp-asvs.png
---

Abbiamo appena rilasciato la versione 2.8 del [Security Plugin for SonarQube](/it/sonarqube-security) che ti consente di conoscere la 
conformità a standard come OWASP Top 10 o CWE/SANS Top 25 e ora per la prima volta include la possibilità di generare 
un rapporto di sicurezza da verificare conformità con [OWASP Application Security Verification Standard](https://owasp.org/www-project-application-security-verification-standard/) (**ASVS**).

<br>

<img src="/img/sonarqube-security/owasp-asvs-header.png" alt="OWASP ASVS Security Assessment Summary with Rating" width="100%">

[Controlla questo progetto di esempio nella nostra istanza demo>](http://sonarqube.bitegarden.com/project/extension/bitegardenSecurity/asvs_report_page?id=org.owasp%3Abenchmark&qualifier=TRK)

<br>

Il progetto ASVS (Application Security Verification Standard) OWASP fornisce una base per testare la tecnica delle applicazioni web
controlli di sicurezza e fornisce inoltre agli sviluppatori un elenco di requisiti per lo sviluppo sicuro.

L'obiettivo principale del progetto **OWASP Application Security Verification Standard (ASVS)** è di normalizzare l'intervallo in
la copertura e il livello di rigore disponibili sul mercato quando si tratta di eseguire la verifica della sicurezza delle applicazioni Web
utilizzando uno standard aperto commercialmente praticabile. Lo standard fornisce una base per testare la sicurezza tecnica dell'applicazione
controlli, nonché qualsiasi controllo tecnico di sicurezza nell'ambiente, da cui si fa affidamento per la protezione
vulnerabilità come Cross-Site Scripting (XSS) e SQL injection. Questo standard può essere utilizzato per stabilire un livello
di fiducia nella sicurezza delle applicazioni Web.

Ottieni l'ultima versione stabile di ASVS (4.0.3) dalla pagina [OWASP ASVS](https://github.com/OWASP/ASVS/tree/v4.0.3#latest-stable-version---403).

## Come fare riferimento ai requisiti ASVS

Ciascun requisito ha un identificatore nel formato `<capitolo>.<sezione>.<requisito>` dove ogni elemento è un numero, ad esempio: 1.11.3.

- Il valore `<capitolo>` corrisponde al capitolo da cui proviene il requisito, ad esempio: tutti i requisiti 1.#.# provengono dal capitolo Architettura.

- Il valore `<sezione>` corrisponde alla sezione all'interno del capitolo in cui compare il requisito, ad esempio: tutti i requisiti 1.11.# si trovano nella sezione Architettura della logica aziendale del capitolo Architettura.

- Il valore `<requisito>` identifica il requisito specifico all'interno del capitolo e della sezione, ad esempio: 1.11.3 che dalla versione 4.0.3 di questo standard è:

> Verificare che tutti i flussi logici di business di alto valore, inclusi l'autenticazione, la gestione delle sessioni e il controllo dell'accesso, siano thread-safe e resistenti alle condizioni di gara del tempo di controllo e del tempo di utilizzo.

## Utilizzo di SonarQube&trade; e Security Plugin per verificare la conformità con OWASP ASVS

La novità di OWASP ASVS 4.0 è una mappatura completa alla Common Weakness Enumeration (CWE). La mappatura CWE consente lo strumento
produttori e coloro che utilizzano software di gestione delle vulnerabilità per abbinare i risultati.

Non tutti gli elementi nell'ASVS hanno un CWE associato e poiché CWE ha una grande quantità di duplicati. I controlli di verifica non sono sempre mappabili
debolezze equivalenti, ma la Fondazione OWASP sta lavorando duramente con la comunità CWE per colmare questa lacuna.

Questo è il motivo per cui potrai vedere nella pagina Security Assessment ASVS quanti requisiti di OWASP ASVS sono coperti nel tuo SonarQube&trade; esempio.
Dipenderà dal tuo SonarQube&trade; edizione, poiché le edizioni commerciali includono regole di sicurezza aggiuntive.

Una volta che accedi alla nuova pagina ASVS per il tuo progetto vedrai il riepilogo del capitolo:

<br>

<img src="/img/sonarqube-security/owasp-asvs-chapter-summary.png" alt="OWASP ASVS Security Assessment Chapter Summary" width="100%">

<br>

Il nostro [Security Plugin per SonarQube](/it/sonarqube-security) ti mostrerà ogni capitolo OWASP ASVS con i requisiti superati o meno.

Abbiamo aggiunto una valutazione del capitolo ASVS OWASP in modo da poter trovare rapidamente dove sono le vulnerabilità con il maggiore impatto sulla sicurezza.

Questa valutazione è calcolata allo stesso modo del SonarQube&trade; livello di sicurezza (sarà E se viene rilevata almeno una vulnerabilità del blocco, ...).

## Verificare la conformità ai requisiti ASVS OWASP

Sotto il riepilogo del capitolo, troverai un elenco completo con tutti i requisiti che non soddisfano in ciascuna sezione.

Troverai la descrizione del requisito con il relativo ID CWE, a condizione che i problemi rilevati in SonarQube&trade; (sia vulnerabilità che hotspot di sicurezza)

<br>

<img src="/img/sonarqube-security/owasp-asvs-chapter-section-requirement.png" alt="OWASP ASVS Security Assessment Requirement Details" width="100%">

<br>

## Come scaricare la nuova versione

Il Security Plugin è disponibile per il download tramite il [Universal Plugin Manager](/it/sonarqube-upm) o direttamente dalla [Pagina di download](/it/sonarqube-security-trial-form).

**Ricevi la tua prova gratuita e migliora la sicurezza del tuo codice oggi stesso!**

<a href = "/it/sonarqube-security#product-block-center" class = "btn btn-primary btn-call-to-action fancybox" style = "font-weight: bold; font-size: 16px; text-transform : mayúsculas; "> Inizia la tua prova gratuita > </a>

<br/>

---
**<span style="color: green">bitegarden</span> team**

_Helping companies to develop better software_