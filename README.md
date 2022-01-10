# Ejercitacion SQL II Alkemy
***

## Tema 1

1. Escriba una consulta para saber cuántos estudiantes son de la carrera Mecánica.
Para la resolucion se usaron las tablas disponibles en el material descargado.

`SELECT COUNT(legajo) FROM ESTUDIANTE WHERE carrera='Mecánica'`

2. Escriba una consulta para saber, de la tabla PROFESOR, el salario mínimo de los profesores nacidos en la década del 80.

`SELECT MIN FROM PROFESOR WHERE fecha_nacimiento BETWEEN '1980-01-01' AND '1989-12-31'`

4. Cantidad de pasajeros por pais:

 `SELECT PAIS.idpais, COUNT(*) as 'Cantidad de pasajeros por pais' FROM PAIS INNER JOIN PASAJERO ON PAIS.idpais=PASAJERO.idpais GROUP BY PAIS.idpais`

5. Suma de todos los pagos realizados:

`SELECT SUM(monto) FROM pago`

6. Suma de todos los pagos que realizo un pasajero. Monto debe aparecer con 2 decimales:

`SELECT ROUND(SUM(monto), 2) FROM pago WHERE idpasajero='algun id de pasajero'`

7. Promedio de los pagos que realizo un pasajero:

`SELECT AVG(monto) FROM pago WHERE idpasajero='algun id de pasajero'`

***
## Tema 2:

