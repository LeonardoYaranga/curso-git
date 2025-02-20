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




# Git: Comandos Básicos y Estrategias

# Estado del Repositorio

`git status`  
Para ver los archivos que están por subir.

# Identificar Cambios y Autores

`git blame "nombreDeArchivo"`  
Muestra quién hizo cambios en cada línea de un archivo.

# Manejo de Ramas

- Ver las ramas existentes:  
  `git branch`

- Eliminar una rama:  
  `git branch -D "nombreRama"`

- Moverse a una rama existente:  
  `git checkout "nombreRama"`

- Crear y moverse a una nueva rama si no existe:  
  `git checkout -b "nombreRama"`

# Estrategia de Branching

Estrategia para evitar conflictos o resolverlos fácilmente. Esto lo define el equipo.

## Git Flow

Las ramas para nuevas funcionalidades se crean a partir de la rama `main` y vuelven a esta para hacer el merge.

- La rama `main` suele ser la de producción.
- Puede haber una rama de `desarrollo` donde se integran varias funcionalidades antes de pasar a producción.

# Subir Cambios

- Agrega todos los archivos en la ubicación actual al área de preparación.  
  `git add . `

- Guarda temporalmente los cambios sin confirmarlos en un "stash" para recuperarlos después  
  `git stash`

# Diferencias entre Archivos en Ramas

- Comparar un archivo entre ramas:  
  `git diff "branchName" "filePath"`

- Ejemplo con un archivo específico:  
  `git diff fix-1 .\index.html`

# Traer Cambios de Otras Ramas

- Unir cambios de otra rama a la actual:  
  `git merge "branchName"`

- Rebase para traer cambios en línea recta:  
  `git rebase`

- Ver el historial de cambios y commits:  
  `git log`


