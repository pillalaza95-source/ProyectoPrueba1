# Auditoría UX y accesibilidad - ClinicPet

## 1. Objetivo
Revisar si la landing page y el flujo de reserva modal de la clínica veterinaria `ClinicPet` cumplen con los requisitos de accesibilidad, semántica HTML5, validación nativa y buenas prácticas de usabilidad.

## 2. Requisitos revisados

### Requisitos funcionales
- Formulario accesible con validación HTML5 y mejora progresiva mediante JavaScript.
- HTML5 nativo para la validación.
- Uso de todos los tipos de entrada solicitados: `text`, `email`, `password`, `number`, `tel`, `url`, `date`, `time`, `file`, `color`, `range`, `checkbox`, `radio`, `search`, `reset`, `submit`, además de `select`, `textarea`, `datalist` y `output`.
- Labels asociados, `fieldset`, `legend`, y estructura semántica clara.
- Idioma en español, título descriptivo y acceso rápido con skip link.

### Requisitos de accesibilidad
- Foco visible y navegación por teclado.
- Contraste adecuado y diseño responsive.
- Atención a `prefers-reduced-motion`.
- Mensajes de ayuda con `aria-describedby` y mensajes nativos del navegador.
- Campos obligatorios marcados con `*`.

### Requisitos de negocio
- Apariencia moderna, con encabezado, introducción, servicios, CTA de reserva, modal de formulario y footer.
- Tema coherente con una clínica veterinaria local.
- Publicación para GitHub Pages.

## 3. Resultados

### Cumple
- El proyecto usa HTML semántico y JavaScript acotado para abrir y cerrar el modal de reserva.
- La validación se apoya en HTML5: `required`, `min`, `max`, `minlength`, `maxlength`, `pattern`, `accept`, `type`, entre otros.
- Se incorpora una estructura clara con `header`, `main`, `section`, `fieldset` y `footer`.
- Se incluye un skip link para saltar al formulario.
- Los inputs tienen labels asociados y el formulario usa agrupaciones semánticas.
- El diseño es responsive para móvil y escritorio.
- Se incluye una adaptación visual moderna para una clínica veterinaria.
- Se atienden casos de movimiento reducido para accesibilidad.
- El CTA principal y el botón flotante abren el formulario sin abandonar la página principal.
- El modal usa `role="dialog"`, `aria-modal`, `aria-labelledby` y `aria-hidden`.
- El modal puede cerrarse con el botón de cierre, el fondo de la ventana o la tecla `Escape`.
- Se bloquea el desplazamiento del documento mientras el modal está abierto.

### Puntos a controlar
- El tamaño máximo real del archivo de `type="file"` no puede validarse solo con HTML5; esa validación requiere servidor o JavaScript.
- El `output` visual puede requerir comportamiento dinámico para reflejar cambios en tiempo real; en este caso se presenta como valor accesible estático para mantener el enfoque sin scripts.
- El modal todavía requiere una gestión avanzada del foco para devolverlo automáticamente al botón que lo abrió y mantenerlo dentro del diálogo durante la navegación por teclado.

## 4. Riesgos
- Si se quiere validar el peso del archivo en el navegador, se necesitaría lógica del lado del cliente o del servidor.
- Si se decide añadir interacciones complejas o mensajes personalizados, sería necesario una capa JavaScript o una validación del backend.
- La reserva no envía datos a un backend real porque el formulario conserva `action="#"`; actualmente funciona como prototipo visual y académico.

## 5. Conclusión
La propuesta de `ClinicPet` cumple con el marco solicitado para una entrega académica de formulario accesible, HTML5 y diseño moderno. La última versión incorpora una reserva modal que reduce el ruido visual de la landing page y mantiene el CTA disponible mediante un botón flotante. Tiene una base sólida para ser publicada y mejorada con contenido real de la clínica en futuras iteraciones.
