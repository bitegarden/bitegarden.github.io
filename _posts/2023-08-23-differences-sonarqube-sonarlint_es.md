---
layout: post_es
title:  ¿Cuáles son las diferencias entre SonarQube y SonarLint?
description: Te explicamos cuáles son las principales diferencias entre SonarQube y SonarLint, las soluciones de análisis de código de Sonar.

permalink: diferencias-sonarqube-sonarlint
english: differences-sonarqube-sonarlint
italian: differenze-sonarqube-sonarlint
cover: /img/posts/2023-08-23-differences-sonarqube-sonarlint.png
---

La tecnología de Sonar ha facilitado la **productividad y eficiencia de los equipos de desarrollo** gracias al lanzamiento de herramientas como SonarQube y Sonarlint. Estos dos analizadores de código estático examinan de forma periódica todas las líneas de un proyecto, pero… ¿Cuáles son las diferencias entre SonarQube y Sonarlint? Sigue leyendo que te lo vamos a explicar.

En primer lugar y antes de conocer las diferencias entre estas dos herramientas de Sonar, vamos a recordar qué son:  

<h2>¿Qué es SonarQube?</h2>

Es una solución de **análisis automático de código** que ayuda a los desarrolladores e implementar Clean Code. SonarQube se integra en el flujo de trabajo de desarrollo existente y detecta errores y problemas de seguridad en la base de código, mientras realiza inspecciones de código continuas de los proyectos.

<h2>¿Qué es SonarLint?</h2>

Es un plugin IDE libre y de código abierto que ayuda a los desarrolladores a **encontrar y solucionar errores** en tiempo real mientras escriben código.

<h3>SonarQube vs Sonarlint: Principales diferencias</h3>

1 - SonarQube **es un servidor** en el que se añaden los proyectos y se analizan. SonarLint **es un plugin** que se utiliza en los IDE (Visual Studio, Eclipse, entre otros).

2 - SonarLint **detecta los errores mientras se escribe el código** (como un corrector ortográfico). Por su parte, SonarQube proporciona una **visión 360º del estado del código** de un proyecto. Analiza de forma continua todo el código de un proyecto, ofrece informes y gráficas de estado, código duplicado, su arquitectura, complejidad, comentarios, potenciales errores, etc.

3 - SonarQube realiza **escaneos con analizadores de terceros**, Sonarlint no.

4 - SonarLint tiene un conjunto de **reglas de análisis por defecto**. SonarQube también, pero además permite **crear nuevas reglas** y asociarlas a cada lenguaje.

5 - SonarLint es una **extensión gratuita**. SonarQube tiene una prueba gratuita de 14 días y tiene **tres planes de pago**, que varían en función de la cantidad de líneas de código. 

<h3>Más funcionalidades para el análisis de código </h3>

La complejidad del código, lenguajes de programación, falsos positivos...¿Añadimos algunos más? Estos conceptos forman parte del ecosistema con el que pelean de forma diaria los desarrolladores para conseguir la **calidad del código, Clean Code**. 

En bitegarden hemos desarrollado unos plugins que extienden las funcionalidades de SonarQube: generación de informes en PDF o Excel, información sobre estándares de seguridad, etc. 

Estos productos los puedes descargar y probar de forma [gratuita aquí](https://www.bitegarden.com/es/products/).

¡Nos leemos en próximos artículos!

---
**<span style="color: green">bitegarden</span> team**

_Helping companies to develop better software_
