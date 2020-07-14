---
layout: post_es
title: Analisis Estatico Del Codigo Con Sonarqube
description: Invertir en el control de la **calidad de los proyectos** significa analizar el código durante todo el proceso y con eso incluir en los flujos de trabajo la code reviews para mantener alta la calidad.

permalink: analisis-estatico-del-codigo-con-sonarqube
english: static-code-analysis-with-sonarqube
cover: /img/thumbs/2020-07-13-static-code-analysis-using-sonarqube-thumb.png
---
Invertir en el control de la **calidad de los proyectos** significa analizar el código durante todo el proceso y con eso incluir en los flujos de trabajo la code reviews para mantener alta la calidad.

Para obtener este resultado es necesario incluir un analizador estático de código, como **[SonarQube](https://www.sonarqube.org/)**.  

![SonarQube](/img/posts/2020-07-13-static-code-analysis-using-sonarqube-logo-300x93.jpg)

## Que es SonarQube y a que sirve

**SonarQube** es un software **open source** que permite hacer **análisis estáticas** del código y obtener métricas que permiten mejorar la calidad del código y descubrir cuales son los problema que tiene. 

Las métricas están basadas en [SQALE](https://www.bitegarden.com/sonarqube-sqale), que podríamos definir como un algoritmo que dice sí las expectativas de calidad que se fijaron durante el ciclo de vida del desarrollo se han cumplido y/o en cuanto tiempo se va a demorar en alcanzarlas.

Seria buena praxis utilizar esta herramienta desde el inicio de los proyectos ya que es **evolutivo**, ósea que va analizando día a día lo que va sucediendo. Utilizar esta herramienta va cambiar el workflow de trabajo, que ya no será codificar, codificar y codificar si no codificar, analizar y corregir. Esta nueva práctica va a evitar que se genere una deuda técnica muy grande y nos va a permitir de mejorar la calidad del proyecto.

Entres las métricas tenemos el código duplicado, cobertura, code smells, bugs, vulnerabilidades factor de riesgo, densidad de violaciones de seguridad y mucho más.

SonarQube está dividido en dos herramientas: el **servidor** donde se encuentra el engine que realiza el análisis, almacena los resultados y es donde se puede definir los proyectos, parámetros de calidad, resultados análisis, quien se encargará de cada tarea y por el otro lado tenemos **SonarQube Scanner** que es el analizador.

SonarQube no está limitado a un único lenguajes, se pueden hacer análisis de diferentes códigos y repositorios.

Actualmente, la última versión es la **8.3.1**, y soporta más de **27 lenguajes de programación**.

![Sonarqube - Lenguajes de programación](/img/posts/2020-07-13-static-code-analysis-using-sonarqube-programming-languages.jpg)

## Análisis estático o dinámico del código fuente

Cuando se habla de **análisis estático** de código se entiende el proceso de evaluación del software sin ejecutarlo, en manera de poder obtener errores y métricas que hablen del código lo más pronto posible.

En cambio, para el **análisis dinámico** se tiene que ejecutar el software para ver el comportamiento y los tiempos. El problema en este caso es que se necesita más casos de prueba para poder definir que nuestro código está funcionando correctamente.

## Funcionalidades más relevantes de SonarQube
  

-   **Vulnerabilidades**: SonarQube posee una gran una DB de code smells y de vulnerabilidades permitiendo conocer el nivel de seguridad del proyecto de manera detallada.
    
-   **Código duplicado**: la herramienta detecta el código duplicado y nos permite optar por refactoring o desacoplar componentes.
    
-   **Standard de programación**: permite saber si se incumplen algún estándar y hay malas prácticas.
    
-   **Cobertura**: monitoriza sí la cobertura de las pruebas es suficiente para los estándares de calidad y si es necesario aumentar la inversión en los tests.
    
-   **Perfiles de calidad**: por cada lenguaje hay un perfil de calidad por defecto pero también hay la posibilidad de crear un perfil personalizado. Se trata de un pack de reglas que se aplican durante el análisis estático del código.

Como has visto, [SonarQube](https://www.sonarqube.org/) es una herramienta muy potente - y además es **gratuita** y **open source** - que con poco esfuerzo permite tener controlado el nivel de calidad. Y si estás cargo de muchos proyectos software te dará la posibilidad de tener todo bajo control.

Estamos seguros que te encantará, así que pruébalo y haznos saber tus experiencias.
