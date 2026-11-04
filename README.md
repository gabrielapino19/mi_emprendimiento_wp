# Elysa · Sitio WordPress

> Sitio web desarrollado para el emprendimiento **Elysa**, enfocado en bienestar integral y terapias holísticas. Proyecto correspondiente a la **Evaluación 03 — Sitios Web y Landing Pages (MKA1203, DUOC)**. Las instrucciones oficiales del proyecto se encuentran en [`indicaciones/README.md`](indicaciones/README.md).

- **Sitio en producción:** https://elysa.free.nf/?i=1
- **Prototipo en Stitch:** https://stitch.withgoogle.com/projects/13663528510219468781
- **Repo del Parcial 02:** https://github.com/gabrielapino19/mi-emprendimiento.git
- **Autor/a:** Gabriela Pino, sección 001D

## Contexto de la web

Elysa es un emprendimiento dedicado al bienestar integral, que ofrece terapias holísticas y productos personalizados para el equilibrio emocional y energético. Está dirigido a personas interesadas en el autocuidado, el autoconocimiento y las alternativas complementarias para su bienestar. El sitio web busca facilitar el acceso a información sobre nuestros servicios y productos, resolviendo las dificultades para conocerlos y encontrar una forma de contacto. Queremos que las personas conozcan Elysa, exploren nuestras opciones y se animen a consultar o solicitar nuestros servicios.

## Mi tema

- [x] **Tema descargado:** Prespa Wellness · [Ficha oficial en WordPress.org](https://wordpress.org/themes/prespa-wellness/)

---

## Instrucciones de tema descargado

### Requisitos del tema

| Dato | Mi tema |
|---|---|
| **Nombre y enlace a la ficha** | Prespa Wellness ([Ficha en WordPress.org](https://wordpress.org/themes/prespa-wellness/)) |
| **Gratis o de pago** | Gratuito (licencia GPLv2 o superior) |
| **Tipo (clásico o de bloques)** | Tema clásico con soporte de bloques Gutenberg (child theme de Prespa) |
| **Versión de WordPress que requiere** | 6.1 o superior |
| **Versión de PHP que requiere** | 5.6 o superior (recomendado 7.4 o superior) |
| **Plugins que necesita (si alguno)** | Ninguno obligatorio; compatible con Contact Form 7 y Easy Appointments |
| **Licencia** | GNU General Public License v2 o posterior |

### Cómo llevar mi sitio de Local a producción

Procedimiento planificado para migración y sincronización de datos entre el entorno local (Local WP) y producción (InfinityFree):

- **Plugin de migración planificado:** All-in-One WP Migration o exportador nativo de WordPress / BackWPup. Gratis (con límite de tamaño estándar de subida en hosting).
- **Qué se exporta:** Entradas del blog, páginas estáticas, imágenes de la biblioteca de medios, menús de navegación y opciones de personalización.

**Pasos:**

1. **En Local:** Generar el archivo de exportación completo (`.wpress` o archivo `.xml` de contenido más respaldo de `wp-content`) desde el plugin de migración o herramientas de exportación.
2. **En producción:** En la instalación limpia de WordPress en InfinityFree, instalar y activar el tema **Prespa Wellness** y los plugins correspondientes.
3. **Importar:** Cargar el paquete exportado utilizando el importador de WordPress o plugin de migración para restaurar la estructura y los medios.
4. **Revisar:** Comprobar la estructura de enlaces permanentes (`/%postname%/`), asignación del menú principal, asignación de la página de inicio estática, visualización de imágenes y funcionamiento del formulario de contacto.
5. **Registro de incidencias:** *(Se documentarán en el Checkpoint del 18 de noviembre conforme avance la fase de implementación).*

---

## Respaldo y reinstalación en otro servidor

El objetivo de este proyecto es que el sitio pueda respaldarse y reinstalarse de forma confiable en cualquier servidor.

**Qué respaldar:**

- Los archivos de WordPress (tema Prespa Wellness, plugins instalados y carpeta `wp-content/uploads` con imágenes y medios).
- La base de datos MySQL (tablas con páginas, entradas, categorías, menús y configuraciones generales).

**Cómo respaldo mi sitio:**  
Se utiliza el plugin **BackWPup** para generar copias completas de la base de datos y de la carpeta `wp-content`. Las copias se descargan en formato comprimido `.zip` a almacenamiento local seguro o se sincronizan con servicios en la nube (Dropbox), realizándose de forma periódica y obligatoriamente antes de cualquier actualización crítica de tema o plugins.

**Cómo lo reinstalo en un servidor nuevo:**

1. **Requisitos del servidor:** PHP 7.4 o superior, MySQL 5.7 o MariaDB 10.4+, WordPress 6.1+ y al menos 500 MB de espacio disponible.
2. **Instalar WordPress limpio:** Instalar la versión base de WordPress en el nuevo servidor (mediante instalador de hosting o subida manual).
3. **Restaurar el respaldo:** Subir y extraer los archivos de `wp-content` e importar la base de datos MySQL (vía phpMyAdmin o a través del plugin de respaldo).
4. **Ajustar:** Actualizar las URLs del sitio si el dominio cambia, guardar la estructura de enlaces permanentes en **Ajustes > Enlaces permanentes**, y verificar la asignación del menú y de la página de inicio en **Ajustes > Lectura**.
5. **Probar:** Realizar una auditoría visual de todas las páginas (Inicio, Nosotros, Servicios, Blog, Contacto), verificar la carga de imágenes y enviar un mensaje de prueba a través de Contact Form 7 para validar la recepción de correos.

---

## Plugins seleccionados / planificados

| Plugin | Para qué lo uso | Gratis o de pago | Versión probada |
|---|---|---|---|
| **Yoast SEO** | Optimización de títulos, meta descripciones, legibilidad y mapas XML para posicionamiento en Google | Gratis (Freemium) | Probado hasta WP 6.7 |
| **Contact Form 7** | Formulario de contacto directo para consultas de terapias holísticas y pedidos florales | Gratis (Open Source) | Probado hasta WP 6.7 |
| **BackWPup** | Generación de respaldos completos de la base de datos MySQL y archivos del sitio | Gratis (Freemium) | Probado hasta WP 6.7 |
| **Akismet Anti-spam** | Filtro automático de spam en los comentarios del blog y envíos de formularios | Gratis (sitios personales) | Probado hasta WP 6.7 |
| **AddToAny Share Buttons** | Botones para compartir artículos de salud y bienestar en redes sociales y WhatsApp | Gratis (100% gratuito) | Probado hasta WP 6.7 |

---

## Páginas y entradas

- **Páginas (Fase 1):**
  1. Inicio (portada y bienvenida)
  2. Contacto (formulario y canales de consulta)
  3. Nosotros (historia, visión holística y valores)
  4. Servicios (detalle de Reiki, Tameana, Tarot terapéutico, Péndulo Hebreo y Flores de Bach)
  5. Blog (artículos educativos sobre bienestar y autocuidado)

- **Entradas del blog:**
  1. Introducción al bienestar holístico y la armonía energética
  2. Beneficios de las Flores de Bach para el equilibrio emocional
  3. Cómo prepararte para tu primera sesión de Reiki

---

## Cómo me organicé

La planificación detallada del proyecto, el cronograma de trabajo con carta Gantt y el análisis de riesgos (Plan B) se encuentran documentados en [`proyecto/decisiones.md`](proyecto/decisiones.md).

---

## Plan de continuidad y rendimiento

*(Apartados correspondientes a la Entrega 4)*
- **Plan de continuidad (etapa 2 de mi web):** [`plan-de-continuidad.md`](proyecto/plan-de-continuidad.md) *(Pendiente para Entrega 4)*
- **Análisis de rendimiento con Lighthouse:** [`lighthouse.md`](proyecto/lighthouse.md) *(Pendiente para Entrega 4)*

---

## Uso de IA

- **Asistente de IA (Gemini / Antigravity):** Utilizado para investigar y validar técnicamente los requisitos oficiales de los plugins en WordPress.org, estructurar el cronograma del proyecto en formato Mermaid y dar formato profesional a la documentación en Markdown siguiendo las pautas de la asignatura. Se hizo revision de todas las decisiones sobre el proyecto.