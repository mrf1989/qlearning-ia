PROJECTO DE INTELIGENCIA ARTIFICIAL - APRENDIZAJE POR REFUERZO - CURSO 2019/20
==============================================================================
Este documento tiene por objetivo servir de manifiesto del trabajo realizado.
Se incluye un resumen del código fuente y un manual de uso rápido de su UI.

Fecha: 2020-06-21
Versión: 1.0

/------------ INDICE------------\
| 1. Objeto                     |
| 2. Autores                    |
| 3. Resumen del código fuente  |
|    3.1. Librerías requeridas  |
|    3.2. Clases implementadas  |
| 4. Guía rápida de uso         |
| 5. Mejoras			|
\-------------------------------/

1. OBJETO

Projecto realizado para la asignatura de Inteligencia Artificial de la
titulación Grado en Ingeniería Informática - Ingeniería del Software de la
Universidad de Sevilla. Curso Académico 2019/2020.

En este trabajo se realiza un acercamiento al algoritmo de aprendizaje por
refuerzo Q-Learning.

2. AUTORES

 - Muñoz Aranda, Alejandro José <alemunara@alum.us.es>
 - Ruano Fernández, Mario <mruano@us.es>

3. RESUMEN DEL CÓDIGO FUENTES

3.1. Librerías requeridas
 - numpy
 - random
 - matplotlib.pyplot
 - graphviz
 - tkinter
 - PIL
 - timeit

3.2. Clases implementadas
 - Board: representa y modula el entorno. En el caso de este trabajo se hace
   referencia a un tablero de casillas únicas numeradas.
 - QLearningAlgorithm: implementa el algoritmo de entrenamiento Q-Learning
   basado únicamente en exploración.
 - QLearningVariantAlgorithm: implemente variante del algoritmo de
   entrenamiento Q-Learning basado en exploración-explotación.

4. GUÍA RÁPIDA DE USO

 - Pasos previos:
	- Es recomendable tener instalado el entorno de ejecución Anaconda 3 y
	  Jupyter Notebook.
	- Contar con las librerías Python indicadas en el punto 3.1.
        - Tener instalado Graphviz en el sistema y referenciado en el PATH.

 - Abrir el archivo "q-learning.ipynb" que se adjunta con este trabajo desde
   Jupyter Notebook.

 - Ejecutar los bloques de código correspondientes al epígrafe "Código fuente":
	- Librerías utilizadas
	- Clase Board (Tablero)
	- Clase QLearningAlgorithm
	- Clase QLearningVariantAlgorithm
	- Funciones Auxiliares

 - El usuario puede ejecutar el código correspondiente a la Fase 1 y Fase 2 que
   se especifica en el enunciado desde el propio notebook.
	- La Fase 1 está indicada en el archivo "q-learning.ipynb"
	- La Fase 2 está indicada en el archivo "q-learning.ipynb"

 - Lanzar la interfaz gráfica de usuario:
	- Suficiente con ejecutar el bloque de código que se especifica bajo el
	  título "Interfaz de usuario: ejecutar y usar".
	- Para hacer uso de la implementación de Fase 1: QLearning
	- Para hacer uso de la implementación de Fase 2: QLearning variado
	- Para experimentar con la Fase 3: Fase 3.

 - El usuario puede seguir fácilmente los pasos indicados por la interfaz de
   usuario.

 - Si se experimenta algún error extraño en la interfaz, es recomendable cerrar
   esta y relanzar el bloque de código fuente de "Interfaz de usuario: ejecutar
   y usar".

 - Es recomendable, para la Fase 3, utilizar la interfaz gráfica de usuario, ya
   que implementa mucha más información que la consola de Jupyter Notebook,
   como un visor gráfico de representación del tablero y el camino tomado por
   el agente, el tiempo de ejecución o las gráficas de rendimiento.

 - El botón "Reiniciar" sirve para volver a la vista de inicio y empezar una
   nueva configuración de entrenamiento sin necesidad de relanzar el bloque de
   código de Jupyter Notebook.

5. MEJORAS

Este trabajo incorpora una serie de mejoras adicionales que no venían indicadas
como requisitos en el enunciado, pero que facilitan el uso de la herramienta y
la aplicación del trabajo experimental:

 - Visor gráfico para representar el tablero y el camino tomado por el agente.
 - Resultado del tiempo de ejecución para la medición y la realización de
   comparativas entre algoritmos y configuraciones de parámetros.