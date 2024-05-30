# Tarea Base de datos 

## 1. Escribir una sentencia que muestre los productos que no se registran su pais de origen 
- sentecia 
```
SELECT COUNT (*) - COUNT (country_of_origin) AS products_without_country
FROM product;
```
- captura 
<img src="Capturas/Captura de pantalla 2024-05-30 153916.png" alt="drawing" width="500"/>

## Escribir una sentencia para poder visualizar el numero de clientes por ciudad 
- sentencia 
```
SELECT DISTINCT city, COUNT(city)
FROM client
GROUP BY (city)
```
- captura
<img src="Capturas/Captura de pantalla 2024-05-30 155555.png" alt="drawing" width="500"/>