# Descripcion y contexto
El microservicio cliente se encarga de la administración de los mismos. Dicho microservicio fue desarrollado usando el framework SpringBoot y para la parte del frontend se hizo uso del framework Angular

## 🙍‍♀️ Clientes
### GET
List Clients

**Request**
```
localhost:8090/api/facturacion/cliente/
```

**Response**
```
[
    {
        "numero_documento": 60370881,
        "nombre_comercial": "Super suelas la unión",
        "nombre": "Maury Anchiney Garcia",
        "pais": "Colombia",
        "departamento": "Norte de santander",
        "ciudad": "Cúcuta",
        "direccion": "calle 10 #9-90 - el llano",
        "correo": "garciamaury928@gmail.com",
        "telefono": "3212030378",
        "contribuyente": "persona natural",
        "regimen_contable": "simplificado",
        "tipo_documento": 1
    },
    {
        "numero_documento": 789452136,
        "nombre_comercial": "Tienda de la esquina",
        "nombre": "pepito perez",
        "pais": "Colombia",
        "departamento": "Norte de santander",
        "ciudad": "Cúcuta",
        "direccion": "a la vuelta ",
        "correo": "tienda@gmail.com",
        "telefono": "3215687450",
        "contribuyente": "persona natural",
        "regimen_contable": "común",
        "tipo_documento": 1
    }
]
```

List Clients by ID

**Request**
```
localhost:8090/api/facturacion/cliente/listar-id/789452136
```
**Response**
```
{
    "numero_documento": 789452136,
    "nombre_comercial": "Tienda de la esquina",
    "nombre": "pepito perez",
    "pais": "Colombia",
    "departamento": "Norte de santander",
    "ciudad": "Cúcuta",
    "direccion": "a la vuelta ",
    "correo": "tienda@gmail.com",
    "telefono": "3215687450",
    "contribuyente": "persona natural",
    "regimen_contable": "común",
    "tipo_documento": 1
}
```

### POST 

**Request**
```
localhost:8090/api/facturacion/cliente/

{
    "numero_documento": 565650,
    "nombre_comercial": "Cinemark",
    "nombre": "Diego calderon",
    "pais": "Colombia",
    "departamento": "Norte de santander",
    "ciudad": "Cucuta",
    "direccion": "ventura plaza",
    "correo": "diegocalderon@gmail.com",
    "telefono": "3651024789",
    "contribuyente": "persona natural",
    "regimen_contable": "simplificado",
    "tipo_documento": 1
}
```

### PUT

**Request**

```
localhost:8090/api/facturacion/cliente/
{
    "numero_documento": 565650,
    "nombre_comercial": "Cinemark",
    "nombre": "Diego calderon",
    "pais": "Colombia",
    "departamento": "Antioquia",
    "ciudad": "Medellin",
    "direccion": "ventura plaza",
    "correo": "diegocalderon123@gmail.com",
    "telefono": "3153651029",
    "contribuyente": "persona natural",
    "regimen_contable": "simplificado",
    "tipo_documento": 1
}
```

### DELETE

**Request**

```
localhost:8090/api/facturacion/cliente/eliminar/789452136
```
