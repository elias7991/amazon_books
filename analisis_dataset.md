# Análisis de dataset de entrada

## Datos de libros - Análisis por columnas

Tenemos en total **212.404** registros en el dataset **books_data**.

### 1. Title

En este caso nos topamos con **1 (un)** registro nulo. Para el caso de la cadena vacía hemos optado por sustituirlo por la cadena **Sin titulo**.

### 2. Description

En este caso nos topamos con **68.442** registros (**32%** de los registros aproximadamente) nulos a los cuales denominamos **Sin descripcion**.

### 3. Rating Counts

Tenemos **162.652** registros nulos (**77%** de los registros aproximadamente). En este caso como ***ratingCounts*** representa al número de calificaciones recibidas de un libro en particular basta con setear estos libros en 0 (cero) para tener datos más legibles. Es decir, simplemente no han sido calificados y por lo tanto les corresponde un valor de 0 (cero).

### 4. Authors

Tenemos **31.413** registros nulos (**15%** de los registros aproximadamente) los cuales setearemos como una lista vacía ([]) para seguir el formato de esta columna que tiene la forma de: **["autor 1", "autor 2", ..., "autor n"]**.

### 5. Categories

Tenemos **41.199** registros nulos (**20%** aproximadamente) a los cuales le aplicaremos el mismo criterio de la columna **authors** debido a su formato.

### 6. Publisher

Tenemos **75.886** registros nulos (**36%** aproximadamente) y como esta columna corresponde a la editorial que publica el libro decidimos que lo setearemos como **Sin editor** para estos casos.

### 7. Published Date

Tenemos **25.305** registros nulos (**12%** aproximadamente) y teniendo en cuenta que esta columna representa a la fecha de publicación del libro decidimos setearlo como un año ficticio **0000** pensando en la facilidad posterior para la visualización de los datos. En este caso deseamos utilizar solamente el año de publicacion para la visualización y evitar añadir cierto grado de complejidad extra al tener que controlar los meses y días faltantes en el dataset.

### 8. Image

Tenemos **52.075** registros nulos (**25%** aproximadamente) que setearemos como **Desconocido** haciendo referencia a la ausencia de link para el campo.

### 9. Info Link

En esta columna nos topamos con una situación similar a la anterior con un total de **23.836** registros nulos (**12%** aproximadamente) que también setearemos como **Desconocido**.

### 10. Preview Link

Aquí también tenemos **23.836** registros nulos que setearemos como **Desconocido**.

## Datos de calificación - Análisis por columnas


