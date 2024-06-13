# Deber base de datos 
# Sentencias where multicriterio

## 1. Contar el número de productos de una categoría específica:
- sentencia
```
SELECT COUNT (*) AS categoria_Audio 
FROM product 
WHERE category = 'Electronics'; 
```
- captura
<img src="Capturas/Captura de pantalla 2024-06-12 192517.png" alt="drawing" width="500"/>

## 2. Contar el número de clientes en una ciudad específica:
- sentencia 
```
SELECT COUNT(*) AS number_of_clients
FROM client
WHERE city = 'San Diego';
```
- captura
<img src="Capturas/Captura de pantalla 2024-06-12 193148.png" alt="drawing" width="500"/>

## 3. Contar el número de productos cuyo precio está dentro de un rango específico:
- sentencia
```
SELECT COUNT (*) AS products_price_range_from_90_to_500 
FROM product 
WHERE price > 90 AND price < 500;
```
- captura 
<img src="Capturas/Captura de pantalla 2024-06-12 193544.png" alt="drawing" width="500"/>

## 4. Seleccionar clientes que viven en una ciudad específica y tienen un tipo de cliente específico:
- sentencia 
```
SELECT * 
FROM client 
WHERE city = 'Philadelphia' AND type_of_client = 'Retai';
```
- captura
<img src="Capturas/Captura de pantalla 2024-06-12 193836.png" alt="drawing" width="500"/>

## 5. Seleccionar productos que pertenecen a una categoría específica y cuyo precio está por encima de un valor específico:
- sentencia 
```
SELECT * 
FROM product 
WHERE category = 'Electronics' AND price >= 90;
```
- captura
<img src="Capturas/Captura de pantalla 2024-06-12 194109.png" alt="drawing" width="500"/>

## 6. Seleccionar productos que fueron producidos en un año específico y en un país de origen específico:
- sentencia
```
SELECT * 
FROM product 
WHERE year_of_production = '2023' AND country_of_origin = 'USA';
```
- captura
<img src="Capturas/Captura de pantalla 2024-06-12 194340.png" alt="drawing" width="500"/>

## 7. Seleccionar clientes cuyo nombre completo comience con 'J':
- sentencia 
```
SELECT * 
FROM client 
WHERE full_name LIKE 'J%';
```
- captura
<img src="Capturas/Captura de pantalla 2024-06-12 194609.png" alt="drawing" width="500"/>

## 8. Seleccionar clientes cuya ciudad contenga la letra 'a':
- sentencia 
```
SELECT * 
FROM client 
WHERE city LIKE '%A%';
```
- captura
<img src="Capturas/Captura de pantalla 2024-06-12 194800.png" alt="drawing" width="500"/>
