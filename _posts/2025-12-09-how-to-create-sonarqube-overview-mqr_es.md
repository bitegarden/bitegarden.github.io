---
layout: post_es
title: ¿Cómo crear un informe PDF para el nuevo Modo Multi Quality Rule (MQR) de SonarQube?
description: Genera informes PDF en SonarQube con el Overview Report y el nuevo modo MQR.

permalink: como-exportar-informe-sonarqube-overview-mqr
english: how-to-create-sonarqube-overview-mqr


cover: /img/posts/2025-12-09-how-to-create-sonarqube-overview-mqr_es.png
---

SonarQube es una herramienta esencial para el análisis de calidad de código. Con la [versión 3.0](/es/new-sonarqube-overview-version-3) del **Overview Report Plugin for SonarQube Server**, ahora puedes generar informes PDF compatibles con el **modo Multi Quality Rule (MQR)**, que ofrecen una visión más completa de la calidad de tus proyectos.

<h2>¿Qué es el Overview Report for SonarQube Server?</h2>

El **Overview Report Plugin for SonarQube&trade; Server** ayuda a tener una visión agregada de las **métricas de los proyectos**. Con este plugin podrás agrupar distintos proyectos, obteniendo así una mejor perspectiva del estado de calidad del software en la organización.

Este plugin presenta una **interfaz dedicada y navegable** de las distintas agrupaciones de proyectos: agrupando toda la instancia, por grupos personalizados definidos en la configuración o utilizando las etiquetas de proyectos.

<h2>¿Qué es el modo Multi Quality Rule (MQR)?</h2>

El **modo MQR** de SonarQube ofrece una forma más precisa de representar el **impacto de un issue en todas las cualidades del software**, asignando una severidad independiente a cada regla según cada calidad que afecte. Esto permite:

- Tener claro el **impacto de cada issue** en todas las cualidades del software, no solo en la más afectada. <br>

- Evaluar de **forma más completa y objetiva** los problemas de calidad. <br>

<h2>¿Qué significa cada tipo de severidad?</h2>

- **Blocker**: Issue con alta probabilidad de consecuencias graves en la aplicación que debe corregirse inmediatamente (incluye bugs que causan fallos en producción o vulnerabilidades de seguridad críticas). <br>

- **High**: Issue con alto impacto en la aplicación que debe corregirse lo antes posible. <br>

- **Medium**: Issue con impacto medio. <br>

- **Low**: Issue con bajo impacto. <br>

- **Info**: Issue sin impacto esperado; solo para fines informativos.

<h2>Cómo generar un informe PDF desde SonarQube</h2>

Para descargar tu informe, sigue estos pasos:

1. Revisa si tienes activado el MQR. <br>

2. [Instala](/es/sonarqube-overview-trial-form.html) el Overview Report Plugin for SonarQube&trade; Server. <br>

3. Ingresa a tu instancia de SonarQube. Dirígete al menú principal y pulsa sobre 'More'. Si has instalado el plugin correctamente, tendrás distintas pestañas del Overview. <br>

4. Haz clic, por ejemplo, en Overview All Projects y pulsa sobre Descargar PDF. <br>

Aquí tienes un ejemplo del PDF que puedes generar:

<img width="100%" src="/img/sonarqube-overview/sonarqube-overview-modo-mqr-pdf.png" alt="Ejemplo de PDF en Modo MQR de SonarQube con el Overview Report for SonarQube"> <br><br>

El **Overview Report Plugin for SonarQube&trade; Server**, combinado con el modo MQR, permite generar informes en PDF que reflejan con precisión el impacto de los issues en todas las cualidades de tu software. Esto facilita la toma de decisiones, la comunicación del estado de los proyectos y la mejora continua de la calidad de tus desarrollos.

---
**<span style="color: green">bitegarden</span> team**

_Helping companies to develop better software_