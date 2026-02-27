# Guía de Instalación de Zsh

## Zsh en Windows

### 1. Activar WSL

Abre PowerShell como administrador y ejecuta:

```bash
wsl --install
```

### 2. Reiniciar tu PC

Después de la instalación, reinicia Windows.

### 3. Instalar Zsh en Ubuntu

Una vez en WSL, abre Ubuntu y ejecuta:

```bash
sudo apt update
sudo apt install zsh
```

### 4. Cambiar el shell predeterminado a Zsh

```bash
chsh -s /usr/bin/zsh
```

Cierra y vuelve a abrir Ubuntu.

### 5. Verificar la instalación

```bash
zsh --version
```

---

## Zsh en macOS

Zsh es el shell predeterminado en macOS desde Catalina (2019).

### Verificar si tienes Zsh

Abre la Terminal y ejecuta:

```bash
echo $0
```

Si muestra `-zsh`, ya estás en Zsh.

### Instalar la última versión de Zsh

Si quieres una versión más reciente:

1. Instala Homebrew (si no lo tienes):

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

2. Instala Zsh actualizado:

```bash
brew install zsh
```

3. Cambia el shell predeterminado:

```bash
chsh -s /usr/local/bin/zsh
```

Cierra y vuelve a abrir la Terminal.

---

## Zsh en Linux

### Instalar Zsh

#### En Ubuntu/Debian:

```bash
sudo apt update
sudo apt install zsh
```

#### En Fedora/RHEL/CentOS:

```bash
sudo dnf install zsh
```

#### En Arch Linux:

```bash
sudo pacman -S zsh
```

### Cambiar el shell predeterminado a Zsh

```bash
chsh -s /usr/bin/zsh
```

Cierra y vuelve a abrir la terminal.

### Verificar la instalación

```bash
zsh --version
```

---

## Personalizar Zsh (Opcional)

### Instalar Oh My Zsh

Oh My Zsh es un framework que facilita la configuración de Zsh:

```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

Durante la instalación, te preguntará si quieres cambiar el shell a Zsh. Selecciona "Y" (Sí).

### Cambiar el tema

Los temas se encuentran en `~/.oh-my-zsh/themes/`. Para cambiar el tema, edita `~/.zshrc` y modifica:

```bash
ZSH_THEME="robbyrussell"
```

Por el tema que prefieras. Algunos populares: `agnoster`, `powerlevel10k`, `spaceship`.

---

## Diferencias entre Bash y Zsh

| Característica | Bash | Zsh |
|---|---|---|
| Autocompletado | Básico | Muy avanzado |
| Sintaxis | POSIX | Extendida |
| Temas | No | Sí (con Oh My Zsh) |
| Plugins | No nativos | Sí (con Oh My Zsh) |
| Compatibilidad | Muy buena | Buena (compatible con Bash) |
