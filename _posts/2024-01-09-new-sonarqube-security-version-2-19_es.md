---
layout: post_es
title: Nueva versión! Security Plugin for SonarQube 2.19
description: La sección ISO 5055 del Security Plugin de SonarQube ahora incluye el desglose de CWE aprobados y no soportados.

permalink: nueva-version-sonarqube-security-2-19
english: new-version-sonarqube-security-2-19
italian: nuova-versione-sonarqube-security-2-19

cover: /img/posts/2024-01-09-new-version-sonarqube_ES.png
---

Lanzamos la versión 2.19 del [Security Plugin for SonarQube](sonarqube-security). Esta actualización trae consigo una nueva funcionalidad que permite mostrar los **CWE Not Supported** y **Passed** como desglose, para darte más información sobre el estado de tu código.

A continuación puedes ver una imagen donde aparecen las nuevas columnas de **Passed** y **Not Supported** en el área de **Security**.

<img src="/img/sonarqube-security/2024-01-09-new-version-sonarqube-security-iso5055-table.png" alt="New breakdown table" width="100%" />
<br >

Además, ahora tienes la  posibilidad de **activar o desactivar** los CWE **No Pasados** cuando generes el Informe ISO 5055 en PDF. Te adjuntamos una imagen para que lo puedas ver: 

<div style="width: 100%; display: flex; flex-direction: row; justify-content: center">
<img src="/img/sonarqube-security/2024-01-09-iso5055-disable-not-supported-cwe.png" alt="Disable ISO5055 Not Supported CWE Option" width="50%">
</div>

A parte, hemos añadido un **enlace directo al proyecto** en el correo electrónico que recibas cuando se realiza un análisis en SonarQube. 

<div style="width: 100%; display: flex; flex-direction: row; justify-content: center">
<img src="/img/sonarqube-security/2024-01-09-new-email-version.png" alt="New Security Plugin Email version" width="70%">
</div>

## Video sobre esta nueva funcionalidad

Aquí te dejamos un video sobre las nuevas funcionalidades de la nueva versión del **Security Plugin de SonarQube**:

<iframe width="560" height="315" src="https://www.youtube.com/embed/Hh8z8Jfdxtw?si=eor1LnbY8H78Sncx" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

## Sobre la ISO 5055

Los **estándares internacionales** garantizan que los productos y servicios que utiliza a diario son **seguros, fiables y de alta calidad**. Si desea más información, puedes visitar la página oficial [ISO 5055](https://www.iso.org/standard/80623.html)


## Descarga la nueva versión

Security Plugin para SonarQube 2.19 ya está disponible para descarga a través del [Universal Plugin Manager](/es/sonarqube-upm)  o desde la página de [descarga del producto](/es/sonarqube-security-trial-form).

Si todavía no has probado este plugin, recuerda que puedes hacerlo de **forma gratuita** a través de este botón.

<a href = "/sonarqube-security#product-block-center" class = "btn btn-primary btn-call-to-action fancybox" style = "font-weight: bold; font-size: 16px; text-transform : mayúsculas; "> Prueba gratuita > </a>

---
**<span style="color: green">bitegarden</span> team**

_Helping companies to develop better software_