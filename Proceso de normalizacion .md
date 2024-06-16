### Importancia de Mostrar Usuarios sin Normalización Previo a la Normalización

En el proceso de normalización de datos, es fundamental comprender la estructura y la calidad de los datos originales antes de aplicar cualquier técnica de normalización. La visualización inicial de los datos sin alteraciones proporciona una base clara y concreta sobre la cual se pueden fundamentar las decisiones y acciones posteriores en el contexto del tratamiento de datos.

#### Claridad en la Interpretación de los Datos Originales

Antes de realizar cualquier transformación o ajuste en los datos, es esencial visualizar y comprender los datos en su forma cruda o sin normalizar. Esta práctica permite a los analistas y científicos de datos:

- **Identificar Patrones y Tendencias:** Observar cómo están estructurados los datos y qué tipos de información contienen.
  
- **Evaluar la Calidad de los Datos:** Detectar posibles problemas como valores atípicos, datos faltantes o inconsistencias que pueden afectar la calidad y confiabilidad de los resultados analíticos.

- **Entender la Distribución de los Datos:** Tener una idea clara de la distribución estadística de los datos, lo cual es crucial para seleccionar las técnicas de normalización más adecuadas.

#### Base para la Normalización Eficiente

Mostrar los datos en su forma original proporciona una base sólida para la implementación efectiva de técnicas de normalización posteriormente. Al tener una comprensión clara de los datos sin procesar, los equipos de análisis pueden:

- **Seleccionar la Técnica de Normalización Adecuada:** Basándose en la distribución y características de los datos, elegir entre técnicas como la normalización min-max, la estandarización z-score u otras más específicas según las necesidades del análisis.

- **Optimizar el Proceso de Transformación:** Evitar errores comunes y pérdida de información relevante al aplicar la técnica de normalización más adecuada para los datos en cuestión.

- **Garantizar Resultados Precisos:** Asegurar que los resultados finales del análisis y modelado estén fundamentados en datos que han sido correctamente preparados y ajustados.






| Codigo_Empleado | Nombre     | Apellido    | Edad | Cedula   | Profesion                   | Empresa               | Direccion               | Telefono   | Email                           | Fecha_Ingreso | Salario | Departamento          | Cargo                   | Jefe_Inmediato   | Nivel_Riesgo | Turno    | Dias_Laborales     | Horas_Trabajo_Semanales | Fecha_Nacimiento | Genero    | Estado_Civil | Numero_Hijos | Pais               | Ciudad            |
|-----------------|------------|-------------|------|----------|-----------------------------|-----------------------|-------------------------|------------|---------------------------------|--------------|---------|-----------------------|-------------------------|------------------|--------------|----------|--------------------|-------------------------|------------------|-----------|--------------|--------------|--------------------|-------------------|
| 57              | Diego      | Ramírez     | 27   | 99990000 | Analista de Datos           | DataAnalytics         | 3434 Calle Treinta y Siete | 555-7879   | diego.ramirez@example.com        | 26/10/2022   | 61000.0 | Tecnología            | Analista de Datos       | Andrea Gómez     | 3            | Nocturno | Lunes a Viernes    | 40                      | 26/09/1995       | Masculino | Soltero      | 0            | México             | Monterrey         |
| 58              | Lucía      | Pérez       | 31   | 11112222 | Ingeniera Civil             | EngineeringSolutions  | 3535 Calle Treinta y Ocho | 555-8081   | lucia.perez@example.com          | 27/08/2021   | 63000.0 | Construcción          | Ingeniera Civil         | José Rodríguez   | 3            | Diurno   | Lunes a Viernes    | 40                      | 27/11/1990       | Femenino  | Casada       | 2            | España             | Madrid            |
| 59              | Gabriel    | Martínez    | 29   | 22223333 | Analista Financiero         | FinancialConsulting   | 3636 Calle Treinta y Nueve | 555-8283   | gabriel.martinez@example.com      | 28/12/2020   | 60000.0 | Finanzas               | Analista Financiero     | María González   | 3            | Diurno   | Lunes a Viernes    | 40                      | 28/09/1992       | Masculino | Soltero      | 0            | Chile              | Valparaíso        |
| 60              | Marina     | Gómez       | 32   | 33334444 | Bióloga Marino              | MarineBiologyResearch | 3737 Calle Cuarenta      | 555-8485   | marina.gomez@example.com          | 29/05/2019   | 58000.0 | Investigación         | Bióloga Marino          | Juan Ramírez     | 3            | Diurno   | Lunes a Viernes    | 40                      | 29/12/1989       | Femenino  | Casada       | 2            | Ecuador            | Guayaquil         |
| 61              | Sergio     | López       | 33   | 11112221 | Ingeniero Mecánico         | Mecánica Total        | 3838 Calle Cuarenta y Uno | 555-8687   | sergio.lopez@example.com          | 30/10/2023   | 62000.0 | Ingeniería            | Ingeniero Mecánico      | Ana Martínez     | 3            | Diurno   | Lunes a Viernes    | 40                      | 30/12/1990       | Masculino | Soltero      | 0            | Argentina          | Rosario           |
| 62              | Valentina  | Herrera     | 29   | 22223322 | Abogada                     | LawFirm               | 3939 Calle Cuarenta y Dos | 555-8889   | valentina.herrera@example.com     | 29/09/2022   | 60000.0 | Legal                 | Abogada                 | Martín Gutiérrez | 3            | Diurno   | Lunes a Viernes    | 40                      | 29/07/1993       | Femenino  | Soltera      | 0            | Chile              | Santiago          |
| 63              | Diego      | Rojas       | 31   | 33334433 | Ingeniero Eléctrico         | ElectroTech           | 4040 Calle Cuarenta y Tres | 555-9091   | diego.rojas@example.com           | 28/06/2021   | 65000.0 | Ingeniería            | Ingeniero Eléctrico     | Carla Gómez      | 3            | Diurno   | Lunes a Viernes    | 40                      | 28/08/1990       | Masculino | Casado       | 2            | México             | Ciudad de México  |
| 64              | María      | Sánchez     | 30   | 44445555 | Economista                  | Economía Global       | 4141 Calle Cuarenta y Cuatro | 555-9293   | maria.sanchez@example.com         | 27/05/2020   | 67000.0 | Finanzas               | Economista              | Javier Ramírez   | 3            | Diurno   | Lunes a Viernes    | 40                      | 17/03/1991       | Femenino  | Soltera      | 0            | Colombia           | Medellín          |
| 65              | Martín     | García      | 28   | 55556666 | Ingeniero Industrial        | IndustrialSolutions   | 4242 Calle Cuarenta y Cinco | 555-9495   | martin.garcia@example.com          | 26/02/2019   | 64000.0 | Ingeniería            | Ingeniero Industrial    | Laura Martínez   | 3            | Diurno   | Lunes a Viernes    | 40                      | 07/11/1993       | Masculino | Soltero      | 0            | Argentina          | Buenos Aires      |
| 66              | Carolina   | Gómez       | 31   | 66667777 | Consultora de Marketing     | MarketingExperts      | 4343 Calle Cuarenta y Seis | 555-9697   | carolina.gomez@example.com         | 25/11/2018   | 68000.0 | Marketing             | Consultora de Marketing | Juan Rodríguez   | 3            | Diurno   | Lunes a Viernes    | 40                      | 26/07/1990       | Femenino  | Casada       | 1            | Chile              | Santiago          |
| 67              | Pedro      | Rodríguez   | 29   | 77778888 | Abogado Corporativo         | CorporateLaw          | 4444 Calle Cuarenta y Siete | 555-9899   | pedro.rodriguez@example.com        | 24/12/2017   | 66000.0 | Legal                 | Abogado Corporativo     | Isabel Gutiérrez | 3            | Diurno   | Lunes a Viernes    | 40                      | 15/05/1992       | Masculino | Soltero      | 0            | Uruguay            | Montevideo        |
| 68              | Fernanda   | Martínez    | 27   | 88889999 | Ingeniera Ambiental         | AmbientalTech         | 4545 Calle Cuarenta y Ocho | 555-0101   | fernanda.martinez@example.com      | 23/01/2017   | 65000.0 | Medio Ambiente        | Ingeniera Ambiental     | Carlos Sánchez   | 3            | Diurno   | Lunes a Viernes    | 40                      | 12/09/1994       | Femenino  | Soltera      | 0            | Venezuela          | Caracas           |
| 69              | Pablo      | Fuentes     | 34   | 99990000 | Psiquiatra                  | MentalHealthClinic   | 4646 Calle Cuarenta y Nueve | 555-0303   | pablo.fuentes@example.com          | 22/02/2016   | 69000.0 | Salud                 | Psiquiatra              | Ana Pérez        | 4            | Diurno   | Lunes a Viernes    | 40                      | 21/12/1988       | Masculino | Casado       | 2            | República Dominicana | Santo Domingo     |
| 70              | Natalia    | Gómez       | 26   | 11112222 | Ingeniera de Sistemas       | TechSolutions         | 4747 Calle Cincuenta     | 555-050

### 1 Formalizacion 

La normalización en bases de datos es un proceso fundamental para organizar la estructura de los datos de manera eficiente y sin redundancias, asegurando así la integridad y consistencia de la información. Este ensayo se enfocará en la primera forma normal (1FN), la cual es el primer paso crucial en el proceso de normalización.

#### ¿Qué es la Primera Forma Normal (1FN)?

La Primera Forma Normal (1FN) es un principio básico en el diseño de bases de datos relacionales. Establece que cada columna en una tabla debe contener valores atómicos, es decir, valores indivisibles que no pueden ser descompuestos en partes más pequeñas con significado propio. Esto significa que no debe haber valores repetidos o múltiples valores en una sola celda de una tabla.

En términos más simples, para cumplir con la 1FN, cada celda en una tabla debe contener un solo valor, no una lista de valores separados por comas u otros delimitadores. Esto ayuda a evitar problemas como la redundancia de datos y asegura que cada pieza de información esté representada de manera única en la base de datos.

#### Ejemplo Práctico

Para ilustrar la importancia de la 1FN, consideremos una base de datos simplificada con tres tablas interrelacionadas:

1. **Tabla Personal**
   - Columnas: Cedula, Nombre, Apellido, Nombre compuesto, Edad, Email, Cargo, Fecha_Ingreso, Departamento, Jefe_Inmediato, Nivel_Riesgo, Turno, Fecha_Nacimiento, Género
Here are the first few rows of the dataset provided:

| Cedula   | Nombre     | Apellido   | Nombre compuesto    | Edad | Email                      | Cargo                  | Fecha_Ingreso | Departamento        | Jefe_Inmediato   | Nivel_Riesgo | Turno     | Fecha_Nacimiento | Genero    |
|----------|------------|------------|---------------------|------|----------------------------|------------------------|---------------|---------------------|------------------|--------------|-----------|------------------|-----------|
| 111122   | Diego      | González   | Diego González      | 29   | diego.gonzalez@example.com  | Analista de Datos     | 17/08/2019    | Tecnología          | Andrea Gómez     | 3            | Nocturno  | 18/07/1990       | Masculino |
| 745896   | Pablo      | Fuentes    | Pablo Fuentes       | 34   | pablo.fuentes@example.com   | Psiquiatra            | 22/02/2016    | Salud               | Ana Pérez        | 4            | Diurno    | 21/12/1988       | Masculino |
| 987642   | Matías     | García     | Matías García       | 28   | matias.garcia@example.com   | Ingeniero Industrial | 22/11/2019    | Ingeniería          | Laura Martínez   | 3            | Diurno    | 07/11/1991       | Masculino |
| 1111159  | Diego      | Hernández  | Diego Hernández     | 28   | diego.hernandez@example.com | Analista de Datos     | 09/11/2018    | Tecnología          | Andrea Gómez     | 3            | Nocturno  | 09/08/1993       | Masculino |
| 1456987  | Gabriel    | Fernández  | Gabriel Fernández   | 29   | gabriel.fernandez@example.com| Analista Financiero   | 28/10/2016    | Finanzas            | María González   | 3            | Diurno    | 28/09/1992       | Masculino |
| 1597536  | Diego      | Gómez      | Diego Gómez         | 28   | diego.gomez@example.com     | Analista de Datos     | 26/10/2021    | Tecnología          | Andrea Gómez     | 3            | Nocturno  | 26/09/1993       | Masculino |

This table includes information such as ID (Cedula), full name (Nombre, Apellido), compounded name (Nombre compuesto), age (Edad), email (Email), job title (Cargo), start date (Fecha_Ingreso), department (Departamento), immediate supervisor (Jefe_Inmediato), risk level (Nivel_Riesgo), shift (Turno), date of birth (Fecha_Nacimiento), and gender (Genero).

Let me know if there's anything specific you would like to explore or analyze further!
2. **Tabla Empresa**
   - Columnas: Cod_empresa, Empresa, Dirección, Teléfono, País, Ciudad
     Aquí está la lista de empresas organizada de manera más legible y completa:

| Cod_empresa | Empresa                   | Dirección                         | Teléfono  | País           | Ciudad          |
|-------------|---------------------------|-----------------------------------|-----------|----------------|-----------------|
| 860045828   | AccountingServices        | Calle Contable 111                | 555-1112  | Colombia       | Bogotá          |
| 860045753   | AdminCorp                 | 789 Calle Tercera                 | 555-9101  | Argentina      | Buenos Aires    |
| 860045855   | AIExperts                 | 1040 Calle Central                | 555-1040  | Colombia       | Cali            |
| 860045778   | AmbientalTech             | 2525 Calle Veintiocho            | 555-6061  | Venezuela      | Maracaibo       |
| 860045858   | AppDev                    | 1100 Calle Este                   | 555-1100  | Chile          | Santiago        |
| 860045836   | BackDev                   | 6768 Calle Norte                  | 555-6768  | Colombia       | Cali            |
| 860045853   | BIConsulting              | 1001 Calle Este                   | 555-1001  | Argentina      | Córdoba         |
| 860045888   | BIConsults                | 1780 Calle Sur                    | 555-1780  | Chile          | Valparaíso      |
| 860045891   | BIExperts                 | 2100 Calle Este                   | 555-2100  | Chile          | Valparaíso      |
| 860045838   | BigDataCorp               | 7172 Calle Este                   | 555-7172  | Uruguay        | Montevideo      |
| 860045883   | BigDataExperts            | 1640 Calle Central                | 555-1640  | España         | Madrid          |
| 860045770   | BioResearch               | 1717 Calle Veinte                 | 555-4445  | Cuba           | La Habana       |
| 860045835   | BizAnalysis               | 6566 Calle Central                | 555-6566  | México         | Monterrey       |
| 860045862   | BizAnalysts               | 1180 Calle Sur                    | 555-1180  | Colombia       | Bogotá          |
| 860045873   | BlockchainExperts         | 1420 Calle Oeste                  | 555-1420  | Argentina      | Córdoba         |
| 860045758   | BuildIt                   | 505 Calle Octava                  | 555-2021  | Venezuela      | Caracas         |
| 860045815   | ChemicalEngineering       | Avenida Química 333               | 555-3334  | Colombia       | Bogotá          |
| 860045798   | CivilEngineering          | Calle Construcción 333            | 555-3334  | Chile          | Santiago        |
| 860045826   | CivilEngineers            | Calle Ingeniería 1010             | 555-1011  | Chile          | Santiago        |
| 860045764   | Clinica Dental             | 1111 Calle Catorce               | 555-3233  | Honduras       | Tegucigalpa     |
| 860045772   | Clinica Salud Mental      | 1919 Calle Veintidós             | 555-4849  | Chile          | Santiago        |
| 860045825   | ClinicalPsychology        | Avenida Psicología 444            | 555-4445  | Ecuador        | Quito           |
| 860045870   | CloudExperts              | 1360 Calle Norte                  | 555-1360  | Perú           | Lima            |
| 860045766   | Comercializadora          | 1313 Calle Dieciséis              | 555-3637  | Panamá         | Ciudad de Panamá|
| 860045834   | CommExperts               | 6364 Calle Oeste                  | 555-6364  | Perú           | Arequipa        |
| 860045761   | Constructora              | 808 Calle Once                    | 555-2627  | Paraguay       | Asunción        |
| 860045768   | ConsultingGroup           | 1515 Calle Dieciocho             | 555-4041  | Puerto Rico    | San Juan        |
| 860045784   | Contabilidad Profesional  | 3232 Calle Treinta y Cinco        | 555-7475  | Colombia       | Bogotá          |
| 860045777   | CorporateLaw              | 2424 Calle Veintisiete           | 555-5859  | Uruguay        | Punta del Este  |
| 860045752   | Creativa SA               | 456 Calle Secundaria              | 555-5678  | México         | Ciudad de México|
| 860045782   | CreativeDesign            | 2929 Calle Treinta y Dos          | 555-6869  | Ecuador        | Quito           |
| 860045893   | CyberExperts              | 2050 Calle Cuarta                 | 555-2050  | Chile          | Santiago        |
| 860045852   | CyberSec                  | 9999 Calle Sur                    | 555-9999  | España         | Barcelona       |
| 860045868   | DataAnalysts              | 1320 Calle Oeste                  | 555-1320  | Chile          | Santiago        |
| 860045786   | DataAnalytics             | 3434 Calle Treinta y Siete        | 555-7879  | México         | Monterrey       |
| 860045898   | DataCorp                  | 2300 Calle Veintinueve           | 555-2300  | España         | Valencia        |
| 860045843   | DataEngineers             | 8182 Calle Este                   | 555-8182  | Perú           | Trujillo        |
| 860045859   | DBAdmins                  | 1120 Calle Oeste                  | 555-1120  | Perú           | Lima            |
| 860045793   | DesignArchitects          | Carrera 60 #70-80                 | 555-8901  | Argentina      | Córdoba         |
| 860045846   | DesignHub                 | 8788 Calle Norte                  | 555-8788  | Argentina      | Buenos Aires    |
| 860045861   | DevOpsExperts             | 1160 Calle Norte                  | 555-1160  | España         | Madrid          |
| 860045839   | DevOpsSolutions           | 7374 Calle Oeste                  | 555-7374  | Venezuela      | Maracay         |
| 860045900   | DigitalAnalysts           | 2240 Calle Oeste                  | 555-2240  | Argentina      | Buenos Aires    |
| 860045903   | DigitalConsults           | 2360 Calle Norte                  | 555-2360  | Argentina      | Córdoba         |
| 860045774   | DigitalDesign             | 2121 Calle Veinticuatro          | 555-5253  | Colombia       | Barranquilla    |
| 860045844   | DigitalMarketers          | 8384 Calle Oeste                  | 555-8384  | México         | Guadalajara     |
| 860045837   | DigitalTransform          | 6970 Calle Sur                    | 555-6970  | Ecuador        | Quito           |
| 860045878   | DigitalTransformers       | 1540 Calle Central                | 555-1540  | Chile          | Santiago        |
| 860045775   | Economía Global           | 2222 Cal

3. **Tabla  Eliminadas**
   - Columnas: Codigo_Empleado, Profesión, Salario, Dias_Laborales, Horas_Trabajo_Semanales, Estado_Civil, Numero_Hijos
   - Aquí está la información de los empleados en español:

| Codigo_Empleado | Profesion                | Salario | Dias_Laborales   | Horas_Trabajo_Semanales | Estado_Civil | Numero_Hijos |
|-----------------|--------------------------|---------|------------------|-------------------------|--------------|--------------|
| 1               | Ingeniero                | 50000.0 | Lunes a Viernes  | 40                      | Soltero      | 0            |
| 2               | Diseñadora               | 45000.0 | Lunes a Viernes  | 40                      | Casada       | 1            |
| 3               | Administrador            | 55000.0 | Lunes a Sábado    | 48                      | Casado       | 2            |
| 4               | Marketing                | 48000.0 | Lunes a Viernes  | 40                      | Soltera      | 0            |
| 5               | Contador                 | 60000.0 | Lunes a Viernes  | 40                      | Divorciado   | 3            |
| 6               | Psicóloga                | 52000.0 | Lunes a Viernes  | 40                      | Casada       | 1            |
| 7               | Programador              | 47000.0 | Lunes a Viernes  | 40                      | Soltero      | 0            |
| 8               | Arquitecta               | 49000.0 | Lunes a Viernes  | 40                      | Soltera      | 0            |
| 9               | Abogado                  | 61000.0 | Lunes a Viernes  | 40                      | Casado       | 2            |
| 10              | Enfermera                | 45000.0 | Lunes a Viernes  | 40                      | Soltera      | 0            |
| 11              | Ingeniero Civil          | 54000.0 | Lunes a Sábado    | 48                      | Casado       | 1            |
| 12              | Periodista               | 46000.0 | Lunes a Viernes  | 40                      | Soltera      | 0            |
| 13              | Chef                     | 50000.0 | Lunes a Sábado    | 48                      | Casado       | 1            |
| 14              | Dentista                 | 55000.0 | Lunes a Viernes  | 40                      | Casada       | 0            |
| 15              | Analista Financiero      | 53000.0 | Lunes a Viernes  | 40                      | Soltero      | 0            |
| 16              | Gerente de Ventas        | 65000.0 | Lunes a Viernes  | 40                      | Casada       | 2            |
| 17              | Desarrollador Web        | 47000.0 | Lunes a Viernes  | 40                      | Soltero      | 0            |
| 18              | Consultora               | 49000.0 | Lunes a Viernes  | 40                      | Soltera      | 0            |
| 19              | Especialista en IT       | 51000.0 | Lunes a Viernes  | 40                      | Casado       | 1            |
| 20              | Bióloga                  | 53000.0 | Lunes a Viernes  | 40                      | Casada       | 1            |
| 21              | Veterinario              | 49000.0 | Lunes a Viernes  | 40                      | Soltero      | 0            |
| 22              | Psicólog

Supongamos que en la tabla "Empleados Eliminados" tenemos datos de empleados donde la columna "Profesión" podría tener múltiples valores separados por comas, lo cual es una violación de la 1FN.

#### Transformación para cumplir con la 1FN

Veamos cómo podría lucir la tabla "Empleados Eliminados" después de aplicar la 1FN:

| Codigo_Empleado | Profesion          | Salario | Dias_Laborales | Horas_Trabajo_Semanales | Estado_Civil | Numero_Hijos |
|-----------------|--------------------|---------|----------------|-------------------------|--------------|--------------|
| 1               | Ingeniero          | 50000.0 | Lunes a Viernes | 40                      | Soltero      | 0            |
| 2               | Diseñadora         | 45000.0 | Lunes a Viernes | 40                      | Casada       | 1            |
| 3               | Administrador      | 55000.0 | Lunes a Sábado  | 48                      | Casado       | 2            |
| ...             | ...                | ...     | ...            | ...                     | ...          | ...          |

En esta nueva estructura, cada fila representa a un empleado con su respectiva profesión separada en una columna individual, cumpliendo así con la 1FN. Esto permite una gestión de datos más eficiente y facilita consultas sin ambigüedades ni redundancias.

#### Importancia de la 1FN

La aplicación de la Primera Forma Normal (1FN) es esencial para garantizar la consistencia y la eficiencia en el diseño de bases de datos. Al cumplir con la 1FN, se logran los siguientes beneficios:

1. **Reducción de la redundancia**: Evita la repetición innecesaria de datos, lo cual reduce el riesgo de inconsistencias y errores.

2. **Facilita la gestión de datos**: Permite consultas más simples y eficientes al asegurar que cada valor esté correctamente separado y definido.

3. **Mejora el rendimiento**: La estructura normalizada puede mejorar el rendimiento de las consultas y operaciones en la base de datos.

Claro, aquí tienes un ensayo que explica la normalización de la base de datos descrita en el formato Markdown:

---



## Introducción

La normalización de bases de datos es una técnica esencial en la gestión de datos, que busca reducir la redundancia y mejorar la integridad de los datos. En este ensayo, exploraremos el proceso de normalización aplicado a un sistema de información de personal, que incluye diversas tablas relacionadas con empleados, empresas, países y turnos laborales.

## Descripción del Sistema

El sistema de información de personal consta de las siguientes tablas principales: `PERSONAL`, `EMPRESA`, `PAIS`, y `TURNO`. Cada una de estas tablas desempeña un papel crucial en la gestión de la información relacionada con los empleados y la estructura organizativa.

### Tabla PERSONAL

La tabla `PERSONAL` contiene información detallada sobre los empleados. Sus columnas incluyen:
- **Cedula**: Identificador único del empleado (PK).
- **Nombre**: Nombre del empleado.
- **Apellido**: Apellido del empleado.
- **Nombre compuesto**: Nombre completo del empleado.
- **Edad**: Edad del empleado.
- **Email**: Correo electrónico del empleado.
- **Cargo**: Cargo del empleado.
- **Fecha_Ingreso**: Fecha de ingreso a la empresa.
- **Departamento**: Departamento al que pertenece.
- **Jefe_Inmediato**: Nombre del jefe inmediato.
- **Nivel_Riesgo**: Nivel de riesgo del cargo.
- **Turno**: Identificador del turno (FK).
- **Fecha_Nacimiento**: Fecha de nacimiento del empleado.
- **Genero**: Género del empleado.

### Tabla EMPRESA

La tabla `EMPRESA` gestiona la información de las empresas y sus ubicaciones. Sus columnas son:
- **cod_empresa**: Identificador único de la empresa (PK).
- **Empresa**: Nombre de la empresa.
- **Direccion**: Dirección de la empresa.
- **Telefono**: Teléfono de la empresa.
- **Pais**: Identificador del país (FK).
- **Ciudad**: Identificador de la ciudad (FK).

### Tabla PAIS

La tabla `PAIS` define las relaciones entre países y ciudades. Sus columnas incluyen:
- **cod_pais**: Identificador único del país (PK1).
- **Pais**: Nombre del país.
- **cod_ciudad**: Identificador único de la ciudad (PK2).
- **Ciudad**: Nombre de la ciudad.

### Tabla TURNO

La tabla `TURNO` detalla los turnos laborales disponibles. Sus columnas son:
- **cod_turno**: Identificador único del turno (PK).
- **turno**: Descripción del turno.

## Normalización a Segunda Forma Normal (2NF)

Para asegurar que la base de datos esté en la Segunda Forma Normal (2NF), debemos eliminar las dependencias parciales. Esto implica que todas las columnas no clave deben depender de la clave primaria en su totalidad.

### Implementación de la 2NF

#### Tabla PERSONAL
En la tabla `PERSONAL`, la clave primaria es `Cedula`. Todas las columnas dependen completamente de esta clave, por lo que la tabla cumple con 2NF.

#### Tabla EMPRESA
En la tabla `EMPRESA`, la clave primaria es `cod_empresa`. Las columnas `Pais` y `Ciudad` actúan como llaves foráneas, referenciando la tabla `PAIS` para evitar la duplicación de información sobre países y ciudades.

#### Tabla PAIS
La tabla `PAIS` tiene una clave primaria compuesta por `cod_pais` y `cod_ciudad`, lo que asegura que cada combinación de país y ciudad sea única.

#### Tabla TURNO
En la tabla `TURNO`, la clave primaria es `cod_turno`, y la columna `turno` depende completamente de esta clave.

## Beneficios de la Normalización

La normalización a 2NF en este sistema de información de personal ofrece varios beneficios:
1. **Reducción de Redundancia**: Al separar la información en tablas relacionadas, se evita la duplicación de datos.
2. **Integridad de los Datos**: Las dependencias de clave garantizan que las relaciones entre tablas sean coherentes y precisas.
3. **Facilidad de Mantenimiento**: Las actualizaciones de datos se pueden realizar en una sola tabla, simplificando el mantenimiento.
4. **Mejora del Rendimiento**: La reducción de redundancias y la eliminación de anomalías mejora el rendimiento de las consultas y operaciones de la base de datos.

## Conclusión

La normalización de la base de datos del sistema de información de personal a la Segunda Forma Normal (2NF) es un paso fundamental para garantizar la eficiencia y la integridad de los datos. Al descomponer la información en tablas relacionadas, se minimiza la redundancia y se facilita el mantenimiento del sistema. Este enfoque no solo mejora la calidad de los datos, sino que también optimiza el rendimiento del sistema, proporcionando una base sólida para la gestión de la información de personal.

---

# Segunda Forma de Normalización (2NF)

La normalización de bases de datos es un proceso utilizado para organizar los datos en una base de datos, reduciendo la redundancia y mejorando la integridad de los datos. Este proceso se realiza en varias etapas, conocidas como formas normales. La Segunda Forma Normal (2NF) es la segunda etapa en este proceso, y su objetivo principal es asegurar que todos los datos dependan completamente de la clave primaria.

## ¿Qué es la Segunda Forma Normal (2NF)?

La 2NF se basa en la Primera Forma Normal (1NF), que requiere que los datos estén organizados en tablas y que cada columna contenga valores atómicos, es decir, indivisibles. Para que una tabla esté en 2NF, debe cumplir con los siguientes requisitos:
1. Debe estar en 1NF.
2. No debe haber dependencias parciales de la clave primaria, es decir, todos los atributos no clave deben depender de toda la clave primaria, no solo de una parte de ella.

En otras palabras, una tabla está en 2NF si y solo si cada atributo no clave es funcionalmente dependiente de la clave primaria completa.

## Ejemplo de Normalización a 2NF

Supongamos que tenemos una base de datos para gestionar la información de los empleados de una empresa. Empezaremos con una tabla que no está normalizada y la transformaremos a 2NF.

### Tabla Inicial (No Normalizada)

```
PERSONAL
| Cedula | Nombre | Apellido | Nombre compuesto | Edad | Email | Cargo | Fecha_Ingreso | Departamento | Jefe_Inmediato | Nivel_Riesgo | Turno | Fecha_Nacimiento | Genero | Empresa | Direccion | Telefono | Pais | Ciudad |
```

En esta tabla, tenemos datos sobre los empleados y también información de la empresa, lo cual puede llevar a redundancias y anomalías de actualización.

### Primera Forma Normal (1NF)

Primero, aseguramos que cada columna contiene valores atómicos. La tabla PERSONAL cumple con esta condición, por lo que ya está en 1NF.

### Segunda Forma Normal (2NF)

Para llevar esta tabla a 2NF, debemos eliminar las dependencias parciales. Observamos que la información sobre la empresa no depende directamente de la clave primaria `Cedula`, sino que es información repetitiva relacionada con la empresa en sí. Por lo tanto, dividimos la tabla en varias tablas más pequeñas y relacionadas:

#### Tabla: PERSONAL

| Cedula (PK) | Nombre | Apellido | Nombre compuesto | Edad | Email | Cargo | Fecha_Ingreso | Departamento | Jefe_Inmediato | Nivel_Riesgo | Turno (FK) | Fecha_Nacimiento | Genero | cod_empresa (FK) |
|-------------|--------|----------|------------------|------|-------|-------|---------------|--------------|----------------|--------------|------------|-------------------|--------|------------------|

#### Tabla: EMPRESA

| cod_empresa (PK) | Empresa | Direccion | Telefono | cod_pais (FK) | cod_ciudad (FK) |
|------------------|---------|-----------|----------|---------------|-----------------|

#### Tabla: PAIS

| cod_pais (PK1) | Pais     | cod_ciudad (PK2) | Ciudad   |
|----------------|----------|------------------|----------|

#### Tabla: TURNO

| cod_turno (PK) | turno    |
|----------------|----------|

### Relaciones Entre Tablas

- La tabla `PERSONAL` ahora contiene un campo `cod_empresa` que es una llave foránea referenciando la tabla `EMPRESA`. Esto elimina la redundancia de información de la empresa en la tabla de empleados.
- La tabla `EMPRESA` contiene campos `cod_pais` y `cod_ciudad`, que son llaves foráneas referenciando la tabla `PAIS`, eliminando redundancias de información sobre países y ciudades.
- La tabla `PERSONAL` también tiene un campo `Turno` que es una llave foránea referenciando la tabla `TURNO`.

### Ventajas de la 2NF

1. **Eliminación de Redundancia**: Al dividir la información en múltiples tablas, se reduce la duplicación de datos. Por ejemplo, la información de la empresa se almacena una sola vez en la tabla `EMPRESA`.
2. **Mejora de la Integridad de los Datos**: Los datos están más organizados, lo que facilita mantener la consistencia y precisión de los datos.
3. **Facilidad de Mantenimiento**: La actualización, inserción y eliminación de datos se vuelve más sencilla y menos propensa a errores.

### Ejemplo de Datos en 2NF

#### Tabla: PERSONAL

| Cedula | Nombre | Apellido | Nombre compuesto | Edad | Email | Cargo | Fecha_Ingreso | Departamento | Jefe_Inmediato | Nivel_Riesgo | Turno | Fecha_Nacimiento | Genero | cod_empresa |
|--------|--------|----------|------------------|------|-------|-------|---------------|--------------|----------------|--------------|-------|-------------------|--------|-------------|
| 1      | Juan   | Pérez    | Juan Pérez       | 30   | jperez@example.com | Ingeniero | 2020-01-15    | Desarrollo     | Ana Gómez      | Medio        | 1     | 1990-05-10        | M      | 1           |
| 2      | María  | López    | María López      | 25   | mlopez@example.com | Diseñadora | 2019-02-20    | Diseño         | Pedro Martínez | Bajo         | 2     | 1995-08-20        | F      | 2           |

#### Tabla: EMPRESA

| cod_empresa | Empresa        | Direccion         | Telefono       | cod_pais | cod_ciudad |
|-------------|----------------|-------------------|----------------|----------|------------|
| 1           | Tech Solutions | 123 Main St       | 555-1234       | 1        | 1          |
| 2           | Creative Minds | 456 Market Ave    | 555-5678       | 2        | 2          |

#### Tabla: PAIS

| cod_pais | Pais           | cod_ciudad | Ciudad          |
|----------|----------------|------------|------------------|
| 1        | Estados Unidos | 1          | Nueva York       |
| 2        | Canadá         | 2          | Toronto          |

#### Tabla: TURNO

| cod_turno | turno         |
|-----------|---------------|
| 1         | Diurno        |
| 2         | Nocturno      |



# Tercera Forma de Normalización (3NF)

La normalización de bases de datos es un proceso crucial para organizar los datos de manera que se minimicen las redundancias y se optimice la integridad de los datos. La Tercera Forma Normal (3NF) es un nivel avanzado de normalización que se basa en las formas anteriores (1NF y 2NF) y tiene el objetivo de eliminar dependencias transitivas.

## ¿Qué es la Tercera Forma Normal (3NF)?

Para que una tabla esté en 3NF, debe cumplir con los siguientes requisitos:
1. Debe estar en Segunda Forma Normal (2NF).
2. No debe haber dependencias transitivas, es decir, los atributos no clave no deben depender de otros atributos no clave.

En otras palabras, un atributo no clave no debe depender de otro atributo no clave; todos los atributos no clave deben depender únicamente de la clave primaria.

## Ejemplo de Normalización a 3NF

Supongamos que tenemos una base de datos para gestionar la información de los empleados y las empresas en las que trabajan. Empezaremos con una tabla que ya está en 2NF y la transformaremos a 3NF.

### Tablas Iniciales en 2NF

#### Tabla: PERSONAL

| Cedula (PK) | Nombre | Apellido | Nombre compuesto | Edad | Email | Fecha_Ingreso | Turno (FK) | Fecha_Nacimiento | Genero |
|-------------|--------|----------|------------------|------|-------|---------------|------------|-------------------|--------|

#### Tabla: EMPRESA

| cod_empresa (PK) | Empresa | Direccion | Telefono | Pais | Ciudad |
|------------------|---------|-----------|----------|------|--------|

#### Tabla: RiesgosProfesionales

| Cargo (PK) | Nivel_Riesgo |
|------------|--------------|

#### Tabla: PAIS

| cod_pais (PK) | Pais       | cod_ciudad | Ciudad   |
|---------------|------------|------------|----------|

#### Tabla: TURNO

| cod_turno (PK) | Turno      |
|----------------|------------|

### Tercera Forma Normal (3NF)

Para llevar estas tablas a 3NF, debemos asegurarnos de que no haya dependencias transitivas. Observamos que la tabla EMPRESA tiene atributos como `Pais` y `Ciudad` que no dependen directamente de la clave primaria `cod_empresa`. Estos atributos dependen de `cod_pais` y `cod_ciudad`, por lo que deben ser movidos a una tabla separada.

#### Tabla: PERSONAL

| Cedula (PK) | Nombre | Apellido | Nombre compuesto | Edad | Email | Fecha_Ingreso | Turno (FK) | Fecha_Nacimiento | Genero |
|-------------|--------|----------|------------------|------|-------|---------------|------------|-------------------|--------|

#### Tabla: EMPRESA

| cod_empresa (PK) | Empresa | Direccion | Telefono | cod_pais (FK) | cod_ciudad (FK) |
|------------------|---------|-----------|----------|---------------|-----------------|

#### Tabla: RiesgosProfesionales

| Cargo (PK) | Nivel_Riesgo |
|------------|--------------|

#### Tabla: PAIS

| cod_pais (PK) | Pais       |
|---------------|------------|

#### Tabla: CIUDAD

| cod_ciudad (PK) | Ciudad   | cod_pais (FK) |
|-----------------|----------|---------------|

#### Tabla: TURNO

| cod_turno (PK) | Turno      |
|----------------|------------|

### Relaciones Entre Tablas

- La tabla `PERSONAL` contiene una llave foránea `Turno` que referencia la tabla `TURNO`.
- La tabla `EMPRESA` contiene llaves foráneas `cod_pais` y `cod_ciudad` que referencian las tablas `PAIS` y `CIUDAD`, respectivamente.
- La tabla `CIUDAD` contiene una llave foránea `cod_pais` que referencia la tabla `PAIS`.

### Ventajas de la 3NF

1. **Eliminación de Dependencias Transitivas**: Asegura que los atributos no clave no dependan de otros atributos no clave.
2. **Reducción de Redundancia**: Mejora la organización de los datos y reduce la duplicación de información.
3. **Integridad y Consistencia de los Datos**: Facilita la gestión y mantenimiento de la base de datos, asegurando que los datos sean precisos y consistentes.

### Ejemplo de Datos en 3NF

#### Tabla: PERSONAL

| Cedula | Nombre | Apellido | Nombre compuesto | Edad | Email | Fecha_Ingreso | Turno | Fecha_Nacimiento | Genero |
|--------|--------|----------|------------------|------|-------|---------------|-------|-------------------|--------|
| 1      | Juan   | Pérez    | Juan Pérez       | 30   | jperez@example.com | 2020-01-15 | 1     | 1990-05-10        | M      |
| 2      | María  | López    | María López      | 25   | mlopez@example.com | 2019-02-20 | 2     | 1995-08-20        | F      |

#### Tabla: EMPRESA

| cod_empresa | Empresa        | Direccion         | Telefono       | cod_pais | cod_ciudad |
|-------------|----------------|-------------------|----------------|----------|------------|
| 1           | Tech Solutions | 123 Main St       | 555-1234       | 1        | 1          |
| 2           | Creative Minds | 456 Market Ave    | 555-5678       | 2        | 2          |

#### Tabla: RiesgosProfesionales

| Cargo      | Nivel_Riesgo |
|------------|--------------|
| Ingeniero  | Medio        |
| Diseñadora | Bajo         |

#### Tabla: PAIS

| cod_pais | Pais           |
|----------|----------------|
| 1        | Estados Unidos |
| 2        | Canadá         |

#### Tabla: CIUDAD

| cod_ciudad | Ciudad          | cod_pais |
|------------|-----------------|----------|
| 1          | Nueva York      | 1        |
| 2          | Toronto         | 2        |

#### Tabla: TURNO

| cod_turno | Turno            |
|-----------|------------------|
| 1         | Diurno           |
| 2         | Nocturno         |





## Conclusión sobre la Normalización en 1NF, 2NF y 3NF

La normalización de bases de datos es un proceso esencial en el diseño de esquemas relacionales eficientes y consistentes. Este proceso se realiza en varias etapas o formas normales (1NF, 2NF y 3NF), cada una de las cuales contribuye a reducir la redundancia y mejorar la integridad de los datos. A continuación, se presenta una conclusión conjunta sobre las tres primeras formas de normalización:

### Primera Forma Normal (1NF)

La 1NF establece los cimientos de la normalización asegurando que los datos en una tabla sean atómicos y que cada campo contenga solo un valor único. Esto elimina la duplicación de grupos repetitivos y asegura que la tabla tenga una estructura tabular clara. Al cumplir con la 1NF, se facilita el acceso y la manipulación de los datos al garantizar que no haya celdas que contengan conjuntos de valores o listas.

### Segunda Forma Normal (2NF)

La 2NF se basa en la 1NF y añade el requisito de eliminar dependencias parciales, es decir, que los atributos no clave deben depender completamente de la clave primaria completa. Este paso es crucial para descomponer las tablas de manera que se eliminen las redundancias derivadas de dependencias parciales. Al asegurar que todos los atributos no clave estén completamente dependientes de la clave primaria, se mejora la integridad y se minimiza la duplicación de datos.

### Tercera Forma Normal (3NF)

La 3NF se basa en la 2NF y elimina las dependencias transitivas, garantizando que los atributos no clave no dependan de otros atributos no clave. Este nivel avanzado de normalización asegura que cada atributo no clave sea directamente dependiente de la clave primaria y nada más. Al cumplir con la 3NF, se optimiza aún más la estructura de la base de datos, se reduce la redundancia y se mejora la integridad referencial, facilitando así el mantenimiento y la actualización de los datos.

### Beneficios Conjuntos de 1NF, 2NF y 3NF

- **Reducción de Redundancia**: A través de cada nivel de normalización, se minimiza la duplicación de datos, lo cual reduce el espacio de almacenamiento necesario y previene inconsistencias.
- **Mejora de la Integridad de Datos**: La normalización asegura que las relaciones entre los datos sean claras y precisas, lo que contribuye a mantener la consistencia y precisión de la información.
- **Facilidad de Mantenimiento**: Con una estructura de datos más organizada y menos redundante, las operaciones de actualización, inserción y eliminación se vuelven más sencillas y menos propensas a errores.
- **Optimización de Consultas**: Las bases de datos normalizadas permiten consultas más eficientes, ya que los datos están estructurados de manera lógica y coherente, lo que mejora el rendimiento general del sistema.

En resumen, la normalización a través de 1NF, 2NF y 3NF es un proceso fundamental para diseñar bases de datos robustas y eficientes. Cada nivel de normalización aborda diferentes tipos de redundancias y dependencias, asegurando que la base de datos sea fácil de mantener, consistente y optimizada para el rendimiento.


#**puedes descargar la base de datos en con su normalizacion en el siguiente link* https://drive.google.com/file/d/1MiDZFwbkoJcRHW6mHUix5tE3bCSBmCYv/view?usp=sharing  


