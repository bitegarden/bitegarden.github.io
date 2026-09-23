---
layout: post_es
title: Cómo exportar informes de SonarQube a PDF y Excel paso a paso
description: Aprende a exportar resultados de SonarQube a PDF y Excel, incluyendo bugs, code smells, cobertura y duplicaciones, de forma rápida y sencilla. 

permalink: exportar-informes-sonarqube-pdf-excel
english: export-reports-sonarqube-pdf-excel


cover: /img/posts/2026-09-04-export-reports-sonarqube-pdf-excel_es.png
---

SonarQube permite consultar **una gran cantidad de información** sobre la calidad y seguridad del código. El problema aparece cuando necesitas compartir esos resultados, documentarlos para una auditoría o presentar el estado de un proyecto a personas que no trabajan directamente con SonarQube.

¿Cómo exportar los resultados de **SonarQube a PDF o Excel**? ¿Cómo generar un **informe detallado** con bugs, code smells, cobertura y duplicaciones? Desde bitegarden te recomendamos utilizar los **Report Plugins for SonarQube&trade;**, que permiten convertir las métricas de tus proyectos en informes preparados para compartir, revisar o documentar.

<h2>¿Qué información puedes exportar de SonarQube?</h2>

Dependiendo del informe y de la versión de SonarQube utilizada, puedes **recopilar en un mismo documento información** como: Bugs e incidencias de código, Vulnerabilidades y hotspots de seguridad, Code smells, Cobertura de código, Duplicación, Métricas de fiabilidad, seguridad y mantenibilidad, Quality Gate y sus condiciones y Métricas generales del proyecto.

<h2>Cómo generar un informe PDF de SonarQube</h2>

Con **Report Plugin for SonarQube&trade; Server** puedes generar un informe PDF directamente desde la interfaz de SonarQube.

El proceso es sencillo: **instala el plugin, accede al proyecto que quieres analizar y genera el informe desde SonarQube**. El PDF recopila las métricas más relevantes del proyecto y las presenta en un formato preparado para compartir. La principal ventaja es que no necesitas preparar manualmente el documento ni copiar los datos de SonarQube a otro formato.

<img width="90%" src="/img/sonarqube-report/bitegarden-report-pdf.png" alt="Ejemplo de PDF extraido de SonarQube">
<br><br>
 <h2>Cómo exportar bugs, code smells, cobertura y otras métricas a Excel</h2>

Si necesitas trabajar posteriormente con los datos, un documento editable **puede resultar más práctico que un PDF**. El Report Plugin permite crear informes personalizados utilizando plantillas **Open Document (ODT) y Excel**. De esta forma, puedes definir cómo quieres presentar la información y añadir contenido adicional al documento.

Por ejemplo, puedes utilizar una **plantilla corporativa** para añadir:

- Información del proyecto. <br>

- Datos del equipo. <br>

- Observaciones de una revisión. <br>

- Información de auditoría. <br>

- Conclusiones. <br>

- Acciones pendientes. <br>

El plugin recopila **automáticamente las métricas disponibles en SonarQube** y las incorpora a la plantilla. Así puedes pasar de los datos técnicos de SonarQube a un documento que pueda utilizarse en **una revisión interna, auditoría, reunión de proyecto o informe para clientes**.

<h2>Cómo generar un informe detallado de SonarQube</h2>

Si necesitas algo más que un resumen ejecutivo, el informe puede utilizarse para documentar con mayor profundidad el estado de un proyecto. En función del formato seleccionado, puedes incluir información relacionada con:

- **Issues**: bugs, vulnerabilidades y code smells detectados durante el análisis.

- **Seguridad**: información relacionada con vulnerabilidades y hotspots de seguridad.

- **Calidad**: cobertura, duplicación, fiabilidad y mantenibilidad.

- **Quality Gate**: estado del Quality Gate y condiciones evaluadas.

De esta forma, el informe puede servir tanto para una visión rápida del proyecto como para una revisión técnica más detallada.

<h2>¿Y si utilizas SonarQube Cloud?</h2>

Para proyectos analizados con SonarQube Cloud (SonarCloud) existe **Report for SonarQube&trade; Cloud**, una alternativa específica para generar informes sin depender de la interfaz de SonarQube Server. Puedes utilizarlo para generar desde un informe ejecutivo de una sola página, con las métricas principales, hasta un informe más completo con información sobre: Bugs, Vulnerabilidades, Security Hotspots, Code smells, Métricas de calidad y Estado del proyecto.

Además, los informes pueden generarse **desde un pipeline CI/CD**, lo que permite automatizar la creación de documentación después de determinados análisis.

<h2>Generar informes automáticamente desde CI/CD</h2>

Si generar informes forma parte de tu proceso habitual, hacerlo manualmente después de cada análisis puede convertirse en una tarea repetitiva. Report for SonarQube&trade; Cloud puede integrarse opcionalmente en un pipeline CI/CD para automatizar la generación de informes. En el caso de SonarQube Cloud, una vez descargado el producto dispondrás de un fichero .jar ejecutable.

Puedes ubicarlo en tu sistema de ficheros y ejecutarlo con --help para consultar las opciones disponibles. Las propiedades pueden proporcionarse mediante argumentos del sistema utilizando -D o mediante un fichero de configuración personalizado. Esto permite incorporar la generación de informes como un paso más del proceso de integración continua.

 <h2>¿PDF, Excel o un informe personalizado? </h2>

La elección depende de lo que quieras hacer con los resultados:

- **PDF**: ideal para compartir el estado de un proyecto, presentar resultados o generar documentación que no necesite edición.

- **Excel**: útil cuando necesitas trabajar posteriormente con los datos o analizarlos en un formato editable.

- **ODT**: una buena opción cuando quieres utilizar una plantilla y adaptar el documento a las necesidades de tu organización.


<h2>¿Por qué utilizar un plugin para generar informes de SonarQube? </h2>

SonarQube está pensado principalmente para **analizar y visualizar la calidad del código**. Cuando necesitas convertir toda esa información en documentación, hacerlo manualmente puede implicar revisar diferentes pantallas y trasladar los datos a otro documento.

Los Report Plugins de bitegarden automatizan ese proceso. En pocos clics puedes obtener un **informe actualizado** con las métricas de tu proyecto y, cuando lo necesitas, utilizar plantillas personalizadas para adaptarlo a tu propio formato.

Si necesitas exportar **SonarQube a PDF, generar un Excel** con las métricas del proyecto o crear un informe detallado con bugs, code smells, cobertura, duplicaciones y seguridad, los Report Plugins de bitegarden pueden simplificar considerablemente el proceso.

[Aquí puedes descargar](https://marketplace.bitegarden.com/product/bitegardenReport) el Report Plugin for SonarQube&trade; Server y si trabajas con SonarQube Cloud puedes [descargar aquí](https://marketplace.bitegarden.com/product/bitegardenSonarCloudReport) el Report for SonarQube&trade; Cloud. 
