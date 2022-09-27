## Palabras reservadas

- `use` Permite elegir la base de datos con la que se va a trabajar.
- `db` Informa la base de datos que se está usando o se tiene elegida.
- `show dbs` Muestra las bases de datos que se han creado (Si se crea una base de datos pero no se le ingresa aún nada, no se mostrará con este comando).
- `insertOne` Inserta un registro en una colección.
- `insertMany` Inserta un o varios registro en una colección.
- `find` Encuentra los documentos de la colección. El parámetro de filtrado es opcional.
- `{"nombre_de_campo":0}` Quita ese 'nombre_de_campo' del documento obtenido.
- `replaceOne` Actualiza un documento
- `{upsert: false}`: No inserta un documento nuevo así no lo encuentre. Si está en true, hace lo contrario.
- `update`: Sirve para modificar varios documentos.
- `remove`: Sirve para eliminar uno o varios documentos.

## Comandos


-  `db.movie.insertOne({"Doc1":"Start Wars"})`: Inserta un documento en una colección (movie) de la base de datos en uso. Si la colección no existe, la crea.
-  `db.movie.insertMany([{"Pelicula":"El libro de la selva", "anio":1987}, {"Pelicula":"La ballena azul"}])`: Inserta dos documentos en la colección (movie) en la base de datos que esté en uso.
-  `db.movie.find()`: Trae todos los documentos de la colección movie
-  `db.movie.find({"anio":1987})`: Trae todos los documentos de la colección movie que tengan como 'anio' 1987
-  `db.movie.replaceOne({"Doc1":"Start Wars"},{"Pelicula": "Stars Wars"})`: Actualiza el primer documento que cumpla el filtro.
-  `db.movie.update({"Pelicula":"Stars Wars"}, {$set:{"Pelicula":"Stars Wars", "anio":1975}})`: Actualiza todos los documentos que cumplan el filtro.
-  `db.movie.remove({"Pelicula":"Stars Wars"})`: Elimina las películas que tengan como parámetro "Pelicula":"Stars Wars".


### Glosario
- **Documento:** Es equivalente a un registro en una base de datos relacional.
- **Colección:** Es equivalente a una tabla en una base de datos relacional.
- **Operaciones CRUD:** 
  - **C**reate - Crear
  - **R**eade - Leer    
  - **U**pdate - Actualizar   
  - **D**elete - Eliminar   
