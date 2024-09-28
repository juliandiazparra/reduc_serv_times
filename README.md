# Estableciendo KPI’s en una prestadora de telecomunicaciones 
En este proyecto tomamos los datos del area de soporte técnico de una prestadora de telecomunicaciones en el departamento del Cesar. Los datos están compuestos por las solicitudes de servicio que registran los usuarios y las visitas que hacen los técnicos para solucionarlas. 

## Objetivo:
El proyecto busca establecer los indicadores de desempeño relevantes (KPI, por sus siglas en inglés). Con esto, se definen estándares para el desempeño de los trabajadores y se desarrolló una escala para clasificarlos de acuerdo a su rendimiento. 

## Datos 
Se utilizó la data recopilada a través del software Mikrowisp, la cual tiene información de los tickets abiertos por los usuarios y la resolución de estos por parte del área técnica. Para enriquecer esta data, se implementaron dos procesos paralelos: un formulario para el registro de material utilizado y otra encuesta de satisfacción para que los usuarios califiquen al personal que les atendió.

##Métodos
Los datos eran descargados del servidor de la empresa con cierta periodicidad. Se empleó Python para hacer la limpieza y análisis de los datos. Los siguientes fueron los pasos para el manejo de los datos:
**1. Importación, limpieza y centralización de datos **
Se importaron los datos, se eliminaron valores faltantes o outliers, se clasificaron variables categóricas y se formatearon los string, fechas y números para su adecuada manipulación. Se exportaron los datos a formatos .csv agrupados por años

**2. Staging**
Con los datos limpios y procesados, se ensamblan las bases de datos con la información necesaria y se exportan estas bases de trabajo. Estas son actualizadas con los nuevos datos para garantizar un análisis actualizado. De esta manera, se procede al…

**3. Análisis**
Se definieron 3 indicadores principales: 
- Porcentaje de encuestas de material respondidas
- Satisfacción del cliente
- Tiempo de resolución

Estos fueron calculados y se realizaron visualizaciones para observar su evolución en el tiempo. También, se hicieron visualizaciones necesarias para la operación, las cuales incluían comparaciones durante el mes y la semana del desempeño del personal. Finalmente, se automatizaron reportes mensuales para la retroalimentación con los colaboradores.

**4. Visualización**
Se exportaron 3 tipos de visualizaciones:
- Reportes de Excel mensuales por cada trabajador. Resumían principales resultados del mes y calculaban su cumplimiento y desempeño.
- Un reporte semanal con los principales resultados.
- Un dashboard con el resumen del área técnica para que la coordinación pudiera tomar decisiones en tiempo real.

## Resultados
<img width="572" alt="tasas_categoria_servicio" src="https://github.com/user-attachments/assets/72ac95a0-54b7-41ef-8e1b-5eba02adc976">

Se calcularon las tasas de solicitudes de cada categoría como el porcentaje del total de usuarios.

<img width="679" alt="Captura de pantalla 2024-09-28 a la(s) 1 52 57 p m" src="https://github.com/user-attachments/assets/1c4cb15b-65f4-4cbe-bd5b-7820b1767e21">

Se diseñaron 4 indicadores para medir a los técnicos y se definieron niveles de desempeño.

<img width="590" alt="Captura de pantalla 2024-09-28 a la(s) 1 54 37 p m" src="https://github.com/user-attachments/assets/b6988d75-4fcf-459e-a15e-2a6d8d611d53">

Con esto, se automatizó la producción de reportes mensuales para que la gerencia y coordinación técnicas pudieran tomar decisiones.


<img width="430" alt="Reducción tiempos" src="https://github.com/user-attachments/assets/0646dd7b-20d3-4916-98e1-0098e3ef65fd">

**Resultado principal:**
Se puede observar que los tiempos de respuesta para todas las categorías de solicitudes se redujeron en alrededor de un 40 a 50% al cabo de 3 meses de implementar las medidas.
