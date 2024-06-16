# Implementación de la base de datos

Una vez hayamos aplicado la normalización a nuestra base de datos procedemos a la implementación mediante un Sistema de Gestión de Bases de Datos (SGBD) apropiado, en este caso usaremos MySQL Workbench 8.0.36 que podrán descargar gratuitamente del siguiente [link](https://dev.mysql.com/downloads/workbench/).

## Paso 1: Creación de la Base de Datos y las Tablas

Procederemos a crear la base de datos y las tablas usando los archivos que ya se subieron previamente normalizados, donde encontramos la base datos en crudo con el nombre Base de Datos Cruda.md y las tablas normalizadas estan en el apartado Proceso de normalizacion.md al final encontraran el link para descargar el archivo correspondiente

```sql
-- crear base de datos atsq
-- -----------------------------------------------------
CREATE SCHEMA IF NOT EXISTS `atsq` DEFAULT CHARACTER SET utf8mb4 COLLATE utf8mb4_0900_ai_ci ;
USE `atsq` ;

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
## Paso 2: Insertar los datos a las Tablas

El llenado de las tablas se realizo directamente de importacion de tabla por tabla, ya creada la base de datos llamada atsq damos click izquierdo saldra una serie de opciones que en la cual escojemos:

![image](https://github.com/mandres1987/proyectoPAR/assets/170149039/a3698d75-22b1-4c18-817a-ae8cbd37209c)

segun la imagen elegimos la opcion Table data import wizard, despues buscamos el archivo guardado en formato cvs 

![image](https://github.com/mandres1987/proyectoPAR/assets/170149039/57ad2acb-311c-493c-ae50-46dacd52894c)

y de damos click en next a todas las ventanas que nos valla saliendo hasta el fin
le damos a actualizar 

![image](https://github.com/mandres1987/proyectoPAR/assets/170149039/8bdb6ebb-db3c-4bc4-8516-71480048a611)

y ya nos va aparecer la tabla con sus respectivos datos
tabla personal

![image](https://github.com/mandres1987/proyectoPAR/assets/170149039/89574e7d-857d-432a-a1f6-3f8774fbc703)

tabla empresa

![image](https://github.com/mandres1987/proyectoPAR/assets/170149039/fc7e22fc-4ad7-4511-acf5-f6997d481055)

tabla pais

![image](https://github.com/mandres1987/proyectoPAR/assets/170149039/85f5b260-9b55-4897-a572-8ce977c660a4)

tabla turno

![image](https://github.com/mandres1987/proyectoPAR/assets/170149039/fa5c179d-d14a-43d8-b6c5-ee51b6f81e42)

tabla riesgosprofesionales

![image](https://github.com/mandres1987/proyectoPAR/assets/170149039/dcf0496f-c037-4a66-81df-91c57534286f)


## Paso 3: consultas SQL







