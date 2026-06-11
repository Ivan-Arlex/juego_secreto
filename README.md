# Juego Secreto 🎮

¡Bienvenido al proyecto **Juego Secreto**! Este repositorio fue creado con fines educativos para la práctica y aprendizaje de flujos de trabajo, buenas prácticas y comandos esenciales utilizando **Git y GitHub**.

## 📝 Descripción del Juego

El proyecto consiste en un juego interactivo donde el sistema genera un número secreto de forma aleatoria. El objetivo del usuario es adivinar cuál es ese número ingresando sus intentos en la aplicación.

*   **Rango del juego:** Por defecto, el usuario debe ingresar un número entre **1 y 100**.
*   **Configurable:** El límite máximo de $X$ (actualmente 100) es completamente editable dentro del código fuente, lo que permite expandir o reducir el nivel de dificultad del juego según se requiera.
*   **Retroalimentación:** El sistema le indicará al jugador si el número secreto es mayor o menor que el intento ingresado, ayudándole a deducir el resultado.

---

## 🚀 Guía Rápida de Comandos de Git

A continuación, se presenta una lista ordenada con los comandos fundamentales de Git utilizados durante el desarrollo de este curso, sirviendo como hoja de referencia para el control de versiones:

### 1. Inicialización y Configuración
*   `git init`: Inicializa un nuevo repositorio de Git local en la carpeta del proyecto.
*   `git clone <url-del-repositorio>`: Descarga una copia exacta de un repositorio remoto (como este de GitHub) a tu computadora local.

### 2. El Flujo de Trabajo Diario (Guardar Cambios)
*   `git status`: Muestra el estado actual de los archivos (cuáles han sido modificados, cuáles están listos para guardarse y cuáles no rastrea Git).
*   `git add .`: Envía todas las modificaciones y nuevos archivos al área de preparación (*Staging Area*), listos para el commit.
*   `git commit -m "Mensaje corto"`: Registra los cambios guardados en el historial con un título descriptivo (máximo 72 caracteres).
*   `git commit`: Abre el editor de texto de la terminal para redactar un mensaje estructurado (Título largo, línea en blanco obligatoria y cuerpo con detalles/coautores).

### 3. Conexión y Envío Remoto (GitHub)
*   `git remote add origin <url-del-repositorio>`: Vincula tu repositorio local con el repositorio remoto en GitHub por primera vez.
*   `git push -u origin main`: Sube los commits locales a la rama principal en GitHub y memoriza el camino de forma permanente.
*   `git push origin main`: Sube los cambios a GitHub en el momento, pero sin recordar el enlace predeterminado para el futuro.
*   `git push`: Envía los nuevos commits a GitHub de forma directa y simplificada (requiere que el enlace ya esté memorizado o que el proyecto sea un clon).
*   `git pull`: Descarga y fusiona de forma automática los últimos cambios del repositorio de GitHub en tu computadora local.

### 4. Trabajo Colaborativo y Coautoría
*   Para dar crédito a tus compañeros cuando programan juntos desde tu PC, puedes usar la siguiente estructura al final de tu commit (dejando dos líneas en blanco antes):
```text
    Co-authored-by: NOMBRE <nombre@email.com>
    ```

### 5. Edición del Pasado y Enmiendas (Antes del Push)
*   `git commit --amend`: Abre el último commit para agregar archivos olvidados o modificar su mensaje de texto usando el editor de la terminal.
*   `git commit --amend --no-edit`: Absorbe los archivos agregados recientemente con `git add .` dentro del commit anterior de forma instantánea, manteniendo intacto el mensaje original.

### 6. Deshacer Cambios y Corrección de Errores
*   `git revert <id-del-commit>`: Crea un commit completamente nuevo que hace lo opuesto al ID especificado. Es la forma más segura de deshacer una equivocación sin alterar el historial existente.
*   `git reset --hard <id-del-commit-bueno>`: Regresa el proyecto en el tiempo como una máquina del tiempo radical, eliminando del historial todos los commits posteriores al ID indicado.
