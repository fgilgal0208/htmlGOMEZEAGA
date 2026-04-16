# Migración Web: De WordPress a Arquitectura Estática (HTML5/CSS3)

**Proyecto:** Desarrollo de sitio web para despacho jurídico
**Empresa:** Taller Empresarial 2.0  
**Contexto:** Prácticas Profesionales (FEOE) - Taller Empresarial 2.0
**Tecnologías:** HTML5, CSS3 (Flexbox/Grid), JavaScript (ES6+), FormSubmit.

## 1. Descripción del Proyecto
Durante mi periodo de prácticas en **Taller Empresarial 2.0**, realicé la migración completa de un sitio web originalmente construido en **WordPress** hacia una arquitectura estática pura. El objetivo fue optimizar el rendimiento (WPO), mejorar la seguridad y permitir un control absoluto sobre el código fuente, eliminando la carga de plugins y bases de datos innecesarias.

## 2. Desarrollo y Soluciones Técnicas

### A. Modularización del Diseño (CSS3)
Para mantener la escalabilidad del proyecto, estructuré los estilos de forma modular:
* **Arquitectura de Estilos:** Separación de estilos globales (`estilos.css`), específicos de la sección de contacto (`estilosContacto.css`) y de las páginas informativas (`EstilosIncidente.css`).
* **Responsive Design:** Implementación de *Media Queries* para garantizar que la navegación, las cuadrículas de imágenes y el formulario se adapten correctamente a dispositivos móviles y tablets.

### B. Sistema de Contacto "Ready for Production"
Desarrollé un sistema de envío de mensajes funcional sin necesidad de backend propio mediante la integración de **FormSubmit** y **JavaScript (Fetch API)**:
* **Entrega Parametrizada:** Siguiendo los estándares de flujo de trabajo de la empresa, el formulario se entregó con el atributo `action=""` pendiente de configuración. Esto permite que la dirección de producción (el correo final del cliente) sea asignada por el superior técnico o el cliente de forma segura antes del despliegue final.
* **Gestión Asíncrona:** El envío se procesa mediante una petición AJAX, evitando la recarga de la página y mejorando la fluidez de la navegación.

### C. UI/UX: Alerta de Confirmación Personalizada
En lugar de utilizar alertas nativas del sistema, diseñé una **ventana modal dinámica** integrada en el DOM:
* **Feedback Visual:** Implementación de un pop-up con fondo difuminado (*backdrop-filter*) e iconografía de FontAwesome que confirma visualmente el éxito del envío.
* **Lógica de Navegación:** Una vez que el usuario acepta la confirmación, un script de redirección lo devuelve automáticamente a la página de inicio (`index.html`), cerrando el ciclo de interacción de forma profesional.

## 3. Resultados Obtenidos
1. **Rendimiento Máximo:** La web es ahora un sitio estático de carga instantánea.
2. **Escalabilidad:** Código limpio y comentado, listo para ser mantenido o ampliado sin las restricciones de un CMS.
3. **Flujo de Trabajo Profesional:** Demostración de prácticas de desarrollo reales, separando la lógica funcional de los datos sensibles para la entrega final al cliente.

---
### **Propiedad Intelectual**
**Nota:** Todos los derechos sobre el código fuente, el diseño y los materiales desarrollados en este proyecto pertenecen exclusivamente a **Taller Empresarial 2.0**. Queda prohibida su reproducción o uso sin autorización expresa de la empresa.

---
*Proyecto desarrollado íntegramente en Córdoba (España) bajo la supervisión de Taller Empresarial 2.0.*