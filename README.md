# ClinicPet

Proyecto final para una clínica veterinaria con enfoque en UX, accesibilidad y diseño moderno usando HTML5 + Bootstrap.

## Objetivo
Crear una landing page profesional con un formulario accesible, validación nativa de HTML5 y una experiencia de reserva clara para usuarios en dispositivos móviles y escritorio.

## Archivos principales
- `index.html`: estructura principal del sitio y formulario de reserva.
- `styles.css`: estilos personalizados y ajustes de accesibilidad visual.
- `AUDITORIA-UX-ACCESIBILIDAD.md`: documento de revisión de UX y accesibilidad.
- `.github/workflows/deploy.yml`: configuración para desplegar en GitHub Pages.

## Tecnologías usadas
- HTML5 semántico.
- Bootstrap 5.3.
- CSS personalizado.
- Validación nativa del navegador.
- GitHub Pages para publicación.

## Requisitos atendidos
- Formulario accesible con labels, fieldset, legend y skip link.
- Uso de inputs HTML5 y validación nativa.
- Diseño responsive con enfoque en usabilidad.
- Modales con cierre por botón, fondo y tecla Escape.
- Foco visible, contrastes adecuados y soporte para preferencia de reducción de movimiento.
- Documentación de auditoría UX y accesibilidad incluida.

## Vista local
Se puede abrir directamente en el navegador o servir con un servidor local:

```bash
py -m http.server 8000
```

Luego ir a:

```text
http://localhost:8000/
```

## Publicación en GitHub Pages
El repositorio está preparado para desplegarse con GitHub Pages usando una GitHub Action. El sitio se publica desde la rama `main` o desde la carpeta raíz del proyecto.

## Despliegue
1. Haz push del repositorio.
2. En GitHub, entra a Settings > Pages.
3. Activa GitHub Pages desde la rama `main` y la carpeta raíz.
4. La página quedará disponible en una URL pública.
