# Taller de prefectura: Diseñar comunidad con IA

Auditoría de la propuesta original (generada con ChatGPT), agenda integrada y
plantillas HTML reutilizables para el área de prefectura, Residencias Campus
Monterrey.

## 1. Auditoría de la propuesta

### Qué se mantiene tal cual
- El posicionamiento de la facilitadora ("copiloto de acompañamiento que usa
  IA", no especialista técnica en IA) es correcto y evita la pregunta
  incómoda de por qué ella y no un profesor del área.
- El **semáforo verde/amarillo/rojo** de uso responsable es el mejor
  artefacto de la propuesta original: concreto, memorizable y aplicable a las
  cuatro funciones reales del puesto (eventos, conversaciones 1:1,
  mantenimiento, guardias).
- El marco de Design Thinking (Escuchar → Enfocar → Idear → Probar →
  Aprender) como brújula y la IA como copiloto dentro de cada etapa.

### Verificación de datos citados
Se verificaron dos afirmaciones institucionales de la propuesta original:

- **SWACUHO Student Staff Leadership Conference**: existe y corresponde a lo
  descrito — antes llamada "RA Conference", conferencia regional que cubre
  Texas, Oklahoma, Arkansas, partes de Luisiana/Missouri y México, enfocada en
  liderazgo y desarrollo de personal estudiantil de residencias.
- **Borrego de Oro / Premios LiFE**: confirmado que existe la categoría
  **"Liderazgo en Residencias"**, con al menos un caso documentado de una
  persona ganadora que fue prefecta y participó en la conferencia SWACUHO como
  parte de su trayectoria.

### Corrección necesaria
- La URL de Premios LiFE citada por la propuesta original (`premioslifegdl`)
  corresponde al sitio de **LiFE Guadalajara**, no al de Monterrey. El sitio
  correcto para Campus Monterrey es `life-cem`. Es un detalle menor pero vale
  la pena no citarlo en vivo si alguien lo busca durante el taller.

### Ajustes de fondo integrados en la agenda de abajo
1. **Colchón de tiempo.** La propuesta original suma exactamente 90:00 sin
   margen para arranque tardío, dudas o fallas técnicas. Se recortaron ~8-10
   min de las secciones más ambiciosas (Laboratorio de IA y Cuatro
   estaciones) y se redistribuyeron como colchón.
2. **Dependencia de wifi/dispositivos en vivo.** La propuesta original asume
   que cada equipo tendrá laptop + wifi + cuenta de IA funcionando en los
   minutos 40-57. Ese es exactamente el riesgo operativo que motivó construir
   las plantillas HTML de este repositorio: los ejercicios de mapa de
   contexto y canvas de intervención se llenan **sin conexión**, y el uso de
   una IA real se vuelve un paso opcional/plus dentro del mismo bloque, no un
   bloqueante.
3. **"Cuatro estaciones" como referencia, no como práctica en vivo.** Rotar 4
   estaciones en 11 minutos con contenido real es inviable. Se reconvierte en
   material de consulta (la ficha `semaforo-ia.html` y la biblioteca de
   prompts en `copiloto-prompts.html`) que se entrega para después del
   taller, liberando tiempo para reforzar la sección de crítica cruzada, que
   es donde se practica pensamiento crítico real.

## 2. Agenda integrada (90 minutos, con colchón)

| Bloque | Min | Contenido |
|---|---|---|
| 1. La comunidad no es un calendario de eventos | 0–8 | Pregunta detonadora + diferencia evento vs. comunidad |
| 2. Design Thinking como brújula, IA como copiloto | 8–17 | Escuchar → Enfocar → Idear → Probar → Aprender, con el aporte posible de IA en cada etapa |
| 3. Reto de diseño residencial | 17–24 | Equipos eligen uno de 5 retos (pertenencia, integración de perfiles, confianza 1:1, mantenimiento, guardias) |
| 4. Empatía antes que prompting | 24–36 | Llenan **`mapa-contexto.html`** en su laptop, sin conexión |
| 5. Laboratorio de prompts | 36–52 | Arman su prompt con **`copiloto-prompts.html`**; si hay wifi, lo prueban en una IA real; si no, generan el prompt y lo evalúan igual en equipo |
| 6. Crítica cruzada | 52–65 | Un equipo revisa la propuesta de otro con la pregunta: ¿qué perfil queda excluido, qué supuesto no está comprobado, qué riesgo de privacidad existe? |
| 7. De evento a buena práctica | 65–80 | Llenan **`canvas-intervencion-residencial.html`** con la idea trabajada |
| 8. Cierre y compromiso | 80–88 | Tres compromisos: qué delego a IA, qué nunca delego, qué señal de comunidad empiezo a documentar |
| Colchón | 88–90 | Preguntas, ajuste de tiempos |

Material de consulta para después del taller (no se cubre en vivo, se
entrega en PDF/enlace): `semaforo-ia.html` y la biblioteca de 5 prompts
dentro de `copiloto-prompts.html`.

## 3. Recursos entregados

Todas las plantillas son archivos HTML autocontenidos (sin dependencias
externas, funcionan sin internet), con:
- Guardado automático en el navegador (`localStorage`) mientras se llenan.
- Botón **"Descargar como PDF"** que usa la función nativa de impresión del
  navegador — sin necesidad de subir nada a un servidor ni instalar software.
- Botón para limpiar el formulario y reutilizarlo en la siguiente actividad.

| Archivo | Uso |
|---|---|
| `index.html` | Hub de navegación entre todas las plantillas |
| `mapa-contexto.html` | Mapa de contexto mínimo (empatía, Design Thinking) |
| `canvas-intervencion-residencial.html` | Canvas de 10 preguntas para documentar una intervención |
| `copiloto-prompts.html` | Constructor de prompts C.O.P.I.L.O.T.O. + biblioteca de 5 prompts reutilizables |
| `semaforo-ia.html` | Ficha de referencia del semáforo verde/amarillo/rojo |

Estas plantillas están pensadas para reutilizarse en cualquier actividad
futura del área de prefectura, no solo en este taller: cada vez que se
organice un evento, una conversación 1:1 difícil, un seguimiento de
mantenimiento o una postulación a congreso/Premios LiFE, el mismo archivo
sirve como punto de partida.
