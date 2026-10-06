# Documentación de la interfaz — Estirón

App Android de una cadena de tiendas de ropa y calzado infantil de 0 a 14 años, con prototipo de alta fidelidad en Figma siguiendo Material Design 3.
Autor: Sergio Mitchell Bocero ([@sergiomitbo](https://github.com/sergiomitbo)), 2.º DAM, MEDAC.

## 1. Justificación del diseño

### 1.1 Importancia del diseño centrado en el usuario

En Estirón casi nunca compra quien va a llevar la ropa. Compra una madre con el bebé en brazos, un padre a la salida del colegio o un abuelo que solo sabe la edad de su nieta. Los tres tienen poco tiempo, usan el móvil con una mano y dudan con las tallas. Si la app se diseña a partir del catálogo y no de estas personas, el resultado es previsible: compras que se quedan a medias y devoluciones porque la talla no era la buena. Y si alguien elige mal la talla, el fallo no es suyo: la mayoría de los errores de uso son errores de diseño (Norman, 2013).

Por eso el proyecto sigue el ciclo de diseño centrado en el usuario de la norma ISO 9241-210 (International Organization for Standardization [ISO], 2019): entender quién compra y en qué situación (sección 2), diseñar a partir de lo aprendido (sección 3), probar el diseño con personas (sección 4) y corregirlo con lo que salga de las pruebas (apartado 4.3). La regla que aplico es que cada decisión de la interfaz tiene que poder justificarse con un objetivo o con un insight de este documento. Si no se puede, sobra.

### 1.2 Objetivos y metas del proyecto

Cada objetivo tiene un indicador y una meta. Tres se comprueban en las pruebas con usuarios (sección 4) y el cuarto en la guía de estilo (apartado 3.3).

| Objetivo | Indicador | Meta | Dónde se mide |
|---|---|---|---|
| **O1. Comprar rápido**, con el móvil en una mano. | Tiempo desde Inicio hasta Confirmación. | 120 s o menos en cada participante. | Pruebas, tarea T1 |
| **O2. Acertar la talla a la primera**, sin conocerla de antemano. | Participantes que eligen la talla correcta sin ayuda. | 100 %. | Pruebas, tarea T2 |
| **O3. Equivocarse sin consecuencias.** | Participantes que recuperan con «Deshacer» un producto eliminado, y tiempo que tardan. | 100 %, en 10 s o menos. | Pruebas, tarea T3 |
| **O4. Que se lea y se toque bien a cualquier edad.** | Parejas color/on-color con contraste de 4,5:1 o más, y elementos interactivos con área táctil de 48 × 48 dp o más. | 100 % en ambos casos. | Guía de estilo (3.3) y revisión en Figma |

### 1.3 Beneficios esperados

| Para quien compra | Para la cadena |
|---|---|
| Compra completa en un par de minutos y con una sola mano. | Más pedidos terminados y menos carritos abandonados. |
| Talla elegida por edad y altura, con la guía a un toque. | Menos devoluciones por talla, que cuestan envíos, gestión y, a veces, el cliente. |
| Cambio gratis en cualquier tienda y opción de recoger el pedido en tienda. | Más visitas a las tiendas físicas, donde el cliente puede comprar algo más. |
| Favoritos para decidir más tarde o guardar ideas de regalo. | Saber qué productos interesan y dar motivos para volver a la app. |
| Letra legible, buen contraste y compra sin registrarse. | Llegar también a abuelos y compradores de regalos que hoy solo compran en tienda. |

Tras el lanzamiento, estos beneficios se seguirían con tres indicadores: tasa de conversión de la app, porcentaje de devoluciones con motivo «talla» y número de pedidos con recogida en tienda.

## 2. Investigación y análisis de usuarios

### 2.1 Datos demográficos y segmentación

La investigación es básica y parte de tres fuentes: el encargo de la cadena (quién compra y en qué contexto), el análisis de tres apps de la competencia (apartado 2.3) y las dos personas construidas a partir de ambos (apartado 2.2). Divido a quien compra en tres segmentos según su relación con el niño, porque eso cambia cuánto sabe de tallas y con qué frecuencia compra.

| Segmento | Edad aprox. | Frecuencia de compra | Contexto de uso | Lo que más necesita |
|---|---|---|---|---|
| Madres y padres | 28-45 | Alta: los niños cambian de talla varias veces al año, y a eso se suman las temporadas y la vuelta al cole. | Ratos sueltos y con interrupciones, a menudo con el niño en brazos o empujando la sillita. | Reponer rápido, tallas fiables y no perder la compra si les interrumpen. |
| Abuelas y abuelos | 60-75 | Media-baja, concentrada en cumpleaños, Navidad y Reyes. | En casa y sin prisa, pero con poca confianza al pagar con el móvil y con la letra del sistema aumentada. | Entender la talla sin conocerla, textos legibles y un pago claro. |
| Familiares y amigos que regalan | 25-55 | Puntual: nacimientos, bautizos y cumpleaños. | Compra rápida, muchas veces sin conocer bien al niño. | Ideas por edad, ticket regalo y cambio fácil. |

Los tres segmentos comparten tres rasgos que condicionan todo el diseño. Compran desde el móvil, y la app sale solo para Android. Lo usan a menudo con una sola mano: casi la mitad de la gente sujeta el móvil así (Hoober, 2013), y este público suele tener además la otra mano ocupada con el niño. Y ninguno es experto en tallas infantiles, que dependen más de la altura del niño que de su edad. Además, la cadena tiene tiendas físicas, así que la recogida y el cambio en tienda son una ventaja que una tienda solo online no puede ofrecer.

### 2.2 Personas

#### Persona 1: Laura Sánchez, la madre que repone sobre la marcha

| Campo | Detalle |
|---|---|
| **Edad y ocupación** | 34 años. Enfermera con turnos rotativos en un hospital de Getafe. |
| **Familia** | Dos hijos: Leo, de 4 años y 108 cm, y Martina, de 9 meses. |
| **Dispositivo y contexto** | Android de gama media. Compra en el autobús o mientras da el biberón, con una mano libre, y la interrumpen constantemente. |
| **Objetivos** | Reponer pijamas, bodies y zapatillas en pocos minutos; acertar la talla de Leo, que está dando el estirón; recoger el pedido en la tienda de su barrio al salir del turno. |
| **Frustraciones** | Formularios largos en el móvil, botones pequeños que toca sin querer, perder el carrito cuando tiene que dejar el móvil y que cada marca talle distinto, lo que la obliga a devolver. |
| **Frase** | «Si no lo compro en dos minutos, ya no lo compro.» |

#### Persona 2: Antonio Ruiz, el abuelo que quiere acertar con el regalo

| Campo | Detalle |
|---|---|
| **Edad y ocupación** | 68 años. Jubilado; trabajó como administrativo en una gestoría de Zaragoza. |
| **Familia** | Su nieta Lucía vive en Sevilla y cumple 6 años el mes que viene. La ve pocas veces al año. |
| **Dispositivo y contexto** | Android con el tamaño de letra aumentado. Compra desde el sofá y sin prisa, pero desconfía de pagar con el móvil. |
| **Objetivos** | Regalarle a Lucía un vestido que le quede bien sin preguntar a su hija, para que sea sorpresa; enviarlo directamente a Sevilla con ticket regalo; saber que se puede cambiar. |
| **Frustraciones** | Letra pequeña e iconos sin texto; no entender qué significa «116» o «6A»; mensajes de error que no explican qué ha hecho mal; apps que le obligan a registrarse para comprar una sola vez. |
| **Frase** | «Sé que cumple seis años, pero ¿eso qué talla es?» |

### 2.3 Análisis de la competencia

Revisé las apps Android de tres cadenas que venden ropa infantil en España con el mismo recorrido en todas: entrar en la sección infantil, buscar un pijama de 4 años y llegar al carrito.

| App | Qué hace bien | Qué hace mal | Qué me llevo a Estirón |
|---|---|---|---|
| **H&M** | Indica las tallas infantiles por altura en centímetros junto a la edad orientativa, que es más fiable que la edad sola. Filtra por talla, color y precio, y cada tarjeta tiene su corazón de favoritos. | Algunas prendas usan tallas dobles (por ejemplo, 110/116) que obligan a abrir la tabla para entenderlas, y la sección infantil es tan grande que sin filtros cuesta encontrar algo. | Edad y altura en cada opción del selector de talla, sin tallas dobles, y filtros visibles desde el principio. |
| **Zara** | Separa la sección infantil por franjas de edad y por sexo desde el primer nivel, así que en dos toques se llega a la sección correcta. Fotografía grande y limpia, y al elegir talla avisa si quedan pocas unidades. | Estética muy minimalista, con textos pequeños y finos y poco contraste en algunos elementos, lo que complica la lectura a personas mayores. | Categorías por edad en Inicio y el estado del stock dentro del propio selector de talla, pero con textos de 14 sp o más y contraste AA. |
| **Kiabi** | Precios muy visibles, lotes de básicos (bodies, calcetines) y recogida gratuita en tienda. | La pantalla de inicio acumula banners y promociones que compiten entre sí por la atención. | La recogida y el cambio en tienda como ventaja principal, porque Estirón tiene tiendas físicas, y un Inicio con una sola zona de novedades. |

### 2.4 Insights y hallazgos clave

Cada insight sale de la investigación anterior y acaba en una decisión concreta que se puede ver en el prototipo.

| # | Insight | Origen | Decisión de diseño | Pantalla |
|---|---|---|---|---|
| I1 | La edad no basta para acertar la talla: Leo tiene 4 años pero mide 108 cm, más que la talla de 4 años (104 cm). | Encargo, Persona 1, H&M | Selector de talla propio (SelectorTalla) con edad y altura en cada opción, y botón «Guía de tallas» junto a él que abre un bottom sheet con la altura que cubre cada talla. | Detalle |
| I2 | Se compra con una mano y con interrupciones. | Encargo, Persona 1, Hoober (2013) | Acciones principales en la mitad inferior de la pantalla (navigation bar y botón principal fijo abajo), áreas táctiles de 48 × 48 dp como mínimo y un carrito que se conserva al salir de la app. | Todas |
| I3 | Con una mano se toca sin querer, y un diálogo de confirmación castiga a quien sí quería borrar. | Persona 1 | Eliminar del carrito al momento y ofrecer «Deshacer» en un snackbar. | Carrito |
| I4 | Quien regala no conoce la talla y teme equivocarse. | Persona 2, Kiabi | «Cambio gratis en cualquier tienda» visible en Detalle y Confirmación; en Checkout, envío a cualquier dirección, recogida en tienda y ticket regalo. | Detalle, Checkout, Confirmación |
| I5 | Las personas mayores abandonan ante letra pequeña, iconos sin texto y errores que no explican nada. | Persona 2, Zara | Texto de contenido de 14 sp o más (16 sp en formularios), etiquetas siempre visibles en la navigation bar, contraste AA y errores que dicen cómo corregirse, por ejemplo «Escribe el código postal completo (5 cifras)». | Todas, Checkout |
| I6 | Hay poco tiempo y nadie quiere registrarse para una compra puntual. | Personas 1 y 2 | Categorías por edad en Inicio que llevan al catálogo ya filtrado, y compra como invitado en una sola pantalla de checkout. | Inicio, Catálogo, Checkout |

## 3. Diseño de la interfaz

### 3.1 Mapa de navegación

La navigation bar tiene tres destinos: Inicio, Catálogo y Favoritos. El carrito no ocupa un hueco en ella porque se visita al final de la compra y no durante; está siempre a mano en el icono de la top app bar, con un badge que indica cuántos artículos hay. Al pulsar «Añadir al carrito», la app lleva directamente al carrito, porque Laura y Antonio suelen comprar una o dos prendas y así se ahorran un paso (O1); desde allí, «Seguir comprando» devuelve al catálogo. Detalle, Carrito, Checkout y Confirmación ocultan la navigation bar para dejar sitio a un único botón principal abajo: en cada pantalla tiene que ser evidente qué hacer sin pararse a pensar (Krug, 2014).

```mermaid
flowchart TD
    subgraph NAV["Navigation bar: 3 destinos"]
        INI["Inicio<br/>categorías por edad, novedades y buscador"]
        CAT["Catálogo<br/>filter chips y ordenación"]
        FAV["Favoritos<br/>pie con la palabra del día"]
    end

    INI <-->|"navigation bar"| CAT
    CAT <-->|"navigation bar"| FAV
    FAV <-->|"navigation bar"| INI

    INI -->|"categoría o búsqueda"| CAT
    INI -->|"novedad"| DET
    CAT -->|"tarjeta de producto"| DET
    FAV -->|"producto guardado"| DET

    DET["Detalle de producto<br/>carrusel y selector de talla"] -->|"Guía de tallas"| GT[["Guía de tallas<br/>bottom sheet (overlay)"]]
    GT -->|"Entendido o tocar fuera"| DET
    DET -->|"elegir talla y Añadir al carrito"| CAR["Carrito<br/>cantidad, eliminar con Deshacer y resumen"]
    ICO(["Icono del carrito en la top app bar<br/>(desde cualquier pantalla)"]) -.-> CAR
    CAR -->|"Seguir comprando"| CAT
    CAR -->|"Tramitar pedido"| CHK["Checkout<br/>text fields con validación"]
    CHK -->|"Pagar"| CON["Confirmación<br/>número de pedido"]
    CON -->|"Volver al inicio"| INI

    classDef overlay stroke-dasharray: 6 4
    class GT overlay
```

De Inicio a Confirmación hay seis toques si no hay que corregir ningún dato: categoría, producto, talla, «Añadir al carrito», «Tramitar pedido» y «Pagar».

### 3.2 Wireframes

Siete wireframes de baja fidelidad en escala de grises, en frames de 360 × 800 dp, hechos en la página «Wireframes» de Figma (versión guardada: «Reto 2 – wireframes»). En esta fase solo decidí estructura y jerarquía: qué hay en cada pantalla, en qué orden y qué queda al alcance del pulgar.

<table>
  <tr>
    <td align="center"><img src="capturas/wireframes/01-inicio.png" width="160" alt="Wireframe de Inicio"><br>Inicio</td>
    <td align="center"><img src="capturas/wireframes/02-catalogo.png" width="160" alt="Wireframe de Catálogo"><br>Catálogo</td>
    <td align="center"><img src="capturas/wireframes/03-detalle.png" width="160" alt="Wireframe de Detalle de producto"><br>Detalle</td>
    <td align="center"><img src="capturas/wireframes/04-carrito.png" width="160" alt="Wireframe de Carrito"><br>Carrito</td>
  </tr>
  <tr>
    <td align="center"><img src="capturas/wireframes/05-checkout.png" width="160" alt="Wireframe de Checkout"><br>Checkout</td>
    <td align="center"><img src="capturas/wireframes/06-confirmacion.png" width="160" alt="Wireframe de Confirmación"><br>Confirmación</td>
    <td align="center"><img src="capturas/wireframes/07-favoritos.png" width="160" alt="Wireframe de Favoritos"><br>Favoritos</td>
    <td></td>
  </tr>
</table>

| Pantalla | Qué fija el wireframe |
|---|---|
| Inicio | Buscador arriba, tres tarjetas grandes de categoría por edad y un carrusel horizontal de novedades. |
| Catálogo | Fila de filter chips (edad y talla, color, precio) y botón de ordenar sobre una cuadrícula de dos columnas. |
| Detalle | Carrusel de fotos, precio, selector de talla en dos filas con «Guía de tallas» al lado y botón «Añadir al carrito» fijo abajo. |
| Carrito | Lista con selector de cantidad y botón de eliminar, resumen del importe y botón «Tramitar pedido» fijo abajo. |
| Checkout | Tipo de entrega, formulario corto, ticket regalo, método de pago y botón «Pagar». |
| Confirmación | Mensaje de éxito, número de pedido, recordatorio del cambio en tienda y botón «Volver al inicio». |
| Favoritos | Cuadrícula de productos guardados y pie con la palabra del día. |

Palabra del día: ______
