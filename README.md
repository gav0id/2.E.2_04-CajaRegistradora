Ejercicio 2.E.2 04 - Caja Registradora

Lógica del programa
Para resolver este ejercicio, diseñé la clase `CajaRegistradora` con el objetivo de llevar el control del dinero ingresado y la cantidad de operaciones. Para esto, definí dos atributos: `montoRecaudado` (double) y `totalVentasRealizadas` (int). 

Implementé un constructor sin parámetros que se encarga de inicializar explícitamente ambos atributos en `0` cada vez que se crea una nueva caja.

Para el comportamiento, desarrollé dos métodos:
1. `registrarVenta(double monto)`: Un método de tipo `void` que actualiza el estado del objeto. Recibe el importe de una venta, lo acumula en el `montoRecaudado` y aumenta en 1 el contador de `totalVentasRealizadas`.
2. `obtenerPromedioVenta()`: Un método con retorno que calcula el ticket promedio. Para hacerlo robusto, incluí una estructura condicional (`if/else`) que verifica que `totalVentasRealizadas` sea mayor a 0 antes de hacer la división. De esta manera, evito un error matemático de división por cero en caso de que se llame al método antes de registrar la primera venta.

Dentro de la clase `Main`, implementé la siguiente lógica de prueba:
1. Instancié un objeto de tipo `CajaRegistradora`.
2. Evoqué el método `registrarVenta()` tres veces consecutivas, pasándole distintos montos de prueba (67.0, 93.0 y 250.0).
3. Finalmente, imprimí por consola el resultado devuelto por el método `obtenerPromedioVenta()` para verificar que el cálculo y la actualización de los atributos funcionaran de manera conjunta.

#Ejecución en consola
<img width="1366" height="719" alt="{F190B15A-046B-4399-ABAC-3D7FABBE4CA0}" src="https://github.com/user-attachments/assets/7b48eeaf-c95f-40bb-a00e-c67408e7fa0e" />
