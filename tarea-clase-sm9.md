# Deber de base de datos
# Usando la base de datos de EVENTS generar las siguientes sentencias:

## 1. Obtener la edad promedio de los miembros:
- sentencia 
```
SELECT AVG(age) AS average_age 
FROM members;
```
- captura
<img src="image.png" alt="drawing" width="500"/>

## 2. Obtener la edad mínima de los miembros:
- sentencia
```
SELECT MIN(age) AS minimum_age
FROM members;
```
- captura
<img src="Capturas/Captura de pantalla 2024-06-11 234746.png" alt="drawing" width="500"/>

## 3. Obtener el número total de registros asistidos:
- sentencia
```
SELECT COUNT(*) AS total_registrations
FROM registers;
```
- captura
<img src="Capturas/Captura de pantalla 2024-06-11 235203.png" alt="drawing" width="500"/>

## 4. Obtener el número total de asistentes a todas las conferencias: 
- sentencia 
```
SELECT COUNT(DISTINCT member_id) AS total_attendees
FROM registers;
```
-captura
<img src="Capturas/Captura de pantalla 2024-06-11 235631.png" alt="drawing" width="500"/>

## 5. Obtener el número total de eventos por cada ciudad:
- sentencia
```
SELECT city, COUNT(*) AS total_events
FROM conferences
GROUP BY city;
```
- captura 
<img src="Capturas/Captura de pantalla 2024-06-12 000012.png" alt="drawing" width="500"/>

## 6. Obtener el número de registros por cada miembro:
- sentecia 
```
SELECT member_id, COUNT(*) AS registrations_count
FROM registers
GROUP BY member_id;
```
- captura 
<img src="Capturas/Captura de pantalla 2024-06-12 000248.png" alt="drawing" width="500"/>

## 7. Obtener el número de registros por cada conferencia:
- sentencia 
```
SELECT member_id, COUNT(*) AS registrations_count
FROM registers
GROUP BY member_id; 
```
- captura 
<img src="Capturas/Captura de pantalla 2024-06-12 000612.png" alt="drawing" width="500"/>