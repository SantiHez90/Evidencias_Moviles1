<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 3 


<!-- Su documentación aquí -->

## Actividad: Análisis de la Clase 'Jugadores' en Java"

Analizar y comprender las diferentes partes de la clase "Jugadores" proporcionada. La clase representa a los jugadores de un equipo deportivo y contiene atributos y métodos para gestionar la información de los jugadores. El objetivo principal es identificar y comprender las distintas secciones de la clase, incluyendo sus atributos y métodos.

**1. Examinar detenidamente la clase "Jugadores" proporcionada en el enunciado.**<br>

Clase “Jugadores” en: https://doc-pami.vercel.app/docs/actividades/actividad3
<br>

**2. Identificar y etiquetar cada una de las siguientes partes de la clase:**<br>

**a. Atributos (variables de instancia)**<br>

```
private String nombre;
private int edad;
private String posicion;
private int numero_camiseta;
private String equipo;
```
<br>

**nombre:** Este es de tipo cadena (String) y tiene un modificador de tipo privado.<br>
**edad:** Es de tipo entero (int) y tiene un modificador de tipo privado.<br>
**posicion:** Es de tipo cadena (String) y tiene un modificador de tipo privado.<br>
**numero-camiseta:** Es de tipo entero (int) y tiene un modificador de tipo privado.<br>
**equipo:** Es de tipo cadena (String) y tiene un modificador de tipo privado.<br>

**b. Constructor**<br>
```
public Jugadores(String nombre, int edad, String posicion, int numero_camiseta, String equipo) {
    this.nombre = nombre;
    this.edad = edad;
    this.posicion = posicion;
    this.numero_camiseta = numero_camiseta;
    this.equipo = equipo;
}
```

El constructor permite inicializar la clase, este tiene el mismo nombre de la clase, no retorna nada, además el constructor establece los tipos de variables que se tienen que recibir para crear un objeto de la clase Jugadores.

**c. Métodos de acceso (getters) para cada atributo**<br>

```
public String getNombre() {
    return nombre;
}

public int getEdad() {
    return edad;
}

public String getPosicion() {
    return posicion;
}

public int getNumero_camiseta() {
    return numero_camiseta;
}

public String getEquipo() {
    return equipo;
}
```

Estos son los métodos “getters”, estos métodos permiten acceder a los atributos, independientemente si es público o privado

**d. Métodos de modificación (setters) para cada atributo**<br>

```
public void setNombre(String nombre) {
    this.nombre = nombre;
}

public void setEdad(int edad) {
    this.edad = edad;
}

public void setPosicion(String posicion) {
    this.posicion = posicion;
}

public void setNumero_camiseta(int numero_camiseta) {
    this.numero_camiseta = numero_camiseta;
}

public void setEquipo(String equipo) {
    this.equipo = equipo;
}
```

Estos son los metodos "setters", esots métodos permiten actualizar el atributo

**e. Método "toString()" para representación en cadena**<br>

```
  public String toString() {
    return "Jugadores{" +
        "nombre='" + nombre + '\'' +
        ", edad=" + edad +
        ", posicion='" + posicion + '\'' +
        ", numero_camiseta=" + numero_camiseta +
        ", equipo='" + equipo + '\'' +
        '}';
  }
```

**3. Crear una presentación de diapositivas que incluya:**<br>

**a. Una diapositiva introductoria con el título de la actividad.**<br>
**b. Diapositivas etiquetadas para cada parte de la clase identificada en el paso 2.**<br>
**c. Diapositivas explicativas que detallen las funciones y utilidades de las partes de la clase.**<br>

https://www.canva.com/design/DAFtUn5dw0E/btm7NezsJyIRMtz31XD66A/view?utm_content=DAFtUn5dw0E&utm_campaign=designshare&utm_medium=link&utm_source=publishsharelink

**4. Presentar la presentación de diapositivas al grupo, compartiendo los hallazgos y conclusiones.**<br>