# Crear PAT (Personal Access Token) en GitHub

> **¿Para qué sirve?** Necesitas un PAT para hacer `git push` (y otras operaciones) desde la terminal cuando GitHub te pide usuario y contraseña.

Un PAT es una cadena larga que empieza por `ghp_`, por ejemplo:
```text
ghp_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
```

---

## Cómo crear el token

1. En [GitHub](https://github.com), haz clic en tu **avatar** (arriba a la derecha).
2. Entra en **Settings**.
3. En el menú izquierdo, baja hasta **Developer settings**.
4. Entra en **Personal access tokens** → **Tokens (classic)**.
5. Pulsa **Generate new token** → **Generate new token (classic)**.
6. Configura el token:
   - **Note:** pon un nombre descriptivo, por ejemplo: `Git push mei`.
   - **Expiration:** 30 días, 90 días o *No expiration*, según lo que vayas a usar.
   - **Scopes:** marca **repo** (y deja marcadas todas las subopciones de `repo`).
7. Pulsa **Generate token**.

> **Importante:** el token **solo se muestra una vez**. Cópialo y guárdalo en un lugar seguro antes de cerrar la página.

---

## Usar el PAT al hacer push

Cuando ejecutes:

```bash
git push -u origin main
```

Git te pedirá **usuario y contraseña**. En ese momento:

| Campo      | Qué poner |
|-----------|-----------|
| **Username** | Tu usuario de GitHub (ej: `miUsuario`) |
| **Password** | **El PAT** que generaste (ej: `ghp_xxxx...`), **no** tu contraseña de GitHub |

Es decir: en *Password* no pones tu contraseña de la cuenta, sino el token (la cadena que empieza por `ghp_`).

---

## Resumen rápido

```bash
# Clonar un repo
git clone https://github.com/miUsuario/repo.git

# Hacer push (ahí te pedirá Username y Password = PAT)
git push -u origin main
```

- **Username:** `miUsuario`  
- **Password:** `ghp_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx` (tu PAT)