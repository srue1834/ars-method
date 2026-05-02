## Evolución del proyecto de Funciones Avanzadas 1 y 2"

En este proyecto se encuentran las **dos pruebas de evaluación** de la asignatura: la **revisión** (rama `main` y uso de GitHub) y el **proyecto de experimentos** (ramas de experimento). Lo que hagas aquí —seguir los vídeos en `main` y trabajar en tus ramas— es la base de tu nota en ambas pruebas.

En este curso vas a reproducir la aplicación que el profesor construye en clase. Esto te servirá para aprender todos los conceptos de la asignatura y para usarla en tus aplicaciones futuras.  Tu objetivo es que **la rama `main` de tu repositorio sea una copia 1:1 de la del profesor**. Al final de cada video tendrás que crear un commit.

Para **experimentar y hacer pruebas**, usarás **ramas aparte** que **nunca** se mezclarán con `main`.

---

## 🥇 Regla de oro

- **`main` = Código que se hace en clase y commit tuyo al final de cada video**  
- **Las ramas de experimento NUNCA se mezclan en `main`**  
  - Nada de `merge`, `rebase` ni `cherry-pick` hacia `main`.

---

## 🛠️ Setup inicial (Clase 1)

1. Crea un repositorio remoto en Github
1. Crea la aplicación de Vue. 
2. Entra en la carpeta de la aplicación.
2. Ejecuta estos comandos una sola vez:

```bash
git init
git add .
git commit -m "TU_USERNAME_UPV: Inicio de la app"
git remote add origin https://github.com/TU_USERNAME_UPV/NOMBRE_REPO.git
git push -u origin main
```

> Sustituye `TU_USERNAME_UPV` y la URL por los tuyos reales.

---

## 🔄 Commits al final de cada video

1. Asegúrate de tener todo como en el vídeo.
2. La aplicación debe correr bien y no tener fallos.
2. Haz el commit con este formato:

```bash
git add .
git commit -m "TU_USERNAME_UPV: Descripción breve"
git push origin main
```

Reglas:


- Si te equivocas en un commit, puedes hacer **un commit corrector inmediatamente después** en `main`
  (por ejemplo: `TU_USERNAME_UPV: Corrección tras el error`), siempre que:
  - No borres ni reescribas el commit anterior.
  - El resultado final de la app sea el mismo que en los vídeos.
- Para probar otras soluciones o cambios más grandes, usa **ramas de experimento**, pero **no reescribas la historia de `main`** (`rebase`, `commit --amend`, `reset --hard`, etc. prohibidos).

---

## 🧪 Ramas para experimentar (sin tocar `main`)

Cuando quieras probar cosas sin romper `main`:

1. Ponte en el commit de la clase donde quieres empezar a experimentar  
   (normalmente será el final de la clase que acabas de ver):

```bash
git checkout -b experimento-Nº   # Que el número de los experimentos esté ordenado en el tiempo
```

2. Juega libremente en esa rama:

   - Puedes hacer los commits que quieras.
   - Puedes romper el código, rehacerlo, probar ideas, etc.
   - Estos commits formarán parte de tu evaluación (creatividad, esfuerzo, cuidado del código, etc.).

   Si estás en una rama de experimento y **aún no has hecho commit** y quieres descartar todos los cambios del working copy (volver al estado del último commit de esa rama):

   ```bash
   git checkout -- .
   ```

3. Sube la rama a GitHub:

```bash
git push origin experimento-Nº
```

4. Para volver a la rama oficial del curso:

```bash
git checkout main
```

> Importante: **no hagas `merge` ni `rebase` desde las ramas de experimento hacia `main`.**

### 🔎 Experimentos desde un commit antiguo

A veces querrás hacer un experimento **a partir de una versión anterior** de la app (un commit que está más abajo en el historial de `main`).

#### 1. Localizar el commit en el historial

En la rama `main`:

```bash
git checkout main
git log --oneline
```

Verás algo así:

```bash
a1b2c3d TU_USERNAME_UPV: Descripción breve
9f8e7d6 TU_USERNAME_UPV: Descripción breve
...
```

- El código corto del principio (`a1b2c3d`) es el **hash del commit**.
- Apunta el hash del commit desde el que quieres empezar el experimento.

#### 2. Crear una rama de experimento desde ese commit

Con el hash apuntado:

```bash
git checkout -b experimento-Nº a1b2c3d
```

- `experimento-Nº` → nombre de la rama de experimento.
- `a1b2c3d` → hash del commit elegido de `git log`.

Ahora:

- Tienes una **rama nueva** que empieza exactamente en ese commit antiguo.
- Puedes hacer commits y probar cambios sin tocar `main`.

#### 3. Subir la rama al remoto

```bash
git push -u origin experimento-clase-4
```

> Esta rama también forma parte de tu evaluación: usar bien Git y explorar soluciones cuenta.

---

## 🚫 Estrictamente prohibido en `main`

- **Hacer `merge` de cualquier rama hacia `main`.**
- **Commits extra en `main`** que no sean los del final de los vídeos.
- **Reescribir la historia de `main`** (`git rebase main`, `git commit --amend`, `git reset --hard`, etc.).

---

## ✅ Check final antes de entregar

Antes de entregar, comprueba que tu repositorio cumple las normas.

1. **Revisar la historia de `main`:**

```bash
git log --oneline main
```

- Debe coincidir (en orden e intención) con los commits que aparecen en los vídeos.

2. **Ver ramas remotas (experimentos):**

```bash
git branch -r
```

- Aquí pueden aparecer tus ramas de experimento (`origin/experimento-...`), sin problema.

---

## 📦 Qué entregarás

- **Enlace al repositorio de GitHub** donde:
  - `main` sea la reproducción exacta de mi proyecto.
  - Tengas subidas tus **ramas de experimento** (no las borres), con tus pruebas y soluciones alternativas.

Parte de tu nota saldrá de:
- Cómo de fiel es `main` al proyecto de clase.
- Qué has trabajado y probado en las ramas de experimentos.