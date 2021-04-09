## Espaciado

Para el espaciado se usarán más que nada los *márgenes, padding y display* (block y flex).

### Margin y Padding

Las clases para los márgenes y padding empiezan con la primera letra de la propiedad (si es "margin" será "m", padding, "p") seguido de la dirección (top, right, bottom, left), si quieres que se aplique a todas entonces no coloques dierección y la cantidad. Ejemplo: `m-5`, `ml-auto`, `pb-10`, `px-auto`

En las clases de tailwind se usan los ejes X y Y para decir que los estilos se aplicarán tanto para "top", como "bottom" o "left" como "right". De manera que `mx-auto` es equivalente a `ml-auto mr-auto` o `my-10` es igual a `mt-10 mb-10`

Si quieres **centrar elementos** algo muy común es usar el margin para cada lado (o directamente usar los ejes anterior mencionados) con el valor "auto" (justo como vimos antes) para que sin importar el tamaño del elemento o la cantidad de elementos al lado, siempre haya el mismo margin a los lados del elemento. 

En otras palabras, **para centrar elementos se usará ya sea** `mx-auto` o `my-auto`.

El caso del padding solo se usará para agregar más *"relleno"* a un elemento. **Si tienes un input o un contenedor y ves que sus elementos tienen que ir separados de las esquinas, entonces usa un padding**. Aunque a diferencia del margin, con el padding no se usa `p-auto` , esto da totalmente igual. Todo lo demás es exactamente igual al margin.

### Display

El display se puede usar de muchas maneras, pero solo hay dos que vamos a usar por ahora: `flex` y `block`. Usaremos `flex` en un contenedor para que sus elementos se coloquen uno al lado del otro y `block` cuando queramos lo contrario, que estén uno arriba del otro.

Otra cosita acerca del display es que dependiendo de este podremos *"desbloquear"* algunas propiedades. Por ejemplo, elementos como  los inputs tienen por defecto `display: inline` por lo cual no aceptan width ni margin, pero si le colocamos la clase de tailwind `block` ya podremos usar las demás propiedades.

Sobre el display flex, se pueden hacer muchas más cosas luego de usarlo, como centrar vertical y horizontalmente, esto se logra colocando en el elemento con la clase `flex` otras que son las del *justify-content* en CSS y cada una empieza con "justify" seguido del valor, por ejemplo `justify-center` (para centrar), `justify-between` (para colocar espacio entre los elementos) y así según los valores que quieras usar.
