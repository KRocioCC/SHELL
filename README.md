# Guía de Instalación de Bash

## Bash en Windows

## 1. Activar WSL

Abre PowerShell como administrador.

Ejecuta:

```bash
wsl --install
```

Esto habilita WSL y descarga automáticamente una distribución de Linux (por defecto, Ubuntu).

## 2. Reiniciar tu PC

Después de la instalación, reinicia Windows para que los cambios se apliquen.

## 3. Configurar Linux

Al reiniciar, se abrirá Ubuntu.

Te pedirá crear un usuario y contraseña.

Ya tienes Bash disponible.

## 4. Usar Bash

Puedes abrirlo desde el menú inicio buscando **Ubuntu** o **WSL**.

También puedes usarlo en **Windows Terminal** seleccionando la pestaña de Ubuntu.

Para verificar:

```bash
bash --version
```

---

## Bash en macOS

Bash viene preinstalado en macOS (aunque es una versión antigua).

### Verificar qué shell estás usando

Abre la Terminal y ejecuta:

```bash
echo $0
```

Si muestra `-bash`, ya estás en Bash.

Si muestra `-zsh`, estás en Zsh (el shell predeterminado desde macOS Catalina).

### Cambiar a Bash

Para usar Bash, simplemente escribe:

```bash
bash
```

O si quieres cambiarlo como predeterminado:

```bash
chsh -s /bin/bash
```

Cierra y vuelve a abrir la Terminal.

---

## Bash en Linux

Bash generalmente viene preinstalado en la mayoría de las distribuciones de Linux.

### Verificar si tienes Bash

Abre la terminal y ejecuta:

```bash
bash --version
```

### Instalar Bash (si no está instalado)

#### En Ubuntu/Debian:

```bash
sudo apt update
sudo apt install bash
```

#### En Fedora/RHEL/CentOS:

```bash
sudo dnf install bash
```

#### En Arch Linux:

```bash
sudo pacman -S bash
```

### Cambiar el shell predeterminado a Bash (si usas otro shell)

```bash
chsh -s /bin/bash
```

Cierra y vuelve a abrir la terminal para que los cambios se apliquen.
