# Respuestas a preguntas sobre Git y GitHub

### a. ¿Cómo se inicializa un repositorio en Git?

Para inicializar un repositorio en Git, se usa el comando `git init`, lo que crea un repositorio vacío en el directorio actual.

**Comando:**

```bash
git init
```

### b. ¿Cómo creas un repositorio en GitHub?

- Inicia sesión en GitHub.
- Haz clic en el botón "New" o "Nuevo" para crear un repositorio.
- Rellena los detalles (nombre, descripción) y crea el repositorio.

### c. ¿Cómo vinculas un repositorio local de Git con uno remoto en GitHub?

Se vincula usando el comando git remote add con la URL del repositorio remoto.

Comando:

```
git remote add origin https://github.com/usuario/nombre-repositorio.git
```

### d. ¿Cuál es el flujo básico de trabajo en Git y GitHub?

El flujo básico de trabajo es:

- git clone: Clonar el repositorio.
- git add: Añadir archivos al área de preparación.
- git commit: Hacer un commit.
- git push: Subir los cambios al repositorio remoto.

Comandos:

```
git clone https://github.com/usuario/repositorio.git
git add .
git commit -m "Mensaje de commit"
git push origin main

```

### e. ¿Para qué sirve el archivo .gitignore?

El archivo .gitignore sirve para especificar qué archivos o directorios no deben ser seguidos por Git (por ejemplo, archivos temporales o configuraciones locales).

Ejemplo de .gitignore:

```
*.log
node_modules/

```

### f. ¿Cuál es el propósito de una rama?

Una rama permite trabajar en una línea de desarrollo separada, lo que facilita experimentar y desarrollar nuevas funcionalidades sin afectar la rama principal (main o master).

Comando para crear una nueva rama:

```
git checkout -b nombre-de-la-rama

```

### g. ¿Qué es una fusión?

Una fusión (merge) es el proceso de integrar los cambios de una rama en otra. Por lo general, se hace para incorporar los cambios de una rama de desarrollo en la rama principal.

Comando para fusionar una rama:

```
git merge nombre-de-la-rama

```

### h. Explica los diferentes tipos de fusión que existen.

Existen dos tipos principales de fusión:

- Fusión automática: Git fusiona las ramas sin conflictos si no hay cambios contradictorios.
- Fusión con conflictos: Git no puede fusionar automáticamente debido a cambios contradictorios y requiere intervención manual.

### i. ¿Cómo puedes ver el historial de tu repositorio?

Para ver el historial de commits en un repositorio, se usa el comando git log.

Comando:

```
git log

```

### j. ¿Cuál es el propósito de una etiqueta?

Una etiqueta (tag) se utiliza para marcar puntos específicos en el historial de commits, generalmente para indicar versiones de lanzamiento.

Comando para crear una etiqueta:

```
git tag -a v1.0 -m "Versión 1.0"

```
