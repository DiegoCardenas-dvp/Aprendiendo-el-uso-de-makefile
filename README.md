# Uso de Makefile

- El objetivo de esta tarea es dominar la estructura y funcionalidad de un Makefile, entendiendo cómo se utiliza para automatizar y estandarizar procesos de programación. Los Makefiles permiten organizar la compilación de programas de manera automática y ordenada, reduciendo errores y facilitando el trabajo en proyectos colaborativos.


### Objetivo de aprendizaje
- Identificar y comprender la estructura básica de un Makefile y su función en la automatización de proyectos.
- Explicar cómo un Makefile ayuda a estandarizar procesos de compilación.

- Aplicar los conocimientos adquiridos para crear un Makefile propio, documentarlo y organizarlo en un repositorio personal.

- Describir el funcionamiento del código del Makefile, reportando resultados de ejecución y explicando cómo se logra la automatización.

- Implementar un archivo .gitignore adecuado, compartiendo únicamente los archivos necesarios para que el repositorio sea claro y funcional.

### Desarrollo de la tarea:
######1. Se reproduce el siguiente ejercicio del <a href="https://github.com/alemanmig/Embedded-Systems-IoT/tree/74ceec830d3b09db4a7037ba9f4c23f553818250/Makefileshttps://github.com/alemanmig/Embedded-Systems-IoT/tree/74ceec830d3b09db4a7037ba9f4c23f553818250/Makefiles">repositorio</a> haciendo uso del makefile en el archivo c ***main.c*** ejecutando el siguiente código:
```
#include <stdio.h>
int main(void) {
    printf("Hola desde un ejemplo basico de Makefile.\n");
    printf("Este programa fue compilado y ejecutado con make.\n");
    return 0;
}
 ```
######2.  Con ayuda del las instrucciones del archivo Makefile, se ejecutan las instrucciones dadas:
```
CC = gcc: Define el compilador. Facilita la portabilidad (por ejemplo, si luego usas g++ para C++).

CFLAGS = -Wall -Wextra -O2: Banderas de compilación.

-Wall -Wextra: Te avisan de prácticamente cualquier error potencial en tu código.

-O2: Optimiza el código para que corra más rápido.

TARGET = hola: El nombre del ejecutable final.

SRCS = main.c: Lista de archivos fuente.

OBJS = $(SRCS:.c=.o): Esta es una sustitución de sufijos. Le dice a Make: "toma todo lo que esté en SRCS y cambia la extensión .c por .o". Así automatizas la lista de archivos objeto.
```
![salidaMainC](\makefileEjercicios\makefile1\makefile1\evidencias\salidaMK1.png "salidaMF")




