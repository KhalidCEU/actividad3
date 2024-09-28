## Actividad 3 - Padrón de habitantes


### Usage

**Compile:** ```find src -name "*.java" | xargs javac -cp bin -d bin```

**Test / Run:**

```java -cp bin src.aplicacion.Principal mostrar``` (shows the 'habitantes' in the .csv)

```java -cp bin src.aplicacion.Principal añadir Andrés Pérez García``` (adds an 'habitante' to the .csv)


### Respuestas

**Ejercicio 10.2**

**P:** Explicación de código

**R:** Tenemos una clase **Habitante** que contiene tres atributos de tipo **String** y con modificadores de acceso **privados** (solo se pueden acceder desde esta misma clase). También contiene tres setters respectivos para esos atributos. Cada setter necesita un parametro (con el mismo nombre que el atributo correspondiente), y dentro se utiliza  ```this``` para asignar el valor del parametro al atributo de la clase.

(PS:  ```this``` en este caso nos permite distinguir y por lo tanto utilizar el mismo nombre para el parametro y el atributo).


-------

**Ejercicio 11.4**

**P:** Explique qué significa que un método sea estático.

**R:** Que un método sea estático significa que pertenece a su clase, con lo cual puede ser invocado sin necesidad de crear objetos (no depende de sus instancias). Es por ello que usamos ```Comprobacion.realizarComprobacion()``` directamente en vez de crear un objeto e invocar su método.

-------

**Ejercicio 12.3**

**P:** Una vez se ha definido el constructor con parámetros para la clase
Habitante, ¿qué es necesario hacer para que siga compilando la siguiente invocacion?
```new Habitante();```

**R:** Ahora como **Habitante** tiene un constructor que requiere 3 parametros, para que siga compilando
al crear un objeto con ```new Habitante();```, debemos pasarle parametros a esa invocación, como
hemos hecho en el fichero **Comprobacion.java** de la siguiente manera : ```new Habitante("Juan", "Torres", "Sanz");```

-------

**Ejercicio 16.4**

**P:** Explique el significado de la declaración ```String[] instrucción```

**R:** La declaracion ```String[] instruccion``` en este caso nos indica que el método ```ejecutar()``` necesita como parametro una lista (un array) de strings.

-------

**Ejercicio 17**

**P:** Explique que es un paquete.

**R:** En Java, un paquete ("package") es un contenedor que sirve para organizar y agrupar clases e interfaces relacionadas dentro de un mismo espacio de nombres ("namespace"). Los paquetes son útiles para gestionar el código, evitar conflictos de nombres y facilitar la mantenibilidad, modularidad y reutilización del código.

