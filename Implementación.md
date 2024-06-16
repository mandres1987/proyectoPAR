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
