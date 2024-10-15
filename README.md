# Conversor de Monedas

Este proyecto es un conversor de monedas que permite realizar conversiones entre varias divisas populares 
y guardar los resultados en un archivo JSON. La aplicación interactúa con una API externa para 
obtener las tasas de conversión actualizadas. 
Está compuesto por varias clases que gestionan la consulta a la API, el procesamiento de los resultados 
y la presentación del cambio realizado.

## Funcionalidades
**Convertir entre las siguientes monedas:**
- Dólar (USD) y Peso Argentino (ARS)
- Dólar (USD) y Real Brasileño (BRL)
- Dólar (USD) y Peso Colombiano (COP)
- Mostrar el resultado de la conversión en pantalla.
- Guardar los resultados de las conversiones en un archivo JSON.
- Finalizar el programa automáticamente después de guardar los resultados.

## Requisitos

- Java 17 o superior.
- Dependencias externas para consultas HTTP (por ejemplo, `HttpClient` de Java o alguna librería como `OkHttp`).
- Clave API válida para realizar consultas de conversión de moneda (obtenida de una API de cambio de divisas).

## Estructura del Proyecto
### Main.java
El punto de entrada de la aplicación. Esta clase coordina las interacciones con el usuario, solicita las monedas y el monto a convertir, 
y luego utiliza la clase ConsultaApi para obtener los datos de la API.

### ConsultaApi.java
Esta clase maneja la conexión a una API externa de conversión de monedas. Recibe como parámetros la moneda base y la moneda objetivo,
y devuelve un objeto ResultadoDelCambio con los detalles de la conversión.

### GeneradorDeJson.java
Responsable de gestionar la estructura de los datos JSON necesarios para interactuar con la API de conversión de monedas.

### ResultadoDelCambio.java
Esta clase es un record que almacena los resultados de la conversión de moneda, como el monto convertido y la tasa de cambio. 
También incluye los métodos mostrarResultado y almacenarResultado para imprimir los resultados y almacenarlos en una lista si es necesario.

## Capturas paso a paso
Mensaje de bienvenida y pedido de una APIKey para funcionar
![Vista previa del conversor](C:/Users/John Marlon/Desktop/java-conversor-monedas/image1.jpeg)

Presentación del menú de opciones

Selección de la opción 1 y el monto a convertir

Devuelve la información de la conversión y ofrece nuevamente el menú de opciones

Este `README.md` cubre la funcionalidad básica del proyecto. Si hay algún aspecto que te gustaría ampliar o modificar, no dudes en decírmelo.







