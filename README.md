# 🎓 ProyectoIntApp — Aplicación Educativa Interactiva

Aplicación de escritorio en **Java (Swing)** que apoya el aprendizaje de **matemáticas, física, álgebra lineal, humanidades y teoría general de sistemas**. Permite resolver problemas de forma interactiva, ver el procedimiento paso a paso y practicar con cuestionarios y un minijuego.

> Proyecto integrador — Universidad UCEVA (Unidad Central del Valle del Cauca), Colombia.

---

## ✨ Características

| Área | Módulos |
|------|---------|
| **Matemáticas** | Evaluación de **funciones**, cálculo de **límites** (incluye infinito) e **integrales** (indefinidas simbólicas y definidas con regla de Simpson compuesta) |
| **Física** | **Vectores** (suma, resta, producto punto, producto vectorial, módulo y ángulo; 2D y 3D) y **matrices** 2×2 / 3×3 (suma, resta, multiplicación, transpuesta y determinante) |
| **Álgebra Lineal** | Solución de sistemas de ecuaciones (hasta 5×5) con **Eliminación Gaussiana** y **Gauss-Jordan**, mostrando los pasos |
| **Humanidades** | Lecturas con cuestionario: *Los Transgénicos* y *El Mundo Según Monsanto* |
| **Teoría General de Sistemas** | Minijuego de preguntas con puntos, vidas y temporizador |
| **Extras** | Pantallas de **Ayuda** y **Acerca de** |

Las funciones matemáticas aceptan operadores `+ - * / ^` y las funciones `sin, cos, tan, sqrt, log, exp, abs`. Ejemplo: `x^2 + 3*x + 2`, `sin(x)/x`.

---

## 🧰 Tecnologías

- **Java** + **Swing / AWT** (interfaz gráfica)
- **Apache NetBeans** (proyecto Ant)
- Sin dependencias externas

---

## 🚀 Cómo ejecutarlo

### Requisitos
- **JDK** instalado (el proyecto está configurado en NetBeans con `javac.source=25`; el código compila correctamente con JDK 21, así que no necesitas la versión más reciente).

### Opción 1: NetBeans
1. Abre NetBeans → `File > Open Project` y selecciona la carpeta `ProyectoIntApp`.
2. Clic derecho sobre el proyecto → **Run**.

> Si NetBeans se queja de la versión de Java, cambia en *Properties > Sources > Source/Binary Format* a la versión de tu JDK.

### Opción 2: Línea de comandos
```bash
# Desde la carpeta raíz del proyecto
mkdir out
javac -encoding UTF-8 -d out src/proyectointapp/*.java
java -cp out proyectointapp.ProyectoIntApp
```

---

## 📁 Estructura

```
ProyectoIntApp/
├── src/proyectointapp/
│   ├── ProyectoIntApp.java        # Ventana principal (menú)
│   ├── Matematicas.java           # Menú de matemáticas
│   │   ├── Funciones.java
│   │   ├── Limites.java
│   │   └── Integrales.java
│   ├── Fisica.java                # Menú de física
│   │   ├── Vectores.java
│   │   └── Matrices.java
│   ├── Algebra.java               # Menú de álgebra lineal
│   │   ├── Gaussiana.java
│   │   └── GaussJordan.java
│   ├── Humanidades.java           # Menú de humanidades
│   │   ├── Transgenicos.java
│   │   └── MundoSegunMonsanto.java
│   ├── TeoriaGeneralSistemas.java # Minijuego TGS
│   ├── Ayuda.java
│   └── AcercaDe.java
├── nbproject/                     # Configuración de NetBeans
├── build.xml
└── manifest.mf
```

---

## 👥 Autores

| Nombre | Código |
|--------|--------|
| Santiago Pérez Bastidas | 230252038 |
| Nicholas Alberto Siavichay Ocampo | 230252027 |
| Samuel Felipe Arias Flechas | 230252026 |
| Jose Alberto Riascos Ruiz | 230252048 |

**Versión:** 1.0

---

## 📄 Licencia

Proyecto académico con fines educativos. Si quieres que otras personas puedan reutilizarlo, agrega un archivo `LICENSE` (por ejemplo MIT) al repositorio.
