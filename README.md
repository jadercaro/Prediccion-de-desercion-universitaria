## Descripción del Repositorio

Proyecto propuesto para el curso de modelos y simulación 2 de la Universidad de Antioquia
Este repositorio se enfoca en la exploración y comparación de distintos métodos de machine learning y deep learning para la predicción de deserción universitaria. Se desarrollará un modelo de clasificación que consta de tres clases principales: "desertor", "graduado" o "matriculado". El objetivo es investigar y analizar la eficacia de diferentes algoritmos en la tarea de identificar patrones y factores predictivos de la deserción en instituciones académicas.
![imagen de referencia](https://github.com/jadercaro/Prediccion-de-desercion-universitaria/assets/96452959/55895259-8659-4218-a9ff-c32dd66a98c3)


**URL del repositorio:** [https://archive.ics.uci.edu/dataset/697/predict+students+dropout+and+academic+success]

### Variables

- **Variable objetivo:** Estado del estudiante (desertor, graduado, matriculado)
- **Variables predictoras:**
## **Descripción de las variables del conjunto de datos:**

| Variable                                   | Descripción                                                                                                 |
|--------------------------------------------|-------------------------------------------------------------------------------------------------------------|
| Marital Status                             | Estado civil del estudiante.                                                                                |
| Application mode                           | Modalidad de ingreso a un programa educativo.                                                                |
| Application order                          | Orden de solicitud (0 - primera opción; 9 - última opción).                                                  |
| Course                                     | Programas educativos en los que están matriculados los estudiantes.                                          |
| Daytime/evening attendance                | Tipo de asistencia: Diurna o Nocturna.                                                                      |
| Previous qualification                     | Tipo de educación anterior obtenida por los estudiantes.                                                      |
| Previous qualification (grade)            | Nota de calificación anterior (entre 0 y 200).                                                               |
| Nationality                                | Nacionalidad del estudiante.                                                                                |
| Mother's qualification                    | Calificación de la madre.                                                                                   |
| Father's qualification                    | Calificación del padre.                                                                                     |
| Mother's occupation                        | Profesión de la madre.                                                                                      |
| Father's occupation                        | Profesión del padre.                                                                                        |
| Admission grade                            | Nota de admisión (entre 0 y 200).                                                                           |
| Displaced                                  | Desplazados (1 - sí; 0 - no).                                                                               |
| Educational special needs                 | Necesidades educativas especiales (1 - sí; 0 - no).                                                          |
| Debtor                                     | Deudor (1 - sí; 0 - no).                                                                                    |
| Tuition fees up to date                    | Matrículas al día (1 - sí; 0 - no).                                                                         |
| Gender                                     | Género (1 - masculino; 0 - femenino).                                                                       |
| Scholarship holder                         | Tiene beca (1 - sí; 0 - no).                                                                                |
| Age at enrollment                          | Edad del estudiante al momento de la inscripción.                                                            |
| International                              | Internacional (1 - sí; 0 - no).                                                                             |
| Curricular units 1st sem (credited)        | Número de unidades curriculares acreditadas en el 1er semestre.                                               |
| Curricular units 1st sem (enrolled)       | Número de unidades curriculares matriculadas en el 1er semestre.                                              |
| Curricular units 1st sem (evaluations)    | Número de evaluaciones a unidades curriculares en el 1er semestre.                                            |
| Curricular units 1st sem (approved)       | Número de unidades curriculares aprobadas en el 1er semestre.                                                 |
| Curricular units 1st sem (grade)          | Promedio de calificaciones en el 1er semestre (entre 0 y 20).                                                  |
| Curricular units 1st sem (without evaluations) | Número de unidades curriculares sin evaluaciones en el 1er semestre.                                       |
| Curricular units 2nd sem (credited)       | Número de unidades curriculares acreditadas en el 2do semestre.                                               |
| Curricular units 2nd sem (enrolled)       | Número de unidades curriculares matriculadas en el 2do semestre.                                              |
| Curricular units 2nd sem (evaluations)    | Número de evaluaciones a unidades curriculares en el 2do semestre.                                            |
| Curricular units 2nd sem (approved)       | Número de unidades curriculares aprobadas en el 2do semestre.                                                 |
| Curricular units 2nd sem (grade)          | Promedio de calificaciones en el 2do semestre (entre 0 y 20).                                                  |
| Curricular units 2nd sem (without evaluations) | Número de unidades curriculares sin evaluaciones en el 2do semestre.                                       |
| Unemployment rate                         | Tasa de desempleo (%).                                                                                      |
| Inflation rate                            | Tasa de inflación (%).                                                                                      |
| GDP                                       | Producto Interno Bruto (GDP).                                                                              |

### Relación variables Númericas - Númericas

![Untitled](https://github.com/jadercaro/Prediccion-de-desercion-universitaria/assets/15114373/786a5310-8c74-445b-85b5-7bf69a27c948)


## Relación variables Categóricas - Categóricas
![imagen](https://github.com/jadercaro/Prediccion-de-desercion-universitaria/assets/96452959/8c66190f-122a-4890-9dbb-073e2d398229)

## Modelos 
|Modelo               |   Paramétros          |Resultado              |
|---------------------|-----------------------|-----------------------|
|Regresión logistica  |tasa aprendizaje = 3   |Precisión:       82.01%|
|K-Vecinos cercanos   |vecinos = 10           |Precisión:       71.53%|
|Ventana de Parzen    |H = 0.5                |Precisión:       68.81%|




