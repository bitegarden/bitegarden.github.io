---
layout: post_es
title:  Como evaluar la deuda técnica en SonarQube
description: Qué es la deuda técnica, cómo medirla y controlarla con SonarQube.

permalink: como-evaluar-deuda-tecnica-sonarqube
english: how-to-evaluate-technical-debt-sonarqube
cover: /img/posts/2021-04-15-how-to-evaluate-technical-debt-sonarqube-1.png
---

Es posible que no sepas a qué nos referimos cuando hablamos de **deuda técnica**, pero seguramente, solo por el hecho de tener la palabra “deuda”, ya te puedas imaginar que no es algo bueno, y que es algo que si no se trata, afectará de alguna forma a nuestros proyectos.
Pues hoy quiero hablarte sobre ello, la deuda técnica, en qué afecta a tus proyectos, y como puedes evitar los problemas que te ocasionaría.

## ¿Qué es la deuda técnica?

En primer lugar, vamos a ver en qué consiste la **deuda técnica**, y para ello, nada mejor que compararlo con una deuda que posiblemente sí conozcas, la deuda económica.

En las ocasiones en que necesitas una elevada cantidad de dinero (compra de una vivienda, creación de una empresa, etc…) necesitas pedir dicha cantidad para que te la presten, y posteriormente, devolverla en pequeños pagos durante varios años, ya que, de otra forma, sería complicado haber reunido el dinero suficiente a tiempo para poder hacer frente a esas compras.

Pues bien, el término deuda técnica, hace referencia a cuando necesitamos, en este caso, una cantidad de tiempo (sí, que en el fondo es dinero) para poder entregar el trabajo acordado en la fecha pactada.

Y esto ocurre, por ejemplo: cuando **copiamos código** en lugar de crear una nueva clase que realice la función que necesitamos, o cuando **duplicamos literales** en lugar de usar constantes.

En esos casos, estamos pidiendo tiempo para entregar antes el código, pero igual que en la deuda técnica, ese tiempo tendremos que devolverlo, ya que de no hacerlo, tendremos problemas en forma de errores en el proyecto, o en el mejor de los casos, de invertir posteriormente el tiempo necesario para que el código siga las buenas prácticas.

Y además, otra cosa en lo que se parece la deuda técnica con la económica, es que se tiene que **pagar con intereses**. Si en la deuda económica, se paga un importe adicional para costear el préstamo, el cambio de contexto hace que se tarde más en resolver un code smell, que sí se hubiera hecho correctamente desde el principio.

Así que, la deuda técnica, no está directamente relacionada con la fiabilidad o seguridad de nuestro proyecto, ya que ello son errores que ocurren en nuestro código, principalmente por desconocimiento. Sino que está relacionado con la **mantenibilidad**, es decir, con la facilidad para que podamos actualizar o hacer evolucionar nuestros proyectos.

## ¿Cómo medir la deuda técnica?

**Bien, y ahora que ya sabes qué es la deuda técnica, ¿cómo se mide? ¿Cuánta deuda técnica tenemos? ¿Es mucha o es poca?**

Como te decía al principio, en la deuda técnica, lo que se pide prestado, es tiempo; así que, lo que **debes devolver es tiempo**. Por otro lado, hemos visto que afecta a la mantenibilidad, y es por eso que puedes ver la primera medida en la que SonarQube puede ayudarte con la deuda técnica: cuando detecta algún code smell, te indica el **tiempo estimado para solucionarlo**.

<img src="img/posts/2021-04-15-how-to-evaluate-technical-debt-sonarqube-1.png" width="100%" alt="Cómo medir la deuda técnica con SonarQube">

## Nivel de la deuda técnica

Es importante ser consciente que ese tiempo depende en gran medida de la experiencia del desarrollador, y también puede verse afectado por las particularidades del proyecto, organización o incluso su infraestructura. Así que, auque no es una información exacta, puede servir como una primera aproximación.

Pero, por otro lado, saber el tiempo que “debemos”, no es suficiente para saber el nivel de deuda técnica del proyecto. 

No es lo mismo que una persona deba 5.000€ en un préstamo para la compra de un coche cuyo precio son 10.000€, a que una organización deba 5.000€ en un préstamo para comprar unas oficinas que cuestan 500.000€.

En el primer caso, la deuda es la mitad del bien (el coche) y en algún caso, si hay un imprevisto (por ejemplo, que el endeudado quedara sin empleo) la deuda pendiente supondría un problema. Mientras que en el segundo caso, la deuda está prácticamente pagada y no debería ocasionar ningún contratiempo a la organización. 

Es por ello, que la **deuda técnica debe relacionarse con el tiempo total del desarrollo del proyecto** (lo que equivaldría al precio total del bien), y de esta forma se muestra también como un porcentaje.

Por ello, cuando hablamos de una deuda técnica del 10%, quiere decir que, si el proyecto se ha desarrollado en unas 1.000 horas, el tiempo de corregir las evidencias relacionadas con la mantenibilidad (code smells) es aproximadamente unas 100 horas.

## Controlar la deuda técnica en SonarQube

SonarQube le da una gran importancia al seguimiento de la deuda técnica.

Tanto es así que lo utiliza como uno de sus tres principales indicadores que, como ya debes saber son: la fiabilidad, la seguridad y la mantenibilidad. 

## Deuda técnica en la calificación global de mantenibilidad

<img src="img/posts/2021-04-15-how-to-evaluate-technical-debt-sonarqube-2.png" width="100%" alt="Deuda técnica en la calificación global de Mantenibilidad en SonarQube">

Y en el caso de la calificación global de mantenibilidad, SonarQube mostrará el resultado en función de la deuda técnica obtenida.

Las calificaciones globales van desde A (mejor calificación) hasta E (peor calificación), y sobre la mantenibilidad, SonarQube puede mostrar los siguientes resultados:

 - A: Deuda técnica inferior al 5%
 - B: Deuda técnica entre 6% y 10%
 - C: Deuda técnica entre 11% y 20%
 - D: Deuda técnica entre 21% y 50% 
 - E: Deuda técnica superior superior al 50%


## Tiempo necesario para resolver la deuda técnica

Por otro lado, SonarQube muestra el tiempo total que suman todos los code smells del proyecto.
Así en la imagen anterior, puedes ver que en el nuevo código (últimos 30 días) existe 1 code smell, cuyo tiempo aproximado de solución es de 30 minutos, así que la deuda técnica del código nuevo será ese tiempo: 30 minutos.

Mientras que en el proyecto completo, existen más de 6.900 code smells, y el tiempo total de solucionarlos será aproximadamente de 164 días.

Hay que tener en cuenta que Sonarqube almacena la deuda técnica en minutos, pero la puede mostrar en horas o en días (1 día = 8 horas de trabajo). 


## Seguimiento de la deuda técnica

Para hacer el seguimiento de la deuda técnica en SonarQube, tenemos distintas opciones.
Por un lado, en la sección de Medidas, puede verse la deuda técnica de todo el código, o únicamente la del nuevo.

<img src="img/posts/2021-04-15-how-to-evaluate-technical-debt-sonarqube-3.png" width="100%" alt="Seguimiento de la deuda técnica en SonarQube">

Mientras que en la **Sección Activity**, podemos ver el historial del resultado de la deuda técnica a lo largo de la vida del proyecto.

<img src="img/posts/2021-04-15-how-to-evaluate-technical-debt-sonarqube-4.png" width="100%" alt="Seguimiento de la deuda técnica en SonarQube">

De esta forma, puedes ver la evolución de tu deuda técnica aunque como hemos dicho antes, únicamente en días. 

Si realmente quieres ver lo que supone para el proyecto, deberías comprobar el ratio de deuda técnica, y de esta forma, podrás ver mejor su evolución, independientemente de que el proyecto haya crecido en número de líneas.

<img src="img/posts/2021-04-15-how-to-evaluate-technical-debt-sonarqube-5.png" width="100%" alt="Technical debt monitoringwith SonarQube">

Y con esto, has podido ver qué es la deuda técnica, y como gracias a SonarQube puedes mantenerla bajo control. 

Así que, intenta no endeudarte mucho, que en el futuro tendrás que pagarlo… ¡y con intereses! 😉


Y si necesita más, hemos creado algunos **Plugins para SonarQube** que mejoran todo su ecosistema de calidad de código.
<br>
<br>
<a href="/products" class="btn btn-primary btn-call-to-action fancybox" style="font-weight:bold;font-size:15px; text-transform: uppercase;">DESCUBRE LOS PLUGINS PARA SONARQUBE > </a>
<br>
<br/>

Happy coding!

---
**<span style="color: green">bitegarden</span> team**

_Helping companies to develop better software_
