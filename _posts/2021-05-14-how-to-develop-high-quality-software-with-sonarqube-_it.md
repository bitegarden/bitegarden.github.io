---
layout: post_it
title:  Come sviluppare un software di alta qualità con SonarQube
description: Come quantificare la qualità di un software e costruire un prodotto di alta qualità.

permalink: come-sviluppare-software-alta-qualita-sonarqube
spanish: como-costruir-software-de-alta-calidad-sonarqube
english: how-to-develop-high-quality-software-sonarqube

cover: /img/posts/2021-05-14-how-to-develop-high-quality-software-with-sonarqube-thumb.png
---

L'utilizzo di uno strumento per l'analisi statica del codice, come **SonarQube**, permette ai programmatori di aumentare la loro produttività mentre aumentano la qualità del codice. Questo è un fatto essenziali già che molte parti dei prodotti software sono condivisi tra diversi teams/persone.

## Come funziona SonarQube

Attraverso l'analisi statica del codice sorgente, SonarQube misura i livelli di affidabilità, manutenibilità, sicurezza, complessità, copertura dei test e duplicazione del codice, assegnando un punteggio in base alla gravità dei difetti riscontrati.

Quando la qualità del software viene mantenuta elevata si genera: una **maggiore sicurezza**, i **costi si abbassano** durante tutto il ciclo di vita del prodotto, **si riducono i tempi di manutenzione** e si crea valore per produttori, clienti e finanziatori.

## Come quantificare la qualità di un software

L'alta qualità del software è legata a:

-- Riduzione dei tempi di collaudo e consegna
-- Riduzione di oltre il 50% su riparazioni e modifiche
-- Aumento della soddisfazione del cliente
-- Riduzione, dopo il lancio, dei costi di manutenzione
-- Riduzione delle controversie sui contratti a progetto
-- Riduzione dei progetti annullati
-- Maggiore affidabilità
-- Riduzione delle falle di sicurezza nelle applicazioni pubblicate

## Categorie delle regole SonarQube

SonarQube per analizzare il codice utilizza regole classificate in quattro tipi: code smell, bug, vulnerabilità e hotspot di sicurezza.

La categoria **code smell** comprende i difetti di programmazione ma che non sono errori in senso stretto, ovvero non pregiudicano l'effettiva correttezza del software, ma rendono meno facile la sua manutenzione.

**I bug** sono errori da cui dipende il comportamento imprevisto o errato del programma e ne riducono l'affidabilità.

**Le vulnerabilità** sono punti deboli che possono essere sfruttati per compromettere la sicurezza del sistema.

**Gli hotspot di sicurezza** sono punti deboli che non sono problematici, ma potrebbero diventare *vulnerabilità*. Alcuni esempi sono l'errata configurazione dei cookies, l'uso di algoritmi crittografici non standard e l'uso di protocolli che non creano connessioni sicure.

*Tramite la piattaforma di SonarQube è anche possibile **creare nuove regole** e/o scegliere un set di regole da associare a ciascun linguaggio di programmazione.*

## Gradi di gravità

Durante l'analisi, i problemi vengono definiti ogni volta che uno snippet di codice infrange una regola. 

Ogni problema è legato a un diverso livello di gravità:
- -- **Blocker**: un bug che può modificare il comportamento del programma e richiede una modifica del codice.
- -- **Critical**: un bug che difficilmente cambierà il comportamento del programma o un difetto di sicurezza. Il codice deve essere verificato.
- - **Mayor**: difetti del codice che riducono la produttività degli sviluppatori, come codice ripetuto, parametri e variabili inutilizzate.
- -- **Minor**: difetti del codice che riducono leggermente la produttività degli sviluppatori, ad esempio righe troppo lunghe.
- -- **Info**: questo non è un vero difetto del software, ad esempio commenti "TODO" o utilizzo di costrutti obsoleti.

## Cinque stati

Un problema, una volta creato, può assumere cinque stati: subito dopo la sua creazione è **(1) aperto**, diventa **(2) confermato** quando l'utente indica che è un problema valido, **(3) risolto** quando l'utente indica che nell'analisi successiva non deve essere più considerato perché sono state apportate modifiche, **(4) riaperto** quando il problema è stato segnalato come risolto ma non è stato effettivamente corretto e **(5) chiuso** quando SonarQube non lo riconosce più come un problema. 

Un problema viene chiuso quando è stato **risolto** o perché la relativa regola che lo riconosce non è più disponibile, perchè **rimossa**.

## Valutazione metrica

Le metriche utilizzate per definire la qualità del codice sono: complessità, duplicazione, manutenibilità, affidabilità, sicurezza, dimensioni e copertura dei test.

#### Grado di affidabilità

- A = 0 errore
- B = almeno un errore minore
- C = almeno un errore maggiore
- D = almeno un errore critico
- E = almeno un bug blocker

#### Classificazione di sicurezza

- A = 0 vulnerabilità
- B = almeno una vulnerabilità minore
- C = almeno una vulnerabilità maggiore
- D = almeno una vulnerabilità critica
- E = almeno una vulnerabilità bloccante

#### Rating del debito tecnico

Dipende dal "rapporto di indebitamento tecnico" (TD ratio) che è il rapporto di indebitamento e il tempo di sviluppo stimato, calcolato come LOCx30min.

- A = rapporto TD <= 5%
- B = rapporto TD compreso tra 6 e 10%
- C = rapporto TD compreso tra 10 e 20%
- D = rapporto TD compreso tra 21 e 50%
- E = rapporto TD> = 50%

## Un software di alta qualità è più economico da sviluppare

Se credi nell'**integrazione continua**, non puoi non utilizzare SonarQube! E' lo strumento perfetto per tenere sotto contro il tuo codice dopo ogni modifica, mantenendo così sempre alta la qualità del tuo software.

Happy coding!

---
**<span style="color: green">bitegarden</span> team**

_Helping companies to develop better software_
