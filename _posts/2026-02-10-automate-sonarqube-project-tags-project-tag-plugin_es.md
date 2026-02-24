---
layout: post_es
title: Cómo automatizar el etiquetado de proyectos con Project Tag for SonarQube™
description: Automatiza el etiquetado de proyectos en SonarQube con Project Tag de bitegarden y mantén consistencia en CI/CD sin gestión manual.

permalink: automatizar-etiquetas-proyectos-sonarqube-plugin-project-tag
english: automate-sonarqube-project-tags-project-tag-plugin

cover: /img/posts/2026-02-10-automate-sonarqube-project-tags-project-tag-plugin_es.png
---

¿Alguna vez has intentado **automatizar el on-boarding** de proyectos en SonarQube usando etiquetas? Si trabajas con múltiples proyectos, sabes lo complicado que puede ser mantener todo organizado manualmente. SonarQube permite gestionar etiquetas en el espacio de proyectos, pero hasta ahora, crear nuevas etiquetas solo era posible de **forma manual**. Aquí es donde entra Project Tag for SonarQube&trade;, el plugin de bitegarden que simplifica este proceso de forma automática y eficiente.

<h2>Por qué automatizar el etiquetado de proyectos</h2>

La gestión manual de etiquetas se vuelve complicada cuando:

- Tienes **cientos de proyectos**.

- Quieres **mantener un estándar de etiquetado** consistente.

- Necesitas **usar metadatos de proyectos** durante el análisis de CI/CD (por ejemplo, en Jenkins).

Con **Project Tag for SonarQube&trade;**, solo necesitas proporcionar la etiqueta como propiedad de línea de comando, y el plugin se encargará de **crear y asignar la etiqueta automáticamente**, manteniendo tanto las etiquetas del sistema como las personalizadas.

<h2>Uso y configuración</h2>

**1 - Especifica la etiqueta en tu análisis**

Añade la siguiente propiedad a tu scanner de SonarQube:

```
-Dbitegarden.project.tag=yourtag
```

**yourtag**: reemplázalo con el nombre de la etiqueta que quieras asignar.

Asegúrate de que los caracteres cumplan las reglas de SonarQube™: a-z, 0-9, '+', '-', '#', '.'.

El **plugin captará automáticamente** esta información y la guardará en SonarQube.
<br><br>

**2 - Lanza el proceso de etiquetado en la administración**

Una vez que tus proyectos hayan sido analizados usando la propiedad de línea de comando:

Ve a **Administration → Configuration → Project Tag.**

Lanza el proceso para etiquetar todos los proyectos.

El plugin se encargará de asignar la etiqueta indicada durante el análisis, sin eliminar etiquetas existentes. Esto significa que tanto las etiquetas del sistema como las personalizadas se conservarán intactas.
<br><br>

**3 - Integración con CI/CD**

Si ya tienes **metadatos del proyecto** (por ejemplo, nombre del equipo, tipo de proyecto o cliente), puedes usar estos datos para configurar automáticamente la etiqueta durante el análisis en tu herramienta de CI/CD como Jenkins, GitLab CI o Azure DevOps. Esto garantiza que cada **proyecto tenga la etiqueta correcta** lo antes posible, sin intervención manual.

<h3>Beneficios clave</h3>

A continuación, te nombramos algunos beneficios que aporta el Project Tag for SonarQube&trade; Server:

- **Automatización completa**: no más creación manual de etiquetas.

- **Consistencia**: todas las etiquetas siguen un estándar definido por tu análisis.

- **Compatibilidad con metadatos de CI/CD**: las etiquetas se pueden generar a partir de propiedades dinámicas de tu pipeline.

- **Seguridad y mantenimiento**: no se eliminan etiquetas existentes, solo se agregan nuevas.

Con **Project Tag for SonarQube&trade; de bitegarden**, automatizar el etiquetado de tus proyectos es muy sencillo sencillo. Configura tus etiquetas en la línea de comando, intégralas con tu pipeline de CI/CD y deja que el plugin se encargue de mantener tus proyectos organizados y consistentes. [Aquí](https://marketplace.bitegarden.com/product/bitegardenProjectTag) tienes el enlace de descarga para probarlo en tu instancia. 

---

**<span style="color: green">bitegarden</span> team**

_Helping companies to develop better software_