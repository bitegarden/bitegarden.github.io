---
layout: post_es
title: 'Overview Report para SonarCloud 1.2'
description: Esta nueva versión incluye nuevas funcionalidades para mejorar los informes generados 

english: new-release-overview-report-sonarcloud-1-2
permalink: nueva-version-overview-report-sonarcloud-1-2
italian: nuova-versione-overview-report-sonarcloud-1-2

cover: /img/posts/2022-07-27-new-release-overview-report-cloud.png
---

Acabamos de liberar una nueva versión de *[bitegarden Overview Report for SonarCloud&trade;](/es/sonarcloud-overview)*, la versión 1.2, que incluye varias novedades interesantes:


### Estado de Salud (Health Rating)

Por un lado incluye en el informe una nueva sección “Health Rating” que permite conocer el estado de salud de la organización de SonarCloud en cuanto a si el código está listo para subir a producción (cumplimiento de los quality gates).

El estado de salud es el porcentaje de proyectos que tienen cumplen con el umbral de calidad (*quality gate*):

-- A: > 80%

-- B: > 60%

-- C: > 40%

-- D: > 20%

-- E: <= 20%

<br>
<img src="/img/posts/2022-07-27-overview-health-rating.png" alt="health rating" width="100%">
<br><br>

### Valores diferenciales

Se incluye la capacidad para poder ver las diferencias con respecto a periodos anteriores. 
Se han incluido por defecto 3 periodos (desde el primer análisis, desde hace seis meses, y en el último mes), 
pero lo interesante es que también se incluye la posibilidad de especificar una fecha concreta desde la cual ver 
las diferencias y evolución. 

Esta información se muestra tanto en la sección “ejecutiva” de la primera página como en el listado de proyectos.

<br>
<img src="/img/posts/2022-07-27-overview-differential-values.png" alt="differential values" width="100%">
<br><br>

### Umbrales de calidad 

Además, en el listado con el detalle de proyectos también se ha incluido estado del quality gate para cada proyecto.

<br>
<img src="/img/posts/2022-07-27-overview-quality-gates.png" alt="quality gates" width="100%">
<br><br>

### Descarga la última versión

Esperamos que os guste esta nueva versión, actualiza para disfrutar de todas las novedades.

Puedes descargar la versión desde [la página del producto](/es/sonarcloud-overview-trial-form).

Y recuerda que el feedback es siempre muy apreciado así que sientete libre de abrir un ticket en 
nuestro [portal de soporte](http://support.bitegarden.com/) para ayudarnos a seguir mejorando el producto.

<a href = "/es/sonarcloud-overview-trial-form" class = "btn btn-primary btn-call-to-action fancybox" style = "font-weight: bold; font-size: 16px; text-transform : mayúsculas; "> Descarga > </a>

<br/>

---
**<span style="color: green">bitegarden</span> team**

_Helping companies to develop better software_