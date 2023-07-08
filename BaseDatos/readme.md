## Data Base

_Pagina Principal MongoDB Compas_

<table align="center">
  <tr>
    <td align="center" style="padding=0;width=50%;">
      <img align="center" style="padding=0;" src="../images/maing.gif" />
    </td>
  </tr>
</table>

## Comands

_Insertar Datos_

```
db.usuarios.insertMany([
    {
        "nombre":"Camila",
        "email":"Camila@mail.com",
        "edad":26
        
    },
    {
        "nombre":"fabiola",
        "email":"fabiola@fabi.com",
        "edad":30,
        "genero": "F"
    }
])
```

_ver las colecciones_

```
show collections
```

_ver las bases de datos

```
show db
show databases
```

_Insert Documents Example_

```
db.collection.insertOne({'nombre': 'brian', 'apellido':'marquez'})
db.collection.insertMany([{'nombre': 'brian1', 'apellido':'marquez1'}, {'nombre': 'brian2', 'apellido':'marquez2'}])
```

_Monstar Informacion_

```
db.collection.find()
```


_ Ejemplo base de Datos_

```
use peliculas;
db.peliculas.save({titulo:'Batman el caballero oscuro'});
db.peliculas.find();
show dbs;
```