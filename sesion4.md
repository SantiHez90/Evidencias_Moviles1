<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 4


<!-- Su documentación aquí -->

## Actividad: Creación de una clase de producto con modificadores de acceso y getters y setters

**Objetivo:**<br>

Evaluar la capacidad de para crear clases con modificadores de acceso, private, default, protected, final, static. Además, evaluar el uso de getter y setter.

**Descripción:**<br>

Crear una clase llamada Producto con los siguientes atributos:

nombre: un atributo de tipo String que representa el nombre del producto.<br>
precio: un atributo de tipo double que representa el precio del producto.<br>
cantidad: un atributo de tipo int que representa la cantidad disponible del producto.<br>
fabricante: un atributo de tipo String que representa el fabricante del producto.<br>
marca: un atributo de tipo String que representa la marca del producto.<br>
categoría: un atributo de tipo String que representa la categoría del producto.<br>

Utilizar los modificadores de acceso para controlar el acceso a los atributos de la clase. Por ejemplo, el atributo nombre debería ser público, el atributo precio debería ser privado, el atributo cantidad debería ser protegido, el atributo fabricante debería ser final, el atributo marca debería ser static, y el atributo categoría debería ser default.

Utilizar getter y setter para acceder y modificar los valores de los atributos de la clase. Por ejemplo, el método getNombre() debería devolver el valor del atributo nombre, y el método setNombre() debería establecer el valor del atributo nombre.

**Instrucciones:**<br>

Cree una clase llamada Producto.
Agregue los atributos nombre, precio, cantidad, fabricante, marca y categoría a la clase Producto.
Utilice los modificadores de acceso para controlar el acceso a los atributos de la clase.
Agregue getter y setter para acceder y modificar los valores de los atributos de la clase.
Pruebe la clase Producto creando una instancia de la clase y accediendo a los atributos de la instancia.


## Solcucion

```
public class Producto {

    public String nombre;
    private double precio;
    protected int cantidad;
    final String fabricante = "Fabricante SA";
    static String marca = "Adidas";
    String categoria;

    //Constructor
    public Producto(String nombre, double precio, int cantidad, String categoria) {
        this.nombre = nombre;
        this.precio = precio;
        this.cantidad = cantidad;
        this.categoria = categoria;
    }

    //Propiedades GET
    public String getNombre() {
        return nombre;
    }

    public double getPrecio() {
        return precio;
    }

    public int getCantidad() {
        return cantidad;
    }

    public String getFabricante() {
        return fabricante;
    }

    public static String getMarca() {
        return marca;
    }

    public String getCategoria() {
        return categoria;
    }

    //Propiedades Sett
    public void setNombre(String nombre) {
        this.nombre = nombre;
    }

    public void setPrecio(double precio) {
        this.precio = precio;
    }

    public void setCantidad(int cantidad) {
        this.cantidad = cantidad;
    }

    public static void setMarca(String marca) {
        Producto.marca = marca;
    }

    public void setCategoria(String categoria) {
        this.categoria = categoria;
    }
}
```