---
layout: post_es
title:  ¡Nueva versión del Overview Report for SonarQube™ Server ya disponible!
description: Incluimos soporte para reportes en el Modo MQR

permalink: nuevo-sonarqube-overview-version-3
english: new-sonarqube-overview-version-3
cover: /img/posts/2025-08-20-new-sonarqube-overview-version-3_es.png
---

## Novedades principales de la nueva versión
En bitegarden hemos publicado la versión del plugin **Overview Report for SonarQube Server 3.0**. Esta actualización incluye soporte para reportes en **Modo MQR (Multi-Quality Rule)**, lo que abre la puerta a una visualización mucho más completa de la calidad de los proyectos.

#### Modo MQR
Si tu instancia está en Modo MQR, el plugin lo reconoce de inmediato y muestra los reportes bajo ese formato.

<img width="100%" src="/img/sonarqube-overview/sonarqube-overview-modo-mqr.png" alt="Overview All projects Modo MQR">

*Imagen de la página Overview All Projects con el Modo MQR activado*
<br>

#### Standard Experience
Si tu instancia está en Standard Experience, los reportes se mostrarán en este modo por defecto.

<img width="100%" src="/img/sonarqube-overview/sonarqube-overview-modo-standard.png" alt="Overview All projects Modo Standard">

*Imagen de la página Overview All Projects con el Modo Standard activado*
<br>

### Opción para forzar el modo Standard
Una de las novedades más útiles es la posibilidad de forzar el modo Standard incluso cuando tu instancia está configurada en MQR. Esta opción se encuentra en la configuración del plugin, pensada para usuarios que prefieren mantener la vista tradicional.

## Casos de uso: ¿cuándo conviene cada modo?

### Cuando usar MQR
El Modo MQR es ideal si tu organización ya trabaja con métricas de calidad avanzadas y quieres reportes alineados con esa configuración.

### Cuando usar Standard Experience
El Standard Experience sigue siendo la mejor opción si prefieres reportes más simples y directos, o si tu equipo aún no utiliza MQR como estándar.

## Cómo actualizar el plugin Overview Report
Si tienes el [Universal Plugin Manager for SonarQube Server™ (UPM)](//marketplace.bitegarden.com/product/bitegardenUniversalPluginManager) simplemente tendrás que darle al botón de actualizar en la administración de tu instancia.

---
**<span style="color: green">bitegarden</span> team**

_Helping companies to develop better software_