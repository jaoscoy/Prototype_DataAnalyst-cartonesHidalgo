# Analisis de la información

Una vez que la información fue exportada desde el kernel [**_'../adquisicionDatos/raw.ipynb'_**](../adquisicionDatos/raw.ipynb), usaremos este dataframe para analizar la información más relevante de las operaciones de venta y las relaciones existentes entre los clientes y las categorias de cada producto.

A continuacion describire el significado de cada columna y el objetivo en cada kernel de esta carpeta.

## Columnas

1. foliointerno: El folio que tiene cada orden de compra asignado por el cliente. Es un valor unico.

2. _id: El ObjectId de cada orden.

3. Usuario.razonSocial: El nombre de la organización para identificar al cliente.

4. Productos.idLocal: El id unico con el que cada cliente identifica el articulo comprado.

5. Productos.unidades: Las unidades de la venta. Siempre es en millares.

6. Productos.cantidad: Cantidad de millares por articulo.

7. Productos.importe: Precio total de compra por articulo.

8. Especificaciones.estructura: El tipo de la forma de la caja vendida.

9. Especificaciones.tipo: La configuración de fabricación para pegado.

10. Especificaciones.calibreECT: El calibre del carton de cada articulo.

11. Especificaciones.caraExterior: El tipo de acabado pintura del corrugado.

12. Especificaciones.largo: Las dimensiones en cm del largo del articulo.

13. Especificaciones.ancho: Las dimensiones en cm del ancho del articulo.

14. Especificaciones.alto: Las dimensiones en cm del alto del articulo.

15. Especificaciones.tipoUnion: El metodo y posición de la ceja para cerrar el articulo.

16. Especificaciones.suaje: Booleano en caso de llevar un acabado especial para doblado especifico.

17. Productos.precioUnitario: El precio pagado por unidad (millar) de cada articulo por el cliente.

18. precios.precioGeneralm2: El precio por 1 caja solamente importado desde la lista oficial.

19. fechaEmision: El dia de la compra.

20. Especificaciones.longitudLamina: Largo de la materia prima. 

21. Especificaciones.anchoLamina: Ancho de la materia prima.

22. areaM2: El area total por cada caja. Con ella se calcula el precio de lista.

23. precioListaMillares: El precio de lista por millar de cada articulo.

### Análisis especificos

1. El archivo [**_'precioMaterial.ipynb'_**](precioMaterial.ipynb) contiene los metodos necesarios para relacionar el dataframe original con la lista de precios sugeridos a cotizar **_'../recursos/listaPrecios2020.csv'_** y crear las columnas necesarias para calcular el area total y el costo real de cada producto.

2. El archivo [**_'ventasArticulo.ipynb'_**](ventasArticulo.ipynb) contiene los metodos necesarios y las graficas para representar las **unidades totales vendidas** y el **monto total de venta** por cada cliente.

3. El archivo [**_'consumoTotal.ipynb'_**](consumoTotal.ipynb) contiene los metodos y graficas necesarios para representar el consumo total de materia prima por cada mes de operación, categorizando por calibre para pronosticar un inventario estimado.

4. El archivo [**_'productosOferta'_**](productosOferta.ipynb) contiene un wordCloud para mostrar la configuración de los productos más populares entre nuestros clientes actuales.
 

