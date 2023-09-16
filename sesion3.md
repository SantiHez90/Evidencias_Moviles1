<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 3 


<!-- Su documentación aquí -->
Analizar y comprender las diferentes partes de la clase "Jugadores" proporcionada. La clase representa a los jugadores de un equipo deportivo y contiene atributos y métodos para gestionar la información de los jugadores. El objetivo principal es identificar y comprender las distintas secciones de la clase, incluyendo sus atributos y métodos.
1.	Examinar detenidamente la clase "Jugadores" proporcionada en el enunciado.
<br>
**Clase “Jugadores” en: https://doc-pami.vercel.app/docs/actividades/actividad3**
2.	Identificar y etiquetar cada una de las siguientes partes de la clase:
•	a. Atributos (variables de instancia)
<br>
**private String nombre;
<br>
private int edad;
<br>
private String posicion;
<br>
private int numero_camiseta;
<br>
private String equipo;**
<br>
nombre: Este es de tipo cadena (String) y tiene un modificador de tipo privado.
edad: Es de tipo entero (int) y tiene un modificador de tipo privado.
posicion: Es de tipo cadena (String) y tiene un modificador de tipo privado.
numero-camiseta: Es de tipo entero (int) y tiene un modificador de tipo privado.
equipo: Es de tipo cadena (String) y tiene un modificador de tipo privado.
Al tener el modificador de tipo privado, solo se puede acceder a esta mediante un método y para que no sean modificados
•	b. Constructor
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
•	c. Métodos de acceso (getters) para cada atributo
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
•	d. Métodos de modificación (setters) para cada atributo
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
•	e. Método "toString()" para representación en cadena
 
3.	Crear una presentación de diapositivas que incluya:
•	Una diapositiva introductoria con el título de la actividad.
•	Diapositivas etiquetadas para cada parte de la clase identificada en el paso 2.
•	Diapositivas explicativas que detallen las funciones y utilidades de las partes de la clase.
4.	Presentar la presentación de diapositivas al grupo, compartiendo los hallazgos y conclusiones.







