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

Palabra del día: ______
