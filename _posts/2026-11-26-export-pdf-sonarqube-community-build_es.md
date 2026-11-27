---
layout: post_es
title: Cómo exportar un PDF desde SonarQube Community Build
description: Extrae métricas de tu proyecto con la Web API o descarga un PDF con el plugin de bitegarden. Compara las dos opciones y consulta un informe de ejemplo.

permalink: exportar-pdf-sonarqube-community-build
english: export-pdf-sonarqube-community-build

cover: /img/posts/2026-11-26-export-pdf-sonarqube-community-build_es.png

---

Con el [plugin de informes de bitegarden](https://marketplace.bitegarden.com/product/bitegardenReport) puedes descargar un PDF desde tu proyecto en **SonarQube Community Build**. Puedes elegir un resumen ejecutivo para compartir el estado del proyecto o un informe con el desglose de incidencias para revisar los hallazgos con tu equipo.

Los [informes nativos en PDF de Sonar](https://docs.sonarsource.com/sonarqube-server/user-guide/viewing-reports/pdf-reports) están disponibles a partir de **SonarQube Server Enterprise Edition** y se centran principalmente en el código nuevo y en las condiciones del Quality Gate. En Community Build también puedes extraer las métricas con la Web API y preparar tu propio PDF.

<h2>Cómo preparar un informe con la Web API</h2>

Esta opción te sirve si necesitas unas pocas métricas para revisar una entrega o ya tienes una plantilla de informes. La API devuelve los datos en JSON. Tú eliges qué métricas incluir y cómo presentarlas en el PDF.

1. Ejecuta un análisis y localiza la clave del proyecto en SonarQube. Crea un token de usuario con acceso al proyecto y guárdalo en la variable de entorno `SONAR_TOKEN` de tu terminal.
2. Consulta las métricas que quieras compartir. El comando de ejemplo solicita la cobertura, el porcentaje de líneas duplicadas y las líneas de código de WebGoat. Sustituye la URL y la clave por las de tu instancia. Consulta la [documentación de la Web API](https://docs.sonarsource.com/sonarqube-community-build/extension-guide/web-api) para comprobar cómo autenticarte y qué endpoints admite tu versión.

```bash
curl --fail --silent --show-error --get \
  --header "Authorization: Bearer ${SONAR_TOKEN}" \
  --data-urlencode 'component=org.owasp.webgoat:webgoat' \
  --data-urlencode 'metricKeys=coverage,duplicated_lines_density,ncloc' \
  --output sonarqube-metrics.json \
  'https://sonarqube.example.com/api/measures/component'
```

Abre `sonarqube-metrics.json` y busca `component.measures`. Pasa los valores que necesites a una hoja de cálculo o a una plantilla, añade el nombre del proyecto y la fecha del análisis, y exporta el documento a PDF. Si preparas el mismo informe a menudo, puedes usar esa consulta para alimentar una plantilla o tu herramienta de informes.

<h2>Cómo descargar un PDF con el plugin de bitegarden</h2>

Antes de instalar el plugin, comprueba en la ficha del marketplace qué versión es compatible con tu instalación de Community Build.

1. Descarga la versión compatible del plugin y sigue la [guía de instalación y configuración](/es/sonarqube-report-documentation).
2. Abre un proyecto que ya hayas analizado y ve a **More > Reporting**.
3. Descarga el **resumen ejecutivo en PDF** para revisar el estado del proyecto de un vistazo. Si necesitas revisar los hallazgos, elige un informe con el desglose de incidencias.

Descarga el [informe ejecutivo de ejemplo de WebGoat (PDF)](/pdf/sonarqube-sample-executive-report-webgoat.pdf) para ver cómo presenta bitegarden las métricas del proyecto en un documento que puedes compartir.

[Prueba el plugin gratis durante 14 días](https://marketplace.bitegarden.com/download/download-form/55){: .btn .btn-primary .btn-call-to-action}

<h2>Qué opción elegir para tu proyecto</h2>

| Qué necesitas | Por dónde empezar |
| --- | --- |
| Unas métricas para una hoja de cálculo o una plantilla interna | Usa la Web API y exporta el documento a PDF cuando esté listo. |
| Un PDF desde el proyecto para una revisión o una entrega | Usa el plugin de bitegarden y elige el nivel de detalle. |
| Un PDF integrado y ya tienes Enterprise Edition | Revisa qué incluye el informe nativo para tu proyecto. |

<br>

Si también necesitas un archivo editable, consulta la [guía para exportar informes a PDF y Excel](/exportar-informes-sonarqube-pdf-excel).

---
**<span style="color: green">bitegarden</span> team**

_Helping companies to develop better software_
