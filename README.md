# Punto de Venta con TDD · Flutter + SQLite

**Materia:** Desarrollo de Aplicaciones Móviles
**Universidad:** UTNG, Dolores Hidalgo
**Profesor:** Anastacio Rodríguez García
**Alumno:** González López Yael Isaac
**Fecha:** 26 - octubre - 2026

## Descripción

Punto de venta que guarda productos y ventas en una base de datos SQLite local (funciona sin internet). Calcula totales, IVA y cambio usando centavos enteros, descuenta el inventario al cobrar con una transacción y hace el corte del día. Se desarrolló con TDD (prueba en rojo, código en verde, refactor).

## Estructura del proyecto

![Estructura del proyecto](capturas/01_estructura.jpeg)

## Pruebas de dominio (11 pruebas)

### Prueba 1: Dinero · formatea centavos

#### Éxito
![Prueba 1 éxito](capturas/02_dominio_01_exito.png)

#### Fallo
![Prueba 1 fallo](capturas/02_dominio_01_fallo.png)

### Prueba 2: Dinero · convierte texto a centavos

#### Éxito
![Prueba 2 éxito](capturas/02_dominio_02_exito.png)

#### Fallo
![Prueba 2 fallo](capturas/02_dominio_02_fallo.png)

### Prueba 3: Dinero · rechaza texto inválido

#### Éxito
![Prueba 3 éxito](capturas/02_dominio_03_exito.png)

#### Fallo
![Prueba 3 fallo](capturas/02_dominio_03_fallo.png)

### Prueba 4: Producto · ida y vuelta a mapa conserva los datos

#### Éxito
![Prueba 4 éxito](capturas/02_dominio_04_exito.png)

#### Fallo
![Prueba 4 fallo](capturas/02_dominio_04_fallo.png)

### Prueba 5: Producto · copiarCon cambia solo lo indicado

#### Éxito
![Prueba 5 éxito](capturas/02_dominio_05_exito.png)

#### Fallo
![Prueba 5 fallo](capturas/02_dominio_05_fallo.png)

### Prueba 6: Carrito · suma cantidades del mismo producto

#### Éxito
![Prueba 6 éxito](capturas/02_dominio_06_exito.png)

#### Fallo
![Prueba 6 fallo](capturas/02_dominio_06_fallo.png)

### Prueba 7: Carrito · no excede existencias

#### Éxito
![Prueba 7 éxito](capturas/02_dominio_07_exito.png)

#### Fallo
![Prueba 7 fallo](capturas/02_dominio_07_fallo.png)

### Prueba 8: Carrito · desglosa IVA 16% del total

#### Éxito
![Prueba 8 éxito](capturas/02_dominio_08_exito.png)

#### Fallo
![Prueba 8 fallo](capturas/02_dominio_08_fallo.png)

### Prueba 9: Carrito · calcula cambio

#### Éxito
![Prueba 9 éxito](capturas/02_dominio_09_exito.png)

#### Fallo
![Prueba 9 fallo](capturas/02_dominio_09_fallo.png)

### Prueba 10: Carrito · pago insuficiente lanza

#### Éxito
![Prueba 10 éxito](capturas/02_dominio_10_exito.png)

#### Fallo
![Prueba 10 fallo](capturas/02_dominio_10_fallo.png)

### Prueba 11: Carrito · carrito vacío no cobra

#### Éxito
![Prueba 11 éxito](capturas/02_dominio_11_exito.png)

#### Fallo
![Prueba 11 fallo](capturas/02_dominio_11_fallo.png)

## Pruebas de datos (6 pruebas)

### Prueba 12: guarda y busca producto

#### Éxito
![Prueba 12 éxito](capturas/03_datos_01_exito.png)

#### Fallo
![Prueba 12 fallo](capturas/03_datos_01_fallo.png)

### Prueba 13: código duplicado lanza excepción de dominio

#### Éxito
![Prueba 13 éxito](capturas/03_datos_02_exito.png)

#### Fallo
![Prueba 13 fallo](capturas/03_datos_02_fallo.png)

### Prueba 14: cobrar descuenta inventario y registra venta

#### Éxito
![Prueba 14 éxito](capturas/03_datos_03_exito.png)

#### Fallo
![Prueba 14 fallo](capturas/03_datos_03_fallo.png)

### Prueba 15: si falla el cobro NO se descuenta inventario

#### Éxito
![Prueba 15 éxito](capturas/03_datos_04_exito.png)

#### Fallo
![Prueba 15 fallo](capturas/03_datos_04_fallo.png)

### Prueba 16: corte del día suma ventas de hoy

#### Éxito
![Prueba 16 éxito](capturas/03_datos_05_exito.png)

#### Fallo
![Prueba 16 fallo](capturas/03_datos_05_fallo.png)

### Prueba 17: bajo inventario alerta

#### Éxito
![Prueba 17 éxito](capturas/03_datos_06_exito.png)

#### Fallo
![Prueba 17 fallo](capturas/03_datos_06_fallo.png)

## Todas las pruebas juntas

![Todas las pruebas en verde](capturas/04_todas_las_pruebas.jpeg)

## Evidencia de la aplicación

### Catálogo de productos
![Catálogo](capturas/05_catalogo.jpeg)

### Cobro exitoso
Dos nieves de limón, pago de $100.00, cambio de $50.00 y existencias de 40 a 38.

![Cobro exitoso](capturas/06_cobro_exitoso.jpeg)

### Pago insuficiente
![Pago insuficiente](capturas/07_pago_insuficiente.jpeg)
