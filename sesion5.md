<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 5 


<!-- Su documentación aquí -->

## Actividad: Implementación de las Clases Automóvil y Motocicleta utilizando la herencia en java

Implementar las clases derivadas (Automovil y Motocicleta) que hereden de la clase base (Vehiculo) en Java.

```
// Clase base: Vehiculo
class Vehiculo {
    protected String marca; // Cambiamos a protegido
    protected String modelo; // Cambiamos a protegido
    private int año;

    public Vehiculo(String marca, String modelo, int año) {
        this.marca = marca;
        this.modelo = modelo;
        this.año = año;
    }

    public void mostrarInformacion() {
        System.out.println("Marca: " + marca);
        System.out.println("Modelo: " + modelo);
        System.out.println("Año: " + año);
    }
}
```

**Implementación de la clase Automovil.**

**1. Crear la clase Automovil como una clase derivada de Vehiculo y agregar los siguientes atributos privados:**

**numPuertas (int):** Número de puertas del automóvil.<br>

**tipoTransmision (String):** Tipo de transmisión del automóvil (manual o automática).<br>

**2. Implementar un constructor en la clase Automovil que acepte todos los atributos de Vehiculo (marca, modelo, año), así como los nuevos atributos (numPuertas y tipoTransmision). El constructor debe llamar al constructor de la clase base (Vehiculo) utilizando super().**

**3. Implementar el método mostrarInformacionAutomovil() en la clase Automovil. El nuevo método debe mostrar toda la información del automóvil, incluyendo el número de puertas y el tipo de transmisión.**

**4. Crear un objeto de la clase Automovil en el programa principal (main) y utilizarlo para probar la funcionalidad de la clase Automovil. Debe mostrar la información del automóvil utilizando el método mostrarInformacionAutomovil().**

**5. Agregar métodos adicionales a la clase Automovil según su creatividad y utilizarlos en el programa principal (main).**

**Implementación de la clase Motocicleta.**

**1.Crear la clase Motocicleta como una clase derivada de Vehiculo y agregar los siguientes atributos privados:**

tipo (String): El tipo de motocicleta (deportiva, crucero, etc.).

cilindraje (int): El cilindraje de la motocicleta en centímetros cúbicos (cc).

**2.Implementar un constructor en la clase Motocicleta que acepte todos los atributos de Vehiculo (marca, modelo, año), así como los nuevos atributos (tipo y cilindraje). El constructor debe llamar al constructor de la clase base (Vehiculo) utilizando super().**

Implementar el método mostrarInformacionMotocicleta() en la clase Motocicleta. El nuevo método debe mostrar toda la información de la motocicleta, incluyendo el tipo y el cilindraje.

Crear un objeto de la clase Motocicleta en el programa principal (main) y utilizarlo para probar la funcionalidad de la clase Motocicleta. Debe mostrar la información de la motocicleta utilizando el método mostrarInformacionMotocicleta().

Agregar métodos adicionales a la clase Motocicleta según su creatividad y utilizarlos en el programa principal (main).