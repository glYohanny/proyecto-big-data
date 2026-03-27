# Mapeo de Notebooks - Google Cloud Skills Boost

Este documento relaciona los notebooks del repositorio con los labs correspondientes en [Google Cloud Skills Boost](https://www.cloudskillsboost.google/) (anteriormente Qwiklabs). Los labs de referencia permiten profundizar los conceptos practicados localmente usando servicios reales de Google Cloud Platform.

---

## Como acceder a Google Cloud Skills Boost

1. Ve a https://www.cloudskillsboost.google/
2. Crea una cuenta gratuita o inicia sesion con tu cuenta de Google
3. Busca el lab por su codigo (ej: GSP002) en la barra de busqueda
4. Algunos labs son gratuitos; otros requieren creditos que se pueden obtener mediante suscripcion o a traves de programas educativos

> **Nota importante:** Los notebooks de este repositorio estan disenados para ejecutarse **localmente con Docker**. Los labs de Google Cloud Skills Boost son un complemento para practicar con infraestructura cloud real. No es necesario completar los labs en la nube para aprobar la asignatura.

---

## EA1: Fundamentos de Big Data

| Notebook del Repo | Lab Google | Codigo | Descripcion del Lab |
|--------------------|------------|--------|---------------------|
| `01_introduccion_spark.ipynb` | A Tour of Google Cloud Hands-on Labs | GSP002 | Introduccion general a la plataforma de labs |
| `01_introduccion_spark.ipynb` | Creating a Virtual Machine | GSP001 | Creacion de VM para entender infraestructura cloud |
| `02_rdds_basico.ipynb` | Introduction to Docker | GSP055 | Contenedores y su relacion con Big Data |
| `03_dataframes_intro.ipynb` | Running Apache Spark Jobs on Dataproc | GSP123 | DataFrames de Spark en Dataproc (Spark en la nube) |
| `04_arquitecturas_bigdata.ipynb` | BigQuery: Qwik Start - Command Line | GSP064 | Introduccion a BigQuery como ejemplo de arquitectura |

---

## EA2: ETL y Procesamiento Batch

| Notebook del Repo | Lab Google | Codigo | Descripcion del Lab |
|--------------------|------------|--------|---------------------|
| `01_ingesta_datos.ipynb` | Cloud Storage: Qwik Start - CLI/SDK | GSP073 | Almacenamiento de datos en Cloud Storage |
| `01_ingesta_datos.ipynb` | Dataflow: Qwik Start - Python | GSP207 | Ingesta de datos con Apache Beam en Dataflow |
| `02_transformacion_limpieza.ipynb` | Cloud Dataprep: Qwik Start | GSP105 | Limpieza y preparacion de datos en la nube |
| `02_transformacion_limpieza.ipynb` | Dataproc: Qwik Start - Console | GSP050 | Cluster Spark en GCP para transformaciones |
| `03_spark_sql.ipynb` | Creating a Data Warehouse Through Joins and Unions | GSP281 | SQL avanzado para data warehouse |
| `03_spark_sql.ipynb` | BigQuery: Qwik Start - Console | GSP072 | Consultas SQL a gran escala con BigQuery |
| `03_spark_sql.ipynb` | BigQuery: Qwik Start - Command Line | GSP071 | BigQuery desde la linea de comandos |
| `04_hive_metastore.ipynb` | Creating a Data Transformation Pipeline with Cloud Dataprep | GSP407 | Pipeline de transformacion de datos |
| `04_hive_metastore.ipynb` | Using BigQuery to do Analysis | GSP413 | Analisis de datos con BigQuery (similar a Hive) |
| `04_hive_metastore.ipynb` | Explore an Ecommerce Dataset with SQL in BigQuery | GSP406 | Exploracion de datos con SQL |
| `05_machine_learning_spark.ipynb` | Predict Visitor Purchases with a Classification Model in BigQuery ML | GSP247 | ML con BigQuery ML |
| `05_machine_learning_spark.ipynb` | BigQuery Machine Learning Using the Google Cloud Console | GSP136 | Machine Learning en la nube |
| `06_visualizacion_datos.ipynb` | Explore and Create Reports with Looker Studio | GSP409 | Visualizacion con Looker Studio |
| `06_visualizacion_datos.ipynb` | Exploring Dataset Metadata Between Projects with Data Catalog | GSP718 | Catalogo de datos y metadata |

---

## EA3: Procesamiento en Tiempo Real

| Notebook del Repo | Lab Google | Codigo | Descripcion del Lab |
|--------------------|------------|--------|---------------------|
| `01_kafka_introduccion.ipynb` | Pub/Sub: Qwik Start - Console | GSP096 | Pub/Sub como alternativa cloud a Kafka |
| `01_kafka_introduccion.ipynb` | Streaming Data Processing: Publish Streaming Data into Pub/Sub | GSP903 | Publicacion de datos en streaming |
| `02_ingesta_tiempo_real.ipynb` | Streaming Analytics into BigQuery | GSP294 | Ingesta de streaming hacia BigQuery |
| `02_ingesta_tiempo_real.ipynb` | Pub/Sub: Qwik Start - Python | GSP192 | Pub/Sub con Python |
| `03_spark_structured_streaming.ipynb` | Streaming Data Pipelines | GSP855 | Pipelines de datos en streaming con Dataflow |
| `03_spark_structured_streaming.ipynb` | Streaming Data Pipelines into Bigtable | GSP857 | Streaming hacia Bigtable |
| `04_dashboard_tiempo_real.ipynb` | Creating a Streaming Data Pipeline for a Real-Time Dashboard with Dataflow | GSP730 | Dashboard en tiempo real con Dataflow y Looker |

---

## Otros Labs Relevantes

Labs adicionales que complementan los temas del curso aunque no se mapean directamente a un notebook especifico:

| Lab Google | Codigo | Tema Relacionado | Descripcion |
|------------|--------|------------------|-------------|
| Bigtable: Qwik Start - Hbase Shell | GSP185 | Bases de datos NoSQL | Introduccion a Cloud Bigtable |
| Cloud Composer: Qwik Start - Console | GSP848 | Orquestacion de workflows | Apache Airflow en la nube |
| Dataproc Serverless for Spark Batches | GSP621 | Spark serverless | Spark sin gestion de cluster |
| Creating a Persistent Disk | GSP261 | Almacenamiento | Discos persistentes en GCP |
| Autoscaling TensorFlow Model Deployments with TF Serving and Kubernetes | GSP1040 | ML en produccion | Despliegue de modelos |
| Cloud Spanner: Qwik Start | GSP431 | Bases de datos distribuidas | Base de datos distribuida global |
| Cloud Monitoring: Qwik Start | GSP009 | Monitoreo | Monitoreo de infraestructura cloud |
| AI Platform: Qwik Start | GSP823 | ML Platform | Plataforma de ML en la nube |

---

## Relacion entre Herramientas Locales y Servicios Cloud

| Herramienta Local (Docker) | Equivalente en Google Cloud | Notas |
|---|---|---|
| **Apache Spark** (Bitnami) | **Dataproc** | Cluster Spark gestionado |
| **Apache Kafka** (Bitnami) | **Pub/Sub** | Mensajeria y streaming gestionado |
| **Apache Hive** | **BigQuery** | Data warehouse serverless |
| **PostgreSQL** (Hive Metastore) | **Cloud SQL** | Base de datos relacional gestionada |
| **JupyterLab** | **Vertex AI Workbench** | Notebooks gestionados |
| **HDFS** (simulado) | **Cloud Storage (GCS)** | Almacenamiento de objetos |

---

## Nota sobre practica local vs. labs en la nube

El objetivo principal de este repositorio es que practiques **conceptos de Big Data** (Spark, Kafka, Hive, ETL, streaming) sin depender de una cuenta en la nube ni de costos asociados.

Los labs de Google Cloud Skills Boost son **opcionales y complementarios**:

- Permiten ver como se aplican los mismos conceptos en infraestructura cloud real
- Ayudan a prepararse para certificaciones de Google Cloud
- Algunos labs son gratuitos, otros requieren creditos
- Los conceptos fundamentales (DataFrames, SQL, streaming, ML) son los mismos independientemente de si se ejecutan localmente o en la nube

> **Recomendacion:** Primero domina los notebooks locales del repositorio. Luego, si quieres profundizar, explora los labs en la nube como complemento.

---

<p align="center">
  <strong>DUOC UC</strong> | Big Data (BIY7131) | Semestre 2026-1
</p>
