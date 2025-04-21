# Listado de Mejoras UX/UI para Columns - Web

## 1. Navegación y Flujo de Usuario General

- La navegación entre las secciones no es clara.  
  **Propuesta:** usar *breadcrumbs* (por ejemplo: `Home / Files / Stats`) y agregar botones de retroceso para mejorar el flujo.

- En las vistas **Stats** y **Table View**, falta una forma directa de navegar hacia el **Visualizador 3D**.  
  **Propuesta:** agregar botones (¿en el nav o dentro del cuerpo?).

- El botón de **Login/Register** debería desaparecer según el contexto (por ejemplo, no mostrar "Login" cuando ya estás en esa vista).

- Actualmente, si un usuario logeado va a la ruta `/home`, es redirigido automáticamente a **View Tables** (Home = landing page).

---

## 2. Diseño Visual y Consistencia

- Inconsistencias en botones: tamaño, color, tipografía y estilo.  
  **Propuesta:** definir una **paleta de colores única** y unificar estilos visuales de botones, inputs, tarjetas, acciones, encabezados y navegación.

- Asegurar que los títulos, subtítulos y botones de acción se diferencien claramente en **tamaño**, **peso** y **color**.

- Otros detalles de CSS a mejorar:
  - Cambios bruscos en la posición de los elementos al mostrar errores.
  - Espaciado poco intuitivo entre elementos de formularios.
  - Elementos fuera de estilo general que se perciben aislados.

- **Propuesta general:** mejorar la ubicación de elementos para una mejor jerarquía visual.

- Posibilidad de agregar **modo oscuro**.

---

## 3. Contenido y Explicaciones

- Faltan textos descriptivos en varias secciones.  
  Por ejemplo: la **landing page** debería explicar claramente el propósito de la aplicación.

- Las vistas carecen de instrucciones o contexto que ayuden al usuario a entender qué está viendo o qué acción debe realizar.  
  **Propuesta:**
  - Dar **feedback visual** al usuario: mensajes de confirmación al subir/eliminar/modificar archivos o columnas.
  - Incluir **pantallas informativas** cuando no hay contenido cargado (por ejemplo: sin archivos subidos).
  - Utilizar **tooltips** en botones con íconos sin texto.

---

## Sección de Vistas Específicas

### 4. Navbar

- Exponer tanto el logo como el título es redundante.
- El botón de **View Files** podría reemplazarse con la navegación entre secciones (breadcrumbs), o separarse del logo.

---

### 5. Autenticación (Login / Register)

- Las pantallas de Login y Register son casi idénticas; solo cambia el texto.  
  **Propuesta:**
  - Incluir textos orientativos según el contexto:
    - “¿Ya tienes una cuenta? Inicia sesión `[link]`”
  - Agregar enlaces a "Términos de uso" y "Política de privacidad".

- Ajustar posiciones de **labels** y **mensajes de error** para evitar que la caja de Login se agrande de forma poco estética al mostrar errores.

---

### 6. View Files

- Incorporar un sistema de **búsqueda** y **paginación** para facilitar la navegación en listas extensas de archivos.

---

### 7. Carga y Gestión de Archivos (Upload Files)

- Al subir un archivo CSV, los campos del formulario (descripción, compañía, nombre de la mina, ubicación) no se visualizan en la UI.  
  **Propuesta:** mostrar esta información en las tarjetas de archivo del listado. (ver link del repo)

- El formulario debe:
  - Validar campos obligatorios (como nombre de archivo).
  - Mostrar errores si no se adjunta archivo.

- El espaciado entre los inputs del formulario es confuso; falta separación clara entre secciones.  

---

### 8. Table View

- Luego de agregar una columna, el **dropdown** no se cierra automáticamente.
- El estilo visual del dropdown no sigue el diseño general, generando inconsistencia visual.

---

### 9. Visualizador 3D

- Los **selectores** no se reinician tras una selección inicial.
- Falta mayor consistencia espacial entre la selección de opciones y la visualización resultante.

---

## 10. Otros Elementos por Mejorar

- Hacer que el **logo** redirija a `/home` o `/files`.
- Agregar más **íconos representativos** en botones y elementos interactivos.
