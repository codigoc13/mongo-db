## Instalar Mongo DB

- [Descargar Mongo DB](https://www.mongodb.com/try/download/community)
- Ejcutar el archivo descargado
- Aceptar términos de licencia  
![image](https://user-images.githubusercontent.com/64823934/192156043-b75a28f0-3a84-41d3-bcde-7c2d1766568c.png)
- Elegir _Completa_  
![image](https://user-images.githubusercontent.com/64823934/192156064-9521ce50-2b92-442f-932c-81895999121a.png)
- Elegir _Instalar Mongo DB como un servicio_  
![image](https://user-images.githubusercontent.com/64823934/192156099-20d99ac2-ef54-453b-92b9-1c4b892681f6.png)
- Dejar _'clickeado' Instalar MongoDB Compass_  
![image](https://user-images.githubusercontent.com/64823934/192156132-45fea8af-29f4-4823-b33e-5dc4d2bb2307.png)
- Finalizar instalación (clics en _next_ y conceder permiso en caso de que lo solicite)
- Reiniciar el equipo (solo cuando se halla intalado Mongo DB por completo)

-----

Una vez instalado Mongo DB, con el objetivo de iniciarlo facilmente desde cualquier consola, procedemos a agregar el PATH donde quedó instalado Mongo DB a las variables de entorno.

- Localizar el PATH donde quedó instalado Mongo, el cual normalmente por defecto queda instalado en 
`C:\Program Files\MongoDB\Server\6.0\bin` y copiarlo en el portapapeles `Ctrl + C` (**Importante:** validar que esta ruta es la misma en la que quedó Mongo instalado en su equipo)
- Ejecute los siguientes pasos: 
  - Inicio
  - Escribir `Editar las variables de entorno del sistema` 
  - Variables de entorno
  - En el recuadro que dice _Variables del sistema_, dar **doble click** en _Path_
  - Nuevo
  - Pegar el PATH donde quedó instalado Mongo DB `Ctrl + V` (_recuerde que lo tiene en el portapapeles_)
  - Aceptar
  - Aceptar
  - Aceptar
  
----

Para poder ejecutar Mongo DB, debemos crear una carpeta llamada _data_ y luego crear en esta una carpeta llamada _db_ a la cual Mongo accede para crear nuestras bases de datos.

- Crear en _Disco C:_ `/data/db`

----

Probando la ejecución de Mongo DB

- Abrir cualquier terminal o consola
- Ejecutar `mongod.exe`

Debe Mongo quedarse en ejecución en segundo plano:  

![image](https://user-images.githubusercontent.com/64823934/192157397-5adcb092-6d34-4c03-8166-0ad996191e70.png)

-------

## Instalar Mongo DB Shell (mongosh)

Lo anterior ha sido para levantar Mongo DB en local. Para poder interactuar con este, debemos intalar una Shell de Mongo DB (mongosh):

- [Descargar Shell Mongo DB (mongosh)](https://www.mongodb.com/try/download/shell) (en _Platform_ cambia `Windows 64-bit (8.1 +)` por `Windows 64-bit (8.1 +) (MSI)`)
- Ejecutar el archivo descargado y elegir next hasta finalizar su instalación


Probando el cliente para Mongo DB

Manteniendo una consola en ejecución de Mongo DB con `mongod.exe`:
- Abrir una segunda terminal o consola
- Ejecutar `mongosh`

Debe quedar en espera de un comando:  

![image](https://user-images.githubusercontent.com/64823934/192158530-dcd67b4c-627a-4217-aa99-5471e732c005.png)

**Todo listo para empezar a usar Mongo DB**
