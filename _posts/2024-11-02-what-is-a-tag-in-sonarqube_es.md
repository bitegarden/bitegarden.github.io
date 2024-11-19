---
layout: post_es
title: Tags en SonarQube, uso y utilidades en los proyectos
description: Aprende a utilizar los tags en SonarQube y cómo te pueden ayudar nuestros productos a mejorar su gestión

permalink: que-es-un-tag-en-sonarqube
english: what-is-a-tag-in-sonarqube


cover: /img/posts/2024-11-02-what-is-a-tag-in-sonarqube_ES.png
---

Las **etiquetas o tags de SonarQube** son una herramienta bastante útil para gestionar y encontrar los proyectos de tu organización. Así que en este artículo vamos a explicarte cómo puedes utilizarlos y cómo puedes ampliar sus funcionalidades gracias a los productos de bitegarden. 

<h2>¿Qué es un tag en SonarQube?</h2>

Las **tags en SonarQube** son etiquetas que se añaden en los proyectos y que permiten categorizarlos para facilitar su administración. Los tags se pueden gestionar a través de la pestaña 'Project Information' en la barra lateral izquierda. En la sección 'tags' aparecen las etiquetas configuradas de ese proyecto y la opción para añadir más. 

En esta imagen puedes ver un ejemplo de su localización: 

<img src="/img/sonarqube-project-tag/tags-project-sonarqube.png" alt="Tags in SonarQube" width="100%" />
<br/>
<br/>


<h2>¿Cómo añadir tags a un proyecto de SonarQube?</h2>

En esta misma pestaña, clicando sobre el botón '+' podrás **añadir más etiquetas o crear nuevas** si no están ya creadas. Es una forma sencilla e intuitiva de clasificar proyectos para, posteriormente, encontrarlos según los criterios que desees. 

Sin embargo, cuando el usuario desea crear etiquetas cuando hay muchos proyectos, se encuentra ante un problema. La acción de crear y asignar etiquetas es totalmente manual, pero en bitegarden tenemos **dos productos** que te pueden ayudar durante la gestión y configuración de etiquetas. 

Con **Project Tag for SonarQube**, podrás configurar y etiquetar proyectos de forma automática. Por su parte, con el **Control Center for SonarQube** podrás asignar etiquetas a proyectos de forma masiva. Vamos paso por paso aprendiendo cómo realizar estas acciones. 

<h2>¿Cómo automatizar la configuración de tags en SonarQube?</h2>

A continuación, te explicamos paso a paso **cómo puedes automatizar** la creación de etiquetas en SonarQube: 

1 - Escribe el tag a través de la propiedad "-Dbitegarden.project.tag=YOUR_TAG" en cualquiera de tus scanners y el plugin captará la información y la guardará en SonarQube.
<br>

2 - Una vez que tus proyectos han sido analizados usando la propiedad, puedes lanzar el proceso que etiquetará los proyectos. En concreto, tienes que ir a Administration -> Configuration -> Project Tag y pulsar sobre el botón 'Update project tags'.
<br>


<img src="/img/sonarqube-project-tag/project-tag-administration.png" alt="Tags in SonarQube" width="90%"/>

Si quieres probar en tu instancia este plugin, puedes descargarlo a través de [este enlace](/es/sonarqube-project-tag#product-block-center)


<h2>¿Cómo etiquetar proyectos de forma masiva en SonarQube?</h2>

Si tu objetivo es etiquetar los proyectos de forma masiva deberás seguir los siguientes pasos en SonarQube: 

1 - Dirígete a Administration -> Configuration -> Control Center - Project Management

2 - En la pantalla te aparecerán todos los proyectos. Es entonces cuando debes seleccionar qué proyectos quieres etiquetar.

3 - Pulsa el botón Bulk Actions -> Bulk Apply Tags y selecciona los tags que quieres añadir a los poryectos seleccionados.


<img src="/img/sonarqube-control-center\control-center-add-tags.png" alt="Tags in Control Center for SonarQube" width="90%"/>


Si quieres probar en tu instancia este plugin, puedes descargarlo a través de [este enlace](/es/sonarqube-control-center#product-block-center)

Si tienes alguna pregunta o quieres ampliar la información de nuestros productos, no dudes en ponerte en contacto con nuestro equipo. 

---
**<span style="color: green">bitegarden</span> team**

_Helping companies to develop better software_