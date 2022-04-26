# Diferencias-entre-primitivo-y-referencia

* Las variables de tipo referencia como String, Thread, File y otros

* Las variables de referencia no son punteros, sino un identificador del objeto que se crea en la heap memory

* La variable tipo primitivo nunca puede ser null, mientras que las referenciadas si son null sino se le asigna ningun valor

### Pasar la primitiva y la variable de referencia como argumento del método

* Los parámetros formales son aquellos que se enumeran (junto con su tipo) en la declaración del método, por ejemplo, en getName(Employee e), e es un parámetro formal

* Los parámetro reales son aquellos que se pasan al método durante la invocación por ejemplo , getName(new Employee("John")) 
 
* Cuando pasa valores primitivos a un método, los valores se pasan al método, pero cuando pasa la variable de referencia, solo se copia el identificador. lo que significa que para las primitivas, cambiar el valor del parámetro formal no afecta el valor del parámetro real.

* Mientras que en el caso de los tipos de referencia, cambiar el identificador del parámetro formal no afecta la dirección del parámetro real, pero cambiar los valores internos del parámetro formal sí afecta el objeto del parámetro real porque se refieren al mismo objeto en la memoria.

* Para comparar tipos de datos referenciados toca usar x.equals(y)

### Retorno de un método

* Cuando devuelve tipos primitivos de un método, se devuelve el valor primitivo. Todas las variables locales primitivas se destruyen una vez que el método finaliza su ejecución. 

* Cuando devuelve un tipo de referencia, solo se devuelve el identificador. Esto significa que un objeto creado localmente puede sobrevivir incluso después de que el método termine su ejecución, si se devolvió desde un método o si se almacenó en cualquier variable miembro.



### Apilar vs Montón

* Las variables primitivas se crean en la pila, mientras que la variable de referencia se crea en el espacio de almacenamiento dinámico, que es administrado por Garbage Collector. 

### El consumo de memoria

* Las variables primitivas de tamaño ocupan menos memoria que las variables de referencia porque no necesitan mantener los metadatos del objeto.
