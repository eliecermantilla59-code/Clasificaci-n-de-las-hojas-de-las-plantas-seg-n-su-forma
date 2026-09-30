# 🌿 Clasificación de las hojas de las plantas según su forma

> *«Hola, me sorprende que alguien esté leyendo esto. Si lo lees, gracias por visitar este sitio. Espero que lo disfrutes.»*

Aplicación web educativa e interactiva para aprender la **clasificación de las hojas de las plantas según su forma**. Incluye **24 formas ilustradas en SVG**, un **comparador** de hasta tres formas, una **guía de nervaduras** y un **quiz** de diez preguntas.

Todo está en **un único archivo `index.html`**: sin dependencias, sin instalación, sin conexión a internet. Las 24 hojas están dibujadas con vectores SVG generados por código, por lo que se ven nítidas en cualquier tamaño de pantalla y se recolorean con el tema oscuro.

---

## 📸 Contenido de la aplicación

| Sección | Qué permite hacer |
| --- | --- |
| **Explorar** | Galería de las 24 formas con buscador instantáneo (nombre, alias, ejemplos, características, nervadura) y filtros por categoría. Cada tarjeta abre una ficha completa. |
| **Comparar** | Selecciona hasta tres formas y contrástalas rasgo a rasgo. Los valores que difieren se resaltan en ámbar para que las similitudes destaquen. |
| **Nervaduras** | Los cuatro patrones básicos de nervadura con su dibujo esquemático y ejemplos de plantas reales. |
| **Quiz** | Diez hojas al azar, cuatro opciones cada una, corrección inmediata y explicación con la ficha de la forma. |

### Funcionalidades adicionales

- **Tema claro y oscuro** con detección automática de la preferencia del sistema y recuerdo en `localStorage`.
- **Navegación por teclado**: `/` o `Ctrl/⌘ + K` enfoca el buscador, `←` y `→` recorren la ficha abierta, `Esc` cierra, y las pestañas responden a las flechas.
- **Rutas profundas** por hash: `#explorar`, `#comparar`, `#nervaduras`, `#quiz`.
- **Responsive** de 320 px a pantallas grandes, con Tipografía fluida y diseño *mobile first*.
- **Accesible**: HTML semántico, `aria-label` y `role` en los controles, `aria-live` en los mensajes de estado, foco visible y respeto a `prefers-reduced-motion`.
- **Imprimible**: al imprimir se ocultan menús y se muestran todas las fichas en una grilla limpia.
- Sin peticiones de red, sin cookies, sin rastreadores.

---

## 🗂️ Estructura del proyecto

```
.
├── index.html   # Aplicación completa: HTML + CSS + JavaScript
├── README.md    # Esta documentación
└── LICENSE      # Licencia MIT
```

Todo vive en `index.html` por decisión deliberada: el proyecto se abre con doble clic, sin proceso de compilación ni servidor local.

---

## 🧬 Catálogo de formas

### Formas simples (14)

| Forma | Sinónimos | Ejemplos |
| --- | --- | --- |
| Ovalada | ovada, elíptica | Cerezo, naranjo, jazmín, membrillo |
| Lanceolada | en forma de lanza | Laurel, olivo, salvia, eucalipto |
| Acuminada | con punta larga, apuntada | Higo, áloe, ficus, bambú |
| Cordada | en forma de corazón, acordada | Tilo, violeta, girasol, balsa del India |
| Sagitada | en forma de flecha, flechada | Elodea, sagitaria, caladio, papa |
| Reniforme | en forma de riñón, arriñonada | Malva, alcatraces, violeta, ñame |
| Orbicular | redonda, circular | Eucalipto joven, nenúfar, malva, bayas |
| Peltada | umbilicada, en escudo | Nabo, malva, petunia, capuchina |
| Espatulada | en forma de cuchara, obovada | Diente de león, violeta, ajo, plátano |
| Oblonga | oblongada | Azafrán, café, eucalipto adulto, áloe |
| Lineal o ensiforme | acicular, estrecha | Césped, maíz, romero, aguja de pino |
| Truncada | cortada | Lirio, tulipán, áloe, arbusto del té |
| Emarginada | escotada, hendida en el ápice | Marrubio, chirla, madreselva, melón |
| Caudada | con cola, aristada | Chirimoya, achiote, pachira, ruellia |

### Bordes lobulados (3)

| Forma | Descripción corta | Ejemplos |
| --- | --- | --- |
| Pinnatifida | Lóbulos a ambos lados del nervio medio, corte menor de la mitad | Diente de león, roble, acedera, girasol |
| Pinnatisecta | Lóbulos completamente separados, cada uno con nervadura propia | Cardo, eneldo de mar, bledo, papa |
| Palmatilobada | Lóbulos en abanico desde un solo punto basal | Arce, higuera, vid, ginseng |

### Hojas compuestas (5)

| Forma | Descripción corta | Ejemplos |
| --- | --- | --- |
| Ternada | Tres folíolos: uno terminal y dos laterales | Trébol, judía, maní, arándano |
| Digitada | Folíolos iguales naciendo de un único punto | Vid, cáñamo, loto, castaño de indias |
| Paripinnada | Número par de folíolos, sin folíolo terminal | Rosa, robinia, fresa, vicia |
| Imparipinnada | Número impar de folíolos, con folíolo terminal | Nogal, fresno, arce, aciano |
| Bipinnada | Doble nivel de ramificación de los ejes | Mimosa, acacia, cebil, albizia |

### Formas especiales (2)

| Forma | Descripción corta | Ejemplos |
| --- | --- | --- |
| Perfoliada | El limbo envuelve el tallo y parece atravesado por él | Menta, eucalipto joven, contramue, cerezo de Peters |
| Rizada u ondulada | Borde plegado en ondas o bucles | Col rizada, espinaca, salvia, lavanda |

### Tipos de nervadura

| Nervadura | Descripción corta | Ejemplos |
| --- | --- | --- |
| Pinnada reticulada | Nervio medio del que salen venas laterales que se ramifican | Roble, cerezo, olivo, girasol |
| Palmatada o digitada | Varias venas principales irradian desde la base | Arce, vid, higuerilla, castaño de indias |
| Paralela | Venas rectas y casi paralelas entre sí | Maíz, trigo, palmeras, iris |
| Uninervia | Una única vena sin ramificar | Ginkgo, pino, abeto, ciprés |

> **Regla práctica:** nervadura reticulada y ramificada → dicotiledónea. Nervadura paralela → monocotiledónea. Una sola vena sin ramificar → muchas gimnospermas.

---

## 🔬 Cómo se clasifica una hoja

La forma de una hoja se describe en **tres ejes**, y un buen identificador los combina:

1. **Contorno general del limbo** — ovalada, lanceolada, cordada, orbicular, reniforme…
2. **Tipo de borde** — entero, dentado, serrado, lobulado, ondulado o rizado.
3. **Grado de división del limbo** — simple, lobulado o compuesto (y en este último, pinnado o digitado).

Las **nervaduras** actúan como rasgo de confirmación: son más constantes que la forma, que varía con la luz, la edad de la hoja y las condiciones del ambiente.

---

## 🚀 Cómo usarlo

### Abrir en el navegador

Basta con abrir `index.html` en cualquier navegador moderno (Chrome, Edge, Firefox o Safari). No requiere servidor, compilación ni instalación de nada.

### Servidor local opcional

Si prefieres probarlo con `http://` (por ejemplo, para ver la navegación por hash en todos los casos):

```bash
# Python
python -m http.server 8000

# Node.js
npx serve .
```

Después visita <http://localhost:8000>.

### Publicar

Al ser un sitio estático, sirve en **GitHub Pages**, **Netlify**, **Vercel**, **Cloudflare Pages** o cualquier servidor web. En GitHub Pages: *Settings → Pages → Source: `main` / `/ (root)`*.

---

## 🛠️ Tecnologías

- **HTML5** semántico
- **CSS3** moderno: custom properties, `color-mix()`, `clamp()`, `backdrop-filter`, container-free responsive design
- **JavaScript (ES2020)** sin frameworks ni librerías: array de datos, renderizado por DOM y funciones pequeñas y separadas por responsabilidad
- **SVG** inline generado por código para las 28 ilustraciones (24 hojas + 4 esquemas de nervadura)
- Cero dependencias, cero build, cero peticiones externas

Navegadores objetivo: cualquier navegador con soporte de ES2020 y CSS custom properties (Chrome/Edge 90+, Firefox 90+, Safari 15+).

---

## ⌨️ Atajos de teclado

| Tecla | Acción |
| --- | --- |
| `/` o `Ctrl/⌘ + K` | Enfocar el buscador |
| `←` / `→` | Hoja anterior / siguiente dentro de una ficha abierta |
| `Esc` | Cerrar la ficha |
| `←` / `→` sobre las pestañas | Cambiar de sección |

---

## 🤝 Cómo contribuir

¡Las contribuciones son bienvenidas! Algunas ideas:

- **Añadir formas**: agrega un objeto al array `HOJAS` en `index.html` con `id`, `nombre`, `alias`, `grupo`, `borde`, `venacion`, `desc`, `rasgos`, `ejemplos` y `svg`. El filtro, el buscador, el comparador y el quiz se actualizan solos.
- **Mejorar los dibujos**: los SVG se describen en un `viewBox` de `200 × 220` con el nervio medio en `x = 100` y la base del pecíolo alrededor de `y = 200`. Mantener esa convención hace que todos los dibujos encajen en el mismo estilo.
- **Ampliar el quiz**: `nuevoQuiz()` elige 10 formas al azar entre las 24; basta con cambiar el número o los distractores.
- **Ampliar categorías**: registra la clave en `GRUPOS` y asigna `grupo` a las hojas correspondientes.

Al enviar un *pull request*, mantén el estilo del código existente (2 espacios, comillas dobles, `const`/`let` sin `var`) y comprueba que la página sigue funcionando al abrirla directamente en el navegador.

---

## 📄 Licencia

Código y contenido bajo la licencia **MIT**. Eres libre de usar, modificar y distribuir este proyecto.

---

## 👤 Autor

**Eliecer Mantilla** — [github.com/eliecermantilla59-code](https://github.com/eliecermantilla59-code)

---

<div align="center">

🌱 *«Aquí encontrarás la clasificación de las hojas de las plantas según su forma.»*

</div>
