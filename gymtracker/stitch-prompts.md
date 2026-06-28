# GymTracker — Prompts para Google Stitch

> Pega el Prompt 0 primero. Luego cada pantalla en orden, una a la vez.

---

## 🎨 PROMPT 0 — ESTILO GLOBAL

Diseña el sistema visual para una app de seguimiento de entrenamientos llamada GymTracker. Plataforma móvil, orientación portrait.

Estilo: oscuro, intenso y enfocado. El usuario está en el gym, sudando. El diseño debe transmitir energía y motivación sin distracciones.

Paleta de colores: fondo principal #0D0D0D, fondo de tarjetas #1A1A1A, acento principal verde neón #AAFF00, acento secundario gris medio #3A3A3A, texto principal blanco #FFFFFF, texto secundario gris claro #888888.

Tipografía: sans-serif geométrica y bold para títulos (Inter o equivalente), regular para cuerpo. Tamaños grandes, fáciles de leer con las manos ocupadas.

Densidad visual equilibrada: información suficiente por pantalla sin saturar. Botones y áreas de toque generosas.

Elementos decorativos: íconos lineales simples, gradientes sutiles de color en elementos de acento, sin ilustraciones ni fotografías.

Navegación inferior con 4 tabs: Dashboard, Hoy, Historial, Rutinas.

No usar: colores brillantes en fondos, sombras muy marcadas, tipografía serif, elementos decorativos complejos.

---

## 📱 PROMPT 1 — DASHBOARD

> Pantalla de inicio. Le da al usuario un vistazo rápido de su estado y motivación antes de entrenar.

Mantén el estilo visual ya establecido.

Diseña la pantalla de Dashboard para GymTracker. Lo primero que el usuario debe ver al entrar es su racha actual de días consecutivos entrenando, mostrada de forma prominente en la parte superior con un número grande y un texto como "días seguidos".

Debajo, una tarjeta de "Entrenamiento de hoy" que muestra el nombre del día de rutina (ejemplo: "Día 12 — Pecho y Tríceps") con los primeros 3 ejercicios listados como preview (nombre del ejercicio + series x reps), y un botón primario con texto "Empezar entrenamiento" en verde neón que ocupa todo el ancho.

Debajo de esa tarjeta, una fila de dos tarjetas pequeñas lado a lado: la izquierda muestra "Esta semana" con el conteo "3 / 5 sesiones" y una barra de progreso horizontal; la derecha muestra "Último PR" con un ejercicio de ejemplo "Sentadilla — 100 kg".

Navegación inferior visible con el tab "Dashboard" activo.

---

## 📱 PROMPT 2 — ENTRENAMIENTO DEL DÍA

> Pantalla de sesión activa. El usuario la usa mientras entrena, ejercicio por ejercicio.

Mantén el estilo visual ya establecido.

Diseña la pantalla de Entrenamiento del día para GymTracker. En la parte superior, un encabezado con el nombre de la rutina del día (ejemplo: "Día 12 — Pecho y Tríceps") y el conteo de ejercicios completados (ejemplo: "2 / 6 ejercicios").

El cuerpo de la pantalla muestra una lista vertical de ejercicios. Cada ejercicio es una tarjeta con: nombre del ejercicio en texto bold grande, el detalle "4 series × 10 reps — 60 kg", minutaje de descanso como chip pequeño (ejemplo: "⏱ 90 seg descanso"), foco muscular como chip de color (ejemplo: "Pecho"), y un botón circular de check a la derecha para marcarlo como completado. Los ejercicios ya completados se muestran con fondo ligeramente diferente y check en verde neón.

Al fondo de la pantalla, un campo de texto pequeño con placeholder "Notas de la sesión..." y un botón secundario "Finalizar entrenamiento".

Ejemplo de ejercicios en la lista: Press de banca, Fondos en paralelas, Extensión de tríceps en polea, Press inclinado con mancuernas.

---

## 📱 PROMPT 3 — HISTORIAL

> Lista de todas las sesiones pasadas. El usuario revisa qué hizo y cuándo.

Mantén el estilo visual ya establecido.

Diseña la pantalla de Historial para GymTracker. Encabezado simple con el título "Historial" y un total de sesiones (ejemplo: "28 sesiones registradas").

El cuerpo es una lista vertical de tarjetas, una por sesión pasada, ordenadas de la más reciente a la más antigua. Cada tarjeta muestra: fecha en texto pequeño (ejemplo: "Lunes 23 Jun"), nombre de la rutina en bold (ejemplo: "Día 11 — Espalda y Bíceps"), número de ejercicios completados (ejemplo: "6 / 6 ejercicios ✓"), duración de la sesión (ejemplo: "52 min"), y una flecha hacia la derecha para ver el detalle.

Las sesiones completadas al 100% tienen un indicador verde sutil en el borde izquierdo de la tarjeta. Las sesiones incompletas tienen indicador gris.

Ejemplo de sesiones en la lista: 3 entradas visibles, fechas de la semana actual.

---

## 📱 PROMPT 4 — PROGRESO

> Gráficas de evolución de pesos por ejercicio. La pantalla más motivadora de la app.

Mantén el estilo visual ya establecido.

Diseña la pantalla de Progreso para GymTracker. En la parte superior, un selector horizontal tipo chips para elegir el ejercicio a visualizar. Ejemplos de chips: "Press banca", "Sentadilla", "Peso muerto", "Dominadas". El chip activo se muestra en verde neón.

Debajo del selector, una gráfica de línea que muestra la evolución del peso máximo levantado en ese ejercicio a lo largo del tiempo. Eje X: fechas de las últimas 8 semanas. Eje Y: peso en kg. La línea es de color verde neón sobre fondo oscuro. Encima de la gráfica, el título "Progreso — Press de banca" y debajo un resumen de texto: "Empezaste con 60 kg · Ahora levantas 80 kg · +33%".

Debajo de la gráfica, una lista compacta de los últimos 5 registros de ese ejercicio: fecha + peso + reps, en formato lista simple.

---

## 📱 PROMPT 5 — RUTINAS

> Biblioteca de rutinas disponibles y herramienta para importar una nueva.

Mantén el estilo visual ya establecido.

Diseña la pantalla de Rutinas para GymTracker. Encabezado con el título "Rutinas" y un botón secundario pequeño "+ Importar" alineado a la derecha.

El cuerpo muestra las rutinas disponibles en tarjetas verticales. Cada tarjeta tiene: nombre de la rutina en bold (ejemplo: "Rutina Full Body 30 días"), descripción corta en texto secundario (ejemplo: "30 días · 5 días por semana · Intermedio"), barra de progreso horizontal si el usuario la tiene activa (ejemplo: "Día 12 de 30"), y un chip de estado: "Activa" en verde neón o "Disponible" en gris.

Ejemplo de rutinas: "Rutina Full Body 30 días" marcada como activa con progreso, "Rutina Upper/Lower" disponible, "Rutina Fuerza 5×5" disponible.

Al final de la lista, una tarjeta especial con fondo ligeramente diferente titulada "¿Quieres una rutina personalizada?" con texto "Usa este prompt con ChatGPT o Claude para generar tu rutina en el formato correcto" y un botón "Copiar prompt".

---

## 💡 Instrucciones de uso

1. Abre Google Stitch y crea un nuevo proyecto llamado "GymTracker"
2. Pega el **Prompt 0** y genera — establece la identidad visual completa
3. Si el estilo no es lo que esperabas, ajústalo antes de continuar
4. Luego pega cada prompt de pantalla en orden, uno a la vez
5. Si algún resultado no convence, describe qué elemento cambiar y genera un prompt de corrección
