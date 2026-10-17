# CodeQuest: Aprende Programando — Landing Page Oficial

Sitio web promocional y plataforma de captura para el proyecto educativo **CodeQuest: Aprende Programando**, desarrollado para la Fundación Escuela Tecnológica de Neiva "Jesús Oviedo Pérez" (FET).

## 🚀 Repositorio y Despliegue
* **Sitio Web Publicado:** https://chopinnate12.github.io/codequest-landing/
* **Repositorio GitHub:** https://github.com/chopinnate12/codequest-landing

---

## 📝 Bitácora de Prompts e Iteraciones con IA

| PROMPT # | PROBLEMA / OBJETIVO BUSCADO | PROMPT DE AJUSTE ENVIADO A LA IA | RESULTADO OBTENIDO | ¿FUNCIONÓ? |
| :---: | :--- | :--- | :--- | :---: |
| **1** | El menú hamburguesa en dispositivos móviles no se cerraba al hacer clic en un enlace de navegación. | *"El menú móvil se queda abierto cuando presiono un enlace interno. Modifica el JavaScript para que oculte la lista y cambie el atributo aria-expanded al hacer clic en cualquier enlace con clase .mobile-nav-link."* | Se agregó un listener `forEach` que oculta el menú móvil automáticamente tras la selección. | **SÍ** |
| **2** | La personalización de fuentes no cargaba 'Press Start 2P' en Tailwind CSS 4. | *"La tipografía retro no se refleja en los títulos. Configura correctamente la directiva @theme dentro del estilo CSS para Tailwind v4 incluyendo la fuente gamer."* | Se añadió `--font-gamer: 'Press Start 2P', monospace;` dentro de `@theme` haciendo funcionar la clase `font-gamer`. | **SÍ** |
| **3** | El formulario permitía enviar espacios en blanco y no mostraba bordes rojos de error. | *"Modifica la función de envío del formulario para que aplique la clase border-rose-500 a los inputs inválidos y elimine espacios vacíos con .trim()."* | Se integró la validación estricta resaltando visualmente los campos con error en rojo. | **SÍ** |
| **4** | Las tarjetas de los niveles perdían alineación en pantallas medianas (tablets). | *"Haz que el grid de la sección de niveles use grid-cols-1 en celular, grid-cols-2 en tablet (md) y grid-cols-3 en computador (lg) con flex-col para igualar alturas."* | El layout de las tarjetas se adaptó fluidamente en todos los breakpoints. | **SÍ** |
| **5** | El Toast de confirmación aparecía estático en la pantalla desde el inicio. | *"El Toast debe permanecer oculto por defecto con la clase hidden y solo aparecer con animación cuando la validación del formulario sea exitosa, ocultándose tras 4 segundos."* | Se configuró el `setTimeout` a 4000ms gestionando la clase `hidden`. | **SÍ** |

---

## 🛠️ Personalización Manual Realizada a Mano (Sin IA)

1. **Modificación del Estilo del Toast (Cambio 1):** Se agregó manualmente la clase `animate-bounce` de Tailwind al elemento `#toast-success` e ícono emoji `🎉` para darle mayor dinamismo visual al confirmarse el formulario.
2. **Adición de Sección 'Sobre el Equipo FET' (Cambio 2):** Se maquetó directamente a mano una grilla de dos columnas dentro de la sección `#nosotros` para destacar a Valerie Trujillo (Scrum Master), Juan Sebastián Aranda (Product Owner) y Juan José Ramos (Docente Evaluador).
3. **Optimización de Accesibilidad y Foco (Cambio 3):** Se insertaron a mano los atributos `aria-expanded` y `aria-label` en los botones del menú y del acordeón, asegurando que el estado sea interpretado por lectores de pantalla y añadiendo el estilo `focus:ring-2 focus:ring-emerald-500`.