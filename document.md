# 🚀 Bootcamp Git & GitHub - Guía de Onboarding

¡Bienvenido al bootcamp de Git y GitHub! 🎉 Este documento te guiará paso a paso para dominar las herramientas esenciales del desarrollo moderno.

## 📋 Tabla de Contenidos

- [¿Qué es Git y GitHub?](#qué-es-git-y-github)
- [Configuración Inicial](#configuración-inicial)
- [Conceptos Fundamentales](#conceptos-fundamentales)
- [Comandos Esenciales](#comandos-esenciales)
- [Flujo de Trabajo](#flujo-de-trabajo)
- [Mejores Prácticas](#mejores-prácticas)
- [Recursos Adicionales](#recursos-adicionales)

---

## 🤔 ¿Qué es Git y GitHub?

### Git
- **Sistema de control de versiones** distribuido
- Permite rastrear cambios en archivos a lo largo del tiempo
- Funciona localmente en tu computadora
- Es como un "historial" de tu proyecto

### GitHub
- **Plataforma web** que aloja repositorios Git
- Facilita la colaboración en proyectos
- Ofrece herramientas como Issues, Pull Requests, y más
- Es como "Google Drive" para código

---

## ⚙️ Configuración Inicial

### 1. Instalar Git
```bash
# Verificar si Git está instalado
git --version

# Si no está instalado, descárgalo desde:
# https://git-scm.com/downloads
```

### 2. Configurar tu identidad
```bash
# Configurar tu nombre
git config --global user.name "Tu Nombre"

# Configurar tu email
git config --global user.email "tu.email@ejemplo.com"

# Verificar configuración
git config --list
```

### 3. Crear cuenta en GitHub
1. Ve a [github.com](https://github.com)
2. Crea una cuenta gratuita
3. Configura tu perfil

---

## 🧠 Conceptos Fundamentales

### Repositorio (Repo)
- **Carpeta** que contiene tu proyecto
- Puede ser local (en tu PC) o remoto (en GitHub)

### Commit
- **Punto de guardado** en la historia de tu proyecto
- Como un "checkpoint" en un videojuego

### Branch (Rama)
- **Línea de desarrollo** independiente
- Permite trabajar en features sin afectar el código principal

### Remote
- **Conexión** entre tu repo local y GitHub
- Como un "puente" entre tu PC y la nube

---

## 🛠️ Comandos Esenciales

### Inicializar un repositorio
```bash
# Crear un nuevo repo
git init

# Clonar un repo existente
git clone https://github.com/usuario/repo.git
```

### Estados de archivos
```bash
# Ver estado de archivos
git status

# Agregar archivos al staging
git add archivo.txt
git add .  # Agregar todos los archivos

# Hacer commit
git commit -m "Mensaje descriptivo"
```

### Trabajar con ramas
```bash
# Ver ramas
git branch

# Crear nueva rama
git branch nombre-rama

# Cambiar de rama
git checkout nombre-rama
git switch nombre-rama  # Comando más moderno

# Crear y cambiar a nueva rama
git checkout -b nueva-rama
```

### Sincronizar con GitHub
```bash
# Agregar remote
git remote add origin https://github.com/usuario/repo.git

# Subir cambios
git push origin main

# Descargar cambios
git pull origin main
```

---

## 🔄 Flujo de Trabajo Típico

### 1. Trabajo Diario
```bash
# 1. Actualizar tu repo local
git pull origin main

# 2. Crear nueva rama para tu feature
git checkout -b feature/nueva-funcionalidad

# 3. Hacer cambios en tu código
# ... editar archivos ...

# 4. Agregar y commitear cambios
git add .
git commit -m "Agregar nueva funcionalidad"

# 5. Subir tu rama
git push origin feature/nueva-funcionalidad
```

### 2. Crear Pull Request
1. Ve a GitHub en tu navegador
2. Verás un botón "Compare & pull request"
3. Escribe una descripción de tus cambios
4. Asigna revisores si es necesario
5. Haz clic en "Create pull request"

---

## ✅ Mejores Prácticas

### Mensajes de Commit
```bash
# ❌ Malo
git commit -m "fix"

# ✅ Bueno
git commit -m "fix: corregir error de validación en formulario de login"

# Estructura recomendada:
# tipo: descripción breve
# 
# Descripción detallada (opcional)
```

### Tipos de commit
- `feat:` Nueva funcionalidad
- `fix:` Corrección de bug
- `docs:` Cambios en documentación
- `style:` Cambios de formato
- `refactor:` Refactorización de código
- `test:` Agregar o modificar tests

### Organización de ramas
```
main/master     ← Código de producción
├── develop     ← Código de desarrollo
├── feature/    ← Nuevas funcionalidades
├── hotfix/     ← Correcciones urgentes
└── release/    ← Preparación de releases
```

---

## 🎯 Ejercicios Prácticos

### Ejercicio 1: Primer Repositorio
1. Crea una carpeta llamada `mi-primer-proyecto`
2. Inicializa un repositorio Git
3. Crea un archivo `README.md`
4. Haz tu primer commit
5. Sube el repo a GitHub

### Ejercicio 2: Colaboración
1. Clona un repositorio de un compañero
2. Crea una nueva rama
3. Haz algunos cambios
4. Crea un Pull Request

---

## 🆘 Solución de Problemas Comunes

### "Your branch is ahead of origin/main"
```bash
# Subir tus cambios
git push origin main
```

### "Please commit your changes or stash them"
```bash
# Opción 1: Hacer commit
git add .
git commit -m "Mensaje"

# Opción 2: Guardar temporalmente
git stash
# ... hacer otros cambios ...
git stash pop  # Recuperar cambios
```

### Deshacer último commit
```bash
# Mantener cambios en staging
git reset --soft HEAD~1

# Descartar cambios completamente
git reset --hard HEAD~1
```

---

## 📚 Recursos Adicionales

### Documentación Oficial
- [Git Documentation](https://git-scm.com/doc)
- [GitHub Docs](https://docs.github.com)

### Tutoriales Interactivos
- [Learn Git Branching](https://learngitbranching.js.org/)
- [GitHub Learning Lab](https://lab.github.com/)

### Comandos de Ayuda
```bash
# Ayuda general
git help

# Ayuda de comando específico
git help commit
git help push
```

---

## 🎉 ¡Felicidades!

Has completado el onboarding de Git y GitHub. Ahora tienes las herramientas necesarias para:

- ✅ Controlar versiones de tu código
- ✅ Colaborar en proyectos
- ✅ Trabajar con ramas
- ✅ Sincronizar con GitHub
- ✅ Crear Pull Requests

### Próximos Pasos
1. Practica con proyectos personales
2. Contribuye a proyectos open source
3. Aprende sobre Git Flow
4. Explora GitHub Actions

---

**¡Recuerda: La práctica hace al maestro! 🚀**

*¿Tienes preguntas? ¡No dudes en preguntar!*
