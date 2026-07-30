INSTRUCCIONES DE USO:
inicio de aplicacion en puerto 3000 con comando pnpm run dev

Metodos a utilizar en postman

# Usuarios
//Creacion de un usuario 
POST - http://localhost:3000/usuarios/agregar
JSON RECOMENDADO
    {
        "id": idDelUsuario - numero
        "nombre": "nombreDelUsuario",
        "apellido": "apellidoDelUSuario",
        "edad": edadDelUsuario - numero, 
        "correo": "correoDelUSuario@gmail.com",
        "contrasena": contrasenaDelUsuario - numero,
        "rol": "rolDelUsuario",
        "estado": "estadoDelUsuario"
    }


//Listar usuarios
GET - http://localhost:3000/usuarios
Sin JSON


//Actualizacion de un usuario
PUT - http://localhost:3000/usuarios/actualizar/idDelUsuario
JSON RECOMENDADO
    {
        "nombre": "nombreDelUsuario",
        "apellido": "apellidoDelUsuario",
        "edad": edadDelUsuario,
        "correo": "correoDelUsuario@gmail.com",
        "contrasena": contrasenaDelUsuario,
        "rol": "rolDelUsuario",
        "estado": "estadoDelUsuario"
    }
Recomendable o enviar el id en el JSON.


//Eliminar usuario
DELETE - http://localhost:3000/usuarios/eliminar/idDelUsuario
Sin JSON


//Listar un usuario por su id
GET - http://localhost:3000/usuarios/buscar/idDelUsuario
Sin JSON



# Producto
//Creacion de un producto
POST - http://localhost:3000/productos/agregar
JSON RECOMENDADO
{
"idProducto": idDelProducto - numero,
"nombre": "nombreDelProducto",
"descripcion": "descripcionDelProducto",
"precio": precioDelProducto - numero,
"stock": stockDelProducto - numero,
"categoria": "categoriaDelProducto",
"estado": "estadoDelProducto"
}

//Listar productos
GET - http://localhost:3000/productos
Sin JSON

//Actualizacion de un producto
PUT - http://localhost:3000/productos/actualizar/idDelProducto
JSON RECOMENDADO
{
"nombre": "nombreDelProducto",
"descripcion": "descripcionDelProducto",
"precio": precioDelProducto,
"stock": stockDelProducto,
"categoria": "categoriaDelProducto",
"estado": "estadoDelProducto"
}
Recomendable no enviar el idProducto en el JSON.

//Eliminar producto
DELETE - http://localhost:3000/productos/eliminar/idDelProducto
Sin JSON

//Listar un producto por su id
GET - http://localhost:3000/productos/buscar/idDelProducto
Sin JSON


# Pedido
//Creacion de un pedido
POST - http://localhost:3000/pedidos/agregar
JSON RECOMENDADO
{
"idPedido": idDelPedido - numero,
"cliente": "nombreDelCliente",
"producto": "nombreDelProducto",
"cantidad": cantidadDelProducto - numero,
"precioTotal": precioTotalDelPedido - numero,
"estadoPedido": "estadoDelPedido"
}

//Listar pedidos
GET - http://localhost:3000/pedidos
Sin JSON

//Actualizacion de un pedido
PUT - http://localhost:3000/pedidos/actualizar/idDelPedido
JSON RECOMENDADO
{
"cliente": "nombreDelCliente",
"producto": "nombreDelProducto",
"cantidad": cantidadDelProducto,
"precioTotal": precioTotalDelPedido,
"estadoPedido": "estadoDelPedido"
}
Recomendable no enviar el idPedido en el JSON.

//Eliminar pedido
DELETE - http://localhost:3000/pedidos/eliminar/idDelPedido
Sin JSON

//Listar un pedido por su id
GET - http://localhost:3000/pedidos/buscar/idDelPedido
Sin JSON


NOTA: las contraseñas se manejaron con numeros por lo trabajado en clase y las clases como Producto
y Pedido, son las clases del primer ejercicio que se trabajo en esta carpeta, al igual que los menus.