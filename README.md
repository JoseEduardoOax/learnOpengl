# Codigo aprendido de LearnOpenGL

### **[LearnOpengl](https://learnopengl.com/)**

El propósito de este repositorio es ir guardando y realizando los ejemplos que nos enseña [learnOpengl](https://learnopengl.com/).  Estos ejemplos tendrán variaciones porque estructurare el código de forma diferente .

El código de este repositorio solo ha sido probado en linux para ser mas especifico la distribución arch linux.

Librerías necesarias para trabajar
1. OpenGL
2. Glew
3. Glad

En la pagina [LearnOpengl](https://learnopengl.com/) viene mas detalle de como instalar las librearías


# Compilando librería glad
En el curso usan cmake para compilar los ejemplos y librerías, en nuestro caso usaremos los archivos makefile.

En este repositorio se incluye la librería glad que generamos de su pagina.
Para compilar glad ejecutamos los siguientes comandos
```
cd lib/glad
make cleanall
make
```
Nos generara un archivo libglad.a el cual nos servira para nuestros ejemplos que iremos aprendiendo

Esta librería puede ir dentro de cada ejemplo, pero como la misma librearía la usaremos en todos los ejemplos por eso la pongo en un directorio general

# Ejemplos
Cada ejemplo tendra un makefile unico para ser compilado de manera independiente

Para compilar un ejemplo ejecutamos los siguientes comandos
```
cd directorio-ejemplo
make cleanall
make
```
Para correr el ejemplo ejecutamos
```
./program
```

Todos los ejemplos tendrán este nombre genérico si queremos cambiarlo editamos el Makefile y en la sección donde pone **APP** ponemos el nombre que queramos
```
APP		:= program
```

# Referencias

La forma de hacer el Makefile la seguí de este canal, el Makefile que uso tiene algunas variaciones que he ido modificando.

Este profesor tiene mucho material para aprender a programar en c++ en un nivel intermedio y avanzado

>[GameDev C++ 2020: Programación de Videojuegos desde 0 para PC](https://www.youtube.com/watch?v=7YBzHJJYpZo&list=PLmxqg54iaXrhTqZxylLPo0nov0OoyJqiS&ab_channel=ProfesorRetroman)
