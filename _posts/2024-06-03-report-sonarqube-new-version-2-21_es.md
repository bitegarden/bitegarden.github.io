---
layout: post_es
title: '¡Nueva versión! Report Plugin Para SonarQube 2.21'
description: Nuevos campos en los reportes y nuevo endpoint!

permalink: report-sonarqube-nueva-version-2-21
english: report-sonarqube-new-version-2-21
italian: report-sonarqube-nuova-versione-2-21

cover: /img/posts/2024-06-03-bitegarden-report-new-version-2-21_ES.png
---

Tenemos nueva versión del [Report Plugin for SonarQube](/sonarqube-report). Se trata de la **versión 2.21** que trae varias novedades!

Esta versión añade algunos campos nuevos a los reportes, como nos habiais pedido. A partir de ahora, se podrá ver: 

- **Líneas de código**: Ahora se puede visualizar el número total de líneas de código analizadas.
- **Fecha de descarga**: Se ha añadido la fecha en que se descargó el reporte.
- **Versión de SonarQube**: Los reportes ahora incluyen la versión de SonarQube utilizada para el análisis.

<br/>

## Mejora en la Notificación de Correos

Anteriormente, el plugin permitía configurar una lista de correos para que fueran notificados después de cada análisis. Sin embargo, esto estaba generando problemas para algunos clientes y afectaba los tiempos del análisis al darle más trabajo al compute engine.

#### Solución Implementada

En esta versión, se ha incluido un endpoint que permite notificar a los usuarios deseados enviando el listado de correos. De esta forma, el envío de notificaciones ya no se ejecuta en el compute engine, mejorando así el rendimiento y reduciendo los problemas reportados.

<img src="/img/sonarqube-report/bitegarden-report-sonarqube-email-endpoint.png" width="100%" alt="endpoint">

#### Advertencia

Por tanto, al tener un endpoint para ello, se ha marcado como "deprecated" la funcionalidad anterior para solo quedarnos con el nuevo endpoint. Se eliminará en siguientes versiones. 

## Parche Aplicado

Se ha implementado un pequeño parche para resolver el problema de cruce de correos entre diferentes proyectos cuando existían más de un worker configurado en el compute engine. Esta mejora asegura que las notificaciones se envíen correctamente sin mezclar destinatarios entre proyectos distintos.

<br />

## Descarga la nueva versión

Esta nueva versión del **Security Plugin** ya está disponible para descarga a través del [Universal Plugin Manager](/es/sonarqube-upm) o desde la página de [descarga del producto](/es/sonarqube-report-trial-form).

Recuerda, si todavía no tienes este plugin puedes **descargarlo y probarlo de forma gratuita**. 

<a href = "/es/sonarqube-report#product-block-center" class = "btn btn-primary btn-call-to-action fancybox" style = "font-weight: bold; font-size: 16px; text-transform : mayúsculas; ">Prueba gratuita > </a>

---
**<span style="color: green">bitegarden</span> team**

_Helping companies to develop better software_