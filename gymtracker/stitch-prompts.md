# GymTracker — Prompts para Google Stitch

> Pega el Prompt 0 primero. Luego cada pantalla en orden, una a la vez.
> Si el resultado no convence, descríbe qué cambiar antes de continuar.

---

## 🎨 PROMPT 0 — ESTILO GLOBAL

Diseña el sistema visual para una app web llamada GymTracker, para seguimiento de entrenamientos personales. Plataforma web, responsive — móvil y desktop.

Estilo: oscuro, intenso y enfocado. Transmite energía y motivación sin distracciones.

Paleta: fondo principal #0D0D0D, fondo de tarjetas #1A1A1A, acento verde neón #AAFF00, gris medio #3A3A3A, texto blanco #FFFFFF, texto secundario #888888.

Tipografía: sans-serif geométrica bold para títulos, regular para cuerpo. Tamaños grandes, fáciles de leer.

Densidad equilibrada. Botones y áreas de toque generosas.

Elementos: íconos lineales simples, gradientes sutiles en acentos. Sin ilustraciones ni fotografías.

Móvil: navegación inferior con 4 tabs — Dashboard, Hoy, Historial, Rutinas.
Desktop: sidebar izquierdo fijo con los mismos 4 tabs en vertical.

No usar: fondos brillantes, sombras muy marcadas, tipografía serif.

---

## 📱 PROMPT 1 — LOGIN Y REGISTRO

> Puerta de entrada a la app. Limpia y directa, sin distracciones.

Mantén el estilo visual ya establecido.

Diseña la pantalla de autenticación de GymTracker. En la parte superior, el logo "GYMTRACKER" en verde neón bold centrado, con el ícono de rayo a su izquierda.

Debajo del logo, un toggle de dos opciones: "Iniciar sesión" y "Registrarse". El tab activo en verde neón, el inactivo en gris.

Vista "Iniciar sesión": campo de email con label flotante, campo de contraseña con ícono de ojo para mostrar/ocultar, botón primario "ENTRAR" en verde neón ancho completo, enlace pequeño "¿Olvidaste tu contraseña?" en gris debajo del botón.

Vista "Registrarse": campo de nombre, campo de email, campo de contraseña, campo de confirmar contraseña, botón primario "CREAR CUENTA" en verde neón ancho completo.

En la parte inferior de ambas vistas, texto pequeño en gris: "Al continuar aceptas los Términos de uso".

Desktop: formulario centrado en tarjeta con ancho máximo de 420px, con el logo arriba de la tarjeta.

---

## 📱 PROMPT 2 — DASHBOARD

> Pantalla de inicio. Resumen del estado del usuario de un vistazo.

Mantén el estilo visual ya establecido.

Diseña la pantalla Dashboard de GymTracker. Header superior: ícono de rayo a la izquierda, logo "GYMTRACKER" en verde neón centrado, ícono de perfil a la derecha.

Número grande "15" en verde neón con texto "DÍAS SEGUIDOS" debajo en gris mayúscula. Centrado, con espacio generoso.

Tarjeta oscura con borde izquierdo verde neón: título "Día 12 — Pecho y Tríceps" bold. Lista de 3 ejercicios con ícono de flecha: "Press de banca 4×10", "Fondos 3×12", "Extensión de tríceps 3×15". Botón "EMPEZAR ENTRENAMIENTO" al fondo de la tarjeta.

Dos tarjetas pequeñas lado a lado:
- Izquierda: "ESTA SEMANA" en gris, "3 / 5 sesiones" en blanco bold, barra de progreso verde neón.
- Derecha: "ÚLTIMO PR" en gris, "Sentadilla" en blanco, "100 kg" en verde neón bold.

Desktop: contenido centrado, ancho máximo 700px.

---

## 📱 PROMPT 3 — ENTRENAMIENTO DEL DÍA

> Pantalla de sesión activa. El usuario la usa mientras entrena, ejercicio por ejercicio.

Mantén el estilo visual ya establecido.

Diseña la pantalla "Hoy" de GymTracker. Header con logo. Título "Día 12 — Pecho y Tríceps" bold grande. Subtítulo "2 / 6 ejercicios completados" en gris. Separador horizontal verde neón.

Lista de ejercicios en tarjetas. Cada tarjeta tiene:
- Nombre del ejercicio bold (tachado si está completado)
- Campo editable de peso en kg destacado — el usuario puede modificarlo durante el entrenamiento
- Detalle: "4 series × 10 reps"
- Chip de descanso: "90 seg"
- Chip de foco muscular: "Pecho" o "Tríceps"
- Botón circular a la derecha: vacío si pendiente, verde neón con check si completado
- Ejercicio activo: borde izquierdo verde neón
- Ejercicio completado: nombre tachado, check verde

Ejercicios de ejemplo:
1. Press de banca — 60 kg — 4×10 — 90 seg — Pecho (completado)
2. Fondos en paralelas — Peso corporal — 3×12 — 60 seg — Pecho (completado)
3. Extensión de tríceps en polea — 20 kg — 3×15 — 60 seg — Tríceps (activo)
4. Press inclinado con mancuernas — 25 kg — 4×8 — 90 seg — Pecho (pendiente)

Al fondo: campo de texto "Notas de la sesión..." y botón "FINALIZAR ENTRENAMIENTO" ancho completo.

Desktop: columna central 750px máximo.

---

## 📱 PROMPT 4 — HISTORIAL DE SESIONES

> Lista de entrenamientos pasados con acceso a detalle editable.

Mantén el estilo visual ya establecido.

Diseña la pantalla "Historial" de GymTracker con dos sub-vistas accesibles por un toggle en la parte superior: "Sesiones" y "Progreso". El toggle activo en verde neón.

SUB-VISTA SESIONES:
Título "Historial" bold. Subtítulo "28 sesiones registradas" en gris. Ícono de filtro a la derecha.

Tarjetas de sesión, una por entrenamiento, de más reciente a más antigua:
- Borde izquierdo verde neón si completada al 100%, gris si parcial
- Fecha en gris mayúscula + duración con ícono de reloj a la derecha
- Nombre de la sesión bold
- Ejercicios completados con ícono de check verde (completo) o emoji neutro (parcial)
- Flecha "›" para ver y editar el detalle

Ejemplo de sesiones:
1. LUN 23 JUN — 52 min — Día 11 Espalda y Bíceps — 6/6 ✓ (verde)
2. SÁB 21 JUN — 35 min — Día 10 Pecho y Tríceps — 4/6 (gris)
3. JUE 19 JUN — 65 min — Día 09 Pierna y Core — 8/8 ✓ (verde)

DETALLE DE SESIÓN (pantalla al hacer clic en una sesión):
Lista de todos los ejercicios de esa sesión. Cada ejercicio muestra campos editables de peso y reps, y un campo de notas al fondo. Botón "GUARDAR CAMBIOS" al fondo.

Desktop: lista a la izquierda, detalle editable en panel derecho al hacer clic.

---

## 📱 PROMPT 5 — PROGRESO POR EJERCICIO

> Sub-vista de Historial. Evolución visual del peso levantado en el tiempo.

Mantén el estilo visual ya establecido.

Diseña la sub-vista "Progreso" dentro de la pantalla Historial. Toggle "Sesiones / Progreso" en la parte superior con "Progreso" activo en verde neón.

Selector de ejercicio: chips horizontales desplazables. Chip activo fondo verde neón, texto negro bold. Chips inactivos fondo oscuro borde sutil. Ejemplos: "PRESS BANCA" (activo), "SENTADILLA", "PESO MUERTO", "DOMINADAS".

Tarjeta de progreso:
- Título "Progreso — Press de banca" bold
- "Empezaste con 60 kg · Ahora levantas 80 kg" en gris
- Badge "+33%" en verde neón
- Gráfica de línea verde neón sobre fondo oscuro, con puntos circulares en cada valor. Eje X: últimas 8 semanas. Líneas de guía horizontales en gris muy sutil.

Sección "ÚLTIMOS 5 REGISTROS":
Filas separadas por línea sutil — punto de color (verde el más reciente, gris los anteriores), fecha, peso bold, reps en gris.

Datos de ejemplo: HOY 80kg×4, 18 OCT 77.5kg×5, 11 OCT 75kg×5, 04 OCT 75kg×4, 27 SEP 72.5kg×6.

Desktop: gráfica más alta (350px), chips sin scroll horizontal.

---

## 📱 PROMPT 6 — RUTINAS

> Biblioteca de rutinas disponibles para activar o explorar.

Mantén el estilo visual ya establecido.

Diseña la pantalla "Rutinas" de GymTracker. Header con logo. Título "Rutinas" bold. Botón "↓ IMPORTAR" alineado a la derecha, fondo oscuro con borde.

Tarjeta de rutina ACTIVA:
- Nombre "Arnold Split" bold + chip "ACTIVA" verde neón
- "6 días/semana · Intermedio" en gris
- Barra de progreso verde neón con "Día 12 de 30" a la derecha
- Botón "CONTINUAR DÍA 12 →" ancho completo

Tres tarjetas DISPONIBLES:
- "Push Pull Legs (PPL)" — chip "DISPONIBLE" gris — "6 días/semana · Intermedio"
- "Full Body 3 días" — chip "DISPONIBLE" gris — "3 días/semana · Principiante"
- "Upper/Lower" — chip "DISPONIBLE" gris — "4 días/semana · Intermedio"

Tarjeta especial al fondo con borde sutil verde oscuro:
- Título "¿Quieres una rutina personalizada?" en verde neón centrado
- Texto explicativo en gris centrado
- Botón "📋 COPIAR PROMPT" con borde verde neón

Desktop: columna central 750px. Al clic en rutina disponible, detalle en panel lateral derecho.

---

## 📱 PROMPT 7 — IMPORTAR RUTINA

> Pantalla independiente para pegar y previsualizar una rutina en formato Markdown.

Mantén el estilo visual ya establecido.

Diseña la pantalla "Importar Rutina" de GymTracker, accesible desde el botón "IMPORTAR" en Rutinas. Mostrar botón "← Volver" en la parte superior izquierda para regresar a Rutinas.

Título "Importar Rutina" bold. Subtítulo en gris: "Pega el contenido Markdown de tu rutina generada con IA".

Área de texto grande (mínimo 200px de alto) con fondo #1A1A1A, borde sutil, placeholder con el formato de ejemplo:
```
## Día 1 — Pecho y Tríceps
- Press de banca | 4×10 | 60 kg | Descanso: 90 seg | Foco: Pecho
- Fondos en paralelas | 3×12 | Peso corporal | Descanso: 60 seg | Foco: Tríceps
```

Botón "PREVISUALIZAR" en verde neón ancho completo debajo del área de texto.

Sección de previsualización debajo (aparece después de previsualizar): tarjetas compactas por cada día de la rutina con el nombre del día y la lista de ejercicios. Encabezado "VISTA PREVIA — 30 días detectados" en gris.

Al fondo: campo de texto para el nombre de la rutina con label "Nombre de la rutina" y botón "AGREGAR A MIS RUTINAS" ancho completo.

Desktop: columna central 750px. Área de texto y previsualización lado a lado en dos columnas.

---

## 💡 Instrucciones de uso

1. Pega el Prompt 0 en Stitch — establece el estilo global
2. Valida que el estilo sea correcto antes de continuar
3. Pega cada prompt de pantalla en orden, uno a la vez
4. Si algo no convence, describe qué elemento cambiar antes de seguir
5. Cuando todas las pantallas estén aprobadas, toma capturas y úsalas en los prompts de Horizons
