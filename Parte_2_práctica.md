# Práctica 2 - Parte 2

## Ejercicio 5 y 7
Creamos un nuevo documento html y en el escribimos hola mundo. **Es importante nombrarlo *Index.html* para que se abrá en el navegador**

## Ejercicio 6
Utilizaremos el **mismo comando** que el *paso 4* pero cambiando el nombre del contenedor

~~~
docker run -dit --name asir_web1 -p 8000:80 -v "$PWD"/htdocs:/usr/local/apache2/htdocs/ httpd:2.4
~~~

**Importante parar el otro contenedor, ya que tiene el mismo puerto**



