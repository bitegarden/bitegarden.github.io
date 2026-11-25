---
layout: post_es
title: 5 plugins para SonarQube con modo oscuro
description: Descubre cinco plugins para SonarQube con modo oscuro de bitegarden. Consulta qué cambia en cada versión y descarga los plugins desde el Marketplace.

permalink: plugins-sonarqube-modo-oscuro
english: plugins-sonarqube-dark-mode

cover: /img/posts/2026-11-10-plugins-sonarqube-dark-mode_es.png

---

Los **plugins para SonarQube Server** de bitegarden que presentamos en este artículo ya se adaptan al tema claro u oscuro que tengas seleccionado en tu cuenta. El cambio se nota al pasar del panel de un proyecto a un tablero de **Quality Gates, al revisar un informe de seguridad o al abrir el gestor de extensiones**. Según el plugin, también se adaptan los selectores, los avisos y los iconos de estado.

Estas son las versiones que incorporan la mejora y los elementos que cambian en cada una. Si vas a **actualizar varios plugins**, puedes usar esta lista para identificar qué pantallas revisar.

<h2>Plugins para revisar la calidad y la seguridad del código</h2>

<h3>Quality Gates Board versión 1.1.5</h3>

Quality Gates Board reúne en un solo tablero varios umbrales de calidad y muestra qué condiciones cumple el proyecto. Por ejemplo, puedes comprobar si una rama satisface tanto los requisitos básicos como los de un nivel de calidad más exigente. Si tienes que [configurar varios umbrales de calidad](https://www.bitegarden.com/nuevo-producto-quality-gates-board-sonarqube), la guía de bitegarden explica dónde definirlos.

Con el **modo oscuro activo, los fondos, los textos, los botones, el selector de ramas y los iconos de estado** siguen el tema de SonarQube. 

<h3>Security Assessment versión 2.36.2</h3>

Security Assessment organiza los hallazgos de SonarQube en informes que puedes consultar durante una revisión de seguridad. Si estás preparando una auditoría, puedes consultar los resultados agrupados según OWASP ASVS o PCI DSS y generar un PDF para compartirlos con tu equipo. La ficha del plugin detalla los [informes disponibles en Security Assessment](https://www.bitegarden.com/es/sonarqube-security).

La **versión 2.36.2 adapta todos los informes** en pantalla al modo oscuro, incluidos OWASP, CWE, CWE KEV, ASVS, CASA, PCI DSS, ISO 5055 y STIG. El tema se aplica a las tablas, los gráficos, los botones, los desplegables y las ayudas emergentes. La ventana de progreso que ves al descargar un PDF también sigue el tema activo.

Para consultar los informes con el tema oscuro, [descarga Security Assessment](https://marketplace.bitegarden.com/download/download-form/52) desde el Marketplace.

<h3>Dependency Track versión 1.1</h3>

Dependency Track permite consultar **desde el proyecto de SonarQube las vulnerabilidades** detectadas en sus dependencias. Puedes empezar por el resumen de componentes y vulnerabilidades y, a continuación, revisar el desglose por gravedad para decidir qué incidencias examinar primero. La documentación explica cómo [configurar la conexión con Dependency Track](https://www.bitegarden.com/es/sonarqube-dependency-track-documentation).

La versión 1.1 adapta al tema oscuro las tablas, el selector de versiones, los avisos y las ayudas emergentes. Para probar la vista adaptada al tema oscuro, [descarga Dependency Track 1.1](https://marketplace.bitegarden.com/download/download-form/61?selectedVersion=1.1).

<h2>Plugins para administrar proyectos y extensiones en SonarQube</h2>

<h3>Project Tag desde la versión 1.3.6</h3>

Project Tag permite **asignar una etiqueta durante el análisis** mediante una propiedad del escáner. Si tus proyectos ya tienen metadatos en el pipeline, puedes aprovecharlos para etiquetarlos por equipo o aplicación y encontrarlos después en SonarQube.

Desde la versión 1.3.6, los **textos, enlaces, botones y demás elementos de la página del plugin** se adaptan al tema del usuario. Los mensajes de éxito o error que aparecen al actualizar etiquetas usan los colores del tema elegido. La versión 1.3.7 también incluye esta compatibilidad.

Si gestionas etiquetas desde esta vista, [descarga Project Tag 1.3.7](https://marketplace.bitegarden.com/download/download-form/58?selectedVersion=1.3.7).

<h3>Universal Plugin Manager (UPM) versión 1.7.5</h3>

UPM permite **instalar y actualizar plugins** desde la administración de SonarQube Server. Puedes consultar el catálogo de bitegarden desde tu instancia o subir un archivo JAR si necesitas instalar una extensión personalizada.

La versión 1.7.5 adapta los fondos, botones, avisos, enlaces e iconos de licencia al modo oscuro. Si quieres gestionar tus extensiones desde SonarQube, [descarga Universal Plugin Manager](https://marketplace.bitegarden.com/download/download-form/59).


<h2> Cómo comprobar el modo oscuro después de actualizar</h2>

1. Comprueba en la ficha del Marketplace qué versión del plugin es compatible con tu instancia de SonarQube Server.
2. Instala o actualiza el plugin y selecciona el tema oscuro en tu cuenta de SonarQube.
3. Abre la vista que usas normalmente. Por ejemplo, cambia de rama en Quality Gates Board o abre un informe en Security Assessment para ver cómo se adaptan los controles al tema elegido.

Puedes **volver al tema claro desde tu cuenta**. Los cinco plugins siguen esa preferencia automáticamente.

Si una pantalla conserva el aspecto anterior, comprueba primero la versión instalada y el tema activo en tu cuenta. Verifica que estás viendo la página del plugin dentro de SonarQube. En Security Assessment, por ejemplo, la mejora descrita se aprecia al abrir un informe en pantalla o al iniciar la descarga del PDF.

---

**<span style="color: green">bitegarden</span> team**

_Helping companies to develop better software_