# CODESTYLE

Cada equipo debe crear un archivo `CODESTYLE.md` en su repositorio del proyecto, dentro de una carpeta llamada `/docs`.

## **Contenido Requerido:**

### **1. Nombres de Variables y Funciones**

- **Variables:** Usar `camelCase` (ejemplo: `miVariable`, `nombreUsuario`).
- **Funciones/Clases:** Usar `PascalCase` (ejemplo: `ClaseVehiculo`, `HistorialMantenimiento`).

### **2. Reglas de Indentación**

- Usar **4 espacios** por nivel de indentación. **No utilizar tabuladores**.

### **3. Longitud Máxima de Líneas de Código**

- Limitar las líneas de código a un **máximo de 80 caracteres** para mejorar la legibilidad.

### **4. Formato de Comentarios y Documentación**

- **Comentarios en línea:** Usar `//` para explicaciones breves.
- **Comentarios de bloque:** Usar `/* */` para documentar funciones o clases.

### **5. Nombres de Commits**

Deben seguir la convención **Conventional Commits** con la estructura:

```
tipo: Descripción del cambio
```

Ejemplos:

- `feat: añadir funcionalidad de búsqueda de vehículos por año`
- `fix: corregir error en la validación de tipo de combustible`
- `docs: agregar estilo de codificación a CODESTYLE.md`

**Tipos de commits permitidos:**

- `feat`: Nuevas características.
- `fix`: Corrección de errores.
- `docs`: Cambios en documentación.
- `style`: Cambios estéticos o de formato.
- `refactor`: Mejoras en código sin alterar funcionalidad.

### **6. Nombres de Ramas**

Utilizar una convención de nombres basada en la funcionalidad desarrollada:

- `feat/<nombre-funcionalidad>` → Para nuevas características.
- `fix/<descripción-error>` → Para corrección de errores.
- `docs/<actualización-documentación>` → Para cambios en documentación.

Ejemplos:

- `feat/agregar-vehiculo`
- `fix/corregir-validacion-combustible`
- `docs/actualizar-readme`

> [!IMPORTANT]
> El archivo `CODESTYLE.md` **debe estar presente** en el repositorio del proyecto, ya que será evaluado en cada entrega de sprint en relación con el uso adecuado de GitHub.
