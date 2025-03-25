# **Taller GitHub #1**

## **Detalles de la Entrega**

- **Modalidad:** Individual.
- **Tiempo Estimado:** Entre 1.5 y 2 horas en total (30 minutos por repositorio).
- **Plazo de Entrega:** Según lo indicado en clase.

### **Objetivo**

Este taller busca que los estudiantes adquieran habilidades básicas y avanzadas en el uso de GitHub, enfocándose en:

- **Gestión de repositorios:** Aprender a crear forks, navegar en proyectos y seguir flujos de trabajo colaborativos.
- **Resolución de conflictos:** Entender cómo surgen los conflictos de fusión (merge conflicts) y cómo resolverlos.
- **Revisión de código:** Familiarizarse con el proceso de revisión de pull requests para trabajar en equipo.
- **Buenas prácticas:** Establecer estándares de codificación y documentación para proyectos futuros.

## **Pasos del Taller**

### **Repositorios a Trabajar**

Cada estudiante debe realizar un _fork_ de los siguientes repositorios y completar los cursos en GitHub:

1. **Repositorio 1:** [skills/introduction-to-github](https://github.com/skills/introduction-to-github)

   - **Descripción:** Introducción a GitHub (duración: ~30 minutos).
   - **Objetivo:** Familiarizarse con los conceptos básicos de GitHub.

2. **Repositorio 2:** [skills/resolve-merge-conflicts](https://github.com/skills/resolve-merge-conflicts)

   - **Descripción:** Resolución de conflictos de fusión (duración: ~30 minutos).
   - **Objetivo:** Entender cómo manejar y resolver conflictos en Git.

3. **Repositorio 3:** [skills/review-pull-requests](https://github.com/skills/review-pull-requests)
   - **Descripción:** Revisión de pull requests (duración: ~30 minutos).
   - **Objetivo:** Aprender a colaborar mediante revisiones de código.

---

### **¿Cómo Completar Cada Curso?**

1. **Hacer un _fork_ del repositorio:**

   - Dirígete al enlace de cada repositorio y haz clic en _"Fork"_ (esquina superior derecha).
   - Asegúrate de que el fork se guarde en **tu cuenta personal de GitHub**.

2. **Iniciar el curso:**

   - Dentro de tu repositorio forkeado, lee el **README.md** y haz clic en el botón verde **"Start course"**.
   - Al activar el curso, se ejecutará un _pipeline_ automático que guiará las actividades.

3. **Seguir las instrucciones:**
   - Después de iniciar el curso o completar una actividad, **espera 20-30 segundos y actualiza la página** (`F5`) para ver la siguiente tarea.

> [!IMPORTANT]
> Al finalizar cada curso, aparecerá un README de **"Finish"**.

## **Entregables**

### **Dentro de la Clase:**

Elabora un **informe en formato PDF** que incluya:

1. **Enlaces a tus 3 repositorios forkeados** (uno por cada curso).
2. **Capturas de pantalla** de los README de finalización (con el mensaje de _"Finish"_ visible y también de su perfil de GitHub).
3. **Respuestas a las siguientes preguntas** (máximo 2 párrafos por respuesta):
   - _¿Qué aprendió durante este proceso?_
   - _¿Cómo integraría lo aprendido a su proyecto?_
   - _¿Qué desafíos encontró y cómo los resolvió?_

### **Fuera de Clase (Trabajo en Equipo):**

Cada equipo debe crear un archivo `CODESTYLE.md` en su repositorio del proyecto, dentro de una carpeta llamada `/docs`.

#### **Contenido Requerido:**

##### **1. Nombres de Variables y Funciones**

- **Variables:** Usar `camelCase` (ejemplo: `miVariable`, `nombreUsuario`).
- **Funciones/Clases:** Usar `PascalCase` (ejemplo: `ClaseVehiculo`, `HistorialMantenimiento`).

##### **2. Reglas de Indentación**

- Usar **4 espacios** por nivel de indentación. **No utilizar tabuladores**.

##### **3. Longitud Máxima de Líneas de Código**

- Limitar las líneas de código a un **máximo de 80 caracteres** para mejorar la legibilidad.

##### **4. Formato de Comentarios y Documentación**

- **Comentarios en línea:** Usar `//` para explicaciones breves.
- **Comentarios de bloque:** Usar `/* */` para documentar funciones o clases.

##### **5. Nombres de Commits**

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

##### **6. Nombres de Ramas**

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
