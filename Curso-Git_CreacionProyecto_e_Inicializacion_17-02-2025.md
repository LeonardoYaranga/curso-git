# CreacionProyecto_e_Inicializacion_17-02-2025

## Descripción
Este repositorio es un curso sobre Git, donde se cubren los siguientes pasos y configuraciones básicas.

## Pasos iniciales

1. **Crear repositorio con el mismo nombre que el usuario:**
   - Descripción de la cuenta en el README.

2. **Guiarse de Alan1108**

---

## Crear el repositorio

Crear repositorio `curso-git`:

```bash
git clone https://github.com/LeonardoYaranga/curso-git.git
echo "# curso-git" >> README.md
git init
```


## Configuración y primer commit

1. Configurar la rama por defecto:
git config init.defaultBranch main

2. Renombrar la rama:
git branch -M main

3. Añadir y hacer commit:
git add README.md
git commit -m "first commit"

4. Conectar a GitHub:
git remote remove origin  # Borrar la conexión anterior

git remote add origin https://github.com/LeonardoYaranga/curso-git.git

git push -u origin main

---

## Setear credenciales

Configurar tus credenciales:

git config --global user.name "LeonardoYaranga"

git config --global user.email "leonardo.yaranga@hotmail.com"

### Git Credential Manager

Cuando usas varias cuentas de Git, puedes configurar un Git Credential Manager para gestionar credenciales de forma más sencilla.

https://github.com/git-ecosystem/git-credential-manager




