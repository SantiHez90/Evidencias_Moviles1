<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 9 


<!-- Su documentación aquí -->

**1. Completar la implementación de la aplicación de convertidor de unidades en Java, siguiendo las instrucciones de la sesión 9.**

```
public class Divisas extends Conversor{

    public Divisas(String unidadOrigen, String unidadDestino) {
        super(unidadOrigen, unidadDestino);
    }
    @Override
    public double convertir(double cantidad) {
        if (unidadOrigen.equals("Dolar") && unidadDestino.equals("Euro")){
            return (cantidad * 0.98);
        } else if (unidadOrigen.equals("Euro") && unidadDestino.equals("Dolar")) {
            return (cantidad * 1.06);
        } else if (unidadOrigen.equals("Dolar") && unidadDestino.equals("Peso colombiano")) {
            return (cantidad * 4073.34);
        } else if (unidadOrigen.equals("Peso colombiano") && unidadDestino.equals("Dolar")) {
            return (cantidad * 0.00025);
        } else if (unidadOrigen.equals("Euro") && unidadDestino.equals("Peso colombiano")) {
            return (cantidad * 4312.24);
        } else if (unidadOrigen.equals("Peso colombiano") && unidadDestino.equals("Euro")) {
            return (cantidad * 0.00023);
        }else {
            throw new IllegalArgumentException("Divisas no compatibles");
        }
    }
}
```
```
public class Longitud extends Conversor {
    public Longitud(String unidadOrigen, String unidadDestino) {
        super(unidadOrigen, unidadDestino);
    }
    @Override
    public double convertir(double cantidad) {
        if(unidadOrigen.equals("Metros") && unidadDestino.equals("Pies")){
            return (cantidad * 3.28084);
        } else if (unidadOrigen.equals("Pies") && unidadDestino.equals("Metros")) {
            return (cantidad * 0.3048);
        } else if (unidadOrigen.equals("Kilometros") && unidadDestino.equals("Millas")) {
            return (cantidad * 0.621371);
        } else if (unidadOrigen.equals("Millas") && unidadDestino.equals("Kilometros")) {
            return (cantidad * 1.60934);
        } else if (unidadOrigen.equals("Centimetros") && unidadDestino.equals("Pulgadas")) {
            return (cantidad * 0.393701);
        } else if (unidadOrigen.equals("Pulgadas") && unidadDestino.equals("Centimetros")) {
            return (cantidad * 2.54);
        } else if (unidadOrigen.equals("Yardas") && unidadDestino.equals("Metros")) {
            return (cantidad * 0.9144);
        } else if (unidadOrigen.equals("Metros") && unidadDestino.equals("Yardas")) {
            return (cantidad * 1.09361);
        } else if (unidadOrigen.equals("Millas Nauticas") && unidadDestino.equals("Kilómetros")) {
            return (cantidad * 1.852);
        } else if (unidadOrigen.equals("Kilómetros") && unidadDestino.equals("Millas Nauticas")) {
            return (cantidad * 0.539957);
        } else if (unidadOrigen.equals("Micrometros") && unidadDestino.equals("Milimetros")) {
            return (cantidad * 0.001);
        } else if (unidadOrigen.equals("Milimetros") && unidadDestino.equals("Micrometros")) {
            return (cantidad * 1000);
        } else if (unidadOrigen.equals("Decimetros") && unidadDestino.equals("Metros")) {
            return (cantidad * 0.1);
        } else if (unidadOrigen.equals("Metros") && unidadDestino.equals("Decimetros")) {
            return (cantidad * 10);
        }else {
            throw new IllegalArgumentException("Longitudes no compatibles");
        }
    }
}
```

```
public class Peso extends Conversor {
    public Peso(String unidadOrigen, String unidadDestino) {
        super(unidadOrigen, unidadDestino);
    }
    @Override
    public double convertir(double cantidad) {
        if(unidadOrigen.equals("Kilogramos") && unidadDestino.equals("Libras")){
            return (cantidad * 2.20462);
        }else if (unidadOrigen.equals("Libras") && unidadDestino.equals("Kilogramos")){
            return (cantidad * 0.453592);
        }else if (unidadOrigen.equals("Gramos") && unidadDestino.equals("Libras")){
            return (cantidad * 0.00220462);
        }else if (unidadOrigen.equals("Libras") && unidadDestino.equals("Gramos")){
            return (cantidad * 453.592);
        }else if (unidadOrigen.equals("Kilogramos") && unidadDestino.equals("Gramos")){
            return (cantidad * 1000);
        }else if (unidadOrigen.equals("Gramos") && unidadDestino.equals("Kilogramos")){
            return (cantidad * 0.001);
        }else if (unidadOrigen.equals("Toneladas") && unidadDestino.equals("Kilogramos")){
            return (cantidad * 1000);
        }else if (unidadOrigen.equals("Kilogramos") && unidadDestino.equals("Toneladas")){
            return (cantidad * 0.001);
        }else if (unidadOrigen.equals("Libras") && unidadDestino.equals("Onzas")){
            return (cantidad * 16);
        }else if (unidadOrigen.equals("Onzas") && unidadDestino.equals("Libras")){
            return (cantidad * 0.0625);
        }else if (unidadOrigen.equals("Gramos ") && unidadDestino.equals("Onzas")){
            return (cantidad * 0.035274);
        }else if (unidadOrigen.equals("Onzas") && unidadDestino.equals("Gramos")){
            return (cantidad * 28.3495);
        }else if (unidadOrigen.equals("Toneladas") && unidadDestino.equals("Libras")){
            return (cantidad * 2204.62);
        }else if (unidadOrigen.equals("Libras") && unidadDestino.equals("Toneladas")){
            return (cantidad * 0.000453592);
        }else if (unidadOrigen.equals("Toneladas") && unidadDestino.equals("Gramos")){
            return (cantidad * 1000000);
        }else if (unidadOrigen.equals("Gramos") && unidadDestino.equals("Toneladas")){
            return (cantidad * 0.000001);
        }else if (unidadOrigen.equals("Toneladas") && unidadDestino.equals("Miligramos")){
            return (cantidad * 1000000000);
        }else if (unidadOrigen.equals("Miligramos") && unidadDestino.equals("Toneladas")){
            return (cantidad * 0.000000001);
        }else if (unidadOrigen.equals("Kilogramos") && unidadDestino.equals("Miligramos")){
            return (cantidad * 1000000);
        }else if (unidadOrigen.equals("Miligramos") && unidadDestino.equals("Kilogramos")){
            return (cantidad * 0.000001);
        }else{
            throw new IllegalArgumentException("Pesos no compatibles");
        }
    }
}
```
**2.Agregar la subclase programador que contenga siguientes conversiones:**

Decimal a Binario<br>

```
```

Decimal a Hexadecimal<br>

Binario a Decimal<br>

Hexadecimal a Binario<br>