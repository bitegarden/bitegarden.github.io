---
layout: post_es
title: ¿Qué es un Quality Gate en SonarQube?
description: Te enseñamos autilizar los Quality Gates para garantizar la seguridad y calidad de tu código

permalink: que-es-un-quality-gate-sonarqube
english: what-is-quality-gate-sonarqube


cover: /img/posts/2025-03-02-what-is-quality-gate-sonarqube_es.png
---

SonarQube es una herramienta clave para analizar el código. Está compuesto de una serie de **mecanismos** que ayudan a los desarrolladores a **garantizar la calidad y la seguridad del código**. Uno de ellos, son los Quality Gates y en este artículo vamos a explicar qué son y cómo los puedes configurar en una instancia de SonarQube Server.

<h2>¿Qué es un Quality Gate?</h2>

Un Quality Gate es un **conjunto de criterios** que miden si un proyecto cumple con unos estándares de calidad. El usuario define un conjunto de condiciones para poder medir los proyectos y responder a la siguiente pregunta: **¿Mi proyecto está listo para su lanzamiento?**. Ejemplos de estas condiciones son: no tener issues y la cobertura del código no puede ser superior a 40%. 

¡Ojo! **No todos los proyectos utilizan el mismo Quality Gates**. ¿Por qué? No es práctico para todos los proyectos. Por ejemplo, un proyecto web no necesita la misma cobertura de código que un proyecto de Java. 

Por esto, el usuario puede definir varios Quality Gates. A continuación, te enseñamos cómo crear uno. 

<h2>¿Cómo definir un Quality Gate en SonarQube?</h2>

Para establecer un Quality Gate en SonarQube Server debes de seguir estos pasos: 

1 - **Accede a tu instancia** de SonarQube. <br>
2 - En el **menú superior** accede a Quality Gates. <br>
3 - Pulsa el botón **Create** y se te abrirá una pantalla para que **añadas un nombre** al Quality Gate. <br>
4 - Por defecto, en la sección **Conditions** ya aparece un listado para que puedas **editar los valores** (issues, security hotspots reviewed, coverage, % líneas duplicadas)
5 - Si quieres **añadir más condiciones**, tienes que pulsar el botón **Unlock** y después el de **Add conditions**. 

Una vez tienes tu Quality Gate creado puedes **configurarlo como predeterminado**.

<h2>Beneficios de utilizar los Quality Gates</h2>

A continuación, te indicamos algunos de los beneficios de utilizar los Quality Gates para corregir tus proyectos: 

- Asegura la calidad del código

- Da visibilidad al proceso de calidad

- Mantiene la seguridad del código

- Fomenta el uso de buenas prácticas

- Aumenta la confianza sobre el desarrollo del código

SonarQube en su documentación tiene información específica sobre los [Quality Gates](https://docs.sonarsource.com/sonarqube-server/10.8/instance-administration/analysis-functions/quality-gates/){:target="_blank"}

<h3>Utiliza el Quality Gates Board for SonarQube</h3>

En **bitegarden** desarrollamos un plugin para que puedas validar tu código contra **más de un umbral de calidad**. Hablamos de **Quality Gates Board for SonarQube**, que añade una página dentro del proyecto para que puedas validar si tu código cumple contra más de un umbral de calidad.

En esta nueva página podrás **personalizar el título de los umbrales de calidad** para que sea más fácil leer el análisis de la información. A continuación, te dejamos un ejemplo de esta página dentro de un proyecto de SonarQube Server: 

<img width="100%" src="/img/sonarqube-quality-gates-board/quality-gates-board-2.png" alt="quality gates board with passed failed conditions">


Si quieres probar este plugin en tu instancia, puedes descargarlo a través de [este enlace](/es/sonarqube-quality-gates-board-trial-form). 

---
**<span style="color: green">bitegarden</span> team**

_Helping companies to develop better software_
