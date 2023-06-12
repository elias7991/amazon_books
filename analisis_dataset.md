# Análisis de dataset de entrada

## Datos de libros - Análisis por columnas

Tenemos en total **212.404** registros en el dataset **books_data**.

### 1. Title

Este campo representa al título del libro en cuestión.

En este caso nos topamos con **1 (un)** registro nulo. Para el caso de la cadena vacía hemos optado por sustituirlo por la cadena **Sin titulo**.

### 2. Description

Brinda una breve descripción del libro.

En este caso nos topamos con **68.442** registros (**32%** de los registros aproximadamente) nulos a los cuales denominamos **Sin descripcion**.

### 3. Rating Counts

Proporciona la cantidad de calificaciones registradas para este libro en particular.

Tenemos **162.652** registros nulos (**77%** de los registros aproximadamente). En este caso como ***ratingCounts*** representa al número de calificaciones recibidas de un libro en particular basta con setear estos libros en 0 (cero) para tener datos más legibles. Es decir, simplemente no han sido calificados y por lo tanto les corresponde un valor de 0 (cero).

### 4. Authors

Listado de autores del libro.

Tenemos **31.413** registros nulos (**15%** de los registros aproximadamente) los cuales setearemos como una lista vacía ([]) para seguir el formato de esta columna que tiene la forma de: **["autor 1", "autor 2", ..., "autor n"]**.

### 5. Categories

Listado de categorías a las cuales pertenece el libro.

Tenemos **41.199** registros nulos (**20%** aproximadamente) a los cuales le aplicaremos el mismo criterio de la columna **authors** debido a su formato.

### 6. Publisher

Representa a la editorial que publica el libro.

Tenemos **75.886** registros nulos (**36%** aproximadamente) y como esta columna corresponde a la editorial que publica el libro decidimos que lo setearemos como **Sin editor** para estos casos.

### 7. Published Date

Fecha de publicación del libro.

Tenemos **25.305** registros nulos (**12%** aproximadamente) y teniendo en cuenta que esta columna representa a la fecha de publicación del libro decidimos setearlo como un año ficticio **0000** pensando en la facilidad posterior para la visualización de los datos. En este caso deseamos utilizar solamente el año de publicacion para la visualización y evitar añadir cierto grado de complejidad extra al tener que controlar los meses y días faltantes en el dataset.

### 8. Image

Brinda una dirección en la cual se aloja la imagen de portada del libro.

Tenemos **52.075** registros nulos (**25%** aproximadamente) que setearemos como **Desconocido** haciendo referencia a la ausencia de link para el campo.

### 9. Info Link

Dirección que podemos visitar para obtener mayor información sobre el libro.

En esta columna nos topamos con una situación similar a la anterior con un total de **23.836** registros nulos (**12%** aproximadamente) que también setearemos como **Desconocido**.

### 10. Preview Link

Dirección para acceder al libro.

Aquí también tenemos **23.836** registros nulos que setearemos como **Desconocido**.

## Datos de calificación - Análisis por columnas

### 1. Price

Costo (en dólares) del libro.

Aquí los registros nulos los consideraremos como costo **0**.


### 2. User id

Identificador del usuario que calificó el libro.

A los registros nulos en este caso le asignamos el valor de **XXXXXXXXXXXXXXXX**.

### 3. Profile name

Representa al nombre del usuario que calificó el libro.

A los registros nulos le asignamos el valor de **Desconocido**.

### 4. Review Helpfulness

Representa a la utilidad de la reseña.

A los valores nulos le hemos asignado **0/0**.

### 5. Review Time

Representa a la fecha de la reseña en formato UNIX, es decir, segundos transcurridos desde la medianoche UTC del 1 de enero del año 1970.

A los valores nulos le hemos asignado **0**.

### 6. Review score

Calificación en escala de 0 a 5 del libro.

A los registros nulos le hemos asignado el valor **0**.

### 7. Review Text

Reseña completa del libro.

A los registros nulos le hemos asignado el valor **Desconocido**.

### 8. Review Summary

Representa al resumen de **Review Text**

A los registros nulos le hemos asignado el valor **Sin resumen**.