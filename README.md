# Integrantes : 
 - Jhon Jader Caro Sanchez
 - Jagler David Velasquez Velasquez
 - Alejandro Arias Ortiz
 


## Descripción del Repositorio

Proyecto propuesto para el curso de modelos y simulación 2 de la Universidad de Antioquia
Este repositorio se enfoca en la exploración y comparación de distintos métodos de machine learning y deep learning para la predicción de deserción universitaria. Se desarrollará un modelo de clasificación que consta de tres clases principales: "desertor", "graduado" o "matriculado". El objetivo es investigar y analizar la eficacia de diferentes algoritmos en la tarea de identificar patrones y factores predictivos de la deserción en instituciones académicas.
![imagen de referencia](https://github.com/jadercaro/Prediccion-de-desercion-universitaria/assets/96452959/55895259-8659-4218-a9ff-c32dd66a98c3)


**URL del repositorio:** [https://archive.ics.uci.edu/dataset/697/predict+students+dropout+and+academic+success]

### Variables

- **Variable objetivo:** Estado del estudiante (desertor y no-desertor)
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

### Relación variables Númericas - Númericas (Correlación)

![Untitled](https://github.com/jadercaro/Prediccion-de-desercion-universitaria/assets/15114373/786a5310-8c74-445b-85b5-7bf69a27c948) 
![imagen](https://github.com/jadercaro/Prediccion-de-desercion-universitaria/assets/96452959/62183760-b665-4f62-a398-545f04d9eca6)

## Relación variables Categóricas - Categóricas (V-Cramer)
![imagen](https://github.com/jadercaro/Prediccion-de-desercion-universitaria/assets/96452959/b3d0cb86-ed4a-4535-8c39-149b1184fdb7) 





## Conclusiones de Correlaciones

| No. | Comparación                                            | Correlación | Target  | Resultado |
|-----|--------------------------------------------------------|-------------|---------|-----------|
| 1   | Credited 1 ➡ Enrolled 1 : Credited 2        | 0.77 : 0.94       | 0.029    | Eliminar🔴       |
| 2   | Enrolled 1 ➡ Credited 1 : Approved 1 : Credited 2 : Enrolled 2             | 0.77 : 0.77 : 0.75 : 0.94 | 0.124    | Eliminar🔴       |
| 3   | Evaluations 1 ➡ Evaluations 2          | 0.78        | 0.090   | Eliminar🔴       |
| 4   | Approved 1 ➡ Approved 2 : Enrolled 1                 | 0.9 : 0.77         | 0.480    | Conservar🟢        |
| 5   | Grade 1 ➡ Grade 2                      | 0.84        | 0.480    |   Eliminar🔴         |
| 6   | Credited 2 ➡ Credited 1 : Enrolled 1             | 0.94        | 0.033   | Conservar🟢          |
| 7   | Enrolled 2 ➡ Enrolled 1                | 0.94        | 0.141    | Conservar🟢          |
| 8   | Evaluations 2 ➡ Evaluations 1          | 0.78        | 0.154   | Conservar🟢          |
| 9   | Approved 2 ➡ Approved 1 : Grade 2               | 0.9 : 0.76         | 0.569   | Eliminar🔴         |
| 10  | Grade 2 ➡ Grade 1 : Approved 2                   | 0.84 : 0.76        | 0.571   | Conservar🟢       |
| 11  | Daytime/evening attendance ➡ Course                    | 0.998       | 0.078   | Eliminar🔴         |
| 12  | Course ➡ Daytime/evening attendance                    | 0.998       | 0.253   | Conservar🟢          |
| 13  | Nationality ➡ International                            | 0.998       | 0.000   | Eliminar🔴         |
| 14  | International ➡ Nationality                            | 0.998       | 0.000   | Eliminar🔴         |
| 15  | Educational special needs                            | -      | 0.000   | Eliminar🔴         |





