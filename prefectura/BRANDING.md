# Sistema visual — "Diseñar comunidad con IA"

Guía breve para que todo material nuevo del taller (plantillas, presentación,
futuros recursos) se vea como parte de una misma serie, en vez de piezas
sueltas. Cualquier archivo nuevo del área de prefectura puede reutilizar
estas reglas copiando el bloque de estilos (`:root { ... }`) y el footer
estándar de la sección 5.

## 1. Paleta

| Uso | Variable | Color |
|---|---|---|
| Texto principal / encabezados | `--ink` | `#1E2A32` |
| Texto secundario | `--ink-soft` | `#57646B` |
| Fondo de página | `--paper` | `#F6F3EC` |
| Fondo de tarjetas | `--card` | `#FFFFFF` |
| Líneas y bordes | `--line` | `#E4DED2` |
| Acento primario (botones, links, kicker) | `--teal` | `#2F6F6B` |
| Acento primario hover | `--teal-dark` | `#24534F` |
| Fondo tinte acento | `--teal-soft` | `#E3EEEC` |
| Acento secundario (destacados, "buena práctica") | `--gold` | `#C79A3D` |
| Fondo tinte dorado | `--gold-soft` | `#F5EAD2` |
| Semáforo — verde | `--verde` | `#4C8C63` |
| Semáforo — amarillo | `--amarillo` | `#D9A441` |
| Semáforo — rojo | `--rojo` | `#C1503A` |

El fondo cálido (`--paper`) y el acento verde-azulado (`--teal`) evitan el
look genérico de plantilla de formulario; el dorado se reserva para
momentos que conectan con logros y reconocimiento (Premios LiFE, Borrego de
Oro, buenas prácticas documentadas), nunca como color de uso general.

## 2. Tipografía

- **Encabezados** (`h1`, `h2`, `h3`, kickers): serif — `Georgia, 'Iowan Old
  Style', 'Palatino Linotype', 'Book Antiqua', serif`. Da un tono editorial
  de "taller" en vez de "dashboard".
- **Cuerpo, formularios, botones**: sans del sistema — `-apple-system,
  'Segoe UI', Roboto, Arial, sans-serif`. Máxima legibilidad al llenar
  campos.
- Los "kickers" (etiquetas pequeñas antes de un título, ej. "BLOQUE 4 · 24–36
  MIN") van en mayúsculas, `--teal`, `letter-spacing: 1px`, `font-weight:
  bold`, tamaño 13px.

## 3. Componentes

- **Marca**: una pastilla `DC·IA` (fondo `--teal`, texto blanco, esquinas
  redondeadas) junto al nombre corto "Diseñar comunidad con IA" — funciona
  como logotipo sin depender de imágenes externas.
- **Tarjetas**: fondo `--card`, `border-radius: 14px`, sombra suave
  (`0 10px 24px rgba(30,42,50,.08)`), sin bordes duros.
- **Botones primarios**: forma de píldora (`border-radius: 999px`), fondo
  `--teal`, texto blanco, hover `--teal-dark`.
- **Botones secundarios** (limpiar, cancelar): mismo radio, fondo
  transparente, borde `--line`, texto `--ink-soft`.
- **Barra superior**: línea de 5px en gradiente `--teal` → `--gold` al
  inicio de cada página, como firma visual consistente.

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

**Nota sobre la licencia:** este material se produjo con correo
institucional (`kareng@tec.mx`) para un programa del Tecnológico de
Monterrey. Antes de distribuir las plantillas ampliamente fuera del área de
prefectura (por ejemplo, presentarlas en SWACUHO o publicarlas en un
repositorio público), vale la pena confirmar con tu institución que puedes
licenciar tú misma este contenido bajo CC BY-NC-SA. Si el material se
considera propiedad del Tec, la nota de licencia debería ajustarse a lo que
indique la política institucional correspondiente.

## 5. Aplicado en

- `index.html`, `mapa-contexto.html`, `canvas-intervencion-residencial.html`,
  `copiloto-prompts.html`, `semaforo-ia.html`, `presentacion-taller.html`.
