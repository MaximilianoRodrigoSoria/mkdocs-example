# 💾 Base de datos

## Creacion de tabla

```sql

CREATE SCHEMA IF NOT EXISTS esquema_ejemplo;

SET search_path TO esquema_ejemplo;

CREATE TABLE usuario (
                          ID SERIAL PRIMARY KEY,
                          dni INTEGER,
                          nombre VARCHAR(255),
                          apellido VARCHAR(255),                          
                          error TEXT,
                          status VARCHAR(50),
                          file_name VARCHAR(255),
                          update_date DATE,
                          start_date DATE
                         
);

```


## Insertar datos

```sql
INSERT INTO usuario (dni, nombre, apellido, error, status, file_name, update_date, start_date) 
VALUES (12345678, 'Juan', 'Pérez', NULL, 'Activo', 'documento1.pdf', '2024-05-03', '2024-04-01');

INSERT INTO usuario (dni, nombre, apellido, error, status, file_name, update_date, start_date) 
VALUES (87654321, 'María', 'Gómez', NULL, 'Inactivo', 'documento2.pdf', '2024-05-02', '2024-03-15');

INSERT INTO usuario (dni, nombre, apellido, error, status, file_name, update_date, start_date) 
VALUES (98765432, 'Pedro', 'López', NULL, 'Activo', 'documento3.pdf', '2024-04-30', '2024-02-20');

INSERT INTO usuario (dni, nombre, apellido, error, status, file_name, update_date, start_date) 
VALUES (23456789, 'Laura', 'Martínez', NULL, 'Inactivo', 'documento4.pdf', '2024-04-29', '2024-01-10');

INSERT INTO usuario (dni, nombre, apellido, error, status, file_name, update_date, start_date) 
VALUES (34567890, 'Ana', 'Rodríguez', NULL, 'Act
```