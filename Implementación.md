# Implementación de la base de datos

Una vez hayamos aplicado la normalización a nuestra base de datos procedemos a la implementación mediante un Sistema de Gestión de Bases de Datos (SGBD) apropiado, en este caso usaremos MySQL Workbench 8.0.36 que podrán descargar gratuitamente del siguiente [link](https://dev.mysql.com/downloads/workbench/).

## Paso 1: Creación de la Base de Datos y las Tablas

Procederemos a crear la base de datos y las tablas usando los archivos que ya se subieron previamente normalizados, donde encontramos la base datos en crudo con el nombre Base de Datos Cruda.md y las tablas normalizadas estan en el apartado Proceso de normalizacion.md al final encontraran el link para descargar el archivo correspondiente

```sql
-- crear base de datos atsq
-- -----------------------------------------------------
CREATE SCHEMA IF NOT EXISTS `atsq` DEFAULT CHARACTER SET utf8mb4 COLLATE utf8mb4_0900_ai_ci;
USE `atsq`;

-- -----------------------------------------------------
-- crear la tabla empresa`
-- -----------------------------------------------------
CREATE TABLE IF NOT EXISTS `atsq`.`empresa` (
  `cod_empresa` INT NULL DEFAULT NULL,
  `Empresa` TEXT NULL DEFAULT NULL,
  `Direccion` TEXT NULL DEFAULT NULL,
  `Telefono` TEXT NULL DEFAULT NULL,
  `Pais` INT NULL DEFAULT NULL,
  `Ciudad` INT NULL DEFAULT NULL)
ENGINE = InnoDB
DEFAULT CHARACTER SET = utf8mb4
COLLATE = utf8mb4_0900_ai_ci;


-- -----------------------------------------------------
-- crear la tabla pais`
-- -----------------------------------------------------
CREATE TABLE IF NOT EXISTS `atsq`.`pais` (
  `cod_pais` INT NULL DEFAULT NULL,
  `Pais` TEXT NULL DEFAULT NULL,
  `Ciudad` TEXT NULL DEFAULT NULL)
ENGINE = InnoDB
DEFAULT CHARACTER SET = utf8mb4
COLLATE = utf8mb4_0900_ai_ci;


-- -----------------------------------------------------
-- crear la tabla personal
-- -----------------------------------------------------
CREATE TABLE IF NOT EXISTS `atsq`.`personal` (
  `Cedula` INT NULL DEFAULT NULL,
  `Nombre` TEXT NULL DEFAULT NULL,
  `Apellido` TEXT NULL DEFAULT NULL,
  `Nombre compuesto` TEXT NULL DEFAULT NULL,
  `Edad` INT NULL DEFAULT NULL,
  `Email` TEXT NULL DEFAULT NULL,
  `Cargo` TEXT NULL DEFAULT NULL,
  `Fecha_Ingreso` TEXT NULL DEFAULT NULL,
  `Departamento` TEXT NULL DEFAULT NULL,
  `Jefe_Inmediato` TEXT NULL DEFAULT NULL,
  `Nivel_Riesgo` INT NULL DEFAULT NULL,
  `Turno` TEXT NULL DEFAULT NULL,
  `Fecha_Nacimiento` TEXT NULL DEFAULT NULL,
  `Genero` TEXT NULL DEFAULT NULL)
ENGINE = InnoDB
DEFAULT CHARACTER SET = utf8mb4
COLLATE = utf8mb4_0900_ai_ci;


-- -----------------------------------------------------
-- crear la tabla riesgosprofesionales
-- -----------------------------------------------------
CREATE TABLE IF NOT EXISTS `atsq`.`riesgosprofesionales` (
  `chip` INT NULL DEFAULT NULL,
  `Cargo` TEXT NULL DEFAULT NULL,
  `Nivel_Riesgo` INT NULL DEFAULT NULL)
ENGINE = InnoDB
DEFAULT CHARACTER SET = utf8mb4
COLLATE = utf8mb4_0900_ai_ci;


-- -----------------------------------------------------
-- crear la tabla turno`
-- -----------------------------------------------------
CREATE TABLE IF NOT EXISTS `atsq`.`turno` (
  `TURNO` TEXT NULL DEFAULT NULL,
  `MyUnknownColumn` TEXT NULL DEFAULT NULL)
ENGINE = InnoDB
DEFAULT CHARACTER SET = utf8mb4
COLLATE = utf8mb4_0900_ai_ci;


SET SQL_MODE=@OLD_SQL_MODE;
SET FOREIGN_KEY_CHECKS=@OLD_FOREIGN_KEY_CHECKS;
SET UNIQUE_CHECKS=@OLD_UNIQUE_CHECKS;
```
##Ingenieria Inversa
![image](https://github.com/mandres1987/proyectoPAR/assets/169571131/3050f3f1-d694-4ebc-a85b-9e4591bde012)


## Paso 2: Insertar los datos a las Tablas

El llenado de las tablas se realizo directamente de importacion de tabla por tabla, ya creada la base de datos llamada atsq damos click izquierdo saldra una serie de opciones que en la cual escojemos:

![image](https://github.com/mandres1987/proyectoPAR/assets/170149039/a3698d75-22b1-4c18-817a-ae8cbd37209c)

segun la imagen elegimos la opcion Table data import wizard, despues buscamos el archivo guardado en formato cvs 

![image](https://github.com/mandres1987/proyectoPAR/assets/170149039/57ad2acb-311c-493c-ae50-46dacd52894c)

y de damos click en next a todas las ventanas que nos valla saliendo hasta el fin
le damos a actualizar 

![image](https://github.com/mandres1987/proyectoPAR/assets/170149039/8bdb6ebb-db3c-4bc4-8516-71480048a611)

y ya nos va aparecer la tabla con sus respectivos datos

1. tabla personal

![image](https://github.com/mandres1987/proyectoPAR/assets/170149039/89574e7d-857d-432a-a1f6-3f8774fbc703)

2. tabla empresa

![image](https://github.com/mandres1987/proyectoPAR/assets/170149039/fc7e22fc-4ad7-4511-acf5-f6997d481055)

3. tabla pais

![image](https://github.com/mandres1987/proyectoPAR/assets/170149039/85f5b260-9b55-4897-a572-8ce977c660a4)

4. tabla turno

![image](https://github.com/mandres1987/proyectoPAR/assets/170149039/fa5c179d-d14a-43d8-b6c5-ee51b6f81e42)

5. tabla riesgosprofesionales

![image](https://github.com/mandres1987/proyectoPAR/assets/170149039/dcf0496f-c037-4a66-81df-91c57534286f)


## Paso 3: consultas SQL

1.  Listar todos los turnos

```sql
SELECT * FROM atsq.turno;
```
![image](https://github.com/mandres1987/proyectoPAR/assets/170149039/e7ebd7d9-70dc-4e6c-8e67-08d554af151f)

2. Listar empresas por país

```sql
SELECT e.Empresa, p.Pais
FROM atsq.empresa e
JOIN atsq.pais p ON e.Pais = p.cod_pais;
```
![image](https://github.com/mandres1987/proyectoPAR/assets/170149039/ad5793ad-719a-4e85-bab7-957bea3d80f9)

3. Listar empleados por departamento

```sql
SELECT p.Nombre, p.Apellido, p.Departamento
FROM atsq.personal p;
```
![image](https://github.com/mandres1987/proyectoPAR/assets/170149039/50739e97-25b3-4fd4-a883-c4533a71a7e7)

4. Listar empleados por nivel de riesgo

```sql
SELECT p.Nombre, p.Apellido, p.Nivel_Riesgo
FROM atsq.personal p
ORDER BY p.Nivel_Riesgo;
```
![image](https://github.com/mandres1987/proyectoPAR/assets/170149039/1e32d89c-5cc2-4adb-b6fc-79b347334b8a)

5. Listar nombre por edad mayor a  29

```sql
SELECT Nombre
FROM personal
WHERE Edad > 29;
```
![image](https://github.com/mandres1987/proyectoPAR/assets/170149039/291e9d81-a312-4b08-9a0f-5529611b0769)

6. Listar empleados por cargo

```sql
SELECT p.Nombre, p.Apellido, p.Cargo
FROM atsq.personal p;
```
![image](https://github.com/mandres1987/proyectoPAR/assets/170149039/c9edee7f-332c-422c-9f96-77eaf9e52e6c)

7. Listar empleados por edad

```sql
SELECT p.Nombre, p.Apellido, p.Edad
FROM atsq.personal p
ORDER BY p.Edad;
```
![image](https://github.com/mandres1987/proyectoPAR/assets/170149039/7a87b75b-96ef-4cf4-ad24-3d82180c0c9e)

8.	Listar empleados por género femenino

```sql
SELECT *
FROM personal
WHERE Genero = 'Femenino';
```
![image](https://github.com/mandres1987/proyectoPAR/assets/170149039/440a347e-af3d-4ab3-a849-ce66582a005b)

9. Listar nombre y apellido por fecha de nacimiento entre 15/11/1970 y 20/03/1998

```sql
SELECT Nombre, Apellido
FROM atsq.personal
WHERE Fecha_Nacimiento  BETWEEN '15/11/1970' AND '20/03/1998';
```
![image](https://github.com/mandres1987/proyectoPAR/assets/170149039/010b54c9-6960-49ed-a587-1b5ca2c0c17f)

10. -- listar las ciudades del país Argentina

```sql
SELECT p.Ciudad
FROM atsq.pais p
WHERE p.Pais = 'Argentina';
```
![image](https://github.com/mandres1987/proyectoPAR/assets/170149039/1845ff13-ffef-4d8b-b488-3b512efd149d)

11. obtener el nombre y el salario de los empleados que ganan más de 50000.0

```sql
SELECT p.Nombre, p.Apellido, p.Email, p.Cargo, p.Fecha_Ingreso, p.Departamento, p.Jefe_Inmediato, p.Nivel_Riesgo, p.Turno, p.Fecha_Nacimiento, p.Genero
FROM atsq.personal p
WHERE p.Email > '50000.0';
```
![image](https://github.com/mandres1987/proyectoPAR/assets/170149039/994961e9-2368-4c8c-b562-5efd31b48799)

12. listar las personas que tienen en su profesión "Ingeniero"

```sql
SELECT * 
FROM atsq.personal 
WHERE Cargo LIKE '%Ingeniero%';
```
![image](https://github.com/mandres1987/proyectoPAR/assets/170149039/90dd52d2-5f31-49cf-8d44-2b92cdc9ad29)

13. Listar fecha_ingreso entre dos fechas específicas

```sql
SELECT Fecha_Ingreso, Nombre, Apellido
FROM atsq.personal
WHERE Fecha_Ingreso BETWEEN '01/01/2019' AND '12/12/2021';
```
![image](https://github.com/mandres1987/proyectoPAR/assets/170149039/40ce3450-56b0-44e1-a31f-f338dcbc4dc3)

14. listar los apellidos con terminación en "ez"

```sql
SELECT Apellido
FROM atsq.personal
WHERE Apellido LIKE '%ez';
```
![image](https://github.com/mandres1987/proyectoPAR/assets/170149039/14836793-726c-4516-8be2-330b8355a775)

15. Listar nombres con turno diurno

```sql
SELECT Nombre, Turno
FROM personal
WHERE Turno = 'Diurno';
```
![image](https://github.com/mandres1987/proyectoPAR/assets/170149039/83405a0e-18c7-41d4-af17-bae2ef2be10a)





