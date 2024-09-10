# Proyecto de Generación de Datos Falsos con Faker y Google Colab

Este proyecto utiliza la librería `Faker` para generar datos falsos y los combina con otras librerías como `sqlite3`, `pandas`, y `requests` para realizar diversas tareas en Google Colab, incluyendo el montaje de Google Drive.

## Requisitos

Antes de comenzar, asegúrate de tener instaladas las siguientes dependencias:

- Python 3.x
- Google Colab (para ejecutar el código en la nube)
- Módulos de Python:
  - `Faker`
  - `pandas`
  - `requests`
  - `sqlite3` (incluido en la biblioteca estándar de Python)
  - `numpy`
  - `shutil`
  - `uuid`
  - `google-colab` (para montar Google Drive)


## Conectar y extraer datos desde SQLite
Este proyecto también permite la conexión a una base de datos SQLite almacenada en Google Drive para extraer datos y realizar un Análisis Exploratorio de Datos (EDA).

## Conexión a la base de datos
La base de datos utilizada para este ejemplo se encuentra almacenada en Google Drive. Puedes montar tu Google Drive en Google Colab de la siguiente manera:

![image](https://github.com/user-attachments/assets/38c97bcc-b991-4178-830a-15f17f7dd4ca)

drive.mount('/content/drive')
Una vez que la unidad de Google Drive esté montada, puedes conectar y leer los datos desde la base de datos SQLite:

![image](https://github.com/user-attachments/assets/480f13ea-aaf2-491f-af8e-72e050760dda)
## Análisis Exploratorio de Datos (EDA)
El código incluye un análisis exploratorio de datos utilizando la tabla tbl_corrected_transactions. El EDA analiza la completitud de los datos, genera estadísticas descriptivas, visualiza la distribución de las variables y analiza las correlaciones entre las variables numéricas.

## Visualización de la Completitud de los Datos
Se utiliza la biblioteca missingno para visualizar la completitud de los datos:

![image](https://github.com/user-attachments/assets/dd621c8b-a6fa-4b22-995d-6619946be247)

## Estadísticas Descriptivas
Se generan estadísticas descriptivas para todas las variables:

![image](https://github.com/user-attachments/assets/625b2bcb-797c-4be2-9c94-5697ea98956a)

## Distribución de Variables Numéricas
El código genera histogramas para visualizar la distribución de las variables numéricas y una matriz de correlación para analizar la relación entre ellas:

![image](https://github.com/user-attachments/assets/06c016d7-e7d5-4254-a1e0-804ed0ecaaa4)

## Creación de Tablas y Datos Falsos con Faker
Este proyecto también permite la creación de tablas en la base de datos SQLite y la generación de datos falsos utilizando la librería Faker.

## Crear tablas en SQLite3
Crea las tablas customers, branches, transaction_types y transactions en la base de datos
## Generar datos falsos
El siguiente código genera datos falsos para las tablas customers, branches, transaction_types y transactions:

![image](https://github.com/user-attachments/assets/7f2270e5-d1e9-4733-82a5-dd5014cd00ce)

## Guardar la base de datos en Google Drive
Finalmente, puedes guardar la base de datos generada en Google Drive:

![image](https://github.com/user-attachments/assets/6739f907-385b-4f24-a5b3-c0f20482ccfd)

## Conclusión
Este proyecto integra el uso de SQLite, la generación de datos falsos con Faker, y el análisis exploratorio de datos con pandas, seaborn, y matplotlib, permitiendo una solución completa para la generación y análisis de datos.

![image](https://github.com/user-attachments/assets/588b35a9-8a65-419d-9654-2ce9d65014a1)
