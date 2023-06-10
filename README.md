# cotizaciones_dolar_argentina
Proyecto de  Data Engineering
# Tareas realizadas por el DAG

![Captura de pantalla](images/dags.png)

Aquí puedes agregar una descripción o detalles adicionales sobre las tareas realizadas por el DAG.

## Tareas del DAG

- `task_1`: Conexión a la base de datos - Esta tarea establece una conexión a la base de datos de Redshift. Utiliza la función `conexion_redshift` y recibe como argumento la fecha (`{{ ds }}`) y la hora de ejecución (`{{ execution_date.hour }}`).

- `task_2`: Crear tabla - Esta tarea crea una tabla en la base de datos. Utiliza la función `creacion_de_tablas`.

- `task_3`: Extraer datos - Esta tarea extrae datos de alguna fuente. Utiliza la función `extraer_data` y recibe como argumento la fecha (`{{ ds }}`) y la hora de ejecución (`{{ execution_date.hour }}`).

- `task_4`: Cargar tabla - Esta tarea carga los datos extraídos en la tabla previamente creada. Utiliza la función `cargar_datos` y recibe como argumento la fecha (`{{ ds }}`) y la hora de ejecución (`{{ execution_date.hour }}`).

- `task_5`: Enviar correo de confirmación - Esta tarea envía un correo electrónico de confirmación. Utiliza la función `enviar`.



