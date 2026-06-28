# GymTracker — Prompts para Hostinger Horizons

> **Cómo usar estos prompts:**
> - Pégalos en orden, uno a la vez
> - Adjunta las imágenes indicadas antes de enviar
> - Espera que Horizons termine antes de pasar al siguiente
> - Si algo no queda bien, corrígelo antes de continuar

> **Sobre el estilo visual:**
> La imagen hace el trabajo. Solo describe comportamiento, desktop y datos — no el diseño visual.
> Los prompts 2 en adelante ya incluyen "Mantén el estilo visual ya establecido".

---

## PROMPT 1 — Fundación + Dashboard

📎 **Adjuntar:** `dashboard.png`

```
Construye una app web llamada GymTracker para seguimiento de entrenamientos personales. Replica el diseño de la imagen adjunta de forma exacta.

NAVEGACIÓN:
- Móvil: barra inferior con 4 tabs — Dashboard, Hoy, Historial, Rutinas.
- Desktop: sidebar izquierdo fijo con los mismos 4 tabs en vertical. Contenido principal a la derecha.

INTERACCIONES DEL DASHBOARD:
- El botón "EMPEZAR ENTRENAMIENTO" navega a la pantalla Hoy.
- Las dos tarjetas inferiores son solo informativas, sin acción.

DESKTOP: contenido centrado con ancho máximo de 700px dentro del área principal.

ESTADO VACÍO (primera vez que el usuario abre la app):
- Racha: mostrar "0 DÍAS SEGUIDOS"
- Tarjeta de hoy: mostrar "No hay rutina activa — ve a Rutinas para comenzar"
- Tarjetas inferiores: "0 / 0 sesiones" y "Sin registros aún"
```

---

## PROMPT 2 — Entrenamiento del día

📎 **Adjuntar:** `entrenamiento_del_dia.png`

```
Mantén el estilo visual ya establecido. Construye la pantalla "Hoy" replicando la imagen adjunta de forma exacta.

INTERACCIONES:
- Al hacer clic en el botón circular de un ejercicio, se marca como completado: nombre tachado, botón verde con check, el siguiente ejercicio pasa a estado activo (borde izquierdo verde).
- El contador "X / 6 ejercicios completados" se actualiza en tiempo real con cada check.
- El botón "FINALIZAR ENTRENAMIENTO" solo se activa cuando al menos 1 ejercicio fue completado. Al presionarlo, guarda la sesión y navega al Dashboard.

DESKTOP: columna central de 750px máximo. En pantallas mayores a 1200px, mostrar un panel lateral derecho con un timer de cuenta regresiva que se activa automáticamente al completar un ejercicio, mostrando los segundos de descanso indicados en el chip.

ESTADO VACÍO: si no hay rutina activa, mostrar mensaje centrado "No tienes un entrenamiento programado para hoy" con botón "Ver rutinas" que navega a Rutinas.
```

---

## PROMPT 3 — Historial + Progreso

📎 **Adjuntar:** `historial_de_entrenamientos.png` y `progreso_por_ejercicio.png`

```
Mantén el estilo visual ya establecido. Construye la pantalla "Historial" replicando la primera imagen adjunta. Dentro de esta misma sección, agrega una sub-pantalla "Progreso" replicando la segunda imagen adjunta.

NAVEGACIÓN INTERNA:
- La pantalla Historial tiene dos vistas accesibles desde tabs o toggle en la parte superior: "Sesiones" y "Progreso".
- "Sesiones" muestra la lista del historial.
- "Progreso" muestra las gráficas por ejercicio.
- Ambas vistas comparten el tab "Historial" activo en la barra de navegación.

INTERACCIONES — SESIONES:
- Al hacer clic en una sesión, se abre el detalle con todos los ejercicios, pesos y notas de esa sesión.
- El ícono de filtro permite filtrar por mes.

INTERACCIONES — PROGRESO:
- Al seleccionar un chip de ejercicio, la gráfica y la lista de últimos registros se actualizan mostrando los datos de ese ejercicio.

DESKTOP: columna central de 750px máximo. En Sesiones, al hacer clic en una sesión, el detalle se abre en un panel lateral derecho en lugar de navegar a otra página.

ESTADO VACÍO — SESIONES: "Aún no has registrado ningún entrenamiento. ¡Empieza hoy!"
ESTADO VACÍO — PROGRESO: "Completa al menos un entrenamiento para ver tu progreso."
```

---

## PROMPT 4 — Rutinas

📎 **Adjuntar:** `biblioteca_de_rutinas.png`

```
Mantén el estilo visual ya establecido. Construye la pantalla "Rutinas" replicando la imagen adjunta de forma exacta.

INTERACCIONES:
- El botón "CONTINUAR DÍA X" de la rutina activa navega a la pantalla Hoy con esa sesión cargada.
- Al hacer clic en una rutina disponible, se muestra un modal de confirmación: "¿Activar esta rutina? Esto reemplazará tu rutina actual." con botones Cancelar y Confirmar.
- El botón "IMPORTAR" abre un modal con un campo de texto para pegar el contenido markdown de una rutina. Al confirmar, la parsea y la agrega a la biblioteca.
- El botón "COPIAR PROMPT" copia al portapapeles el texto definido en el Prompt 6B.

DESKTOP: columna central de 750px máximo. Al hacer clic en una rutina disponible, el detalle se despliega en un panel lateral derecho mostrando los días y ejercicios de la rutina.

ESTADO VACÍO: si no hay ninguna rutina, mostrar solo la tarjeta "¿Quieres una rutina personalizada?" con el botón "COPIAR PROMPT".
```

---

## PROMPT 5 — Datos de ejemplo

📎 **Sin imágenes**

```
Mantén el estilo visual ya establecido. Agrega datos de ejemplo al backend para que la app se vea funcional desde el primer momento.

RUTINAS A CREAR:

Rutina 1 — "Rutina Full Body 30 días" (marcarla como ACTIVA en Día 12):
- Estructura: 5 días de entrenamiento + 2 de descanso por semana, durante 30 días
- Grupos alternados: Pecho/Tríceps, Espalda/Bíceps, Piernas/Core, repetir
- Cada día: 5 a 8 ejercicios con series, reps y peso sugerido en kg
- Incluir días de descanso activo marcados claramente

Rutina 2 — "Rutina Upper/Lower" (DISPONIBLE):
- 4 días por semana, enfoque hipertrofia, nivel avanzado
- 2 días upper body + 2 días lower body

Rutina 3 — "Rutina Fuerza 5×5" (DISPONIBLE):
- 3 días por semana, enfoque fuerza base, nivel principiante
- Basada en los 5 levantamientos compuestos principales

HISTORIAL A CREAR:
- 12 sesiones pasadas distribuidas en las últimas 6 semanas
- Al menos 2 sesiones incompletas (4/6 ejercicios) para que el historial se vea realista
- Pesos progresivos en cada sesión para que las gráficas de progreso muestren una curva ascendente
- La racha actual debe quedar en 15 días consecutivos

EJERCICIOS EN LA BIBLIOTECA:
Press de banca, Fondos en paralelas, Extensión de tríceps en polea, Press inclinado con mancuernas, Dominadas, Remo con barra, Curl de bíceps, Sentadilla, Peso muerto, Prensa de pierna, Extensión de cuádriceps, Curl femoral, Plancha.
```

---

## PROMPT 6 — Funcionalidad y conexiones

📎 **Sin imágenes**

```
Mantén el estilo visual ya establecido. Conecta toda la funcionalidad de la app.

FLUJO PRINCIPAL:
1. Dashboard → botón "EMPEZAR ENTRENAMIENTO" → carga el día actual de la rutina activa en la pantalla Hoy.
2. Pantalla Hoy → marcar ejercicios → botón "FINALIZAR ENTRENAMIENTO" → guarda la sesión en el historial con fecha, ejercicios completados, pesos y notas → navega al Dashboard → actualiza la racha.
3. Rutinas → botón "CONTINUAR DÍA X" → misma pantalla Hoy con esa sesión.

LÓGICA DE RACHA:
- Aumenta en 1 cada vez que se finaliza un entrenamiento en un día nuevo.
- Si pasan más de 36 horas sin finalizar un entrenamiento, la racha vuelve a 0.
- El número en el Dashboard siempre refleja la racha actual en tiempo real.

LÓGICA DE PROGRESO:
- Cada vez que se finaliza un entrenamiento, los pesos registrados se guardan en el historial de ese ejercicio.
- La gráfica de Progreso usa esos datos para mostrar la evolución.
- El "Último PR" del Dashboard muestra el ejercicio donde el usuario superó su peso máximo más recientemente.

TEXTO DEL BOTÓN "COPIAR PROMPT" EN RUTINAS:
"Eres un entrenador personal experto. Crea una rutina de entrenamiento en formato Markdown con esta estructura exacta por cada día:

## Día [N] — [Nombre del grupo muscular]
- [Nombre del ejercicio] | [Series]×[Reps] | [Peso sugerido] kg | Descanso: [X] seg | Foco: [músculo]

Incluye días de descanso marcados como:
## Día [N] — Descanso activo

Parámetros de mi rutina:
- Duración: [30/60/90] días
- Días por semana: [3/4/5]
- Nivel: [principiante/intermedio/avanzado]
- Objetivo: [fuerza/hipertrofia/resistencia/pérdida de grasa]"
```

---

## Notas de uso

- **No saltes prompts** — cada uno asume que el anterior fue construido correctamente
- **Si Horizons no replica la imagen** — describe el elemento específico que falló y pide corrección antes de continuar
- **Prompt 3 lleva dos imágenes** — adjunta ambas a la vez antes de enviar
- **El texto del prompt de IA (Prompt 6)** — puedes editarlo según el tipo de rutina que uses
