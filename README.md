# Http-server-content

Proyecto creado en node en el cual puedes usar diferentes rutas y metodos.

Las siguientes rutas estan habilitadas y se mostrará un caso de uso en cada una

## Comenzando 🚀
### /
El primer endpoint es la raiz "/", en el cual se despliega un html saludando al usuario

### /books
El segundo endpoint es "/books", en este se encuentran 3 comportamientos dependiendo de el metodo http usado
```
GET
Devuelve todos los libros que se encuentran en el archivo de texto del directorio, books.txt
POST
Las peticiones POST a este endpoint te permiten añadir informacion al archivo de texto books.txt
DELETE
Se elimina el contenido de books.txt
```
### /file-viewer
Este endpoint funciona con un query parameter que te permite recuperar el contenido de archivos dentro del directorio del proyecto
```
http://localhost:8087/file-viewer?name=src/handlers/index.js
```
Como en el ejemplo, se tiene que comenzar siempre con la palabra name, signo de igual y luego la ruta relativa del archivo, dentro del directorio del proyecto.

### /server-status
En este endpoint se recupera un archivo tipo json con las especificaciones del equipo que hostea la aplicación.
