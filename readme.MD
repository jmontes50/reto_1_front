 # Reto 1: Cards de Menú (Grid + Navbar)

En este proyecto tienes un reto para replicar la interfaz de la imagen de referencia: `dashboardcards.png` (cards de menú en modo claro).

Resuélvelo con **CSS puro**.

---

## Reglas generales

- **No entregues solo el CSS**: entrega la página funcionando (HTML + estilos).
- **Cambia la temática**: no te quedes con la temática, son solo ejemplos

---

## Reto 1: Cards de Menú (Grid + Navbar)

**Referencia**: `dashboardcards.png`

![Referencia Reto 1 - Cards de Menu](./dashboardcards.png)

### Objetivo
Construir una página tipo restaurante con:

- Barra superior simple
- Sección con título "Nuestro Menu", descripción y un **grid de 3 cards**.

### Estructura sugerida (HTML)
- `header`
  - `nav`
    - `div.brand` (logo circular + "Sabor & Co")
- `main`
  - `section`
    - `h1` Nuestro Menu
    - `p` descripción
    - `div.grid`
      - `article.card` x3
        - `img`
        - `div.card-body`
          - `div.row` (nombre + precio)
          - `p` descripción del plato

### Requisitos visuales mínimos
- Fondo claro con contenedor centrado.
- Cards con:
  - Imagen arriba con bordes redondeados.
  - Nombre del plato a la izquierda y precio a la derecha.
  - Separación/espaciado consistente (padding y gap).
- Grid de 3 columnas en desktop.

### Antes de escribir código

Vale la pena tomarse unos minutos para pensar antes de arrancar. No hay un orden correcto, pero estas preguntas pueden ayudarte:

1. ¿Cuántas secciones tiene la página? Obsérvala bien antes de tocar el editor.
2. ¿Qué HTML necesitas? Intenta identificar los bloques principales primero.
3. ¿Qué nombres de clases tienen sentido? Definirlos antes hace el CSS más fácil de escribir.
4. ¿Por dónde empiezas a estilizar? Una buena pista: de lo general a lo particular.

---

### Sobre el layout: Grid vs Flex

Puedes usar **Flexbox** en este reto, pero considera cuál es la herramienta ideal según el caso:

| Situación | Recomendado |
|---|---|
| Grid de cards (2D, filas y columnas) | `display: grid` |
| Navbar (elementos en línea horizontal) | `display: flex` |
| Fila nombre + precio dentro de la card | `display: flex` |
| Centrar contenido verticalmente | `display: flex` |

**Regla simple**: usa `grid` cuando pienses en filas **y** columnas a la vez; usa `flex` cuando el contenido fluya en **una sola dirección**.

No está mal combinarlos: Grid para la estructura general, Flex para los detalles internos.

### Checklist de entrega
- [ ] Navbar simple y limpia.
- [ ] Grid de 3 columnas.
- [ ] Cards consistentes (misma altura visual aproximada).
- [ ] Imágenes ajustadas sin deformarse (cover).
- [ ] Tipografía/jerarquía: título, subtítulo, contenido.

---

## Sugerencia de entrega

- Incluye un `index.html`.
- Incluye tu `styles.css`.
- Subelo a Discord con tu nombre

---

## Uso de IA

Puedes apoyarte en herramientas de IA, pero úsalas como apoyo al aprendizaje, no como reemplazo. Aquí algunas prácticas recomendadas:

- **Haz preguntas conceptuales**: "¿Para qué sirve `display: grid`?" o "¿Cuál es la diferencia entre `padding` y `margin`?"
- **Pide explicaciones de código que no entiendes**: copia un fragmento y pregunta qué hace línea por línea.
- **Usa autocompletado como sugerencia**, no como respuesta final; revisa y entiende lo que acepta.
- **Pregunta por alternativas**: "¿Hay otra forma de centrar un elemento con CSS?"
- **No le pidas que haga el reto por ti**: si le pides el HTML y CSS completos, te estás robando el aprendizaje.
- **Valida lo que te da**: si la IA te sugiere algo, pruébalo, rómpelo, entiéndelo. Eso es lo que queda.
