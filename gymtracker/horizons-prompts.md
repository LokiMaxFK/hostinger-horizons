# GymTracker — Prompts para Hostinger Horizons

> **Cómo usar estos prompts:**
> - Pégalos en orden, uno a la vez
> - Adjunta las imágenes indicadas en cada prompt antes de enviar
> - Espera que Horizons termine de construir antes de pasar al siguiente
> - Si algo no queda bien, corrígelo antes de continuar al siguiente prompt

> **Sobre el estilo visual:**
> No necesitas agregar nada extra. Los prompts 2 al 6 ya incluyen la frase "Mantén el estilo visual ya establecido" al inicio. El Prompt 1 es el que define el estilo — los demás lo heredan automáticamente.

---

## PROMPT 1 — Fundación visual + Dashboard

📎 **Imagen a adjuntar:** `dashboard.png`

```
Construye una app web llamada GymTracker para seguimiento de entrenamientos personales. Usa la imagen adjunta como referencia visual exacta para colores, tipografía y layout.

ESTILO VISUAL (extraído de la imagen):
- Fondo principal: negro #0D0D0D
- Fondo de tarjetas: #1A1A1A
- Acento principal: verde neón #AAFF00
- Texto principal: blanco #FFFFFF
- Texto secundario: gris #888888
- Tipografía: sans-serif geométrica, bold para títulos, tamaños generosos
- Sin bordes redondeados exagerados, estilo oscuro y energético

NAVEGACIÓN:
- Móvil: barra de navegación inferior con 4 tabs — Dashboard, Hoy, Historial, Rutinas — con íconos y etiquetas de texto. Tab activo en verde neón.
- Desktop: sidebar izquierdo fijo con el logo GYMTRACKER arriba, los mismos 4 tabs en vertical con íconos y texto, y el contenido principal a la derecha ocupando el resto del ancho.

PANTALLA — DASHBOARD:
Construye la pantalla Dashboard con estos elementos en orden:

1. Header superior: ícono de rayo a la izquierda, logo "GYMTRACKER" en verde neón centrado, ícono de perfil a la derecha.

2. Número grande "15" en verde neón con el texto "DÍAS SEGUIDOS" debajo en gris mayúscula. Centrado, con espacio generoso arriba y abajo.

3. Tarjeta oscura con borde izquierdo verde neón: título "Día 12 — Pecho y Tríceps" en blanco bold. Lista de 3 ejercicios con ícono de flecha pequeño: "Press de banca 4×10", "Fondos 3×12", "Extensión de tríceps 3×15". Botón texto "EMPEZAR ENTRENAMIENTO" en la parte inferior de la tarjeta.

4. Dos tarjetas pequeñas lado a lado:
   - Izquierda: etiqueta "ESTA SEMANA" en gris pequeño, texto "3 / 5 sesiones" en blanco bold, barra de progreso verde neón debajo.
   - Derecha: etiqueta "ÚLTIMO PR" en gris pequeño, nombre "Sentadilla" en blanco, valor "100 kg" en verde neón bold.

LAYOUT DESKTOP del Dashboard: el número de racha y las tarjetas se organizan en una columna central con ancho máximo de 700px, centrada en el área de contenido. Las dos tarjetas pequeñas se muestran lado a lado igual que en móvil.
```

---

## PROMPT 2 — Entrenamiento del día

📎 **Imagen a adjuntar:** `entrenamiento_del_dia.png`

```
Mantén el estilo visual ya establecido. Construye la pantalla "Hoy" usando la imagen adjunta como referencia exacta.

PANTALLA — ENTRENAMIENTO DEL DÍA:

Header: mismo header de la app con logo GYMTRACKER.

Título de la sesión: "Día 12 — Pecho y Tríceps" en blanco bold grande. Debajo: "2 / 6 ejercicios completados" en gris. Separador horizontal verde neón debajo del subtítulo.

Lista de ejercicios, uno debajo del otro. Cada ejercicio es una tarjeta con:
- Nombre del ejercicio en blanco bold (tachado si está completado)
- Detalle en gris: "4 series × 10 reps — 60 kg"
- Chip de tiempo: ícono de reloj + "90 seg"
- Chip de músculo: texto con fondo oscuro borde sutil, ejemplo "Pecho" o "Tríceps"
- Botón circular a la derecha: vacío si pendiente, verde neón con check si completado
- Ejercicio activo (en progreso): borde izquierdo verde neón y texto del detalle en verde
- Ejercicio completado: nombre tachado, botón check verde

Usar estos 4 ejercicios de ejemplo:
1. Press de banca — 4 series × 10 reps — 60 kg — 90 seg — Pecho (completado)
2. Fondos en paralelas — 3 series × 12 reps — Peso corporal — 60 seg — Pecho (completado)
3. Extensión de tríceps en polea — 3 series × 15 reps — 20 kg — 60 seg — Tríceps (activo)
4. Press inclinado con mancuernas — 4 series × 8 reps — 25 kg — 90 seg — Pecho (pendiente)

Al final de la lista:
- Campo de texto con placeholder "Notas de la sesión..."
- Botón primario ancho completo "FINALIZAR ENTRENAMIENTO" en blanco sobre fondo oscuro con borde

LAYOUT DESKTOP: columna central de máximo 750px centrada. La lista de ejercicios ocupa todo el ancho de esa columna. En pantallas muy anchas (1200px+), mostrar un panel lateral derecho con un timer de descanso grande cuando el usuario marca un ejercicio como completado.
```

---

## PROMPT 3 — Historial de entrenamientos

📎 **Imagen a adjuntar:** `historial_de_entrenamientos.png`

```
Mantén el estilo visual ya establecido. Construye la pantalla "Historial" usando la imagen adjunta como referencia exacta.

PANTALLA — HISTORIAL:

Header: mismo header de la app.

Título "Historial" en blanco bold grande. Subtítulo "28 sesiones registradas" en gris debajo. Ícono de filtro alineado a la derecha del título.

Lista vertical de sesiones pasadas, ordenadas de la más reciente a la más antigua. Cada sesión es una tarjeta con:
- Borde izquierdo verde neón si la sesión fue completada al 100%, gris si fue parcial
- Fila superior: fecha en gris pequeño mayúscula (ejemplo: "LUN 23 JUN") a la izquierda, duración con ícono de reloj a la derecha (ejemplo: "52 min")
- Nombre de la sesión en blanco bold (ejemplo: "Día 11 — Espalda y Bíceps")
- Fila inferior: texto de ejercicios completados (ejemplo: "6 / 6 ejercicios completados") con ícono de check verde si completo, o ícono neutral si parcial
- Flecha "›" a la derecha para ver el detalle

Usar estas 3 sesiones de ejemplo:
1. LUN 23 JUN — 52 min — Día 11 — Espalda y Bíceps — 6/6 completados ✓ (borde verde)
2. SÁB 21 JUN — 35 min — Día 10 — Pecho y Tríceps — 4/6 ejercicios (borde gris)
3. JUE 19 JUN — 65 min — Día 09 — Pierna y Core pesado — 8/8 completados ✓ (borde verde)

LAYOUT DESKTOP: columna central de máximo 750px centrada. En desktop mostrar también un panel de detalle a la derecha que se abre al hacer clic en una sesión, mostrando todos los ejercicios de esa sesión con los pesos registrados.
```

---

## PROMPT 4 — Progreso por ejercicio

📎 **Imagen a adjuntar:** `progreso_por_ejercicio.png`

```
Mantén el estilo visual ya establecido. Construye la pantalla "Progreso" (que aparece dentro del tab Historial o como sub-sección) usando la imagen adjunta como referencia exacta.

PANTALLA — PROGRESO POR EJERCICIO:

Header: mismo header de la app.

Selector de ejercicio: fila horizontal de chips desplazable. Chip activo con fondo verde neón y texto negro bold. Chips inactivos con fondo oscuro y borde sutil. Ejercicios de ejemplo: "PRESS BANCA" (activo), "SENTADILLA", "PESO MUERTO", "DOMINADAS".

Tarjeta de progreso: fondo #1A1A1A, bordes redondeados suaves.
- Título: "Progreso — Press de banca" en blanco bold
- Línea 1: "Empezaste con 60 kg" en gris con punto separador
- Línea 2: "Ahora levantas 80 kg" en gris, badge "+33%" en verde neón con fondo oscuro
- Gráfica de línea: fondo oscuro dentro de la tarjeta, línea verde neón, puntos circulares en los valores, eje X con "HACE 8 SEM" a la izquierda y "HOY" a la derecha, líneas de guía horizontales en gris muy sutil

Sección "ÚLTIMOS 5 REGISTROS" en gris mayúscula como subtítulo.
Lista de 5 filas, cada fila separada por línea sutil:
- Punto de color a la izquierda (verde si es el más reciente, gris los anteriores)
- Fecha en gris (ejemplo: "HOY", "18 OCT", "11 OCT")
- Peso en blanco bold (ejemplo: "80 kg")
- Reps en gris (ejemplo: "x 4 reps")

Datos de ejemplo para la gráfica y registros: HOY 80kg×4, 18 OCT 77.5kg×5, 11 OCT 75kg×5, 04 OCT 75kg×4, 27 SEP 72.5kg×6.

LAYOUT DESKTOP: columna central de máximo 800px centrada. La gráfica ocupa todo el ancho de esa columna con más altura (350px en desktop vs 200px en móvil). El selector de chips puede mostrar todos los ejercicios sin scroll horizontal.
```

---

## PROMPT 5 — Biblioteca de rutinas

📎 **Imagen a adjuntar:** `biblioteca_de_rutinas.png`

```
Mantén el estilo visual ya establecido. Construye la pantalla "Rutinas" usando la imagen adjunta como referencia exacta.

PANTALLA — RUTINAS:

Header: mismo header de la app.

Título "Rutinas" en blanco bold grande. Botón "↓ IMPORTAR" alineado a la derecha del título, con borde, fondo oscuro y texto blanco pequeño.

Lista de rutinas, una tarjeta por rutina:

TARJETA RUTINA ACTIVA (primera):
- Nombre "Rutina Full Body 30 días" en blanco bold + chip "ACTIVA" en verde neón con fondo oscuro a la derecha del nombre
- Descripción: "30 días · 5 días por semana · Intermedio" en gris
- Etiqueta "Progreso" en gris + "Día 12 de 30" alineado a la derecha, ambos pequeños
- Barra de progreso verde neón (~40% completado)
- Botón "CONTINUAR DÍA 12 →" ancho completo, fondo oscuro con borde blanco

TARJETA RUTINA DISPONIBLE (segunda):
- Nombre "Rutina Upper/Lower" en blanco bold + chip "DISPONIBLE" en gris
- Descripción: "4 días por semana · Hipertrofia · Avanzado" en gris
- Sin barra de progreso, sin botón interno

TARJETA RUTINA DISPONIBLE (tercera):
- Nombre "Rutina Fuerza 5×5" en blanco bold + chip "DISPONIBLE" en gris
- Descripción: "3 días por semana · Fuerza Base · Principiante" en gris

TARJETA ESPECIAL al final (ligeramente diferente, fondo con transparencia o borde sutil):
- Ícono cuadrado centrado con fondo verde oscuro
- Título "¿Quieres una rutina personalizada?" en verde neón centrado
- Texto: "Usa este prompt con ChatGPT o Claude para generar tu rutina en el formato correcto para importarla al tracker." en gris centrado
- Botón "📋 COPIAR PROMPT" con borde verde neón, al hacer clic copia al portapapeles el texto del prompt para generar rutinas en IA

LAYOUT DESKTOP: columna central de máximo 750px centrada. Las tarjetas de rutinas se mantienen en lista vertical. En desktop, al hacer clic en una rutina disponible, se abre un panel lateral derecho con el detalle de la rutina (días, ejercicios por día).
```

---

## PROMPT 6 — Datos de ejemplo + Funcionalidad final

📎 **Sin imágenes — solo texto**

```
Mantén el estilo visual ya establecido. Agrega los datos de ejemplo y conecta la funcionalidad de la app usando el backend de Horizons.

DATOS DE EJEMPLO A CREAR EN EL BACKEND:

Rutina activa: "Rutina Full Body 30 días" con 30 días de entrenamiento. Días alternando grupos musculares: Pecho/Tríceps, Espalda/Bíceps, Piernas/Core, repetir. Cada día con 5-8 ejercicios, cada uno con series, reps y peso sugerido.

Ejercicios base en la biblioteca: Press de banca, Fondos en paralelas, Extensión de tríceps en polea, Press inclinado con mancuernas, Dominadas, Remo con barra, Curl de bíceps, Sentadilla, Peso muerto, Prensa de pierna, Extensión de cuádriceps, Curl femoral, Plancha.

Historial de ejemplo: 12 sesiones pasadas con pesos y fechas reales distribuidas en las últimas 6 semanas. Al menos 2 sesiones incompletas para que el historial se vea realista.

FUNCIONALIDAD A CONECTAR:

1. El botón "EMPEZAR ENTRENAMIENTO" del Dashboard lleva a la pantalla Hoy con la sesión del día actual cargada.

2. Al marcar un ejercicio como completado en la pantalla Hoy, el contador "X / 6 ejercicios completados" se actualiza en tiempo real.

3. El botón "FINALIZAR ENTRENAMIENTO" guarda la sesión en el historial con la fecha actual, los pesos registrados y las notas, y actualiza la racha del Dashboard.

4. El botón "COPIAR PROMPT" en Rutinas copia este texto al portapapeles:
"Eres un entrenador personal experto. Crea una rutina de entrenamiento de 30 días en formato Markdown con esta estructura exacta por cada día:
## Día [N] — [Nombre del grupo muscular]
- [Nombre del ejercicio] | [Series]×[Reps] | [Peso sugerido] kg | Descanso: [X] seg | Foco: [músculo]
La rutina debe ser [nivel: principiante/intermedio/avanzado], [X] días por semana, con objetivo de [objetivo]. Incluye días de descanso marcados como ## Día [N] — Descanso activo."

5. La racha del Dashboard se incrementa automáticamente cada vez que se finaliza un entrenamiento. Si pasan más de 36 horas sin entrenar, la racha vuelve a 0.
```

---

## Notas de uso

- **Orden es importante:** no saltes prompts, cada uno asume que el anterior ya fue construido
- **Si Horizons no replica exactamente la imagen:** describe el elemento específico que no quedó bien y pide corrección antes de continuar
- **Desktop:** todos los prompts ya incluyen instrucciones de layout desktop, no necesitas un prompt separado para eso
- **El prompt del portapapeles (Prompt 6):** puedes personalizar el texto del prompt para IA según el tipo de rutina que quieras generar
