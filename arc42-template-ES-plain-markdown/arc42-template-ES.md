---
date: Enero 2023
title: Plantilla ![arc42](images/arc42-logo.png)
---

# 

**Acerca de arc42**

arc42, La plantilla de documentación para arquitectura de sistemas y de
software.

Por Dr. Gernot Starke, Dr. Peter Hruschka y otros contribuyentes.

Revisión de la plantilla: 7.0 ES (basada en asciidoc), Enero 2017

© Reconocemos que este documento utiliza material de la plantilla de
arquitectura arc42, <https://www.arc42.org>. Creada por Dr. Peter
Hruschka y Dr. Gernot Starke.

# Introducción y Metas {#section-introduction-and-goals}

El sistema ERP del concesionario de carros tiene como objetivo integrar y automatizar los procesos clave del negocio, permitiendo una gestión eficiente de las compras, el inventario y el control financiero.

En particular, el Módulo de Compras busca optimizar la adquisición de vehículos, repuestos y servicios, garantizando trazabilidad, control de costos y una correcta relación con los proveedores.

## Vista de Requerimientos {#_vista_de_requerimientos}
-Registrar, modificar y desactivar proveedores.
- Crear y gestionar órdenes de compra.
- Aprobar o rechazar órdenes según roles definidos.
- Registrar la recepción de productos comprados.
- Mantener actualizado el inventario.
- Generar reportes de compras y costos.

## Metas de Calidad {#_metas_de_calidad}

## Partes interesadas (Stakeholders) {#_partes_interesadas_stakeholders}

+-------------+---------------------------+---------------------------+
| Rol/Nombre  | Contacto                  | Expectativas              |
+=============+===========================+===========================+
| *           | *\<Contact-1\>*           | *\<Expectation-1\>*       |
| \<Role-1\>* |                           |                           |
+-------------+---------------------------+---------------------------+
| *           | *\<Contact-2\>*           | *\<Expectation-2\>*       |
| \<Role-2\>* |                           |                           |
+-------------+---------------------------+---------------------------+

# Restricciones de la Arquitectura {#section-architecture-constraints}

Para el desarrollo del ERP del concesionario se tomaron las siguientes decisiones tecnológicas, buscando simplicidad, coherencia y facilidad de mantenimiento.

## Decisiones Tecnológicas

- El backend será desarrollado en **Java utilizando Spring Boot**, bajo una arquitectura monolítica.
- La base de datos será **PostgreSQL**, por su robustez y soporte para sistemas transaccionales.
- El frontend será una **Aplicación Web (SPA)** desarrollada con **HTML, CSS y JavaScript**.
- La comunicación entre frontend y backend se realizará mediante **HTTP/HTTPS usando JSON**.
- El sistema se integrará con un **Sistema Contable Externo** mediante servicios web.
- 
# Alcance y Contexto del Sistema {#section-context-and-scope}

## Contexto de Negocio {#_contexto_de_negocio}

El ERP del concesionario de carros interactúa con diferentes tipos de usuarios y sistemas externos para cumplir con sus objetivos de negocio.

Los usuarios principales incluyen responsables de compras, gerentes, encargados de bodega y contadores. Además, el sistema se integra con plataformas externas como sistemas de proveedores y sistemas contables.

A continuación, se presenta el Diagrama de Contexto (C1), el cual muestra el sistema ERP como una caja negra y sus interacciones con actores externos.

**\<Diagrama o Tabla\>**

![Diagrama de Contexto](./images/C1.png)
**\<optionally: Explanation of external domain interfaces\>**

## Contexto Técnico {#_contexto_técnico}

**\<Diagrama o Tabla\>**

**\<Opcional: Explicación de las interfases técnicas\>**

**\<Mapeo de Entrada/Salida a canales\>**

# Estrategia de solución {#section-solution-strategy}

# Vista de Bloques {#section-building-block-view}

## Sistema General de Caja Blanca {#_sistema_general_de_caja_blanca}

***\<Diagrama general\>***

Motivación

:   *\<Explicación en texto\>*

Bloques de construcción contenidos

:   *\<Desripción de los bloques de construcción contenidos (Cajas
    negras)\>*

Interfases importantes

:   *\<Descripción de las interfases importantes\>*

### \<Caja Negra 1\> {#_caja_negra_1}

*\<Propósito/Responsabilidad\>*

*\<Interfase(s)\>*

*\<(Opcional) Características de Calidad/Performance\>*

*\<(Opcional) Ubicación Archivo/Directorio\>*

*\<(Opcional) Requerimientos Satisfechos\>*

*\<(Opcional) Riesgos/Problemas/Incidentes Abiertos\>*

### \<Caja Negra 2\> {#_caja_negra_2}

*\<plantilla de caja negra\>*

### \<Caja Negra N\> {#_caja_negra_n}

*\<Plantilla de caja negra\>*

### \<Interfase 1\> {#_interfase_1}

...​

### \<Interfase m\> {#_interfase_m}

## Nivel 2 {#_nivel_2}

### Caja Blanca *\<bloque de construcción 1\>* {#_caja_blanca_bloque_de_construcción_1}

*\<plantilla de caja blanca\>*

### Caja Blanca *\<bloque de construcción 2\>* {#_caja_blanca_bloque_de_construcción_2}

*\<plantilla de caja blanca\>*

...​

### Caja Blanca *\<bloque de construcción m\>* {#_caja_blanca_bloque_de_construcción_m}

*\<plantilla de caja blanca\>*

## Nivel 3 {#_nivel_3}

### Caja Blanca \<\_bloque de construcción x.1\_\> {#_caja_blanca_bloque_de_construcción_x_1}

*\<plantilla de caja blanca\>*

### Caja Blanca \<\_bloque de construcción x.2\_\> {#_caja_blanca_bloque_de_construcción_x_2}

*\<plantilla de caja blanca\>*

### Caja Blanca \<\_bloque de construcción y.1\_\> {#_caja_blanca_bloque_de_construcción_y_1}

*\<plantilla de caja blanca\>*

# Vista de Ejecución {#section-runtime-view}

## \<Escenario de ejecución 1\> {#_escenario_de_ejecución_1}

-   *\<Inserte un diagrama de ejecución o la descripción del
    escenario\>*

-   *\<Inserte la descripción de aspectos notables de las interacciones
    entre los bloques de construcción mostrados en este diagrama.\>*

## \<Escenario de ejecución 2\> {#_escenario_de_ejecución_2}

## ...​

## \<Escenario de ejecución n\> {#_escenario_de_ejecución_n}

# Vista de Despliegue {#section-deployment-view}

## Nivel de infraestructura 1 {#_nivel_de_infraestructura_1}

***\<Diagrama General\>***

Motivación

:   *\<Explicación en forma textual\>*

Características de Calidad/Rendimiento

:   *\<Explicación en forma textual\>*

    Mapeo de los Bloques de Construcción a Infraestructura

    :   *\<Descripción del mapeo\>*

## Nivel de Infraestructura 2 {#_nivel_de_infraestructura_2}

### *\<Elemento de Infraestructura 1\>* {#_elemento_de_infraestructura_1}

*\<diagrama + explicación\>*

### *\<Elemento de Infraestructura 2\>* {#_elemento_de_infraestructura_2}

*\<diagrama + explicación\>*

...​

### *\<Elemento de Infraestructura n\>* {#_elemento_de_infraestructura_n}

*\<diagrama + explicación\>*

# Conceptos Transversales (Cross-cutting) {#section-concepts}

## *\<Concepto 1\>* {#_concepto_1}

*\<explicación\>*

## *\<Concepto 2\>* {#_concepto_2}

*\<explicación\>*

...​

## *\<Concepto n\>* {#_concepto_n}

*\<explicación\>*

# Decisiones de Diseño {#section-design-decisions}

# Requerimientos de Calidad {#section-quality-scenarios}

## Árbol de Calidad {#_árbol_de_calidad}

## Escenarios de calidad {#_escenarios_de_calidad}

# Riesgos y deuda técnica {#section-technical-risks}

# Glosario {#section-glossary}

+----------------------+-----------------------------------------------+
| Término              | Definición                                    |
+======================+===============================================+
| *\<Término-1\>*      | *\<definicion-1\>*                            |
+----------------------+-----------------------------------------------+
| *\<Término-2\>*      | *\<definicion-2\>*                            |
+----------------------+-----------------------------------------------+
