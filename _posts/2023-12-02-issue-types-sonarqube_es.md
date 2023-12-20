---
layout: post_es
title: 'Tipos de issues en SonarQube'
description: Te explicamos qué es un bug, una vulnerabilidad y un code smell

permalink: tipos-issue-sonarqube
english: issue-types-sonarqube
italiano: tipo-di-issue-sonarqube

cover: /img/posts/2023-12-02-issue-types-sonarqube_en.png 
---

SonarQube es una **herramienta esencial** para el desarrollo de software, porque ofrece una visión detallada de la calidad del código. Una de las características más destacadas de SonarQube es su capacidad para identificar y clasificar problemas en el código a través de las issues. En este artículo, vamos a explicar los **diferentes tipos de issues** que SonarQube puede detectar, destacando su importancia y cómo abordarlos para mejorar la calidad del software.

<h2>¿Qué tipos de issues hay en SonarQube?</h2>

<h3>Bugs</h3>

Los bugs son un **error de código** que puede producir un fallo inesperado durante la ejecución del código. En la siguiente imagen podemos ver un ejemplo de bug. SonarQube lo clasifica como tal, indica dónde está y también por qué lo califica como una issue. 

<img src="/img/posts/bug-example.png" width="100%" alt="Bug example in SonarQube">

<h3>Vulnerability</h3>

Una vulnerabilidad es **un punto en el código** que esta al descubierto, vulnerable de recibir ataques externos. En la siguiente imagen podemos ver un ejemplo de vulnerabilidad que ha detectado SonarQube al considerar que una contraseña puede estar expuesta. 

<img src="/img/posts/vulnerability-example.png" width="100%" alt="Vulenrability example in SonarQube">


<h3>Code Smells</h3>

Un code smell es un problema que hace que el **código sea dificil de entender**. En la siguiente imagen podemos ver un ejemplo de code smell en el que SonarQube sugiere eliminar un parámetro que no se utiliza. 

<img src="/img/posts/code-smell-example.png" width="100%" alt="Code Smells example in SonarQube">

Hay que recordar en la **última release de SonarQube 10.3**, Sonar anunció que estos tipos de issues quedarán **obsoletos**. Por lo que en nuevas actualizaciones las issues ahora estarán realacionadas con los atributos de Clean Code y las cualidades de software afectadas. 

Si necesitas más información sobre SonarQube, puedes contactar con nosotros a través de este [formulario](/es/contact.html).


---
**<span style="color: green">bitegarden</span> team**

_Helping companies to develop better software_