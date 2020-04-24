---
layout: post_es
title: Cómo detectar vulnerabilidades en tu código
description: These last weeks have been challenging, we've all changed our habits as well as the companies. Remote work is here to stay and, probably even after the emergency. 

english: how-to-detect-vulnerabilities-in-your-code
permalink: como-detectar-vulnerabilidades-en-el-codigo
---

SonarQube™ se ha convertido en la herramienta de inspección continua y análisis estático por excelencia. 

Desde hace un par de años el equipo de desarrollo se ha centrado en mejorar todas aquellas características de análisis
asociadas a la detección de vulnerabilidades y a los diferentes estándares de seguridad, incluyendo OWASP, SNAS, CWE, ... 
de forma que en estos momentos ya podemos decir que [SonarQube™ es una herramienta SAST](https://www.sonarqube.org/features/security/) 
(Static Application Security Testing). 

Además, si complementamos la herramienta con otros componentes Open Source como 
[OWASP Dependency Check](https://owasp.org/www-project-dependency-check/), o con [nuestro plugin de
seguridad](/sonarqube-security) aumentaremos aún más su capacidad a través de análisis de vulnerabilidades en 
componentes (Software Composition Analysis, SCA) o nuevos informes de cumplimiento de estándares. También puedes aumentar
el conjunto de reglas de seguridad disponible a través de herramientas como [Find Security Bugs](https://find-sec-bugs.github.io)
usando el plugin [sonar-findbugs](https://github.com/spotbugs/sonar-findbugs).

Pero más allá de todo esto, ¿cómo detectamos vulnerabilidades en el código con SonarQube™?

## **Evidencias de seguridad:** Hotspots vs Vulnerabilidades

SonarQube™ diferencia dos tipos de evidencias relacionadas con la seguridad.

La principal diferencia es la **necesidad de una revisión** antes de decidir si se necesita aplicar una solución:

![Vulnerabilidades vs Hotspots](/img/posts/hotspots-vulnerabilities.png){:width="100%" .center-image}

-- En un **Hostspot**, se detecta un trozo de código que es sensible a la seguridad, pero la seguridad de la aplicación 
puede no verse afectada. Es responsabilidad del desarrollador revisar el código para determinar si se requiere un cambio o 
no.

-- En una **vulnerabilidad**, se detecta un problema que impacta en la seguridad de la aplicación, y que tiene que ser
solucionado inmediatamente.

## **Paso 1.** Activa las reglas de seguridad

Si quieres hacer una primera revisión "a lo grande" de la seguridad de tu código, lo primero será configurar tu perfil
de calidad para detectar el mayor número posible de problemas.

Este es el perfil de calidad por defecto: 

![Reglas por defecto](/img/posts/default-security-rules.png){:width="300px" .center-image}

Dispone de 45 reglas de tipo **vulnerabilidad** y otras 31 reglas de tipo **hostspots**. 

Pero aún podéis activar casi 20 reglas más asociadas a seguridad. El perfil por defecto suele ser suficiente pero si 
quieres probar con todas activadas, adelante.

---
> **Consejo:** algunas reglas de tipo bug y code smells también están 
> categorizadas en estándares de seguridad. Búscalas y actívalas para mejorar el análisis de seguridad de tu código-.
>
> Aquí tienes un ejemplo de una regla de tipo **bug** que afecta al estándar OWASP (categoría A6):

![Bug que afecta a seguridad](/img/posts/bug-security-rule.png){:width="100%" .center-image}

> Por eso es importante que no solo te quedes con las evidencias de tipo vulnerabilidad y hotspot, sino que también vayas
> un poco más allá, puesto que algunos bugs o code smells pueden también estar relacionados con futuros problemas de seguridad.

---

## **Paso 2.** Revisa la calificación de seguridad

Una vez analizado tu proyecto, puedes ver tu calificación de seguridad en la página principal:


![calificación de seguridad](/img/posts/overall-security-rating.png){:width="100%" .center-image}

Existe una calificación de seguridad para vulnerabilidades y otra para los hotspots. 

-- En el caso de las vulnerabilidades se calcula teniendo en cuenta la severidad de las vulnerabilidades detectadas.
 
-- En el caso de los hotspots se calcula según el número de hotspots que están pendientes de revisión.

Desde aquí ya puedes empezar a solucionar los problemas de seguridad del código navegando por todas las evidencias 
detectadas. Esto está muy bien para un desarrollador, ¿pero que pasa con un responsable de seguridad o un gestor que no
va a cambiar el código? En ese caso la información que le interesa es más ejecutiva.

## **Paso 3.** Revisa el cumplimiento de estándares

Además de la calificación global, si tienes instalado el plugin [bitegarden Security](/sonarqube-security) también podrás
comprobar el cumplimiento de estándares y algunas métricas adicionales en una sección dedicada dentro del proyecto. 

Esta sección es más "amigable" que estar navegando por todos las evidencias y permite analizar la seguridad de tu código 
desde un punto de vista menos técnico:

![informe cumplimiento](/img/posts/bitegarden-security-owasp-page.png){:width="60%" .center-image}

Con esta información no solo puedes conocer mejor que aspectos de seguridad están mejor o peor en el proyecto, sino que
también puedes decidir que vulnerabilidades del código resolver primero en función de las categorías y de la criticidad.

Por ejemplo, podría interesarte más empezar a resolver problemas de inyección de código antes que problemas de configuración.

## **Paso 4.** Genera un informe en PDF

Por último, si necesitas publicar la información o hacersela llegar a otras personas que no están en el equipo, puedes 
exportar toda la información en PDF con [nuestro plugin](/sonarqube-security) y de esa forma que todo el mundo pueda ver
 como de seguro es tu código:

![informe-owasp-pagina-1](/img/posts/owasp-report-page-1.png){:width="45%"} ![informe-owasp-pagina-2](/img/posts/owasp-report-page-2.png){:width="45%"}

---

## Conclusiones

SonarQube™ ha mejorado su [motor de seguridad](https://blog.sonarsource.com/what-is-taint-analysis) y ya juega en la misma 
liga que otras herramientas más especializadas. Empieza a revisar todos los problemas de seguridad en tu código:

1. Activando las reglas que detectan vulnerabilidades y hotspots
2. Revisando la calificación de seguridad global de tu proyecto
3. Revisando el cumplimiento de estándares de seguridad
4. Compartiendo la información con otros equipos a través de informes en PDF

Prueba [bitegarden Security](/sonarqube-security) para mejorar la forma en que detectas y solucionas las vulnerabilidades
de tu código:

<a href="/es/sonarqube-security-trial-form" class="btn btn-primary btn-call-to-action fancybox">DESCARGA AHORA ></a>

---
**<span style="color: green">bitegarden</span> team**

_Helping companies to develop better software_





