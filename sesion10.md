<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 10 


<!-- Su documentación aquí -->

## Ejercicio 1:

Crea una clase abstracta Vehículo con métodos abstractos acelerar(), frenar() y girar(). Las clases Coche, Moto y Bicicleta heredan de la clase Vehículo y sobreescriben los métodos abstractos para implementar su propio comportamiento.<br>

```
public abstract class Vehiculo {
    public abstract String acelerar();
    public abstract String frenar();
    public abstract String girar();
}
```
## Coche

```
public class Coche extends Vehiculo{

    @Override
    public String acelerar() {
        return "El Coche esta acelerando";
    }

    @Override
    public String frenar() {
        return "El Coche frenando";
    }

    @Override
    public String girar() {
        return "El Coche esta girnado";
    }
}
```
## Moto

```
public class Moto extends Vehiculo{
    @Override
    public String acelerar() {
        return "La Moto esta Acelerando";
    }

    @Override
    public String frenar() {
        return "La Moto esta Frenando";
    }

    @Override
    public String girar() {
        return "La Moto esta girando";
    }
}
```

## Bicicleta

```
public class Bicicleta extends Vehiculo{
    @Override
    public String acelerar() {
        return "La Bicicleta esta acelerando";
    }

    @Override
    public String frenar() {
        return "La bicicleta esta frenando";
    }

    @Override
    public String girar() {
        return "La bicicleta esta girando";
    }
}
```

## Ejercicio 2:

Crea una clase abstracta Producto con métodos abstractos calcularPrecio() y calcularImpuesto(). Las clases Libro, CD y DVD heredan de la clase Producto y sobreescriben los métodos abstractos para implementar su propio cálculo de precio e impuesto.<br>

```
public abstract class Producto {
    private int cantidad;
    private double precio;
    private double impuesto;
    public Producto(int cantidad,double precio,double impuesto) {
        this.cantidad = cantidad;
        this.precio = precio;
        this.impuesto = impuesto;
    }
    public double getImpuesto() {
        return impuesto;
    }
    public int getcantidad() {
        return cantidad;
    }
    public double getPrecio() {
        return precio;
    }
    abstract double calcularPrecio();
    abstract double calcularImpuesto();
}
```

## CD


```
public class CD extends Producto{
    public CD(int cantidad,double precio,double impuesto){
        super(cantidad, precio, impuesto);
    }
    @Override
    double calcularPrecio() {
        double precioCD = getPrecio() * getcantidad();
        return precioCD;
    }
    @Override
    double calcularImpuesto() {
        double impuestosCD =  calcularPrecio() * getImpuesto();
        return impuestosCD;
    }
}
```

## DVD

```
public class DVD extends Producto{
    public DVD(int cantidad,double precio,double impuesto){
        super(cantidad, precio, impuesto);
    }
    @Override
    double calcularPrecio() {
        double precioCD = getPrecio() * getcantidad();
        return precioCD;
    }
    @Override
    double calcularImpuesto() {
        double impuestosCD =  calcularPrecio() * getImpuesto();
        return impuestosCD;
    }
}
```

## Libro

```
public class Libro extends Producto{
    public Libro(int cantidad,double precio,double impuesto){
        super(cantidad, precio, impuesto);
    }
    @Override
    double calcularPrecio() {
        double precioCD = getPrecio() * getcantidad();
        return precioCD;
    }
    @Override
    double calcularImpuesto() {
        double impuestosCD =  calcularPrecio() * getImpuesto();
        return impuestosCD;
    }
}
```

## Ejercicio 3:

Crea una clase abstracta Cuenta con métodos abstractos depositar(), retirar() y consultarSaldo(). Las clases CuentaCorriente, CuentaAhorro y CuentaPlazoFijo heredan de la clase Cuenta y sobreescriben los métodos abstractos para implementar su propio comportamiento.<br>

```
public abstract class Cuenta {
    abstract double depositar();
    abstract double retirar();
    abstract double consultarSaldo();
}
```

## CuentaCorriente

```
public class CuentaCorriente extends Cuenta{


    public CuentaCorriente(double saldo) {
        super(saldo);
    }

    @Override
    double depositar(double valor) {

        return getSaldo();
    }

    @Override
    double retirar(double ValorR) {
        return 0;
    }

    @Override
    double consultarSaldo() {
        return 0;
    }
}
```

```
public class CuentaAhorro extends Cuenta{
    public CuentaAhorro(double saldo) {
        super(saldo);
    }

    @Override
    double depositar(double valor) {
        return 0;
    }

    @Override
    double retirar(double ValorR) {
        return 0;
    }

    @Override
    double consultarSaldo() {
        return 0;
    }
}
```



```
public class CuentaPlazoFijo extends Cuenta{
    public CuentaPlazoFijo(double saldo) {
        super(saldo);
    }

    @Override
    double depositar(double valorD) {
        System.out.println("Valor ingresado: "+valorD);
        double valorDep = getSaldo() + valorD;
        System.out.println("El nuevo saldo es: " + valorDep);
        setSaldo(valorDep);
        return valorDep;
    }

    @Override
    double retirar(double ValorR) {
        return 0;
    }

    @Override
    double consultarSaldo() {
        return 0;
    }
}
```

```
public abstract class Cuenta {
    private double saldo;

    public Cuenta(double saldo) {
        this.saldo = saldo;
    }

    public double getSaldo() {
        return saldo;
    }

    public void setSaldo(double saldo) {
        this.saldo = saldo;
    }

    abstract double depositar(double valorD);
    abstract double retirar(double ValorR);
    abstract double consultarSaldo();
}
```