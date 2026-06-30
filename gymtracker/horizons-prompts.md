# GymTracker — Prompts para Hostinger Horizons

> **Cómo usar:**
> - Pega los prompts en orden, uno a la vez
> - Adjunta las imágenes indicadas antes de enviar
> - Espera que Horizons termine antes de continuar
> - Si algo no replica bien la imagen, corrígelo antes de seguir

> **Consistencia global — aplica a todos los prompts:**
> - El nombre de la app es siempre **GYMTRACKER** con subtítulo **POWER & PRECISION**
> - Todo el texto de la interfaz en **español** (labels, botones, placeholders, mensajes)
> - El sidebar siempre muestra: Dashboard, Hoy, Historial, Rutinas — en ese orden y en español
> - Paleta: fondo #0D0D0D, tarjetas #1A1A1A, acento verde neón #AAFF00, texto blanco, secundario #888888

---

## PROMPT 1 — Fundación + Login

📎 **Adjuntar:** `login_registro.png` + `login_registro_minimalista_mobile.png`

```
Construye una app web llamada GymTracker. Replica el diseño de la 
imagen desktop adjunta de forma exacta. Usa la imagen móvil solo 
como referencia de layout para pantallas pequeñas — no como 
referencia de features ni contenido.

El nombre de la app es GYMTRACKER con subtítulo POWER & PRECISION. 
Todo el texto de la interfaz en español.

NAVEGACIÓN GLOBAL (aplica a toda la app):
- Desktop: sidebar izquierdo fijo con logo GYMTRACKER arriba, 
  4 tabs en vertical — Dashboard, Hoy, Historial, Rutinas — 
  y perfil de usuario al fondo
- Móvil: barra de navegación inferior con los mismos 4 tabs

PANTALLA DE LOGIN:
Replica la imagen desktop exactamente. El toggle muestra 
"Iniciar sesión" y "Registrarse". Al cambiar de tab se 
muestran los campos correspondientes para registro 
(nombre, email, contraseña, confirmar contraseña).

En móvil, usar el layout de la imagen móvil: logo centrado 
arriba, campos con estilo línea inferior, botón ancho completo.
```

---

## PROMPT 2 — Dashboard

📎 **Adjuntar:** `dashboard.png` + `dashboard_mobile.png`

```
Mantén el estilo visual ya establecido. Construye la pantalla 
Dashboard replicando la imagen desktop adjunta exactamente. 
Usa la imagen móvil solo como referencia de layout responsivo.

GYMTRACKER / POWER & PRECISION en el sidebar. Todo en español.

INTERACCIONES:
- El botón "EMPEZAR ENTRENAMIENTO" navega a la pantalla Hoy
- Las tarjetas "Esta semana" y "Último PR" son informativas, 
  sin acción al hacer clic
- Los tres puntos "⋯" en la tarjeta de próxima sesión abren 
  un menú con opción "Ver rutina completa"

ESTADO VACÍO (primera vez sin datos):
- Racha: "0 DÍAS SEGUIDOS"
- Tarjeta central: "No hay rutina activa — ve a Rutinas para comenzar"
- Tarjetas inferiores: "0 / 0 sesiones" y "Sin registros aún"

DESKTOP: contenido centrado, ancho máximo 900px en área principal.
MÓVIL: layout de una columna según imagen móvil adjunta.
```

---

## PROMPT 3 — Hoy: Entrenamiento del día

📎 **Adjuntar:** `hoy_entrenamiento_en_curso.png` + `hoy_entrenamiento_mobile.png`

```
Mantén el estilo visual ya establecido. Construye la pantalla "Hoy" 
replicando la imagen desktop exactamente. Usa la imagen móvil 
solo como referencia de layout responsivo. Todo en español.

INTERACCIONES:
- El cronómetro en la esquina superior derecha cuenta el tiempo 
  total de la sesión desde que se entra a esta pantalla
- El campo de peso (KG) en cada ejercicio es editable — el 
  usuario puede modificarlo antes de marcar el ejercicio
- Al hacer clic en el botón circular de check, el ejercicio 
  se marca como completado: nombre tachado, botón verde, 
  el contador "X / N ejercicios completados" se actualiza
- "FINALIZAR ENTRENAMIENTO" guarda la sesión en el historial 
  con fecha, ejercicios, pesos y notas, luego navega al Dashboard
- "DESCARTAR SESIÓN" elimina la sesión sin guardar, con 
  confirmación previa

ESTADO VACÍO: si no hay rutina activa mostrar "No tienes 
entrenamiento programado para hoy" con botón "Ir a Rutinas".

DESKTOP: columna central 800px máximo.
MÓVIL: según imagen móvil — mostrar el ejercicio activo 
destacado con campos KG y REPS editables por serie.
```

---

## PROMPT 4 — Historial: Sesiones

📎 **Adjuntar:** `historial_sesiones.png` + `historial_sesiones_mobile.png`

```
Mantén el estilo visual ya establecido. Construye la pantalla 
"Historial" con sub-vista "Sesiones" replicando la imagen 
desktop exactamente. Usa la imagen móvil solo como referencia 
de layout. Todo en español.

El toggle en la parte superior alterna entre "Sesiones" y 
"Progreso" (la sub-vista Progreso se construye en el siguiente prompt).

INTERACCIONES — LISTA:
- Al hacer clic en una sesión se abre el detalle en el panel derecho
- El botón "Filtrar" permite filtrar por mes

INTERACCIONES — DETALLE DE SESIÓN (panel derecho):
- Los campos de PESO y REPS de cada set son editables
- El campo de notas es editable
- "GUARDAR CAMBIOS" guarda las modificaciones
- "ELIMINAR SESIÓN" elimina con confirmación previa
- El VOLUMEN TOTAL se recalcula automáticamente al editar pesos

ESTADO VACÍO: "Aún no has registrado ningún entrenamiento. 
¡Empieza hoy!" con botón "Ir a Hoy".

DESKTOP: layout dividido — lista a la izquierda, detalle en 
panel derecho al hacer clic en una sesión.
MÓVIL: lista en pantalla completa, detalle abre como nueva 
pantalla con botón "← Volver".
```

---

## PROMPT 5 — Historial: Progreso

📎 **Adjuntar:** `historial_progreso.png` + `historial_progreso_mobile.png`

```
Mantén el estilo visual ya establecido. Construye la sub-vista 
"Progreso" dentro de la pantalla Historial replicando la imagen 
desktop exactamente. Usa la imagen móvil solo como referencia 
de layout. Todo en español — los chips de ejercicios, labels 
y textos deben estar en español.

El branding en el sidebar es GYMTRACKER / POWER & PRECISION.

INTERACCIONES:
- Al seleccionar un chip de ejercicio, la gráfica y los 
  registros se actualizan para ese ejercicio
- La gráfica muestra la evolución del peso máximo levantado 
  en el tiempo
- El "1 RM ESTIMADO" se calcula automáticamente a partir 
  de los datos registrados
- "VER TODOS" en la sección de registros muestra el historial 
  completo de ese ejercicio

ESTADO VACÍO: "Completa al menos un entrenamiento para ver 
tu progreso."

DESKTOP: gráfica de ancho completo en área central, 350px altura.
MÓVIL: métricas en grid 2×2 arriba, gráfica debajo según 
imagen móvil adjunta.
```

---

## PROMPT 6 — Rutinas

📎 **Adjuntar:** `rutinas.png` + `rutinas_mobile.png`

```
Mantén el estilo visual ya establecido. Construye la pantalla 
"Rutinas" replicando la imagen desktop exactamente. Usa la 
imagen móvil solo como referencia de layout. Todo en español.

INTERACCIONES:
- "CONTINUAR DÍA X" navega a la pantalla Hoy con esa sesión cargada
- Al hacer clic en una rutina disponible se muestra modal de 
  confirmación: "¿Activar esta rutina? Esto reemplazará tu 
  rutina actual." con botones Cancelar y Confirmar
- El ícono de estrella marca/desmarca una rutina como favorita
- "IMPORTAR" navega a la pantalla Importar Rutina
- "COPIAR PROMPT" copia al portapapeles el texto definido 
  en el Prompt 8

RUTINAS POR DEFECTO a crear:
- Arnold Split — 6 días/semana · Intermedio (marcar como ACTIVA)
- Push Pull Legs (PPL) — 6 días/semana · Intermedio
- Full Body 3 días — 3 días/semana · Principiante
- Upper/Lower — 4 días/semana · Intermedio

ESTADO VACÍO: mostrar solo la tarjeta "¿Quieres una rutina 
personalizada?" si no hay rutinas.

DESKTOP: columna central 800px máximo.
MÓVIL: según imagen móvil adjunta.
```

---

## PROMPT 7 — Importar Rutina

📎 **Adjuntar:** `importar_rutina.png` + `importar_rutina_mobile.png`

```
Mantén el estilo visual ya establecido. Construye la pantalla 
"Importar Rutina" replicando la imagen desktop exactamente. 
Usa la imagen móvil solo como referencia de layout. 
Todo en español.

Esta pantalla es accesible desde el botón "IMPORTAR" en Rutinas. 
El tab activo en el sidebar sigue siendo "Rutinas".

INTERACCIONES:
- El área de texto acepta contenido en formato Markdown
- "IMPORTAR AHORA" parsea el markdown, extrae los días y 
  ejercicios, y los agrega a la biblioteca de rutinas
- Si el parsing falla, mostrar mensaje de error con el 
  formato esperado
- Después de importar exitosamente, navegar a Rutinas y 
  mostrar la nueva rutina en la biblioteca

DESKTOP: editor markdown a la izquierda, guía de formato 
visible debajo según imagen adjunta.
MÓVIL: editor en pantalla completa según imagen móvil adjunta.
```

---

## PROMPT 8 — Datos de ejemplo

📎 **Sin imágenes**

```
Mantén el estilo visual ya establecido. Agrega datos de ejemplo 
al backend para que la app se vea funcional.

RUTINAS A CREAR EN EL BACKEND:

Arnold Split (ACTIVA, Día 12 de 30):
Lunes/Jueves — Pecho + Espalda: Press de banca 4×10 80kg, 
Dominadas 4×8 peso corporal, Aperturas 3×12 20kg, Remo con 
barra 4×10 60kg, Pull-over 3×12 25kg
Martes/Viernes — Hombros + Brazos: Press militar 4×10 50kg, 
Elevaciones laterales 3×15 10kg, Curl de bíceps 4×10 30kg, 
Extensión de tríceps 4×12 25kg, Curl martillo 3×12 25kg
Miércoles/Sábado — Piernas + Core: Sentadilla 4×8 100kg, 
Prensa 4×10 140kg, Curl femoral 3×12 40kg, Extensión de 
cuádriceps 3×15 35kg, Plancha 3×60seg peso corporal

Push Pull Legs, Full Body 3 días y Upper/Lower: crear estructura 
básica de días y ejercicios coherentes con cada metodología.

HISTORIAL: 12 sesiones en las últimas 6 semanas, al menos 
2 incompletas. Pesos progresivos para que las gráficas muestren 
curva ascendente. Racha actual: 15 días.

USUARIO DE EJEMPLO: nombre Alex Rivera, email alex@gymtracker.com
```

---

## PROMPT 9 — Funcionalidad y conexiones

📎 **Sin imágenes**

```
Mantén el estilo visual ya establecido. Conecta toda la 
funcionalidad de la app.

FLUJO PRINCIPAL:
1. Login → Dashboard
2. Dashboard → "EMPEZAR ENTRENAMIENTO" → Hoy con sesión del día
3. Hoy → completar ejercicios → "FINALIZAR ENTRENAMIENTO" → 
   guarda sesión → Dashboard con racha actualizada
4. Rutinas → "CONTINUAR DÍA X" → Hoy con esa sesión
5. Rutinas → "IMPORTAR" → pantalla Importar Rutina
6. Historial → clic en sesión → detalle editable en panel derecho

LÓGICA DE RACHA:
- Aumenta 1 cada vez que se finaliza un entrenamiento en un 
  día nuevo
- Si pasan más de 36 horas sin finalizar, vuelve a 0
- Se muestra siempre actualizada en el Dashboard

LÓGICA DE PROGRESO:
- Al finalizar entrenamiento, los pesos se guardan por ejercicio
- La gráfica de Progreso usa esos datos
- "Último PR" en Dashboard muestra el ejercicio donde se 
  superó el peso máximo más recientemente
- El VOLUMEN TOTAL de una sesión = suma de (series × reps × kg) 
  de todos los ejercicios

TEXTO DEL BOTÓN "COPIAR PROMPT" EN RUTINAS:
"Eres un entrenador personal experto. Genera una rutina de 
entrenamiento en formato Markdown con esta estructura:

# Nombre de la rutina

## Día 1 — [Grupo muscular]
- [Ejercicio] | [Series]×[Reps] | [Peso] kg | Descanso: [X] seg | Foco: [músculo]

## Día 2 — Descanso activo

Parámetros:
- Duración: [30/60/90] días
- Días por semana: [3/4/5/6]
- Nivel: [principiante/intermedio/avanzado]
- Objetivo: [fuerza/hipertrofia/resistencia]"
```

---

## Resumen de imágenes por prompt

| Prompt | Desktop | Móvil |
|--------|---------|-------|
| 1 — Login | `login_registro.png` | `login_registro_minimalista_mobile.png` |
| 2 — Dashboard | `dashboard.png` | `dashboard_mobile.png` |
| 3 — Hoy | `hoy_entrenamiento_en_curso.png` | `hoy_entrenamiento_mobile.png` |
| 4 — Historial Sesiones | `historial_sesiones.png` | `historial_sesiones_mobile.png` |
| 5 — Historial Progreso | `historial_progreso.png` | `historial_progreso_mobile.png` |
| 6 — Rutinas | `rutinas.png` | `rutinas_mobile.png` |
| 7 — Importar Rutina | `importar_rutina.png` | `importar_rutina_mobile.png` |
| 8 — Datos de ejemplo | — | — |
| 9 — Funcionalidad | — | — |
