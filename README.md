# Punto de Venta con TDD · Flutter + SQLite

**Materia:** Desarrollo Móvil Integral
**Universidad:** UTNG, Dolores Hidalgo
**Profesor:** Anastacio Rodríguez García
**Alumno:** González López Yael Isaac
**Fecha:** 26 - octubre - 2026

## Descripción

Punto de venta que guarda productos y ventas en una base de datos SQLite local (funciona sin internet). Calcula totales, IVA y cambio usando centavos enteros, descuenta el inventario al cobrar con una transacción y hace el corte del día. Se desarrolló con TDD (prueba en rojo, código en verde, refactor).

## Estructura del proyecto

![Estructura del proyecto](capturas/01_estructura.jpeg)

## Pruebas realizadas

### 1. Pruebas de dominio (11 pruebas)

![Pruebas de dominio](capturas/02_pruebas_dominio.jpeg)

### 2. Pruebas de datos (6 pruebas)

![Pruebas de datos](capturas/03_pruebas_datos.jpeg)

### 3. Todas las pruebas juntas

![Todas las pruebas en verde](capturas/04_todas_las_pruebas.jpeg)

## Evidencia de la aplicación

### Catálogo de productos
![Catálogo](capturas/05_catalogo.jpeg)

### Cobro exitoso
Dos nieves de limón, pago de $100.00, cambio de $50.00 y existencias de 40 a 38.

![Cobro exitoso](capturas/06_cobro_exitoso.jpeg)

### Pago insuficiente
![Pago insuficiente](capturas/07_pago_insuficiente.jpeg)

## Ciclo TDD (opcional)

Captura de una prueba en ROJO antes de crear el código:

![Prueba en rojo](capturas/08_prueba_roja.jpeg)

## Conclusión 
 
 SI