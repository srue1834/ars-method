## 🧾 Revisión de la rama `main` del proyecto de clase

Esta revisión cuenta un **50%** de la nota final de la asignatura.

Además del trabajo en las ramas de experimento, **otra parte de la nota**, la **Revisión**, sale de cómo has seguido las clases en la rama `main` y de cómo mantienes actualizado tu repositorio en GitHub.

---

## 📌 Qué se revisará en la rama `main`

- **Fidelidad al código que se hace en las clases**
  - El resultado final de la aplicación debe ser el mismo que en los vídeos.
  - La estructura del proyecto (carpetas, archivos, nombres) debe coincidir con la versión del profesor.

- **Commits bien ordenados**
  - Los commits en `main` deben estar al final de los videos.
  - Los mensajes de commit deben seguir el formato acordado:  
    - Ejemplo: `TU_USERNAME_UPV: Descripción breve de los cambios`.
  - Si te equivocas en un commit, puedes hacer **un commit de corrección justo después** (por ejemplo: `TU_USERNAME_UPV: Corrección del error`), siempre que:
    - No borres ni reescribas el commit anterior.
    - El resultado final de la app deberá ser el mismo que el de los vídeos.

- **Uso correcto de Git en `main`**
  - No debe haber fusiones (`merge`) de ramas de experimento hacia `main`.
  - No debe reescribirse la historia (`git rebase`, `git reset --hard`, `git commit --amend`, etc.).
  - El historial debe ser claro y entendible.

En resumen: **la rama `main` muestra cómo has seguido las clases paso a paso y cómo entiendes el proceso de desarrollo**.

---

## 🌐 Repositorio en GitHub: actualización día a día

Tu **repositorio en GitHub** debe estar **siempre actualizado al día**:

- Antes de la siguiente **clase**:
  - Haz los commits correspondientes en `main` siguiendo los vídeos.
  - Sube los cambios a GitHub:

    ```bash
    git push origin main
    ```

  - Si esos días has trabajado en alguna rama de experimento, súbela también:

    ```bash
    git push origin experimento-Nº
    ```

- En la corrección miraré:
  - Si `main` y las ramas de experimento aparecen **actualizados de forma progresiva** a lo largo de los días de clase (no todo en un único día al final).
  - Si el uso de GitHub es constante (no solo una subida final sin historia de trabajo).

De esta forma, **la historia de Git + GitHub** mostrará no solo el resultado final, sino también **tu proceso de trabajo día a día**, que también forma parte de la nota.
