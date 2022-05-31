---
layout: post_es
title: ¡OWASP Application Security Verification Standard para SonarQube&trade; disponible!
description: El plugin Security incluye soporte para el estándar OWASP ASVS con un informe completo con el cumplimiento de los requisitos en tu instancia de SonarQube&trade;

english: support-for-owasp-asvs-standard-security-plugin-for-sonarqube
permalink: soporte-para-estandar-owasp-asvs-security-plugin-para-sonarqube
italian: supporto-owasp-asvs-security-plugin-per-sonarqube

cover: /img/posts/2022-05-31-new-release-security-plugin-owasp-asvs.png
---

Acabamos de publicar la versión 2.8 de [Security Plugin for SonarQube](/es/sonarqube-security) que permite conocer el 
cumplimiento de los estándares como OWASP Top 10 o CWE/SANS Top 25, y que ahora por primera vez incluye la capacidad
de generar un informe de seguridad para verificar el cumplimiento de [OWASP Application Security Verification Standard](https://owasp.org/www-project-application-security-verification-standard/) (**ASVS**). 

<br>

<img src="/img/sonarqube-security/owasp-asvs-header.png" alt="OWASP ASVS Security Assessment Resumen con calificación" width="100%">

[Comprueba este proyecto de ejemplo en nuestra instancia de demostración>](http://sonarqube.bitegarden.com/project/extension/bitegardenSecurity/asvs_report_page?id=org.owasp%3Abenchmark&qualifier=TRK)

<br>

El Estándar de Verificación de Seguridad en Aplicaciones (ASVS; por sus siglas en inglés) es una lista de
requisitos o pruebas de seguridad en aplicaciones que puede ser utilizado por arquitectos, desarrolladores,
probadores, profesionales de la seguridad, proveedores de herramientas y consumidores para definir,
construir, probar y verificar aplicaciones seguras.

ASVS tiene dos objetivos principales:

-- Ayudar a las organizaciones a desarrollar y mantener aplicaciones seguras.

-- Permitir que los proveedores de servicios de seguridad, los proveedores de herramientas de seguridad y
los consumidores alineen sus requisitos y ofertas.

Puedes obtener la última versión estable del [estándar traducido al español aquí](https://raw.githubusercontent.com/OWASP/ASVS/v4.0.3/4.0/OWASP%20Application%20Security%20Verification%20Standard%204.0.3-es.pdf).

## Como referenciar los requisitos del estándar ASVS 

Cada requisito tiene un identificador en el formato `<chapter>.<section>.<requirement>` donde cada elemento es un número, por ejemplo: 1.11.3

-- El elemento `<chapter>` corresponde al capítulo del que proviene el requisito, por ejemplo: todos los requisitos de 1.#.# son del capítulo de Arquitectura.

-- El elemento `<section>` corresponde a la sección dentro de ese capítulo donde aparece el requisito, por ejemplo: todos los requisitos de 1.11.# están en la sección Arquitectura de la Lógica del Negocio, del capítulo de Arquitectura.

-- El elemento `<requirement>` identifica el requisito específico dentro del capítulo y la sección, por ejemplo: 1.11.3 que a partir de la versión 4.0.3 del presente estándar es:

> Compruebe que todos los flujos de lógica de negocio de alto valor, incluida la autenticación, la administración de sesiones y el control de acceso, sean seguros para subprocesos y resistentes a las condiciones de tiempo de
comprobación y tiempo de uso.

## Usando SonarQube&trade; y el plugin de Security para verificar el cumplimiento con OWASP ASVS

Lo nuevo en la versión OWASP ASVS 4.0 es un mapeo completo hacia la enumeración de debilidades comunes (CWE; por sus
siglas en inglés), una de las solicitudes de mejora más pedida durante la última década. El mapeo CWE permite
a los fabricantes de herramientas y aquellos que usan software de administración de vulnerabilidades
comparar los resultados de otras herramientas.

No todos los elementos del ASVS tienen un CWE asociado y, dado que CWE tiene una gran cantidad de duplicados, OWASP ASVS ha intentado
asociar el más utilizado en lugar de necesariamente el más cercano.

Los controles de verificación no siempre se pueden asignar a debilidades equivalentes. Agradecemos la discusión en curso de la fundación del proyecto OWASP con la comunidad de CWE y
el campo de la seguridad de la información en general sobre cómo cerrar esta brecha. 

Esta es la razón por la que encontrarás en la página principal de nuestro plugin cuantos requisitos del estándar están cubiertos en tu instancia SonarQube&trade;. 
Esto dependerá de tu versión de SonarQube&trade; así como de la edición, ya que las ediciones comerciales (Developer, Enterprise, Data Center) incluyen reglas adicionales de seguridad
que cubren un mayor número de debilidades CWE.

Una vez que accedes a la nueva página de ASVS para tu proyecto podrás ver un resumen por capítulos:

<br>

<img src="/img/sonarqube-security/owasp-asvs-chapter-summary.png" alt="OWASP ASVS Security Assessment Chapter Summary" width="100%">

<br>

Nuestro [Security Plugin for SonarQube](/es/sonarqube-security) te mostrará cada uno de los capítulos de OWASP ASVS con los requisitos
que se estén cumpliendo o que estén fallando.

Hemos incluido una calificación (rating) para cada capítulo para que rápidamente puedas encontrar en qué capítulo se localizan 
los problemas de seguridad más importantes. 

Esta calificación se calcula de la misma forma que la calificación de Seguridad por defecto (será una E si al menos una de las vulnerabilidades 
encontradas es bloqueante, ...).

## Verifica el cumplimiento de los requisitos de OWASP ASVS

Tras el resumen por capítulo, encontrarás una lista detallada de todos los requisitos que están fallando para cada sección de cada
capítulo del estándar. 

Encontrarás una descripción del requisito con el CWE relacionado, y con el número de evidencias detectadas por SonarQube&trade; (ya sean vulnerabilidades o hotspots de seguridad).

<br>

<img src="/img/sonarqube-security/owasp-asvs-chapter-section-requirement.png" alt="OWASP ASVS Security Assessment Requirement Details" width="100%">

<br>

## Descarga la nueva versión

El Security Plugin ya está disponible para descarga a través del [Universal Plugin Manager](/es/sonarqube-upm)  o desde la página de [descarga del producto](/es/sonarqube-security-trial-form).

**¡Obtén tu prueba gratuita y verifica tu código frente al estándar OWASP ASVS hoy mismo!**

<a href = "/es/sonarqube-security#product-block-center" class = "btn btn-primary btn-call-to-action fancybox" style = "font-weight: bold; font-size: 16px; text-transform : mayúsculas; "> Inicia tu prueba gratuita > </a>

<br/>

---
**<span style="color: green">bitegarden</span> team**

_Helping companies to develop better software_