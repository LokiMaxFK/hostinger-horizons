# Módulo 1 — Landing Page Personal + Diseño con IA

**Proyecto:** Portfolio / landing personal publicada con dominio propio  
**Herramientas:** Google Stitch + Hostinger Horizons  
**Duración estimada:** 4 videos · ~6–8 min cada uno  
**Prerequisito:** Haber visto el M0 (Block Drop) o tener cuenta activa en Horizons

---

## ¿Qué vamos a construir?

Una landing page personal completa con 4 secciones:
- **Hero** — nombre, título profesional y botón de contacto
- **Sobre mí** — foto, bio corta y habilidades
- **Proyectos / Servicios** — grid de cards con lo que haces u ofreces
- **Contacto** — formulario simple o links directos

Al terminar el módulo tendrás una web publicada, con dominio, que puedes mostrarle a cualquier persona.

---

## Lo nuevo de este módulo

| Concepto | ¿Qué es? |
|----------|----------|
| **Google Stitch** | Herramienta de diseño con IA: describes lo que quieres y genera un wireframe o mockup visual antes de construir |
| **Flujo diseño → construcción** | Diseñar primero en Stitch, luego ejecutar en Horizons usando el mockup como referencia |
| **Publicar con dominio** | Conectar un dominio personalizado a tu web en Horizons |

---

## Sección 1 — Diseñar con Google Stitch

**Objetivo:** Tener un wireframe/mockup visual listo antes de abrir Horizons.  
**Por qué primero Stitch:** Ir directo a Horizons sin un plan visual hace que iteres más y el resultado final sea menos coherente. Stitch te da una "foto del destino" en minutos.

### Puntos a cubrir

1. **¿Qué es Google Stitch?**
   - Herramienta de diseño generativo de Google (Labs)
   - Describe en lenguaje natural lo que quieres → genera un mockup
   - No es para construir, es para diseñar y planear

2. **Acceder a Stitch**
   - Entrar a labs.google/stitch
   - Iniciar sesión con cuenta de Google

3. **El prompt de diseño**
   - Ser específico: describir las secciones, el tono y el estilo
   - Ejemplo de prompt:
     ```
     Diseña una landing page personal para un diseñador UX freelance.
     Secciones: hero con nombre y título profesional, sobre mí con foto y
     descripción corta, proyectos en grid de 3 columnas, y contacto.
     Estilo: moderno, oscuro, tipografía limpia, acentos en violeta.
     ```

4. **Leer el resultado de Stitch**
   - Analizar la estructura que generó: ¿tiene las secciones que queremos?
   - Anotar: colores, tipografía, distribución del espacio
   - Ajustar el prompt si algo no quedó bien (iterar 1-2 veces)

5. **Guardar la referencia**
   - Screenshot del mockup o exportar desde Stitch
   - Este archivo es la "guía visual" que usaremos en la Sección 2

---

## Sección 2 — Construir la base en Horizons

**Objetivo:** Tener las 4 secciones de la landing construidas y funcionales en Horizons.  
**Referencia activa:** El mockup de Stitch debe estar visible mientras escribimos los prompts.

### Puntos a cubrir

1. **Abrir Horizons y crear un proyecto nuevo**
   - Ir a horizons.hostinger.com
   - Clic en "Nuevo proyecto"
   - Nombrar el proyecto (ej. "Mi Landing Personal")

2. **El prompt inicial — construir todo de una vez**
   - La estrategia: un prompt completo que describa todas las secciones
   - Mencionar el estilo del mockup de Stitch como referencia
   - Ejemplo de prompt:
     ```
     Crea una landing page personal con 4 secciones:
     1. Hero: fondo oscuro, nombre grande, título "Diseñador UX Freelance",
        subtítulo con propuesta de valor y botón "Contáctame".
     2. Sobre mí: foto circular a la izquierda, bio de 2 párrafos a la derecha,
        3 skills con iconos debajo.
     3. Proyectos: grid de 3 columnas con cards (imagen, título, descripción corta
        y link "Ver proyecto").
     4. Contacto: email clickable, links a LinkedIn y GitHub, y formulario simple
        (nombre, email, mensaje, botón enviar).
     Diseño oscuro (#0D0118 de fondo), tipografía Inter, acentos en violeta (#673DE6).
     ```

3. **Revisar lo que generó Horizons**
   - Comparar con el mockup de Stitch: ¿las secciones coinciden?
   - Identificar qué ajustar en las siguientes secciones

4. **Corregir estructura si algo falta**
   - Si faltó una sección: pedir que la agregue con un prompt específico
   - Ejemplo:
     ```
     Agrega una sección de "Sobre mí" entre el hero y los proyectos.
     Que tenga una foto circular a la izquierda y texto a la derecha.
     ```

---

## Sección 3 — Contenido y estilo

**Objetivo:** Reemplazar todo el contenido de ejemplo por contenido real y personalizado.  
**Principio:** Horizons pone placeholders — en esta sección los hacemos reales.

### Puntos a cubrir

1. **Personalizar el hero**
   - Cambiar nombre, título y subtítulo por los propios
   - Ajustar el CTA ("Contrátame", "Ver mi trabajo", "Hablemos")
   - Ejemplo de prompt:
     ```
     Cambia el hero: nombre "Jordan Martínez", título "Desarrollador Web & Diseñador",
     subtítulo "Construyo interfaces que la gente disfruta usar. Disponible para proyectos freelance."
     Botón: "Ver mi trabajo →"
     ```

2. **Subir foto y personalizar el "Sobre mí"**
   - Subir foto de perfil a Horizons
   - Escribir la bio real (2-3 oraciones directas)
   - Definir 3 habilidades principales con su ícono
   - Ejemplo de prompt:
     ```
     En la sección "Sobre mí": actualiza la bio a "[bio real]".
     Skills: Diseño UI/UX, Desarrollo Frontend, Branding.
     Usa la foto que subí como imagen de perfil.
     ```

3. **Agregar proyectos reales**
   - 3 proyectos con imagen, título y descripción corta
   - Si no tienes proyectos reales: usar proyectos de práctica o conceptuales
   - Ejemplo de prompt:
     ```
     Actualiza los proyectos:
     1. "App de Finanzas" — Rediseño de la experiencia de usuario para una app de ahorro personal. [imagen]
     2. "E-commerce Moda" — Tienda online para una marca local de ropa sustentable. [imagen]
     3. "Dashboard Analytics" — Panel de control de métricas para un SaaS B2B. [imagen]
     ```

4. **Afinar colores y tipografía**
   - Ajustar la paleta para que coincida con el mockup de Stitch
   - Verificar que los acentos de color sean consistentes en toda la página
   - Ejemplo de prompt:
     ```
     Ajusta los colores: fondo principal #0D0118, acentos en #673DE6,
     texto principal blanco, texto secundario rgba(255,255,255,0.65).
     Asegúrate de que los botones usen el color de acento de forma consistente.
     ```

5. **Agregar links reales**
   - LinkedIn, GitHub, email, o las redes que uses
   - Verificar que los links abren en pestaña nueva

---

## Sección 4 — Pulir y publicar

**Objetivo:** Dejar la landing impecable en móvil y desktop, y publicarla con dominio.  
**Resultado final:** URL real que cualquier persona puede abrir.

### Puntos a cubrir

1. **Revisar en móvil**
   - Usar la vista previa responsive de Horizons
   - Problemas comunes: hero muy apretado, grid de 3 cols que no colapsa, foto muy grande
   - Ejemplo de prompt:
     ```
     Revisa que la landing se vea bien en móvil:
     - El hero debe tener el texto más pequeño y el botón centrado
     - Los proyectos deben verse en 1 columna (no 3)
     - La sección "Sobre mí" debe apilarse verticalmente (foto arriba, texto abajo)
     ```

2. **Agregar animaciones de entrada**
   - Fade-in al hero al cargar la página
   - Aparición progresiva de los cards de proyectos al hacer scroll
   - Ejemplo de prompt:
     ```
     Agrega animaciones sutiles:
     - El hero hace fade-in al cargar (0.6s)
     - Las cards de proyectos aparecen con slide-up al entrar en el viewport
     - Los links del nav hacen hover con subrayado animado
     ```

3. **SEO básico**
   - Meta title descriptivo (no "Mi Web")
   - Meta description de 150 caracteres que explique quién eres
   - Ejemplo de prompt:
     ```
     Configura el SEO básico:
     - Title: "Jordan Martínez — Diseñador UX & Desarrollador Web Freelance"
     - Description: "Portfolio de Jordan Martínez. Diseño interfaces y construyo
       webs que combinan buena experiencia de usuario con código limpio. Disponible
       para proyectos freelance."
     ```

4. **Publicar en Horizons**
   - Clic en "Publicar" desde el editor
   - Horizons genera una URL en horizons.site/...
   - Probar la URL antes de conectar el dominio

5. **Conectar dominio personalizado** *(si tienen uno)*
   - Ir a Configuración → Dominio en Horizons
   - Ingresar el dominio comprado en Hostinger
   - Horizons configura el DNS automáticamente
   - Esperar la propagación (puede tomar hasta 24h, suele ser minutos)

6. **Checklist final antes de dar el módulo por terminado**
   - [ ] Las 4 secciones tienen contenido real (no placeholders)
   - [ ] La web se ve bien en móvil y en desktop
   - [ ] Los links de redes sociales funcionan
   - [ ] El formulario de contacto envía correctamente
   - [ ] La URL está activa y carga rápido
   - [ ] El título de la pestaña del navegador es correcto

---

## Prompts completos de referencia

Prompts listos para copiar y pegar durante la grabación:

**Stitch — diseño inicial**
```
Diseña una landing page personal para un profesional creativo freelance.
Secciones: hero con nombre grande y título profesional, sobre mí con foto
circular y bio, proyectos en grid de 3 columnas con cards, y sección de
contacto con formulario y redes sociales. Estilo moderno y oscuro, tipografía
sans-serif limpia, color de acento en violeta.
```

**Horizons — construcción inicial**
```
Crea una landing page personal con fondo oscuro (#0D0118) y acentos en violeta.
Secciones:
1. Hero: nombre en grande, título profesional, frase de propuesta de valor,
   botón "Ver mi trabajo".
2. Sobre mí: foto de perfil circular a la izquierda, bio a la derecha, 3 skills
   con íconos debajo.
3. Proyectos: grid de 3 columnas con cards (imagen, título, descripción, link).
4. Contacto: email, LinkedIn, GitHub y formulario (nombre, email, mensaje).
Usa la fuente Inter. Diseño responsive.
```

**Horizons — corrección responsive**
```
Optimiza para móvil: el hero con texto más pequeño y botón centrado, los
proyectos en 1 columna, el "sobre mí" apilado verticalmente (foto arriba,
texto abajo), y el formulario de contacto a ancho completo.
```

---

## Deck de diapositivas

Archivo: `leccion-02-landing-personal.html` *(por crear)*  
Slides planeados:
1. Portada — "Landing Page Personal"
2. El proyecto — qué vamos a construir y vista del resultado final
3. Sección 1 — Diseñar con Google Stitch
4. Sección 2 — Construir la base en Horizons
5. Sección 3 — Contenido y estilo
6. Sección 4 — Pulir y publicar
7. Cierre — checklist + próximo módulo (Reservas - Barbería)
