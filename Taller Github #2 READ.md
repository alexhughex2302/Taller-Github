# **Taller GitHub #2**

## **Detalles de la Entrega**

- **Modalidad:** Individual.
- **Tiempo Estimado:** 1 hora.
- **Plazo de Entrega:** Según lo indicado en clase.

### **Objetivo**

Aprender a manipular el historial de commits utilizando los comandos `git reset`, `git rebase` y `git cherry-pick`, entendiendo sus riesgos y casos de uso.

### **Comandos**

A continuación, se explican los comandos clave que utilizarás en esta práctica:

1. **`git rebase -i <hash>`**

   - Permite reorganizar, combinar, eliminar o modificar commits de forma interactiva.
   - Opciones útiles:
     - `drop`: Elimina un commit.
     - `reword`: Cambia el mensaje de un commit.
     - `squash`: Combina un commit con el anterior.
     - `fixup`: Similar a `squash`, pero descarta el mensaje del commit.

2. **`git log --oneline`**

   - Muestra el historial de commits de forma resumida (hash abreviado y mensaje).

3. **`git reflog --oneline`**

   - Registra todas las acciones realizadas en el repositorio (incluyendo cambios eliminados).

4. **`git reset --hard <hash>`**

   - Restaura el repositorio a un estado específico, descartando todos los cambios posteriores al commit indicado.

5. **`git cherry-pick <hash>`**
   - Aplica los cambios de un commit específico a la rama actual.

### **Entregables**

El informe debe incluir **exactamente los siguientes pantallazos** correspondientes a cada paso del taller:

1. **Presentación:**

   - Nombre completo, usuario de GitHub y enlace al fork del repositorio.

2. **Evidencias detalladas:**

   - **Parte 1:**
     - `git log --oneline` antes y después de eliminar los commits (paso 1).
     - `git log --oneline` con el nuevo orden de commits (paso 2).
     - Editor de rebase interactivo mostrando la combinación de commits (paso 3).
     - `git log --oneline` con el commit renombrado (paso 4).
   - **Parte 2:**
     - Salida completa de `git reflog --oneline` (paso 1).
     - `git log --oneline` después del reset (paso 2).
   - **Parte 3:**
     - Proceso de cherry-pick (captura de la terminal durante la ejecución).
     - `git log --oneline` final en `main` después del merge (paso 3).

3. **Conclusiones:**
   - Responde en máximo 3 párrafos:
     - ¿Qué lograste al usar `git rebase`, `reset` y `cherry-pick`?
     - ¿Qué utilidad tienen estos comandos en proyectos reales?
     - ¿Qué precauciones debes tomar al manipular el historial de Git?

## **Pasos del Taller**

### **Parte 0: Repositorio Base**

1. **Realizar un _fork_ del repositorio:**
   - Enlace: [cuatrosr/PI1-Git-Commits](https://github.com/cuatrosr/PI1-Git-Commits).
   - **Pasos:**
     - Haz un _fork_ del repositorio a **tu cuenta personal de GitHub**.
     - Clona el repositorio forkeado en tu máquina local:
       ```bash
       git clone https://github.com/[TU-USUARIO]/PI1-Git-Commits.git
       ```

---

### **Parte 1: Git Rebase Interactivo**

1. **Borrar commits consecutivos:**

   - Elimina los commits con mensajes _"commit to remove2"_ y _"commit to remove1"_ usando `git rebase -i`.
   - **Evidencia requerida:**
     - Captura del `git log --oneline` **antes** y **después** del rebase.

2. **Reordenar commits:**

   - Mueve el commit _"add project description"_ después de _"add author"_.
   - **Evidencia requerida:**
     - Captura del `git log --oneline` con el nuevo orden.

3. **Combinar commits:**

   - Fusiona _"add getters on car"_ y _"add setters on car class"_ en un solo commit: _"add getters and setters to car class"_.
   - **Evidencia requerida:**
     - Captura del editor de rebase interactivo mostrando la fusión (uso de `squash` o `fixup`).

4. **Renombrar un commit:**
   - Usa `reword` para cambiar _"add Readme.md"_ a _"add Readme.md for project description"_.
   - **Evidencia requerida:**
     - Captura del `git log --oneline` con el mensaje actualizado.

---

#### **Parte 2: Reflog y Reset**

1. **Recuperar historial:**

   - Usa `git reflog --oneline` para ver todos los cambios.
   - **Evidencia requerida:**
     - Captura del historial completo del `reflog`.

2. **Restaurar estado anterior:**
   - Regresa al estado antes del rebase con `git reset --hard <hash>`.
   - **Evidencia requerida:**
     - Captura del `git log --oneline` después del reset.

---

#### **Parte 3: Git Cherry-pick**

1. **Crear rama auxiliar:**

   - Encuentra el commit _"add car class"_ con `git log --oneline`.
   - Muévete a ese commit: `git checkout <hash>`.
   - Crea una rama nueva: `git branch auxiliar` y cámbiate a ella: `git checkout auxiliar`.

2. **Aplicar commits específicos:**

   - Usa `git cherry-pick <hash>` para incluir en la rama `auxiliar`:
     - _add list on main and add cars on for loop_
     - _add cars toString and print_
     - _add author_
   - **Evidencia requerida:**
     - Captura del proceso de cherry-pick (incluyendo resolución de conflictos si ocurren).

3. **Merge forzado:**
   - Regresa a `main`: `git checkout main`.
   - Resetea `main` al commit _"add car class"_: `git reset --hard <hash>`.
   - Fusiona la rama `auxiliar`: `git merge auxiliar`.
   - Haz push forzado: `git push --force`.
   - **Evidencia requerida:**
     - Captura del `git log --oneline` final en `main`.

---

> [!IMPORTANT]
> Si necesitan más información pueden guiarse de estas fuentes:
>
> - [Guía de Reset, Rebase y Cherry-pick](https://vergaracarmona.es/reset-rebase-cherry-pick/)
> - [Borrar commits en Git](https://jonsegador.com/2015/06/borrar-commits-de-git-reset-rebase-cherry-pick/)
