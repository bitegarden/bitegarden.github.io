---
layout: post_es
title: '¿Es SonarQube una herramienta segura?'
description: Te explicamos por qué con SonarQube vas a entregar código seguro de forma segura. 

permalink: sonarqube-herramienta-segura
english: is-sonarQube-security-tool
italian: sonarqube-uno-strumento-sicuro

cover: /img/posts/2023-10-20-is-sonarqube-security-tool.png
---
 
En este artículo damos algunas razones por las que consideramos que **SonarQube es una buena herramienta para entregar código seguro de forma segura**. Esta solución de Sonar no solo se encarga de enseñarte cómo debes entregar código de calidad, sino que también te permite hacerlo siguiendo los estándares de seguridad. 

### Entrega código seguro con SonarQube

SonarQube detecta los siguientes problemas a partir de unas reglas basadas en estándares y buenas prácticas de codificación: **bugs, vulnerabilidades, code smells y hotsposts**. Es en este último problema en el que vamos a profundizar. 

<h2>¿Qué son los hotspots?</h2>

Los hotspots son fragmentos de código que señalan un posible riesgo de seguridad. Estos fragmentos **deben ser revisados para confirmar o descartar el riesgo**.

> Visualicemos un ejemplo de hotspot: SonarQube destaca la regla *'PASSWORD' detected in this expression, review this potentially hard-coded password*. En el fragmento de código vemos un mensaje que nos está explicando que se ha detectado un string y que, por el contexto, SonarQube cree que es un password. 

<img src="/img/posts/sonarqube-hotspots.png" width="90%" alt="Hotspots en SonarQube">


La detección y análisis de estos hotspots es esencial para mejorar y asegurar la calidad del código. Revisar los hotspots detectados permite comprender un posible riesgo, identificar posibles soluciones y cómo aplicar cambios para proteger el código.
<br>

Por otro lado, cabe destacar que el **equipo de bitegarden** ha desarrollado un plugin que muestra una lista de vulnerabilidades detectadas en SonarQube permitiendo conocer el cumplimiento de seguridad de todo el proyecto de **forma visual y detallada**. Este plugin se llama Security Plugin for SonarQube y lo puedes probar a través de [este enlace](https://www.bitegarden.com/es/sonarqube-security#product-block-center). 

Con respecto al punto del que estábamos hablando de los hotsposts, con este plugin podrás encontrar todas **tus evidencias de OWASP** (tanto vulnerabilidades como hotspots de seguridad) en una sola página ordenadas por severidad. Adjuntamos una captura de pantalla para que la puedes ver:

<img src="/img/sonarqube-security/security-owasp-vulnerabilities.png" width="90%" alt="Security Plugin para SonarQube">


### Entrega código de forma segura con SonarQube

Desde la versión de **SonarQube 8.9 LTS** trabajar con esta solución es aún más seguro, porque han añadido nuevas funcionalidades que refuerzan la seguridad de tu trabajo. Ejemplo de ello son las siguientes características: 

1 - La acción de cambiar las credenciales de administrador pasan a ser obligatoria.<br>
2 - Está por determinado el acceso autenticado.<br>
3 - Acceso limitado complementos para que los plugins de terceros no afecten a la instalación.<br>
4 - Refuerzo por parte de Sonar a su propio proceso de compilación. <br>

Si quieres más información sobre la seguridad de Sonar o nuestros plugins, no dudes en enviarnos tus consultas. 

---
**<span style="color: green">bitegarden</span> team**

_Helping companies to develop better software_