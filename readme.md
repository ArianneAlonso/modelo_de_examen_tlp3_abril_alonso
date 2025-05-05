Autor
Arianne Alonso

Descripción del Proyecto
Este proyecto tiene como objetivo practicar el análisis de datos utilizando la librería pandas y simular operaciones similares a consultas SQL sobre un conjunto de datos. El proyecto se realiza sobre un dataset de calificaciones de estudiantes, aplicando diversas técnicas de limpieza, análisis y visualización de datos.

Actividades Realizadas
1. Importación del Dataset con Pandas
Se importó la librería pandas para cargar el archivo CSV que contiene los datos de las calificaciones en un DataFrame, que es la estructura de datos fundamental para el análisis.

2. Exploración Inicial de los Datos
Se utilizó la función .info() para obtener un resumen general del dataset, como los tipos de datos y los valores nulos, y .describe() para calcular las estadísticas descriptivas de las columnas numéricas.

3. Limpieza y Normalización de los Datos
Asistencia: Se corrigió la columna de "Asistencia" para garantizar que todos los valores no superaran el 100%. Además, se añadió el símbolo de porcentaje en las entradas qe no lo contenian.

Capitalización: Se normalizó la capitalización de los nombres de los estudiantes y de las materias, asegurando un formato consistente (por ejemplo, capitalizando la primera letra de cada palabra).

Valores Nulos: Se reemplazaron los valores vacíos.

4. Obtención de Estadísticas Descriptivas
Se calcularon nuevamente las estadísticas descriptivas para observar el impacto de la limpieza de datos. Esto incluyó la media, desviación estándar, valores mínimo y máximo, así como los percentiles para las columnas numéricas.

5. Visualización de los Datos con Matplotlib
Se crearon gráficos utilizando la librería matplotlib para visualizar la distribución de las calificaciones y la asistencia:

Se generaron histogramas para visualizar la distribución de las calificaciones.

Se creó un gráfico de barras para mostrar la distribución de la asistencia de los estudiantes.

6. Exportación a Base de Datos SQLite
Finalmente, el DataFrame procesado se guardó en una base de datos SQLite. Esto permite almacenar los datos de forma estructurada y realizar consultas eficientes para su posterior análisis.

Instalación y Uso
Sigue los pasos a continuación para ejecutar este proyecto en tu máquina local:

1. Clonar el repositorio

git clone https://github.com/ArianneAlonso/modelo_de_examen_tlp3_abril_alonso.git
2. Ingresar a la carpeta del proyecto

cd modelo_de_examen_tlp3_abril_alonso
3. Crear un entorno virtual (si no existe)

python -m venv modelodeexamen
4. Activar el entorno virtual
En Windows:

modelodeexamen\Scripts\activate
En MacOS/Linux:


source modelodeexamen/bin/activate
5. Instalar las dependencias

pip install -r requirements.txt

6. Ejecutar el archivo Jupyter Notebook
Abre el archivo main.ipynb en VSCode. Asegúrate de seleccionar el entorno virtual df como kernel de Python en la esquina superior derecha de VSCode.