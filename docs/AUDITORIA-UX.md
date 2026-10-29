# Auditoría y Rediseño de UX/UI - App Notas

## 1. Tabla de Auditoría Heurística

| Heurística                         | Problema encontrado                                                      | Solución aplicada                                                              |
| :--------------------------------- | :----------------------------------------------------------------------- | :----------------------------------------------------------------------------- |
| **Visibilidad del estado**         | Al agregar o borrar una nota no sale ningún mensaje de confirmación.     | Se agregó un mensaje informativo visible ("Nota agregada correctamente").      |
| **Coincidencia con el mundo real** | Usa íconos o textos técnicos confusos.                                   | Se renombraron las acciones usando lenguaje claro e intuitivo para el usuario. |
| **Control y libertad**             | Al eliminar una nota, esta se borra de inmediato sin pedir confirmación. | Se añadió una ventana de confirmación antes de eliminar o vaciar notas.        |
| **Prevención de errores**          | Permite guardar notas totalmente vacías.                                 | Se agregó la validación obligatoria para evitar enviar campos vacíos.          |
| **Reconocer, no recordar**         | Los campos no tienen etiquetas `<label>`, solo `placeholder`.            | Se colocaron etiquetas `<label>` visibles en cada campo de entrada.            |

## 2. Aplicación de Leyes de Usabilidad

- **Ley de Fitts:** El botón principal de guardar se diseñó con un alto de 44px y tamaño amplio para facilitar el clic o toque.
- **Ley de Hick:** Se categorizaron o simplificaron las opciones disponibles para agilizar la toma de decisiones.
- **Ley de Miller:** Se organizó la información en bloques cortos y limpios para no saturar la memoria visual.

## 3. Accesibilidad y Principios Visuales

- Variables CSS en `:root` para unificar los colores.
- Etiquetas `<label>` en todos los campos e imágenes con su atributo `alt`.
- Foco visible (`:focus-visible`) para navegación fluida con la tecla Tab.
- Contraste superior a 4.5:1 exigido por WCAG 2.2.
- Puntaje de Accesibilidad en Lighthouse de 90+ puntos.
