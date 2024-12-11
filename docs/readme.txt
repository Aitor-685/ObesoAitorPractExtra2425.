## 1. Creación de la Estructura Inicial del Proyecto

Se creó la estructura de archivos y directorios inicial para el proyecto utilizando los siguientes comandos:

mkdir -p proyecto-patrones/{docs,scripts,images,temp}
touch proyecto-patrones/docs/{manual.txt,guia.md,readme.txt}
touch proyecto-patrones/scripts/{app.js,utils.py,config.js}
touch proyecto-patrones/images/{logo.png,icon.jpg,banner.gif}
touch proyecto-patrones/temp/{pruebas.log,debug.txt,draft.md}

---

## 2. Inicialización del Repositorio Git y Commit Inicial

### Comandos Utilizados:

1. **Inicializar el repositorio:**
   git init

2. **Realizar el primer commit:**
   git commit -m "Commit inicial con la estructura de directorios vacía."

Resultado: La estructura de directorios se encuentra bajo control de versiones, pero no se han añadido archivos específicos aún.

---

## 3. Gestión de Archivos por Ejercicios

### Ejercicio 1: Añadir Archivos `.txt` de la Carpeta `docs/`

1. **Añadir los archivos `.txt` de `docs/` al área de preparación:**
   git add docs/*.txt

2. **Verificar el estado:**
   git status

3. **Hacer un commit:**
   git commit -m "Añadidos los archivos .txt de la carpeta docs."

### Ejercicio 2: Añadir Archivos `.js` de `scripts/` Excluyendo `config.js`

1. **Añadir los archivos `.js` de `scripts/`:**
   git add scripts/*.js

2. **Excluir `config.js`:**
   git reset scripts/config.js

3. **Verificar el estado:**
   git status

4. **Hacer un commit:**
   git commit -m "Añadidos los archivos .js de scripts excluyendo config.js."

### Ejercicio 3: Añadir Imágenes Excepto las que Terminan en `.gif`

1. **Añadir las imágenes `.png` y `.jpg`:**
   git add images/*.png images/*.jpg

2. **Verificar el estado:**
   git status

3. **Hacer un commit:**
   git commit -m "Añadidas imágenes excepto las que terminan en .gif."

---

## 4. Subir el Repositorio a un Remoto

### Pasos Realizados:

1. **Crear un repositorio remoto (por ejemplo, en GitHub).**

2. **Configurar el remoto en el repositorio local:**
   git remote add origin <URL-del-repositorio>

3. **Subir los cambios al repositorio remoto:**
   git push -u origin main
