# Archivos

Esta es una librería simple en Java que te permite realizar diversas operaciones de manipulación de archivos, como leer, escribir, crear, eliminar, copiar y mover archivos.

## Uso

1. **Descargar la librería**: Puedes descargar el archivo `.jar` de la librería desde [aquí](enlace_al_jar).

2. **Agregar la librería a tu proyecto Java**:

    - Si estás utilizando un IDE como Eclipse o IntelliJ, puedes agregar la librería a tu proyecto como una dependencia.
    
    - Si estás compilando desde la línea de comandos, puedes usar el comando `javac` y especificar la ruta al archivo `.jar` de la librería.

3. **Ejemplo de Uso**:

```java
import java.io.IOException;

public class EjemploArchivo {

    public static void main(String[] args) {
        // Crear una instancia de la clase Archivo
        Archivo archivo = new Archivo("miarchivo.txt");

        // Leer el contenido de un archivo
        String contenido = archivo.leer();
        System.out.println("Contenido del archivo:\n" + contenido);

        // Escribir en un archivo
        String textoAEscribir = "Hola, mundo!";
        archivo.escribir(textoAEscribir);

        // Crear un archivo
        archivo.crearArchivo();

        // Eliminar un archivo
        archivo.eliminarArchivo();

        // Copiar un archivo a un directorio de destino
        archivo.copiarArchivo("directorio_destino/");

        // Mover un archivo a un directorio de destino
        archivo.moverArchivo("directorio_destino/");

    }
}
