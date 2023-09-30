<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 7 


<!-- Su documentación aquí -->

## Actividad: Clase Producto con Métodos Sobrecargados

Crea una clase llamada Producto que representará productos en una tienda en línea. La clase debe tener los siguientes atributos privados:

nombre (String): El nombre del producto.<br>
precio (double): El precio del producto.<br>
cantidad (int): La cantidad de unidades disponibles del producto.<br>

La clase Producto debe tener los siguientes constructores sobrecargados:

Un constructor por defecto que inicialice el nombre como "Desconocido", el precio como 0.0 y la cantidad como 0.<br>
Un constructor que tome como argumentos el nombre y el precio del producto, y establezca la cantidad en 0.<br>
Un constructor que tome como argumentos el nombre, el precio y la cantidad del producto.<br>

La clase Producto debe tener los siguientes métodos:

calcularValorTotal(): Un método que calcule y devuelva el valor total del producto en base a su precio y cantidad.<br>
mostrarInformacion(): Un método que muestre por consola la información del producto, incluyendo el nombre, precio, cantidad y valor total.<br>

Además, debes agregar los siguientes métodos sobrecargados:

incrementarCantidad(): Un método sobrecargado que incremente la cantidad en 1 unidad.<br>

incrementarCantidad(int cantidadIncrementar): Un método sobrecargado que permita incrementar la cantidad en una cantidad específica proporcionada como argumento.<br>

actualizarPrecio(double nuevoPrecio): Un método sobrecargado que permita actualizar el precio del producto en dólares con un nuevo valor proporcionado como argumento.<br>

actualizarPrecio(double nuevoPrecio, String moneda): Un método sobrecargado que permita actualizar el precio del producto en dólares con un nuevo valor proporcionado como argumento, teniendo en cuenta la moneda especificada y utilizando las tasas de conversión adecuadas. Debes asumir tasas de conversión fijas para las monedas admitidas.<br>

actualizarPrecio(double nuevoPrecio, String moneda, double tasaCambio): Un método sobrecargado que permita actualizar el precio del producto en dólares con un nuevo valor proporcionado como argumento, teniendo en cuenta la moneda especificada y la tasa de cambio proporcionada.<br>

En el método main, crea tres instancias de la clase Producto utilizando los diferentes constructores, muestra la información de los productos y realiza algunas operaciones para probar los métodos sobrecargados, incluyendo la actualización de precios en euros y pesos colombianos con tasas de conversión específicas.