---
layout: post_es
title:  Cómo desarrollar software de alta calidad con SonarQube
description: Cómo cuantificar la calidad de un software y construir un producto de alta calidad.

permalink: como-costruir-software-de-alta-calidad-sonarqube
english: how-to-develop-high-quality-software-sonarqube
cover: /img/posts/2021-05-14-how-to-develop-high-quality-software-with-sonarqube-thumb.png
---

Utilizar una herramienta como **SonarQube**, conduce a una mayor calidad y productividad para los programadores y facilita una especie de "estandarización" del código, un factor muy importante dado que partes de los productos de software a menudo se comparten entre diferentes personas.

A través del análisis estático del código fuente, SonarQube mide los niveles de confiabilidad, mantenibilidad, seguridad, complejidad, cobertura de prueba y duplicación de código, asignando una puntuación en función de la gravedad de los defectos encontrados.

Cuando la calidad del software se mantiene alta, puede **garantizar una mayor seguridad** y permite **reducir los costos** durante todo el ciclo de vida del producto, **reducir el tiempo de mantenimiento** y crear valor para productores, clientes y financieros.

## Cómo cuantificar la calidad de un software

La alta calidad del software está relacionada con:

- -- Reducción de los tiempos de prueba y entrega
- -- Reducción de más del 50% de reparaciones y modificaciones
- -- Incremento de la satisfacción del cliente
- -- Reducción, después del lanzamiento, de los costos de mantenimiento
- -- Reducción de disputas sobre contratos de proyectos
- -- Reducción de proyectos cancelados
- -- Aumento de la confiabilidad
- -- Reducción de los agujeros de seguridad en las aplicaciones publicadas

## Categorías de las reglas de SonarQube

SonarQube, para analizar el código, usa reglas clasificadas en cuatro tipos: code smell, bug, vulnerabilidades y security hotspot.

La categoría **code smells** incluye las características que indican un defecto de programación pero no revelan errores y, por lo tanto, no afectan la corrección real del software, pero hacen que el código sea menos fácil de mantener.

**Bugs** son errores de los que depende el comportamiento inesperado o incorrecto del programa, reducen la confiabilidad del programa.

Las **vulnerabilidades** son debilidades que pueden explotarse para comprometer el nivel de seguridad del sistema.

Los **security hotspot** son debilidades que no son problemáticas, pero que podrían convertirse en vulnerabilidades. Algunos ejemplos son la mala configuración de las cookies, el uso de algoritmos criptográficos no estándar y el uso de protocolos que no crean conexiones seguras.

*Además es posible **crear nuevas reglas** a través de la plataforma SonarQube, y es posible elegir un conjunto de reglas para asociar con cada lenguaje.*

## Grados de gravedad

Durante el análisis, los problemas se definen cada vez que un fragmento de código rompe una regla. Cada problema está vinculado a un nivel de gravedad diferente:
- -- **Bloqueador**: un error que puede cambiar el comportamiento del programa y requiere un cambio de código
- -- **Crítico**: un error que es poco probable que cambie el comportamiento del programa o una falla de seguridad. El código debe ser verificado
- -- **Mayor**: defectos de código que reducen la productividad del desarrollador, como código repetido, parámetros y variables no utilizadas
- -- **Menor**: defectos de código que reducen ligeramente la productividad de los desarrolladores como lineas demasiado largas
- -- **Información**: no se trata de un defecto de software real, por ejemplo los comentarios "TODO" o el uso de construcciones obsoletas

## Cinco estados

Un problema, una vez creado, puede asumir cinco estados: inmediatamente después de su creación está **(1) abierto**, se convierte en **(2) confirmado** cuando el usuario indica que es un problema válido, **( 3) resuelto** cuando el usuario indica que en el próximo análisis no se debe volver a considerar porque se han realizado cambios, **(4) reabierto** cuando el problema ha sido reportado como resuelto pero realmente no ha sido corregido y **(5) cerrado** cuando SonarQube ya no lo reconoce como un problema. Un problema se cierra cuando ha sido **solucionado** o porque la regla relacionada que lo reconoce ya no está disponible, **eliminado**.

## Calificación de las métricas

Las métricas utilizadas para definir la calidad del código son complejidad, duplicación, mantenibilidad, confiabilidad, seguridad, tamaño y cobertura de prueba.

#### Calificación de confiabilidad

- A = 0 error
- B = al menos un error menor
- C = al menos un error importante
- D = al menos un error crítico
- E = al menos un bloqueador de errores

#### Clasificación de seguridad

- A = 0 vulnerabilidad
- B = al menos una vulnerabilidad menor
- C = al menos una vulnerabilidad importante
- D = al menos una vulnerabilidad crítica
- E = al menos una vulnerabilidad de bloqueador

#### Calificación de deuda técnica

Depende del "ratio de deuda técnica" (TD ratio) que es el ratio de la deuda y el tiempo de desarrollo estimado, calculado como LOCx30min.

- A = relación TD <= 5%
- B = ratio TD entre 6 y 10%
- C = ratio TD entre 10 y 20%
- D = ratio TD entre 21 y 50%
- E = relación TD> = 50%

## El software de alta calidad es más económico de producir

Si crees en la integración continua, no puedes no usar SonarQube, ya que te permitirá verificar el código después de cada cambio, manteniendo así la calidad de tu software siempre alta.

Happy coding!

---
**<span style="color: green">bitegarden</span> team**

_Helping companies to develop better software_
