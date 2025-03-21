---
layout: post_es
title: ¿Cómo crear un informe de seguridad en SonarQube?
description: Aprende a generar un informe en PDF sobre el estado de tu código basado en los estándares de seguridad.

permalink: como-crear-informe-seguridad-sonarqube
english: how-to-create-soanrqube-security-report


cover: /img/posts/2025-03-14-how to-create-sonarqube-security-report_es.png
---

Si quieres **obtener informes de estándares de seguridad** de tu código te lo vamos a poner fácil. ¡Solo tienes que instalarte un plugin! El equipo de bitegarden ha desarrollado el Security Plugin for SonarQube&trade; Server, que te permite obtener este tipo de informes que necesitas para mantener la seguridad y calidad de tu código. En este artículo, te explicamos cómo funciona. 

<h2>Paso 1: Descargar el Security Plugin for SonarQube&trade;</h2>

Lo primero que tienes que hacer es **descargar el Security Plugin for SonarQube&trade; Server** a través de [este enlace](/es/sonarqube-security){:target="_blank"}. Por si no lo conoces, se trata de nuestro producto que añade una nueva página en los proyectos de SonarQube donde podrás ver y gestionar la información relativa a las vulnerabilidades y envidencias clasificadas en los estándares: OWASP TOP 10, CWE SANS Top 25 y OWASP ASVS. 

Tienes una **versión gratuita de 14 días** para que veas cómo funciona este producto en tu instancia. También tenemos este mismo producto para SonarQube Cloud, que lo puedes descargar a través de [este enlace](/es/sonarcloud-security){:target="_blank"}

<h2>Paso 2: Generar los informes</h2>

Aquí ya debes tener instalado el plugin. Entra en el proyecto de SonarQube Server que quieras. Si clicas en la pestaña 'More' se te abrirá un desplegable que incluirá los siguientes informes de seguridad: 

- Security Assessment OWASP ASVS. <br>

- Security Assessment CWE TOP 25 ON THE CUSP. <br>

- Security Assessment CWE TOP 25. <br>

- Security Assessment ISO 5055. <br>

- Security Assessment OWASP TOP 10. <br>

Aquí puedes ver una imagen del lugar donde se encuentran estas opciones: 

<img width="100%" src="/img/sonarqube-security/security-plugin-sonarqube.png" alt="Report image of the Security Plugin for SonarQube Server">
<br>


Pulsa sobre cualquiera de ellos y se te abrirá una nueva página con el análisis de la información de ese estándar de seguridad. Aquí, simplemente tendrás que pulsar sobre el botón 'Download as PDF' para obtener el informe. 

Y hasta aquí este rápido tutorial. Si te interesa, tenemos disponible una oferta del **20% de descuento para el Pack Premium bitegarden**, que incluye todos los productos para SonarQube Server. Puedes aprovechar esta oferta a través de la página de [descarga de productos](https://www.bitegarden.com/es/products/){:target="_blank"}

---
**<span style="color: green">bitegarden</span> team**

_Helping companies to develop better software_