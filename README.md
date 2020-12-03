# Tienda online simple

El objetivo de Simple Online Store es brindar a sus usuarios la capacidad de
seleccionar un producto para comprar, ver la información de compra y agregarlo a
un carrito de compras.

### Consideraciones

- El desarrollo de debe realizar usando React JS
- Los productos de la tienda deben ser obtenidos mediante REST o GraphQL.
- La tematica de la tienda es libre por lo que los datos pueden ser obtenidos de alguna API libre de su preferencia o de alguna siguiente lista: 
  - [APIS REST](https://github.com/public-apis/public-apis)
  - [APIS GRAPHQL](https://github.com/APIs-guru/graphql-apis)
- El wireframe es netamente referencial, la parte visual debe realizarse con una librería de diseño existente. Ejemplo: Chakra UI, Ant Design, Material UI, etc.

## Historias del usuario

- El usuario puede ver el listado de productos en la página inicial
Los productos cuentan con una miniatura del producto, el nombre, el precio, una breve descripción,
un botón `Agregar` y otro botón de `Vista previa`. (Si el API elegida no cuenta con precio, puede generar un precio en base al charCode de la primera letra del producto. Ejemplo: "Avion".charCodeAt(0) = 65 )
- El usuario solo puede agregar como máximo 1 `item` de cada producto y se debería cambiar el botón de `Agregar` por `Eliminar` cuando el producto ya ha sido agregado.
- El usuario puede ver los detalles del producto cuando haga clic en el botón `Vista previa`. Se debe mostrar la misma información de la tarjeta del producto, pero también detalles adicionales sobre el producto; también se deberia poder agregar el producto al carrito desde este detalle.(La información del detalle debe ser consumida del API nuevamente peero esta vez basándose en la ID del producto)
- El usuario puede ver un botón del `Carrito de compras` con la cantidad de productos agregados y el monto total de su compra. (El número y monto debe actualizarse cada vez que se agrega o elimina un porducto)
- El usuario puede hacer clic en el botón `Carrito de compras` para mostrar la compra. Se debería mostrar un menú con la lista de productos y debe permitir eliminar un producto en específico o vaciar todo el carrito.

## Características adicionales

- Agregar test unitarios(Solo agregar 1 test a culaquiera de los componentes desarrollados)
- Agregar mensajes de confirmación al momento de agregar o eliminar un producto(opcional)
- Agregar loaders de carga cuando se obtenga información del API(opcional)
