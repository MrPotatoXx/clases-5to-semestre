# Ingeniería de software

## Clase 1 (16/03/22)

### Etapas del desarrollo de software

- Análisis del sistema
- Diseño del Software
- Construcción del software (Codificación, implementación)
- Pruebas del sistema (Testing o QA)
- Puesta en marcha (Instalación, producción)
- Mantenimiento del software :
    - Perfectivo
    - Correctivo
    - Preventivo
#### Capas del software

1) Capa de presentación -> JSP/HTML
3) Capa de negocio -> Servlet/Java
2) Capa de datos ->Bases de datos

## Clase 2 (17/03/22)

### La web

-> Formularios web (Capa de presentación)

-> Verificar la información (Capa de negocio)

-> Guardar la información en la (Capa de datos)

## Clase 3 (23/03/22)

### Desarrollo orientado a objetos: Paradigma y modelo UML

## Fundamentos del paradigma orientado a objetos

- Elementos:
    - Modularidad: clases y objetos
    - Abstracción: obtener de un elemento concreto la clasificación
    - Encapsulación:


        ```
        nivel           UML
        ------------|---------------
        Private     |    -
        Public      |    +
        Protected   |    #
        Friendly    |    *
        ```
        ```
        - Private: Atributos accesibles dentro de la misma clase.
        - Public: Atributo accesibles para todas las clases.
        - Protected: Atributos accesibles solo para clases seleccionadas.
        - Visible solos para el package.

        ```
    - Herencia: Se hereda todo menos lo privado
    - Polimorfismo

#### La base de UML

- Booch
- Rumbaugh
- Jacobson

##### UML

Para modelar en BPMN se puede usar herramientas CASE:

- Bizagi
- Bonita
- Power designer

Para modelar diagramas de actividades (UML) se pude usar:

- draw.io
- Visio
- Magicdraw
- StarUML
- Power Designer
- Enterprise architect

## Clase 4 (24/03/22)

### Bachillerato actividad 1

https://grupocinco.files.wordpress.com/2007/11/bpmn.pdf

5) Descarta el paper el diagrama de actividad para el modelado de procesos de negocio? Que indica?

6) Como se relacionan BPMN - XPDL - BPEL?

## Clase 5 (30/03/22)

### Fechas de prueba

- 28 abril 15% Informe Exposición 1
- 23 junio 30% Informe Exposición 2
- 06 julio 20% Prototipo Funcional
- 13 julio 15% Elevator Pitch
- 20 julio 20% (Todo el semestre) Acumulativo del semestre
- 27 julio Examen

### Entrega Guía Formulación de Proyecto 1

https://lms.inacap.cl/mod/folder/view.php?id=6748528

Documentos obligatorios:

- FODA.
- Carta gantt.

### A realizar

Proximo miercoles:
1) Encuesta
2) FODA

## Clase 6

### Habla de formación de grupos y proyectos

### Tips para la encuesta:

- Preguntas cerradas o de selección múltiple
- Cantidad acotada de preguntas (10 o 12)
- Progresiones de preguntas (de general a particular)
- Preguntas de no mucha exención
- Preguntas alusivas a la hipótesis
- Mínimo 20 personas

    ```

    ----------------------------------
       Fortaleza       Oportunidades
    ---------------|------------------
                   |
                   |
         1*        |          2*
                   |
                   |
    -------------  |------------------
       Fortaleza       Oportunidades
    ---------------|------------------
                   |
                   |
         1*        |           2*
                   |
                   |

    1* Definiciones internas respecto al proyecto

    2* Definiciones depende dl proyecto mismo pero
       si lo afectan desde el entorno

    Mínimo 4 de cada una

    ```
## Clase 7

Revicion de encuesta y foda

Para la proxima semana traer

Diagramas de casos de uso
Calculo de puntos por caso de uso

### Casos de uso 

```
Monito palo | Actor

Ovalo | Caso de uso

Linea | ÚNICA forma de conectar un actor y un caso de uso

Flecha punteada + << tipo >> | Flecha para representar INCLUDE o EXTEND solo entre casos de uso

Flecha recta | Para generalización o herencia solo entre casos de uso o solo entre actores

```

Caso de uso => Un requerimiento funcional del sistema

Actor => Persona, Entidad o Sistema Externo que interactúa desde fuera con los requerimientos funcionales

Base de datos NO ES UN REQUERIMIENTO FUNCIONAL

El diagrama de C.U. es de un nivel de abstracción alto, por definición. Esto implica que no debería mostrar detalles de implementación, excepto que se explique en la ficha del  caso de uso

![](/Ingenieria%20de%20Software/Material%20de%20apoyo/Caso-de-uso-ej-clase-7.png)

## Clase 8

### Métrica del Análisis de Puntos por Casos de Uso (PCU)

La ecuación se compone de 4 variables:

- Factor de Complejidad Técnica (TCF).
- Factor de Complejidad Ambiental (ECF).
- Puntos de Casos de Uso Desajustados (UUCP).
- Factor de Productividad (PF).

PCU = TCF * ECF * UUCP * PF

El actor es una persona que interactúa a través de una interfaz.