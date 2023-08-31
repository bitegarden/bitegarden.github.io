---
layout: post_es
title: Cómo medir la calidad del código realizado por un proveedor
description: Cómo verificar los objetivos y las métricas cuando trabajas con una empresa externa

permalink: como-medir-calidad-de-codigo-proveedores
english: how-to-measure-code-quality-suppliers
cover: /img/thumbs/2021-07-20-how-to-measure-the-code-quality-suppliers-thumb.png
---

Para asegurar el logro y la verificación de los objetivos cuando se trabaja con un socio externo, es necesario prestar atención a la calidad y solidez del código fuente que se entrega.

Para identificar métricas que brinden una seguridad razonable de que la aplicación está libre de agujeros de seguridad y que adopta las mejores prácticas, se requiere el uso de software de análisis.

## SonarQube&trade;, la herramienta para medir la calidad del código 

[**SonarQube&trade;**](https://www.sonarqube.org/) es una plataforma de software de código abierto ampliamente conocida en la comunidad de desarrolladores, sólida y organizada con complementos con los que enriquecer sus capacidades de análisis.

La instalación es muy rápida y puede basarse en contenedores docker, también alojados en servicios en la nube como, por ejemplo, Azure de Microsoft.
Si necesitas respetar la confidencialidad del código fuente es mejor descartar el servicio cloud de SonarSource, SonarCloud.

## Características de SonarQube&trade;

Es una plataforma capaz de verificar la calidad del código fuente, realizar análisis de errores, código sospechoso y vulnerabilidades de seguridad en más de veinte lenguajes de programación. 

Todos los análisis utilizados por SonarQube&trade; están definidos como [**estáticos**](/analisis-estatico-del-codigo-con-sonarqube), es decir, **no requieren la ejecución del programa**.

Su adopción, durante el ciclo de desarrollo del software, permite:

-- Mejorar los procesos de prueba y desarrollo de componentes

-- Identificar posibles problemas de calidad en el desarrollo, antes de que el software entre en producción

-- Detectar áreas que requieran refactorización o simplificación

-- Identificar errores o defectos de programación

-- Aumentar la comunicación del equipo de desarrollo y animar a los desarrolladores a producir código de alta calidad

Además, se integra perfectamente con la práctica de **Integración Continua** (la creación de una baseline de código fuente que contiene todo el trabajo realizado por el equipo durante el día), sumando la información sobre la calidad alcanzada.

## Funcionamiento

Los [informes creados por SonarQube&trade;](/es/sonarqube-report) se recogen en su plataforma y pueden ser consultados por cada miembro del equipo; estos también se asignan automáticamente al desarrollador que introdujo la posible criticidad (utilizando la información de los commits extraídos del sistema de versionado del código fuente) y se le notifica por correo electrónico para notificarle la necesidad de reconocimiento y resolución.
La adopción de la integración continua permite:

-- Confirmar, incluso varias veces al día, la solidez de la aplicación ejecutando todas las pruebas en un entorno externo al de los desarrolladores.

-- Tener siempre lista la última versión de la aplicación, libre de errores de compilación y con todas las pruebas superadas (**Entrega Continua**).

También es posibile tener monitorear la **[deuda técnica](https://www.bitegarden.com/como-evaluar-deuda-tecnica-sonarqube) acumulada**. La deuda técnica se refiere al tiempo empírico necesario para resolver los informes de SonarQube&trade;. Normalmente esto no requiere la introducción de una tarea específica para resolver las alertas. 

Gracias a su facilidad, el equipo aprende rápidamente a navegar por el panel de SonarQube&trade; y a analizar u ordenar los problemas por prioridad.

## Beneficios de SonarQube&trade;

-- La adopción es muy rápida y requiere pocas operaciones y cambios en las operaciones del equipo.

-- Tener un estándar único compartido por todo el equipo a través de reglas centralizadas

-- Detección de errores preventivos (por ejemplo: partes de código nunca alcanzadas, condiciones de prueba siempre verdaderas, posibles punteros nulos, ...) incluso antes de haber escrito las UnitTests

-- Identificación de posibles problemas de seguridad, gracias a la posibilidad de utilizar database públicos de vulnerabilidades (CWE, Sans, OWASP)

-- Reducción del tiempo de revisión del código. Los miembros más experimentados del equipo son consultados solo sobre problemas realmente complejos y no sobre las mejores prácticas conocidas y ya documentadas

-- Tablero claro con medición de progreso durante todo el desarrollo del proyecto.

SonarQube&trade; es la herramienta perfecta para medir la calidad del trabajo realizado (sea internamente que hecho por proveedores.

<hr>

### Plugins para SonarQube&trade;

Si deseas manejar o descargar los informes de SonarQube&trade;, prueba gratuitamente nuestros [**Plugins para SonarQube&trade;**](/es/products), te brindarán la ayuda extra qué estás buscando.

<a href="/es/downloads" class="btn btn-primary btn-call-to-action fancybox" style="font-weight:bold;font-size:16px; text-transform: uppercase;">Descubre más </a>
<br>

<br>


---
**<span style="color: green">bitegarden</span> team**

_Helping companies to develop better software_
