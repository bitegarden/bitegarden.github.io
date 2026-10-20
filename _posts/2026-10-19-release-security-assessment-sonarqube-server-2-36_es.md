---
layout: post_es
title: Security Assessment for SonarQube 2.36, nuevos informes PCI DSS en PDF y mejoras en MQR
description: Descubre la descarga de informes PCI DSS en PDF y nuevos informes MQR para estándares de seguridad..

permalink: version-security-assessment-sonarqube-server-2-36
english: release-security-assessment-sonarqube-server-2-36

cover: /img/posts/2026-10-19-release-security-assessment-sonarqube-server-2-36_es.png

---

En **bitegarden** seguimos mejorando **Security Assessment for SonarQube&trade; Server** para facilitar el análisis de vulnerabilidades y la evaluación de la seguridad del código. Por ello, lanzamos la versión 2.36 de Security Assessment for SonarQube Server, una actualización que incorpora la **descarga de informes PCI DSS** en PDF y amplía la compatibilidad de los informes en modo MQR con diferentes estándares de seguridad.

<h2>¿Qué es Security Assessment for SonarQube?</h2>

Security Assessment for SonarQube es un plugin de bitegarden para **SonarQube Server** que consolida las vulnerabilidades detectadas por SonarQube en una evaluación de seguridad completa. Su objetivo es proporcionar una visión detallada y visual del nivel de cumplimiento de seguridad de los proyectos, facilitando la interpretación de los resultados y el análisis de las vulnerabilidades en relación con diferentes estándares de seguridad.

De esta forma, los equipos pueden **consultar la información de seguridad de su código** de una manera más estructurada y comprensible y **exportar sus resultados en informes** completos en PDF.

<h2>Novedades de Security Assessment for SonarQube 2.36</h2>

<h3>Descarga de informes PCI DSS en PDF</h3>

Una de las principales novedades de la versión 2.36 es la posibilidad de descargar los **informes PCI DSS** en formato PDF en las ediciones comerciales de SonarQube Server. 

Esta funcionalidad está disponible para los siguientes elementos de SonarQube Server:

**Proyectos**: permite obtener el informe PCI DSS de un proyecto.

**Aplicaciones**: permite descargar el informe correspondiente a una aplicación.

**Portfolios**: permite generar el documento PDF para un portfolio.

Además, la descarga está disponible tanto en modo Standard como en modo MQR (Multi-Quality Rule).


<h3>Nuevos informes MQR para estándares de seguridad</h3>

La versión 2.36 también amplía las posibilidades de evaluación de seguridad mediante la incorporación de informes en modo MQR para cuatro estándares:

- **CWE On the Cusp**: incorporación del informe MQR para analizar los resultados relacionados con esta selección de debilidades de seguridad.

- **OWASP Top 10**: implementación del informe MQR para este estándar de referencia sobre riesgos de seguridad en aplicaciones web.

- **OWASP ASVS**: incorporación del informe MQR para el estándar Application Security Verification Standard de OWASP.

- **ISO 5055**: implementación del informe MQR para este estándar relacionado con la medición de la calidad estructural del software.


<h2>Mejoras en la página de CASA</h2>

Además de los nuevos informes, hemos introducido una mejora en la interfaz de la página de CASA. Ahora, los **selectores de ramas y pull requests** incluyen tooltips que proporcionan información contextual sobre estos elementos.


<h2>¿Cómo actualizar a la nueva versión?</h2>

Si ya eres usuario del [Universal Plugin Manager](https://marketplace.bitegarden.com/product/bitegardenUniversalPluginManager), simplemente accede a la administración de este plugin y pulsa sobre el botón de actualización disponible. Sin embargo, si todavía no has probado **bitegarden Security Assessment for SonarQube&trade; Server**, puedes descargarlo e instalarlo en tu instancia a través de [este enlace](https://marketplace.bitegarden.com/product/bitegardenSecurity). 

---

**<span style="color: green">bitegarden</span> team**

_Helping companies to develop better software_