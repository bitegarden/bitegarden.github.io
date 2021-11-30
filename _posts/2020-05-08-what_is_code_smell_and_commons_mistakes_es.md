---
layout: post_es
title: ¿Qué es un code smell? Errores comunes
description: Un 'code smell', también conocido como 'mala práctica', en el ámbito de la programación se refiere a un síntoma en el código fuente que probablemente nos esté indicando que algo va mal 

english: what-is-code-smell-and-common-mistakes
permalink: que-es-un-code-smell-y-errores-comunes
italian: cosa-sono-code-smell-e-errori-comuni-nel-codice

cover: /img/thumbs/Thumb-what-is-code-smell-mistakes.jpg
---

Te acabas de incorporar a un proyecto en marcha y eso no es fácil, si tienes suerte puede ocurrir que encuentres algunas anotaciones en
el código como estas:  
  
`//TO DO` or `//FIX ME`  
  
Estos textos no agregan funcionalidad, pero subrayan una posible implementación incorrecta o algo para verificar. Algo "huele mal" en ese código.
El verdadero problema, con este tipo de malas prácticas, es que hay que buscarlos y no siempre es un trabajo fácil porque cada desarrollador tiene su "método" para marcarlo.

![que es un code smell - bitegarden](/img/posts/2020-05-08-what_is_code_smell_and_commons_mistakes.png){:width="100%" .center-image}
  
## ¿Qué es un *code smell*?
  
>“Un *code smell*, también conocido como mala práctica (o 'hediondez del código'), en el desarrollo de software, se refiere a cualquier síntoma en el código fuente de un programa que posiblemente indique un problema más profundo. (...)  
>  
>Los *code smells* usualmente no son bug de programación (errores) -- no son técnicamente incorrectos y en realidad no impiden que el programa funcione correctamente.
>  
>En cambio, indican deficiencias en el diseño software que puede ralentizar el desarrollo o aumentan el riesgo de errores o fallos en el futuro."  
>  
>**Fuente:** *[Wikipedia](https://es.wikipedia.org/wiki/Hediondez_del_código)*  
  
## Los errores más comunes
  
-- **Bloatware**: son partes del código (clases, métodos, ...) que han aumentado de manera desproporcionada y se han 
vuelto difíciles de mantener y están haciendo demasiadas cosas en lugar de tener una responsabilidad clara. 
Puede convertirse en un gran problema, especialmente si a nadie le importa su eliminación.
  
-- **Código repetido (duplicado)**: podría suceder cuando un desarrollador no puede cumplir con los plazos (o simplemente porque 
es demasiado vago) y copia y pega partes del código, en lugar de crear algo ad hoc. A veces también ocurre cuantos más programadores están trabajando en el desarrollo del mismo código. 
En el futuro, esto se traducirá en un gran esfuerzo, porque significa un cambio en más de un lugar o, lo que es peor, si uno de ellos es olvidado, funcionará de manera diferente.
  
-- **Clases perezosas (*lazy*)**, como sabéis, mantener el código cuesta tiempo y dinero, por lo que si una clase se 
construyó solo para anticipar las características futuras y no está haciendo mucho en la situación actual, debería eliminarse.
  
Desafortunadamente, a menudo estos elementos no son fáciles de arreglar y necesitan un gran esfuerzo o un cambio importante del código.
  
## ¿Cómo evitar los *code smells*?  
  
[SonarQube](https://www.sonarqube.org/) es una herramienta increíble para controlar el estado de su código y ayudar a mejorar la revisión de estas malas prácticas
  
Una buena práctica para el equipo es comenzar a hacer un análisis continuo del código, a fin de poder ir corrigiendo
las malas prácticas, errores (*bugs*) y vulnerabilidades del código en lugar de crear nuevos procesos específicos para 
resolverlo.
  
Y si ya estás utilizando SonarQube y estás buscando mejorar la gestión de la deuda técnica de tu proyecto para tenerla
bajo control, puedes extender su funcionalidad con [SQALE Plugin](https://www.bitegarden.com/sonarqube-sqale) que es una
herramienta oficial que implementa el método [SQALE](http://www.sqale.org/tools) para gestionar la deuda.

