---
layout: post_es
title: Security Assessment for SonarQube Cloud 1.10, nuevos informes PCI DSS y mejoras en los informes de seguridad
description: Descubre la descarga de informes PCI DSS en PDF y nuevos informes MQR para estándares de seguridad.

permalink: version-security-assessment-sonarqube-cloud-1-10
english: release-security-assessment-sonarqube-cloud-1-10

cover: /img/posts/2026-10-20-release-security-assessment-sonarqube-cloud-1-10_es.png

---

En bitegarden seguimos mejorando Security Assessment for SonarQube&trade; Cloud para facilitar la **evaluación de la seguridad del código** y la generación de informes basados en diferentes estándares de seguridad.

Ya está disponible la versión 1.10 de Security Assessment for SonarQube&trade; Cloud, una actualización que incorpora el **estándar PCI DSS** y mejora la generación de los informes de seguridad existentes.

Entre las principales novedades destacan la generación de informes PCI DSS en PDF, la actualización de los informes OWASP y CWE, y diferentes mejoras de configuración y presentación.

<h2>¿Qué es Security Assessment for SonarQube&trade; Cloud?</h2>

**Security Assessment for SonarQube&trade; Cloud** es una solución de bitegarden que permite **generar informes de seguridad a partir de las vulnerabilidades** detectadas por SonarQube Cloud. Su objetivo es ofrecer una visión estructurada de los resultados de seguridad de los proyectos, relacionándolos con diferentes estándares y referencias de seguridad del software.

<h2>Novedades de Security Assessment for SonarQube&trade; Cloud 1.10</h2>

<h3>Nuevo informe PCI DSS en PDF</h3>

La principal novedad de la versión 1.10 es la **incorporación del estándar PCI DSS** (Payment Card Industry Data Security Standard) a los informes de seguridad. A partir de esta versión, la CLI de Security Assessment permite generar informes PCI DSS en formato PDF para proyectos de SonarQube Cloud.

Esta funcionalidad incluye:

Compatibilidad con **PCI DSS 4.0 y 3.2**.

Generación de informes en modo MQR (Multi-Quality Rule).

**Exportación** de los resultados en formato PDF.

Esta incorporación amplía las posibilidades de evaluación y documentación de la seguridad del código, especialmente para los equipos que necesitan analizar sus proyectos tomando como referencia los requisitos de PCI DSS.

<h2>Mejoras en los informes OWASP Top 10 y CWE</h2>

La versión 1.10 también incluye una revisión de la generación de los informes de seguridad existentes. Entre las novedades se encuentran:

**OWASP Top 10**: incorporación del nuevo informe de seguridad basado en esta referencia de riesgos para aplicaciones web.

**CWE Top 25**: utilización de los informes de proyecto correspondientes a esta clasificación de debilidades de software.

**CWE On the Cusp**: incorporación de los informes de proyecto asociados a esta selección de debilidades de seguridad.

Estas mejoras permiten disponer de informes actualizados para analizar los resultados de seguridad de los proyectos de SonarQube Cloud.

<h2>Configuración común y mejoras en la presentación de informes</h2>

Además de las novedades relacionadas con los estándares de seguridad, hemos introducido diferentes mejoras en la generación y presentación de los informes:


**Identidad visual**: se recupera el logotipo de SonarQube Cloud en la cabecera de los informes.

**Idioma predeterminado**: los informes utilizan por defecto el idioma del sistema.

**Informes ISO 5055**: los CWE no soportados dejan de mostrarse por defecto.

Estos cambios buscan ofrecer una experiencia más coherente y facilitar la consulta de los resultados.

Puedes probar esta nueva versión [descargandola desde el marketplace de bitegarden](https://marketplace.bitegarden.com/product/bitegardenSonarCloudSecurity). 

---


**<span style="color: green">bitegarden</span> team**

_Helping companies to develop better software_