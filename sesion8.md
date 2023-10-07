<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 8 


<!-- Su documentación aquí -->

## Actividad: Clases y métodos abstractos de la superclase "Musica" en Java

Se desea crear una jerarquía de clases que permita representar diferentes tipos de música. Se ha decidido crear una superclase Musica que tenga los métodos y atributos comunes a todas las clases hijas.

La superclase Musica debe tener los siguientes métodos abstractos:

play(): reproduce la música.<br>

stop(): detiene la reproducción de la música.<br>

pause(): pausa la reproducción de la música.<br>

next(): avanza a la siguiente canción.<br>

previous(): retrocede a la canción anterior.<br>

Además, la superclase Musica debe tener un atributo titulo que indique el título de la canción.

Crear las clases hijas necesarias para representar diferentes tipos de música, como por ejemplo:

```
public abstract class Musica {
    private String titulo;
    public Musica(String titulo) {
        this.titulo = titulo;
    }
    public String getTitulo() {
        return titulo;
    }
    public abstract void play();
    public abstract void stop();
    public abstract void pause();
    public abstract void next();
    public abstract void previous();
}
```

1. **Cancion:** representa una canción en general.

Atributos Privados: Declarar dos atributos privados, artista (nombre del artista de la canción) y album (nombre del álbum de la canción).

```
public class Cancion extends Musica{
    private String artista;
    private String album;
}
```
Constructor: Implementar un constructor que acepte tres parámetros: titulo, artista y album, y que inicialice adecuadamente los atributos de la clase "Cancion". Utiliza la palabra clave super para llamar al constructor de la clase base "Musica" pasando el titulo como argumento.

```
public Cancion(String titulo, String artista, String album) {
        super(titulo);
        this.artista = artista;
        this.album = album;
    }
```

Métodos Anulados (Override): Implementar los métodos anulados (override) de la clase base "Musica" para las acciones de reproducción (play), detención (stop), pausa (pause), avanzar (next) y retroceder (previous) en la reproducción de la canción. Cada uno de estos métodos debe imprimir un mensaje informativo adecuado en la consola.

2. **BandaSonora:** representa una banda sonora de una película o serie de televisión.

Atributos Privados: Declarar un atributo privado, pelicula (nombre de la película a la que pertenece la banda sonora).

Constructor: Implementar un constructor que acepte dos parámetros: titulo y pelicula, y que inicialice adecuadamente los atributos de la clase "BandaSonora". Utiliza la palabra clave super para llamar al constructor de la clase base "Musica" pasando el titulo como argumento.

Métodos Anulados (Override): Implementar los métodos anulados (override) de la clase base "Musica" para las acciones de reproducción (play), detención (stop), pausa (pause), avanzar (next) y retroceder (previous) en la reproducción de la banda sonora. Cada uno de estos métodos debe imprimir un mensaje informativo adecuado en la consola.

3. **Album:** representa un álbum de música.

Atributos Privados: Declarar un atributo privado, canciones (una lista de objetos de tipo "Cancion" que representan las canciones del álbum).

Constructor: Implementar un constructor que acepte dos parámetros: titulo (título del álbum) y canciones (una lista de canciones del álbum), y que inicialice adecuadamente los atributos de la clase "Album". Utiliza la palabra clave super para llamar al constructor de la clase base "Musica" pasando el titulo como argumento.

Métodos Anulados (Override): Implementar los métodos anulados (override) de la clase base "Musica" para las acciones de reproducción (play), detención (stop), pausa (pause), avanzar (next) y retroceder (previous) en la reproducción del álbum. Cada uno de estos métodos debe imprimir un mensaje informativo adecuado en la consola y luego ejecutar las acciones correspondientes en cada canción del álbum.

Cada clase hija debe implementar los métodos abstractos de la superclase Musica de manera adecuada para su tipo de música.
