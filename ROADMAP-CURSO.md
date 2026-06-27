# Roadmap del Curso — Hostinger Horizons

Curso completo para aprender a construir proyectos web reales con Hostinger Horizons (IA, sin código). Cada módulo produce un proyecto funcional y publicado. Los módulos están ordenados por complejidad creciente y cada uno introduce un concepto nuevo.

---

## Estructura del curso

| # | Módulo | Proyecto | Concepto clave |
|---|--------|----------|----------------|
| 0 | **Block Drop Game** *(ya grabado)* | Juego arcade de bloques | Generar una app completa con prompts e iterar en secciones |
| 1 | **Landing Personal + Diseño con IA** | Portfolio / landing personal | Flujo Stitch → Horizons: diseñar antes de construir |
| 2 | **Landing con Reservas (Barbería)** | Web con sistema de citas | Formularios, captura de datos y confirmaciones |
| 3 | **Tracker de Ejercicios** | App de seguimiento fitness | Estado persistente, CRUD y visualización de datos |
| 4 | **Punto de Venta para Cafés (POS)** | App de caja / menú digital | Catálogo, carrito y flujo de cobro |
| 5 | **Vender Suscripciones** | Página de membresía con área privada | Pagos recurrentes, acceso exclusivo y gestión de usuarios |
| 6 | **Chatbot con IA** | Asistente conversacional embebido | IA integrada, system prompt y base de conocimiento |
| 7 | **Creador de Imágenes con IA** | Generador visual con galería | Generación de imágenes con IA y gestión de resultados |
| 8 | **IA Integrada a Fondo** *(cierre)* | Mini-proyecto libre | Casos de uso avanzados de IA y prompting profesional |

---

## Módulo 0 — Block Drop Game *(ya está)*

**Concepto:** Generar una app completa con prompts e iterar en secciones.
**Deck:** `leccion-01-block-drop.html`

| Sección | Qué se hace |
|---------|-------------|
| 1 — Crear la base | Tablero 10×20, 7 piezas clásicas, controles de teclado, pantalla de Game Over |
| 2 — Corregir la lógica | Colisiones con paredes y piezas, rotación sin errores, fijar piezas |
| 3 — Sistema de puntaje | Eliminar líneas, score en pantalla, contador de líneas |
| 4 — Pulir la experiencia | Diseño arcade oscuro, responsive, controles táctiles para móvil |

---

## Módulo 1 — Landing Page Personal + Diseño con IA (Google Stitch)

**Concepto:** Introducir el flujo de diseñar con IA *antes* de construir. Google Stitch se usa en la Sección 1 para definir estructura y estilo visual; luego se ejecuta en Horizons.

**Por qué Google Stitch en M1:** Es el módulo más sencillo a nivel técnico, ideal para que el alumno entienda el flujo "diseño → construcción" desde el inicio del curso.

| Sección | Qué se hace | Prompt de ejemplo |
|---------|-------------|-------------------|
| 1 — Diseñar con Google Stitch | Generar el wireframe/mockup de la landing: hero, "sobre mí", proyectos y contacto | *"Diseña una landing page personal para un diseñador freelance. Secciones: hero con nombre y título, sobre mí con foto y bio, proyectos con grid de cards, y formulario de contacto. Estilo: moderno, oscuro, colores violeta."* |
| 2 — Construir la base en Horizons | Tomar el mockup de Stitch como referencia y construir las 4 secciones en Horizons con prompts | *"Crea una landing page personal con hero de pantalla completa, sección de proyectos en grid de 3 columnas y formulario de contacto. Diseño oscuro con acentos en violeta."* |
| 3 — Contenido y estilo | Personalizar copy, fotos, paleta de colores y tipografía para que coincida con el mockup de Stitch | *"Cambia los colores a #673DE6 como acento, actualiza el copy del hero a: 'Hola, soy [nombre] — construyo experiencias digitales', y sube esta foto de perfil."* |
| 4 — Pulir y publicar | Revisar responsive, agregar animaciones de entrada, SEO básico (meta title/description), conectar dominio | *"Asegúrate de que la sección de proyectos se vea bien en móvil: una sola columna, con cards más anchas. Agrega un efecto fade-in al hero al cargar la página."* |

---

## Módulo 2 — Landing con Reservas (Barbería)

**Concepto:** Formularios, captura de datos de citas y confirmaciones automáticas.

| Sección | Qué se hace | Prompt de ejemplo |
|---------|-------------|-------------------|
| 1 — La base | Hero, servicios con precios, galería de trabajos, sección de ubicación | *"Crea una web para una barbería llamada 'Sharp Cuts'. Incluye: hero con foto de fondo y botón 'Reservar ahora', sección de servicios con precios (Corte $15, Barba $10, Combo $22), y galería de 6 fotos."* |
| 2 — Sistema de reservas | Formulario de cita: nombre, teléfono, servicio, fecha y hora | *"Agrega un formulario de reserva con campos: nombre completo, número de teléfono, servicio (select con opciones), fecha (date picker) y hora (selector de slots de 30 minutos entre 9am y 7pm)."* |
| 3 — Gestión y confirmación | Guardar la reserva, enviar confirmación por email, mostrar mensaje de éxito | *"Cuando el formulario se envíe exitosamente, muestra un mensaje de confirmación con los datos de la reserva y envía un email de confirmación al cliente con el asunto 'Tu cita está confirmada - Sharp Cuts'."* |
| 4 — Pulir UX y publicar | Botón de WhatsApp flotante, mapa de Google Maps, responsive, publicar | *"Agrega un botón flotante de WhatsApp en la esquina inferior derecha que abra el chat con el número +1-555-0123 y el mensaje 'Hola, quiero hacer una reserva'. Incrusta un mapa de Google Maps con la dirección de la barbería."* |

---

## Módulo 3 — Tracker de Ejercicios

**Concepto:** App con estado persistente, operaciones CRUD y visualización de progreso (dashboard).

| Sección | Qué se hace | Prompt de ejemplo |
|---------|-------------|-------------------|
| 1 — La base | Interfaz para registrar un ejercicio: nombre, series, repeticiones y peso | *"Crea una app de seguimiento de ejercicios. Pantalla principal con: formulario para agregar ejercicio (nombre, series, reps, peso en kg), y una lista de los ejercicios del día de hoy con sus datos."* |
| 2 — Lógica de datos | Guardar, editar y borrar registros; historial por fecha | *"Agrega la funcionalidad para editar y eliminar cada ejercicio de la lista. Agrega también un historial que muestre los entrenamientos de los últimos 7 días, agrupados por fecha."* |
| 3 — Progreso y estadísticas | Gráfica de progreso por ejercicio, racha de días activos, metas semanales | *"Agrega una sección 'Progreso' con: una gráfica de línea que muestre la evolución del peso levantado para el ejercicio seleccionado en el último mes, y un contador de racha de días consecutivos entrenados."* |
| 4 — Pulir UX y publicar | Modo oscuro/claro, notificaciones de meta alcanzada, responsive, publicar | *"Agrega un toggle de modo oscuro/claro en la esquina superior derecha. Cuando el usuario complete su meta semanal de entrenamientos, muestra una animación de celebración con confeti y el mensaje '¡Meta alcanzada esta semana!'."* |

---

## Módulo 4 — Punto de Venta para Cafés (POS)

**Concepto:** Catálogo de productos, carrito de compras y flujo de cobro.

| Sección | Qué se hace | Prompt de ejemplo |
|---------|-------------|-------------------|
| 1 — La base: catálogo/menú | Grid de productos con foto, nombre, descripción y precio | *"Crea un punto de venta para una cafetería llamada 'La Taza'. Pantalla principal con grid de productos del menú: café americano $2.50, cappuccino $3.50, croissant $2.00, etc. Cada producto con foto, nombre y precio, y un botón '+ Agregar'."* |
| 2 — Carrito y orden | Agregar al carrito, modificar cantidad, calcular subtotal y total | *"Agrega un panel lateral de carrito que aparezca al agregar productos. Muestra los ítems agregados con su cantidad (botones + y −), subtotal por ítem y total general. Botón 'Proceder al cobro' al final."* |
| 3 — Cobro y ticket | Selección de método de pago, generar ticket con detalle de la orden | *"En la pantalla de cobro: muestra los métodos de pago (efectivo, tarjeta, QR). Al completar el cobro, genera un ticket con: número de orden, lista de productos, total, método de pago, fecha y hora."* |
| 4 — Pulir: resumen del día y layout tablet | Dashboard de ventas del día, historial de órdenes, optimizar para pantalla de tablet | *"Agrega una pantalla 'Cierre del día' que muestre: total de ventas del día, número de órdenes, producto más vendido y un botón para exportar el reporte en CSV. Asegúrate de que la interfaz se vea bien en una tablet de 10 pulgadas en landscape."* |

---

## Módulo 5 — Vender Suscripciones

**Concepto:** Pagos recurrentes, área de contenido exclusivo para miembros y gestión de acceso.

| Sección | Qué se hace | Prompt de ejemplo |
|---------|-------------|-------------------|
| 1 — La base: página de planes | Landing con propuesta de valor, tabla comparativa de planes y precios | *"Crea una página de membresía para un newsletter de inversiones llamado 'Mercado Inteligente'. Incluye: hero con propuesta de valor, sección de planes (Básico $9/mes: 1 análisis semanal; Pro $29/mes: análisis diarios + alertas; Elite $99/mes: todo + consultas 1:1) con tabla comparativa."* |
| 2 — Integración de pagos | Conectar pasarela de pago para cobro mensual/anual | *"Integra Stripe para procesar los pagos de suscripción. El plan Básico cobra $9/mes o $90/año (2 meses gratis). Al hacer clic en 'Suscribirse', lleva al formulario de pago de Stripe."* |
| 3 — Área de miembros | Registro/login, contenido exclusivo protegido por plan activo | *"Crea un área privada '/dashboard' que solo sea accesible para suscriptores activos. Muestra los artículos y análisis según el plan del usuario. Si el plan está vencido, muestra un banner para renovar."* |
| 4 — Pulir: emails y gestión | Email de bienvenida, recordatorio de renovación, cancelación de suscripción | *"Configura los emails automáticos: bienvenida al suscribirse (con enlace al dashboard), recordatorio 3 días antes del cobro, y confirmación de cancelación. Agrega en el dashboard un botón 'Cancelar suscripción' con modal de confirmación."* |

---

## Módulo 6 — Chatbot con IA

**Concepto:** Integrar un asistente conversacional con IA, personalizarlo con un system prompt y darle contexto de negocio.

| Sección | Qué se hace | Prompt de ejemplo |
|---------|-------------|-------------------|
| 1 — La base: interfaz de chat | Widget de chat con burbuja flotante, historial de mensajes, input de texto | *"Crea un chatbot para un e-commerce de ropa llamado 'Stilo'. Agrega una burbuja de chat flotante en la esquina inferior derecha. Al abrirla, muestra la interfaz de conversación con el mensaje inicial: '¡Hola! Soy Stilo, tu asistente de moda. ¿En qué te puedo ayudar hoy?'"* |
| 2 — Conectar la IA | Configurar el system prompt con rol, tono y reglas; conectar al modelo de IA de Horizons | *"Configura el chatbot para que responda como un asesor de moda amigable y profesional. Solo debe responder preguntas relacionadas con ropa, tallas, disponibilidad y envíos de Stilo. Si le preguntan algo fuera del tema, debe responder: 'Para ese tema, te sugiero contactar a nuestro equipo en soporte@stilo.com'."* |
| 3 — Contexto y personalidad | Cargar el catálogo de productos y política de envíos como base de conocimiento | *"Entrena al chatbot con esta información: [lista de productos con precios y tallas disponibles], política de envíos (gratis en compras +$50, 3-5 días hábiles), y política de devoluciones (30 días con recibo). El chatbot debe usar esta información para responder con precisión."* |
| 4 — Pulir: historial, embedding y responsive | Guardar el historial de la conversación, poder embeber el widget en cualquier página, responsive | *"Guarda el historial del chat en localStorage para que si el usuario cierra y vuelve a abrir el widget, vea los mensajes anteriores. Genera el código para embeber el chatbot en cualquier sitio web con una sola línea de JavaScript."* |

---

## Módulo 7 — Creador de Imágenes con IA

**Concepto:** Generación de imágenes con IA, manejo de la galería de resultados y opciones de personalización.

| Sección | Qué se hace | Prompt de ejemplo |
|---------|-------------|-------------------|
| 1 — La base: interfaz de generación | Campo de prompt, botón "Generar", área de previsualización, galería de resultados | *"Crea una app llamada 'Pixelia — Generador de Imágenes con IA'. Pantalla principal con: campo de texto grande para el prompt, botón 'Generar imagen', área de previsualización de la imagen generada, y galería de las últimas imágenes creadas en grid de 3 columnas."* |
| 2 — Integrar el modelo de IA | Conectar el modelo de generación de imágenes de Horizons, manejar el estado de carga | *"Conecta el modelo de generación de imágenes de Horizons. Mientras genera, muestra un skeleton/loading animado en el área de previsualización con el texto 'Creando tu imagen...'. Si hay un error, muestra un mensaje en rojo."* |
| 3 — Opciones y estilos | Selector de estilo artístico (foto, ilustración, pixel art, etc.), selector de proporción (1:1, 16:9, 9:16) | *"Agrega opciones antes del botón Generar: un selector de estilo con opciones (Fotografía realista, Ilustración, Acuarela, Pixel Art, Minimalista) y un selector de proporción (Cuadrado 1:1, Paisaje 16:9, Retrato 9:16). Incluye estas opciones en el prompt enviado al modelo."* |
| 4 — Galería persistente y descarga | Guardar imágenes en la galería, botón de descarga, eliminar de la galería | *"Guarda cada imagen generada en la galería de forma persistente. Cada card de la galería debe tener: la imagen, el prompt usado (truncado), un botón de descarga y un botón de eliminar con ícono de basura. La galería debe persistir entre sesiones del usuario."* |

---

## Módulo 8 — IA Integrada a Fondo *(cierre del curso)*

**Concepto:** Módulo teórico-práctico de cierre. Profundizar en las capacidades de IA de Horizons, técnicas avanzadas de prompting y cómo seguir aprendiendo.

| Sección | Qué se hace | Prompt de ejemplo |
|---------|-------------|-------------------|
| 1 — ¿Qué puede hacer la IA en Horizons? | Recorrido completo de capacidades: texto, imagen, chat, automatización, base de datos | *Prompts cortos para demostrar cada capacidad en vivo* |
| 2 — Casos de uso avanzados | Combinar módulos: chatbot + reservas, generador + e-commerce, tracker + notificaciones | *"Toma el chatbot del M6 y conéctalo al sistema de reservas del M2 para que el chatbot pueda hacer reservas directamente desde la conversación."* |
| 3 — Prompting profesional | Técnicas: ser específico, dar contexto, iterar, usar restricciones, encadenar prompts | Comparar 3 versiones de un mismo prompt (malo → bueno → excelente) en vivo |
| 4 — Próximos pasos | Recursos, comunidad, cómo seguir construyendo proyectos propios, CTA de Hostinger | *Proyecto libre: "Elige uno de tus proyectos personales y construye la primera versión hoy."* |

---

## Notas de producción

- **Duración objetivo por sección:** 5-8 minutos.
- **Formato de archivos:** cada módulo tiene su propio deck `leccion-0X-nombre.html` con 7 slides (portada → proyecto → 4 secciones → cierre), siguiendo el mismo patrón que `leccion-01-block-drop.html`.
- **Google Stitch:** se introduce en M1, Sección 1. No necesita módulo propio; queda integrado como herramienta de la etapa de diseño.
- **Orden de grabación sugerido:** M1 → M2 → M3 → M4 → M5 → M6 → M7 → M8. El M0 (Block Drop) ya está listo.
