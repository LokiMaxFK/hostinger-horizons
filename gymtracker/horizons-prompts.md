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

**✅ Al terminar este prompt deberías tener:**
- Pantalla de login visible con fondo negro, logo GYMTRACKER en verde neón y subtítulo POWER & PRECISION
- Toggle funcional entre "Iniciar sesión" y "Registrarse" con sus campos correspondientes
- Botón "ENTRAR" en verde neón
- Sidebar izquierdo generado con los 4 tabs (aunque las pantallas aún estén vacías)
- En móvil: navegación inferior con los 4 tabs
- La app ya tiene colores, tipografía y estructura base correctos

**🚫 No continúes si:**
- El fondo no es oscuro (#0D0D0D)
- El acento no es verde neón (#AAFF00)
- El sidebar no aparece en desktop
- El nombre dice algo diferente a GYMTRACKER

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

**✅ Al terminar este prompt deberías tener:**
- Número de racha grande en verde neón con texto "DÍAS SEGUIDOS"
- Tarjeta de próxima sesión con lista de ejercicios y botón "EMPEZAR ENTRENAMIENTO"
- Dos tarjetas inferiores: "ESTA SEMANA" con barra de progreso y "ÚLTIMO PR"
- Cita motivacional al fondo
- Perfil de usuario visible al fondo del sidebar
- En móvil: layout de una columna con nav inferior

**🚫 No continúes si:**
- El botón "EMPEZAR ENTRENAMIENTO" no es visible o no tiene el estilo correcto
- Las tarjetas inferiores no aparecen lado a lado
- El sidebar no muestra el tab "Dashboard" activo

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

**✅ Al terminar este prompt deberías tener:**
- Lista de ejercicios con chips de músculo y descanso, campo de peso editable y botón circular de check
- Cronómetro visible en la esquina superior derecha
- Contador "X / N ejercicios completados" en tiempo real
- Campo de notas al fondo
- Botón "FINALIZAR ENTRENAMIENTO" en verde neón
- Enlace "DESCARTAR SESIÓN" debajo del botón
- En móvil: ejercicio activo destacado con sets editables por fila

**🚫 No continúes si:**
- El campo de peso no es editable
- El check no marca el ejercicio como completado visualmente
- El cronómetro no aparece

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

**✅ Al terminar este prompt deberías tener:**
- Toggle "Sesiones / Progreso" en la parte superior
- Lista de sesiones a la izquierda con fecha, duración, nombre y estado (completo/parcial)
- Al hacer clic en una sesión, el panel derecho muestra el detalle con tabla de sets editables
- Campos de PESO y REPS editables por set en el detalle
- Campo de notas editable con texto de ejemplo
- Botones "GUARDAR CAMBIOS" y "ELIMINAR SESIÓN" visibles
- VOLUMEN TOTAL visible en el encabezado del detalle
- En móvil: lista en pantalla completa, detalle como pantalla separada

**🚫 No continúes si:**
- El panel de detalle no se abre al hacer clic en una sesión
- Los campos de peso/reps no son editables
- El toggle no alterna entre Sesiones y Progreso

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

**✅ Al terminar este prompt deberías tener:**
- Sub-vista "Progreso" accesible desde el toggle de Historial
- Chips de ejercicios en la parte superior (Press Banca, Sentadilla, Peso Muerto, Dominadas, Remo)
- Gráfica de línea verde neón mostrando evolución de peso
- Badge "+X%" y texto "Empezaste con X kg · Ahora levantas X kg"
- "1 RM ESTIMADO" visible junto a los últimos registros
- Lista de últimos 5 registros con fecha, peso y reps
- En móvil: grid 2×2 de métricas arriba, gráfica debajo

**🚫 No continúes si:**
- La gráfica no aparece o está vacía
- Los chips no cambian el ejercicio mostrado
- El sidebar sigue mostrando "IRON FOCUS" en lugar de "GYMTRACKER"

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

**✅ Al terminar este prompt deberías tener:**
- Rutina activa destacada (Arnold Split) con chip "ACTIVA", barra de progreso y botón "CONTINUAR DÍA X"
- Sección "BIBLIOTECAS DISPONIBLES" con PPL, Full Body 3 días y Upper/Lower
- Cada rutina disponible con chip "DISPONIBLE" e información de días/nivel
- Tarjeta "¿Quieres una rutina personalizada?" con botón "COPIAR PROMPT" al fondo
- Botón "IMPORTAR" visible en la parte superior derecha
- Ícono de estrella en la rutina activa
- En móvil: layout de una columna según imagen móvil

**🚫 No continúes si:**
- No aparecen las 4 rutinas por defecto
- El botón "IMPORTAR" no es visible
- El botón "COPIAR PROMPT" no aparece en la tarjeta inferior

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

**✅ Al terminar este prompt deberías tener:**
- Pantalla independiente accesible desde "IMPORTAR" en Rutinas
- Área de texto grande con ejemplo de formato Markdown visible
- Badge "IA AUTO-PARSING ACTIVADO" visible
- Botón "IMPORTAR AHORA" en verde neón
- Sección "GUÍA DE FORMATO" con 3 tarjetas: Estructura, Ejercicios, Series/Reps
- El tab "Rutinas" sigue activo en el sidebar
- En móvil: editor en pantalla completa con botón "IMPORT NOW" al fondo

**🚫 No continúes si:**
- La pantalla no es accesible desde el botón "IMPORTAR" de Rutinas
- El área de texto no acepta input
- La guía de formato no aparece

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

**✅ Al terminar este prompt deberías tener:**
- Arnold Split con ejercicios reales cargados en el backend (3 días tipo: Pecho/Espalda, Hombros/Brazos, Piernas/Core)
- Las otras 3 rutinas con su estructura básica de días y ejercicios
- 12 sesiones en el historial con fechas reales de las últimas 6 semanas
- Racha de 15 días visible en el Dashboard
- Dashboard mostrando "Día 12 — [nombre del día]" como próxima sesión
- Las gráficas de Progreso con datos reales que muestran curva ascendente

**🚫 No continúes si:**
- El Dashboard no muestra datos (sigue en estado vacío)
- El Historial no tiene sesiones listadas
- La gráfica de Progreso está vacía

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

**✅ Al terminar este prompt deberías tener:**
- "EMPEZAR ENTRENAMIENTO" en el Dashboard carga la sesión del día en la pantalla Hoy
- Finalizar entrenamiento guarda la sesión y actualiza la racha en el Dashboard
- La racha se resetea a 0 si pasan más de 36 horas sin entrenar
- "COPIAR PROMPT" en Rutinas copia el texto de generación de rutinas al portapapeles
- El VOLUMEN TOTAL en Historial se recalcula al editar pesos
- "Último PR" en Dashboard se actualiza cuando se supera un peso máximo
- La app completa es navegable de punta a punta sin errores

**🚫 La app NO está lista si:**
- El flujo Login → Dashboard → Hoy → Historial no funciona completo
- Finalizar un entrenamiento no aparece en el Historial
- La racha no se actualiza tras completar un entrenamiento

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
