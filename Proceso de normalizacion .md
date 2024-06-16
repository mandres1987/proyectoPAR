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




