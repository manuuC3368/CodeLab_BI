# CodeLab_BI
Portafolio de mis implementaciones de Business Intelligence 
Este proyecto configura una base de datos SQLite3 para almacenar información sobre transacciones financieras. La base de datos incluye datos de clientes, sucursales, tipos de transacciones y transacciones. Los datos se generan de manera sintética utilizando la librería Faker y la API randomuser.me.

# CONTENIDOS:
1. Instalación
2. Configuración de la Base de Datos
a. Configuración Inicial y Creación de la Base de Datos
b. Generar y Guardar la Tabla de Clientes
c. Generar y Guardar la Tabla de Sucursales
d. Generar y Guardar la Tabla de Tipos de Transacciones
e. Generar y Guardar la Tabla de Transacciones
3. Verificación y Cierre
4. Imágenes

# Instalación
Asegúrate de tener Python instalado junto con las librerías necesarias. Puedes instalar las dependencias utilizando el siguiente comando:

![image](https://github.com/user-attachments/assets/1b91f086-44e4-48b0-801c-e4e9914f5333)

Si estás ejecutando este código en Google Colab, recuerda montar tu Google Drive.

# Configuración de la Base de Datos
## 1. Configuración Inicial y Creación de la Base de Datos
En esta primera etapa, configuramos la base de datos SQLite3 y creamos las tablas necesarias. Esto incluye la configuración inicial de la conexión a la base de datos y la creación de las tablas para almacenar los datos.
![image](https://github.com/user-attachments/assets/5a048109-f088-4fdf-8317-c4859e952de2)

Descripción del código:
sqlite3: Se utiliza para manejar la base de datos SQLite3.
pandas: Se usa para manipular datos tabulares y guardarlos en la base de datos.
requests: Se utiliza para hacer solicitudes HTTP a la API randomuser.me.
Faker: Se usa para generar datos ficticios, como nombres, direcciones y números de teléfono.
google.colab.drive: Se usa para montar Google Drive en Google Colab.

## 2. Generar y Guardar la Tabla de Clientes
En este paso, obtenemos datos de clientes utilizando la API randomuser.me y los almacenamos en la tabla customers.
![image](https://github.com/user-attachments/assets/4cf676ae-e48b-488f-a985-458d32b3a1d8)

Descripción del código:
get_random_users: Función que realiza una solicitud a la API randomuser.me para obtener datos de clientes. Devuelve una lista de usuarios.
create_customers_table: Función que toma los datos de usuarios, los organiza en un DataFrame y los guarda en la tabla customers en la base de datos.

## 3. Generar y Guardar la Tabla de Sucursales
Aquí, utilizamos Faker para generar datos sintéticos de sucursales y guardarlos en la tabla branches.
![image](https://github.com/user-attachments/assets/0b7607ba-8c3b-4584-bd4a-e62a6354035c)

Descripción del código:
create_branches_table: Función que genera datos ficticios para sucursales, como la ubicación y el nombre del gerente. Estos datos se guardan en la tabla branches.
## 4. Generar y Guardar la Tabla de Tipos de Transacciones
Creamos una tabla sencilla que contiene los diferentes tipos de transacciones.
![image](https://github.com/user-attachments/assets/90cc4c67-3f67-4130-9e9f-1840024f289a)

## 5. Generar y Guardar la Tabla de Transacciones
Finalmente, generamos las transacciones, incluyendo algunas fraudulentas, y las almacenamos en la tabla transactions.
Descripción del código:
create_transactions_table: Función que genera un conjunto de transacciones. Incluye la creación de algunas transacciones fraudulentas y la asignación de una sucursal para las transacciones que ocurren en tiendas físicas.

# Verificación y Cierre
Para asegurarnos de que todo está configurado correctamente, verificamos las tablas en la base de datos SQLite3 y cerramos la conexión.
![image](https://github.com/user-attachments/assets/a558a345-65ca-4d1e-9f26-9e8133a36c29)

Descripción del código:
Verificación: Este código imprime una lista de las tablas que se han creado en la base de datos.
Cierre de conexión: Se cierra la conexión a la base de datos SQLite3.

![image](https://github.com/user-attachments/assets/8eaf1eb7-f3d4-4c2b-a2ba-ef655913a14a)



