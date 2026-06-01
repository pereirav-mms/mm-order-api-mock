# mm-order-api-mock

Repositorio de mock API con archivos JSON estáticos para usar con GitHub Pages.

## Qué hace

Cada pedido se expone como un recurso estático usando la estructura de carpetas para simular una ruta REST.

La URL funciona así:

```text
https://pereirav-mms.github.io/mm-order-api-mock/orders/number/{order}/email/{email}/index.json
```

## Ejemplos de URLs

- `https://pereirav-mms.github.io/mm-order-api-mock/orders/number/1201/email/dummy.customer1@test.com/index.json`
- `https://pereirav-mms.github.io/mm-order-api-mock/orders/number/1208/email/dummy.customer2@test.com/index.json`

## Cómo usarlo

1. Abre la URL en el navegador.
2. O pásala a Postman / curl como si fuera un endpoint.
3. Si la ruta no existe, GitHub Pages devolverá automáticamente un `404`.

## Notas importantes

- GitHub Pages sirve solo archivos estáticos.
- El endpoint simulado es la propia ruta de carpeta + `index.json`.
- Si el cliente codifica el `@`, la URL también funcionará con `%40`.

## Estructura de carpetas

```text
orders/
  number/
    1201/
      email/
        dummy.customer1@test.com/
          index.json
    1208/
      email/
        dummy.customer2@test.com/
          index.json
```

## Estado actual

- Repositorio conectado a GitHub: `https://github.com/pereirav-mms/mm-order-api-mock`
- Rama `main` publicada en el remoto.

Si quieres, puedo añadir también una lista de todos los pedidos disponibles directamente en este README.
