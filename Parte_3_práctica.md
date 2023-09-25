# Practica 2 - Parte 3
## Ejercicio 8
Ahora crearemos el contenedor *asir_web2* y **cambiaremos el puerto** al *9080*

~~~
docker run -dit --name asir_web2 -p 9080:80 -v "$PWD"/htdocs:/usr/local/apache2/htdocs/ httpd:2.4
~~~

## Ejercicio 9
Comprobamos que funciona correctamente introduciendo los **siguientes comandos**:

~~~
http:/localhost:9080
~~~

~~~
http:/localhost:8000
~~~

Nos debería salir el mensaje *Hola mundo* en ambos casos