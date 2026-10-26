# Data Pipelines & Automatization

Este repositorio contiene proyectos y scripts orientados al **procesamiento de datos, automatización de tareas y creación de pipelines ETL/ELT**. 

Aunque mi enfoque profesional principal es el **Desarrollo de Software / Backend**, me gusta realizar programas que automaticen tareas y sirvan para extraer métricas útiles para una organización.

---

## Tecnologías e Infraestructura

- **Lenguaje principal:** Python (Pandas, NumPy, pypdf)
- **Infraestructura & Contenedores:** Docker
- **Bases de Datos & Almacenamiento:** PostgreSQL, MySQL

---

## Flujo de Trabajo y Arquitectura de las Pipelines

Las pipelines desarrolladas en este repositorio ejecutan un ciclo completo de tratamiento de datos organizado en tres fases:

### 1. Extracción Multifuente (*Ingestion*)
Lectura y consolidación de datos procedentes de orígenes heterogéneos:
* **Bases de datos relacionales** (consultas SQL).
* **APIs de terceros** (consumo e integración de endpoints REST).
* **Documentos no estructurados:** Parseo y extracción de información desde archivos `.doc`, `.docx` y `.pdf`.
* **Archivos estructurados:** Procesamiento de ficheros en formatos `.csv` y `.xlsx`.

### 2. Transformación y Enriquecimiento (*Processing*)
Limpieza y manipulación avanzada mediante **Pandas**:
* **Limpieza y filtrado:** Tratamiento de nulos, eliminación de duplicados, tipado riguroso y depuración de inconsistencias.
* **Lógica de negocio:** Operaciones vectoriales entre columnas, transformaciones condicionales y normalización.
* **Agregaciones:** Agrupamientos (*groupby*), tablas dinámicas y cálculos estadísticos acumulados.

### 3. Carga y Generación de Dataset Final (*Output*)
* Construcción y exportación de **datasets consolidados** con métricas clave y listas para el análisis de negocio.
* Persistencia de los resultados en bases de datos objetivo o ficheros de salida listos para consumo por otros servicios o dashboards.

---

## Despliegue con Docker

Varios de los flujos de trabajo están totalmente **contenerizados**, permitiendo aislar el entorno de ejecución y las dependencias de Python.
