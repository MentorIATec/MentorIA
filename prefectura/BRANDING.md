# Sistema visual — "Sol de residencia"

Guía breve para que todo material nuevo del taller (plantillas, presentación,
futuros recursos) se vea como parte de una misma serie, en vez de piezas
sueltas. Cualquier archivo nuevo del área de prefectura puede reutilizar
estas reglas copiando el bloque de estilos (`:root { ... }`) y el footer
estándar de la sección 5.

Este es un estilo **cálido, juvenil y con actitud de sticker** — pensado para
estudiantes prefectos, no para un reporte corporativo. Colores saturados,
bordes gruesos, esquinas muy redondeadas y tipografía grande y pesada, sin
depender de fuentes externas (todo funciona offline).

## 1. Paleta

| Uso | Variable | Color |
|---|---|---|
| Texto principal / encabezados | `--ink` | `#21232B` |
| Texto secundario | `--ink-soft` | `#5B5B66` |
| Fondo de página | `--paper` | `#FFF6E9` |
| Fondo de tarjetas | `--card` | `#FFFFFF` |
| Líneas suaves (divisores) | `--line` | `#EAD9C2` |
| Acento primario (CTA, botones) | `--coral` | `#FF6B4A` |
| Acento primario hover | `--coral-dark` | `#E24F30` |
| Acento secundario (badges, highlights) | `--yellow` | `#FFC93C` |
| Acento terciario (marca, kicker, links) | `--teal` | `#2FB8A6` |
| Acento terciario hover | `--teal-dark` | `#229184` |
| Semáforo — verde | `--verde` | `#3FAE7A` |
| Semáforo — amarillo | `--amarillo` | `#FFC93C` |
| Semáforo — rojo | `--rojo` | `#E5484D` |

El fondo crema cálido evita el blanco clínico; los tres acentos (coral,
amarillo, teal) se usan cada uno con un propósito claro y no se mezclan
libremente: coral es acción (botones principales), amarillo es énfasis
(badges, hover suave, insignias de letras), teal es identidad (marca,
kickers, enlaces).

## 2. Tipografía

Todo en sans del sistema — sin fuentes externas, para que las plantillas
sigan funcionando sin internet: `-apple-system, 'Segoe UI', Roboto, Arial,
sans-serif`.

- **Encabezados** (`h1`, `h2`, `h3`): peso `800`–`900`, tamaño grande,
  `letter-spacing` ligeramente negativo para sensación "chunky". Nada de
  serif — el peso y tamaño hacen el trabajo de dar personalidad.
- **Kickers** (etiqueta antes de un título, ej. "BLOQUE 4 · 24–36 MIN"):
  mayúsculas, `--teal`, `letter-spacing: 1px`, `font-weight: 800`, 12–13px.
- **Cuerpo, formularios, botones**: peso normal/`600` en botones, tamaño
  14–16px, máxima legibilidad al llenar campos.

## 3. Componentes

- **Marca**: pastilla `DC·IA` (fondo `--teal`, texto blanco, esquinas
  redondeadas) junto al nombre corto "Diseñar comunidad con IA".
- **Tarjetas**: fondo `--card`, `border-radius: 20px`–`24px`, borde de 2–3px
  en `--ink` (efecto sticker/cómic) en vez de solo sombra — la sombra se usa
  como acento adicional, no como único recurso de profundidad.
- **Botones primarios**: forma de píldora (`border-radius: 999px`), fondo
  `--coral`, borde 2–3px `--ink`, texto blanco/oscuro con peso alto, hover
  `--coral-dark`.
- **Botones secundarios**: mismo radio, fondo transparente, borde `--line`
  o `--ink`, texto `--ink-soft`.
- **Insignias/badges** (ej. letras de C.O.P.I.L.O.T.O.): círculos o
  cuadrados muy redondeados, alternando `--teal` y `--yellow`, nunca todas
  del mismo color — refuerza la sensación de variedad/juego.
- **Barra superior**: franja de 5–6px en gradiente `--coral` → `--yellow` →
  `--teal` al inicio de cada página, firma visual consistente.

## 4. Footer estándar (obligatorio en todo material nuevo)

Copiar este bloque al final de cualquier página o documento nuevo:

```html
<footer class="site-footer">
  <p class="site-footer-brand"><span class="brand-mark">DC·IA</span> Diseñar comunidad con IA — Taller de Prefectura</p>
  <p>Tecnológico de Monterrey, Campus Monterrey</p>
  <p>© 2026 Karen Ariadna Guzmán Vega · <a href="mailto:kareng@tec.mx">kareng@tec.mx</a></p>
  <p>Contenido bajo licencia <a href="https://creativecommons.org/licenses/by-nc-sa/4.0/deed.es" target="_blank" rel="noopener">CC BY-NC-SA 4.0</a> — puede adaptarse citando a la autora, sin fines comerciales, compartiendo bajo la misma licencia.</p>
</footer>
```

**Sobre "Tecnológico de Monterrey, Campus Monterrey" en el footer:** se
mantiene como identificación en texto plano (sin logo ni escudo oficial),
lo cual es un uso estándar y de bajo riesgo cuando el material es para una
actividad propiamente institucional, como este taller. Distinto es usar el
logo o los colores de marca oficiales del Tec, que sí requeriría
autorización de la oficina de identidad/comunicación.

**Sobre la licencia CC BY-NC-SA:** este material se produjo con correo
institucional (`kareng@tec.mx`) para un programa del Tec. Antes de
distribuir las plantillas ampliamente fuera del área de prefectura (por
ejemplo, presentarlas en SWACUHO o publicarlas en un repositorio público),
vale la pena confirmar con la institución que puedes licenciar tú misma
este contenido. Si se considera propiedad del Tec, ajusta esa nota según la
política de propiedad intelectual correspondiente.

## 5. Aplicado en

- `index.html`, `mapa-contexto.html`, `canvas-intervencion-residencial.html`,
  `copiloto-prompts.html`, `semaforo-ia.html`, `presentacion-taller.html`.
