---
layout: post_es
title: Genera un informe PDF de la calidad de tu código con SonarQube&trade;
description: Diferentes formas de generar informes de tus datos de la calidad del código en SonarQube&trade;

english: generate-code-quality-pdf-report-sonarqube
permalink: genera-informe-pdf-calidad-codigo-sonarqube
cover: /img/thumbs/2020-07-31-generate-pdf-report-with-sonarqube.png
---

SonarQube&trade; es una herramienta hecho por desarrolladores para desarrolladores. Proporciona todo lo 
necesario para escribir código limpio y seguro desde el primer momento y gestionar la deuda técnica para que
tu desarrollo sea sostenible. 

¿Pero qué ocurre si quieres explotar los datos y generar algún informe de calidad de los proyectos? En este sentido 
SonarQube&trade; no ofrece por defecto ninguna gestión informes sencilla, si bien puedes usar la API web para desarrollarlos tu 
 mismo, en la mayoría de ocasiones lo que se busca es algo más rápido y sencillo.
 
# ¿Cómo generar PDFs de forma sencilla?

Con nuestro producto [bitegarden Report for SonarQube&trade;](/es/sonarqube-report) se pueden generar estos informes 
de la manera más sencilla posible. 

Desde el espacio de proyecto en la opción ___"More..."___ encontrarás una sección que te proporciona todos los informes que
necesitas, desde un resumen ejecutivo hasta un informe con todas las evidencias encontradas. Basta con descargar el informe
deseado pulsando en el botón de descarga correspondiente.

![Gestión de informes](/img/sonarqube-report/bitegarden-report-management_es.png){:width="100%" .center-image}

# Configura un logo personalizado

Por defecto el plugin usará el logo de bitegarden en el pie de cada página, pero si lo necesitas, puedes cambiarlo
desde la configuración del plugin para que se utilice el logotipo de tu organización o incluso el logotipo de tu proyecto.

Si quieres cambiar el logotipo para todos los informes de instancia de SonarQube&trade; tan solo tienes que ir a la 
configurcación general del plugin a nivel global (___Administration -> General Settings___) y usar la URL del logo que
quieras que aparezca en el pie de página:

---

![Gestión de informes](/img/sonarqube-report/bitegarden-report-logo-global-settings.png){:width="100%" .center-image}

<p class="center-text">
    Configuración del logotipo del pie de página
</p>

--- 

![Ejemplo de informe con logotipo personalizado](/img/posts/2020-07-31-bitegarden-report-logo-sample.png){:width="100%" .center-image}

<p class="center-text">
    Ejemplo de informe con logotipo personalizado
</p>

---

# Diferentes informes, diferentes objetivos

Cada persona del equipo puede requerir un tipo de informe distinto. Inicialmente pensábamos que ciertos roles de los equipos
accederían a SonarQube&trade; para ver los detalles de las evidencias pero la experiencia nos dice que esto no es así, y
que existen muchos roles que no acceden a la herramienta y por tanto, necesitan trabajar con informes extraídos y en otro
formato distinto.

## Informe con resumen ejecutivo (PDF)

---

**Objetivo**: poder determinar de un vistazo si el proyecto cumple o no con las condiciones de calidad así como los principales
valores para cada una de las dimensiones de calidad analizadas

---

De este informe [ya hablamos en su momento](/nueva-version-report-2-0) cuando liberamos la versión 2.0 del plugin. Se 
trata de un informe en una única página con toda la información importante de la calidad del código de nuestro proyecto, 
que incluye:

-- Los tres ejes del modelo de calidad: **fiabilidad, seguridad y mantenibilidad**

-- **Código repetido** (o duplicado)

-- **Cobertura** de código y **tests unitarios**

-- **Evidencias bloqueantes y críticas** desglosadas por bugs, vulnerabilidades y code smells.

Incluye tanto los valores globales como la información en el periodo de fuga (código nuevo o modificado). 

<a href="http://sonarqube.bitegarden.com/api/bitegarden/report/pdf?resource=apache:airflow&branch=master" target="_blank" class="btn btn-primary btn-call-to-action fancybox">VER EJEMPLO RESUMEN EJECUTIVO ></a>

## Informe resumen de evidencias (PDF)

---

**Objetivo**: conocer un resumen de evidencias de nuestro proyecto (más frecuentes, más severas) y un resumen por regla
con las principales evidencias detectadas (fichero, línea, mensaje) 

---

Este informe está disponible a partir de la versión 2.1 e incluye la página de resumen ejecutivo y añade nuevas páginas
al informe:

-- **Evidencias más detectadas**: listado de las evidencias por frecuencia de aparición. Las reglas con mayor número de 
evidencias aparecerán las primeras.

-- **Evidencias por severidad**: listado de las evidencias por severidad. Las reglas con mayor severidad aparecerán las
primeras independientemente de que no sean las más frecuentes.

-- **Desglose de evidencias por regla**: una página por cada una de las reglas de las que se hayan detectado evidencias
con una pequeña descripción y un listado con un resumen de evidencias detectadas. 

El informe permite tener un mayor nivel de detalle para poder remitirse a equipos externos que no puedan ver la herramienta 
o como informe de auditoría de un proyecto, donde quieran mostrarse las principales evidencias.  

<a href="http://sonarqube.bitegarden.com/api/bitegarden/report/pdf_issues_breakdown?resource=apache:airflow&branch=master" target="_blank" class="btn btn-primary btn-call-to-action fancybox">VER EJEMPLO RESUMEN EVIDENCIAS ></a>

## Informe completo de evidencias (PDF)

---

**Objetivo**: conocer el detalle completo de evidencias de nuestro proyecto

---
  
Este informe es el más completo (y el más "grande") ya que incluye toda la información de los informes anteriores pero 
en lugar de un resumen de una página por regla, se muestran todas las evidencias detectadas. Si una regla tiene 50 evidencias
el informe incluirá la localización de las 50 evidencias (fichero, línea, y mensaje de error).

Este informe permite disponer de TODA la información de la calidad del código del proyecto para entregar a quién pueda
corresponder la revisión del cumplimiento de la calidad del código.

<a href="http://sonarqube.bitegarden.com/api/bitegarden/report/pdf_full_issues_breakdown?resource=apache:airflow&branch=master" target="_blank" class="btn btn-primary btn-call-to-action fancybox">VER EJEMPLO COMPLETO EVIDENCIAS ></a>

## Informe de métricas personalizado (ODT)

---

**Objetivo**: crear informes de métricas con aspecto completamente personalizado que además se puedan editar posteriormente
para incluir información manual 

---
  
Este tipo de informe se crea a partir de una plantilla Open Document (documento ODT).

Permite crear informes con las diferentes secciones completamente personalizadas y con textos, párrafos, estilos y 
tablas según se configure la plantilla. 

La definición de la plantilla se basa en el uso de FreeMarker como variables insertadas en el documento ODT. Nuestro plugin
sustituirá las variables por los valores reales del proyecto según las métricas de SonarQube&trade;. Más información sobre
como utilizarlo [aquí](/es/sonarqube-report-documentation).

<a href="http://sonarqube.bitegarden.com/api/bitegarden/report/odt?resource=apache:airflow&branch=master" target="_blank" class="btn btn-primary btn-call-to-action fancybox">VER EJEMPLO OPEN DOCUMENT ></a>

--- 

### Descubre más ejemplos...

Si quieres ver como funciona la generación de informes en una instancia de SonarQube&trade; en funcionamiento puedes
descargar la [versión de prueba de 14 días](/es/sonarqube-report-trial-form) o acceder a nuestra instancia de demostración
a alguno de los proyectos disponibles, como por ejemplo [Apache Airflow](http://sonarqube.bitegarden.com/project/extension/bitegardenReport/report_page?id=apache%3Aairflow&qualifier=TRK).

¿A qué esperas para generar informes de calidad del código? ¿Tienes sugerencias para crear nuevos informes? 
¡Deja tus comentarios y ayudanos a mejorar el producto!

<a class="btn btn-primary btn-call-to-action fancybox" href="/es/sonarqube-report-trial-form">PROBAR ></a>

