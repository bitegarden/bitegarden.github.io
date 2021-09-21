---
layout: post_es
title: Análisis Estático Del Código Con SonarQube
description: Invertir en el control de la **calidad de los proyectos** significa analizar el código durante todo el proceso y con eso incluir en los flujos de trabajo la code reviews para mantener alta la calidad.

permalink: analisis-estatico-del-codigo-con-sonarqube
english: static-code-analysis-with-sonarqube
italian: gestione-qualita-codice-con-sonarqube

cover: /img/thumbs/2020-07-13-static-code-analysis-using-sonarqube-thumb.png
---

Invertir en el control de la **calidad de los proyectos** significa analizar el código durante todo el proceso y con eso 
incluir en los flujos de trabajo la revisión de código para mantener la más alta la calidad y seguridad.

Para obtener este resultado es necesario incluir un analizador estático de código, como **[SonarQube&trade;](https://www.sonarqube.org/)**.  

![SonarQube](/img/posts/2020-07-13-static-code-analysis-using-sonarqube-logo-300x93.jpg){: .center-image}

---

## ¿Qué es SonarQube&trade; y para qué sirve?

**SonarQube&trade;** es un software **open source** que permite hacer **análisis estático** del código y obtener métricas 
que permiten mejorar la calidad del código y descubrir evidencias de los problemas existentes en el código. 

**SonarQube&trade;** calcula muchas métricas asociadas al código, y las métricas de deuda técnica están basadas en 
[**SQALE**](https://www.bitegarden.com/sonarqube-sqale), que podríamos definir como un algoritmo que dice sí las 
expectativas de calidad que se fijaron durante el ciclo de vida del desarrollo se han cumplido y/o en cuanto tiempo 
se va a demorar en alcanzarlas.

Sería buena praxis utilizar esta herramienta desde el inicio de los proyectos ya que permite conocer la **evolución**, 
analizando día a día lo que va sucediendo. Utilizar esta herramienta nos permitirá adaptar el workflow de trabajo para
escribir mejor código. Esta nueva práctica va a evitar que se genere una deuda técnica muy grande y nos va a permitir
 mejorar la calidad del proyecto de forma natural.

Entre las métricas tenemos el código duplicado, cobertura, code smells, bugs, vulnerabilidades, densidad de evidencias 
de seguridad y mucho más.

**SonarQube&trade;** está dividido en dos herramientas: el **servidor** donde se encuentra el motor de computación que 
realiza el análisis, almacena los resultados y es donde se puede definir los proyectos, parámetros de calidad, 
resultados análisis, quien se encargará de cada tarea y por el otro lado tenemos **SonarQube&trade Scanner** que es el analizador.

**SonarQube&trade;** no está limitado a un único lenguajes, se pueden hacer análisis de diferentes códigos y repositorios.

Actualmente, la última versión es la **8.4**, y soporta más de **27 lenguajes de programación**.

![Sonarqube - Lenguajes de programación](/img/posts/2020-07-13-static-code-analysis-using-sonarqube-programming-languages.jpg)

## Análisis estático o dinámico del código fuente

Cuando se habla de **análisis estático** de código se entiende el proceso de evaluación del software sin ejecutarlo, 
en manera de poder obtener errores y métricas que hablen del código lo más pronto posible.

En cambio, para el **análisis dinámico** se tiene que ejecutar el software para ver el comportamiento y los tiempos. 
El problema en este caso es que se necesita más casos de prueba para poder definir que nuestro código está funcionando correctamente.

## Funcionalidades más relevantes de SonarQube
  
- **Vulnerabilidades**: SonarQube&trade posee un gran conjunto de reglas para detectar bugs, code smells y vulnerabilidades 
y así conocer el nivel de seguridad y calidad del proyecto de manera detallada.
    
- **Código duplicado**: la herramienta detecta el código duplicado y nos permite tomar decisiones para refactorizar o desacoplar componentes.
    
- **Buenas prácticas de programación**: permite saber si se incumplen los estándares y detecta las malas prácticas (code smells).
    
- **Cobertura**: monitoriza sí la cobertura de las pruebas es suficiente para los estándares de calidad y si es necesario aumentar la inversión en los tests.
    
- **Perfiles de calidad**: por cada lenguaje hay un perfil de calidad por defecto pero también hay la posibilidad de crear 
un perfil personalizado. Se trata de un pack de reglas que se aplican durante el análisis estático del código.

Como has visto, [SonarQube&trade](https://www.sonarqube.org/) es una herramienta muy potente - y además es **gratuita** y 
**open source** - que con poco esfuerzo permite tener controlado el nivel de calidad. Y si estás cargo de muchos 
proyectos software te dará la posibilidad de tener todo bajo control.

Y como el ciclo de desarrollo de software (SDLC) también involucra a otros perfiles profesionales, no solo a desarrolladores, 
hemos creado unos [**plugins para SonarQube&trade**](https://www.bitegarden.com/es/products/) capaces de proporcionar a 
SonarQube&trade todas las funcionalidades para generar **informes** que actualmente se echan de menos y que son demandados por **project managers**, **product owners**. 


<a href="/es/products/" class="btn btn-primary btn-call-to-action fancybox">DESCUBRE LOS PLUGINS ></a>

Estamos seguros de que te encantará, así que pruébalos y haznos saber tus experiencias.
