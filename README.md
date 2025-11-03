# Proyecto 4 - Banking Marketing Campaign 📊

## 📖 Descripción del Proyecto
Este proyecto tiene la finalidad de aplicar los conocimientos aprendidos hasta el momento en el curso de Data & Analytics.
Para eso se realizar un análisis exploratorio de los datos en los dos documentos adjuntados en este repositorio: 
1. bank-additional.csv
2. customer-details.xlsx

Estos conjuntos de datos están relacionados con campañas de marketing directo de una institución bancaria portuguesa. Las campañas de marketing se basaron en llamadas telefónicas. A menudo, se requería más de un contacto con el mismo cliente para determinar si el producto (depósito a plazo bancario) sería suscrito o no. Las columnas que tenemos en el primer dataset ('bank-additional.csv') son:
1. age: La edad del cliente.
2. job: La ocupación o profesión del cliente.
3. marital: El estado civil del cliente.
4. education: El nivel educativo del cliente.
5. default: Indica si el cliente tiene algún historial de incumplimiento de pagos (1: Sí, 0: No).
6. housing: Indica si el cliente tiene un préstamo hipotecario (1: Sí, 0: No).
7. loan: Indica si el cliente tiene algún otro tipo de préstamo (1: Sí, 0: No).
8. contact: El método de contacto utilizado para comunicarse con el cliente.
9. duration: La duración en segundos de la última interacción con el cliente.
10. campaign: El número de contactos realizados durante esta campaña para este cliente.
11. pdays: Número de días que han pasado desde la última vez que se contactó con el cliente durante esta campaña.
12. previous: Número de veces que se ha contactado con el cliente antes de esta campaña.
13. poutcome: Resultado de la campaña de marketing anterior.
14. emp.var.rate: La tasa de variación del empleo.
15. cons.price.idx: El índice de precios al consumidor.
16. cons.conf.idx: El índice de confianza del consumidor.
17. euribor3m: La tasa de interés de referencia a tres meses.
18. nr.employed: El número de empleados.
19. y: Indica si el cliente ha suscrito un producto o servicio (Sí/No).
20. date: La fecha en la que se realizó la interacción con el cliente.
21. contact_month: Mes en el que se realizó la interacción con el cliente durante la campaña de marketing.
22. contact_year: Año en el que se realizó la interacción con el cliente durante la campaña de marketing.
23. id_: Un identificador único para cada registro en el dataset.

El segundo set de datos ('customer-details.xlsx') es un archivo Excel que nos da información sobre las características demográficas y comportamiento de compra de los clientes del banco. Este Excel consta de 3 hojas de trabajo diferentes, en cada una de ellas tenemos los clientes que entraron en el banco en diferentes años. Sus columnas son:
1. Income: Representa el ingreso anual del cliente en términos monetarios.
2. Kidhome: Indica el número de niños en el hogar del cliente.
3. Teenhome: Indica el número de adolescentes en el hogar del cliente.
4. Dt_Customer: Representa la fecha en que el cliente se convirtió en cliente de la empresa.
5. NumWebVisitsMonth: Indica la cantidad de visitas mensuales del cliente al sitio web de la empresa.
6. ID: Identificador único del cliente.

Además, hay 4 requisitos para realizar este proyecto:
1. Transformación y limpieza de los datos.
2. Análisis descriptivo de los datos.
3. Visualización de los datos.
4. Informe explicativo del análisis.

El documento final tiene los siguientes apartados:
1. Importación de Librerías.
2. Carga de Datos: La carga de los datos de los dos archivos introducidos anteriormente.
3. Pre-procesamiento y Limpieza de Datos: Teniendo en cuenta, que como está explicado en el último apartado, la calidad de los datos es buena.
4. Fusión de Datasets: A partir del 'ID'. Adicionalmente, como también está explicado en el último apartado, la fusión es exitosa, con un match del 100%.
5. Análisis Exploratorio de Datos (EDA): Este apartado se analiza en profundidad en la sección de Resultados y Conclusiones.
6. Conclusiones Preliminares: Son solo los puntos claves y conslusiones preliminares ya que las conclusiones se explican en profundidad también en la sección de Resultados y Conclusiones.

## 📋 Estructura del Proyecto

- **Carpeta_Archivos:** Contiene los 3 archivos proporcionados: "bank-additional.csv", "customer-details.xlsx" y "DataProject_ Proyecto EDA con Python.docx".
- **proyecto_eda_banking.ipynb:** El archivo que contiene todos los pasos y el código para realizar la exploración de los datos cumpliendo los 4 requisitos presentados.
- **README.md:** Contiene la descripción del proyecto.

## 🛠 Instalación y Requisitos

Este proyecto usa:

- Visual Studio Code: Para realizar el código del proyecto.
- Las siguientes librerías: pandas, numpy, matplotlib y seaborn.
- Finalmente, los dos archivos proporcionados al inicio.

## 📊 Resultados y Conclusiones

Primero, es crucial reconocer que la tasa de suscripción es de solo el 11.27%. Este desequilibrio significativo limita inherentemente la calidad potencial de cualquier análisis predictivo. Una proporción más equilibrada, como 60%-40% o idealmente 50%-50%, produciría resultados más sólidos y fiables.

Segundo, un hallazgo notable de las visualizaciones en la Sección 5.3, 'Variables Demográficas', es que los 'Estudiantes' y los 'Jubilados' muestran las tasas de suscripción más altas, a pesar de representar solo aproximadamente el 7% de los clientes contactados. Basándome en esta observación, recomiendo que el banco portugués implemente campañas de marketing dirigidas específicamente a atraer nuevos clientes jóvenes y jubilados, ya que estos grupos demuestran la mayor propensión a suscribirse.

Tercero, el análisis en la Sección 5.5, 'Variables de la Campaña', revela dos puntos importantes. Por un lado, y de manera natural, las llamadas con mayor duración se correlacionan con tasas de suscripción más elevadas. Esta relación es intuitiva, ya que las llamadas más largas probablemente indican un mayor interés del cliente en obtener más información sobre el producto (en este caso, un depósito a plazo). Por otro lado, el método de contacto también juega un papel importante. El contacto por teléfono móvil demuestra una tasa de suscripción más alta en comparación con el teléfono fijo. Por lo tanto, mi segunda recomendación es priorizar el contacto con los clientes a través del teléfono móvil en lugar del teléfono fijo.

Finalmente, un hallazgo muy relevante surge de la Sección 5.6, 'Análisis Temporal': la tasa de éxito por mes. Los tres meses con las tasas de éxito más altas son octubre, enero y noviembre (en ese orden). Por el contrario, septiembre, mayo y marzo muestran las tasas de éxito más bajas. Por lo tanto, recomiendo implementar campañas temáticas navideñas con promociones especiales para capitalizar aún más las tasas de éxito ya elevadas durante octubre, enero y noviembre."

## 🔄 Próximos Pasos

A partir de este análisis exploratorio, se sugieren una serie de próximos pasos para mejorar aún más las estrategias de marketing del banco. En primer lugar, se recomienda realizar pruebas más exhaustivas para validar las hipótesis generadas a partir de este análisis, como la relación entre la duración de la llamada y la probabilidad de suscripción ya que, como mencionado previamente, la desproporción en la tasa de éxito siendo solo del 11.27% hace que el análisis predictivo no sea tan fiable. Profundizar en el análisis de segmentos de clientes específicos, tales como estudiantes y jubilados. 
Finalmente, todos los hallazgos de este análisis y los resultados de los próximos pasos deben utilizarse para desarrollar una estrategia de marketing integral que abarque todos los aspectos del proceso, desde la segmentación precisa de los clientes hasta la medición detallada de los resultados obtenidos. Mi recomendación principal sería una campaña orientada principalmente al sector jóven (estudiantes) ya que son los que tienen mayor tasa de éxito pero son el segmento más pequeño. Además, son el segmento con mayor potencial por el hecho de que tienen más longevidad estimada comparada a los demás segmentos que tienen mayor edad.
Adicionalmente, sería muy recomendable utilizar los datos al finalizar esta nueva compaña y compararlos con estos para ver lo correlación.

## 🤝 Contribuciones

Las contribuciones son bienvenidas :)

##  ✒ Autores

- Marcos Herrera
