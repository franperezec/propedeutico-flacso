# Propedéutico de Matemáticas y Programación en Python

**FLACSO Ecuador · Facultad Latinoamericana de Ciencias Sociales**

![Python](https://img.shields.io/badge/Python-3.12%2B-3776AB?logo=python&logoColor=white)
![Notebooks](https://img.shields.io/badge/Notebooks-validados%20por%20ejecuci%C3%B3n-1d6b45)
![Idioma](https://img.shields.io/badge/Idioma-Espa%C3%B1ol-7a1e2b)

Curso propedéutico para estudiantes de posgrado en ciencias sociales **sin experiencia previa en programación**. Construye, desde cero y con rigor matemático, las bases de Python y de las herramientas profesionales de trabajo (Google Colab, VS Code, Git y GitHub, entornos virtuales) que se usan en el resto de la formación.

🌐 **[Sitio del curso](https://franperezec.github.io/propedeutico-flacso/)** — todos los materiales (notebooks, manuales y aplicaciones) en una sola página.

📝 **[Pizarra de clase (Miro)](https://miro.com/app/board/uXjVH8KD80I=/?share_link_id=332769285692)** — los apuntes a mano de los profesores, clase por clase.

📄 **[Sílabo del curso (PDF)](silabo_propedeutico_2026.pdf)** — temario completo, calendario, horarios, evaluación y bibliografía del propedéutico (Maestría en Economía del Desarrollo, FLACSO Ecuador).

---

## Cómo usar este repositorio

Hay dos vías, y ambas están cubiertas por los manuales de la carpeta [`manuales/`](manuales/), pensados para leerse **directamente en el navegador** o descargarse en **PDF** para imprimir o consultar sin conexión:

- 🛠️ [Manual de instalación — VS Code, Python y Git (web)](https://franperezec.github.io/propedeutico-flacso/manuales/manual_instalacion_vscode.html) · [PDF](manuales/manual_instalacion_vscode.pdf) — complétalo **primero**: deja tu equipo listo para todo el curso
- 📖 [Manual de GitHub y tu primer entorno (web)](https://franperezec.github.io/propedeutico-flacso/manuales/manual_github_primer_entorno.html) · [PDF](manuales/manual_github_primer_entorno.pdf)
- 📖 [Manual de tu propio repositorio en GitHub (web)](https://franperezec.github.io/propedeutico-flacso/manuales/manual_tu_propio_repositorio.html) · [PDF](manuales/manual_tu_propio_repositorio.pdf)
- 🧭 [El mapa de las herramientas (web)](https://franperezec.github.io/propedeutico-flacso/manuales/manual_mapa_herramientas.html) · [PDF](manuales/manual_mapa_herramientas.pdf) — manual de consulta para todo el curso: qué hace (y qué no) cada herramienta, el semáforo de VS Code y los errores frecuentes

### Vía A — Google Colab (sin instalar nada)

Cada notebook de la carpeta [`clases/`](clases/) puede abrirse directamente en Colab con el botón *Open in Colab*, o desde este enlace de ejemplo (el notebook de conjuntos y producto cartesiano):

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/franperezec/propedeutico-flacso/blob/main/clases/fundamentos_matematicas/conjuntos_producto_cartesiano.ipynb)

> Recuerda guardar tu propia copia: `Archivo → Guardar una copia en Drive`.

### Vía B — Trabajo local (VS Code + entorno virtual)

Requiere haber completado el [**Manual de instalación**](https://franperezec.github.io/propedeutico-flacso/manuales/manual_instalacion_vscode.html) (VS Code, Python 3.12+ y Git). Luego, en la terminal:

```bash
# 1. Clonar el repositorio
git clone https://github.com/franperezec/propedeutico-flacso.git
cd propedeutico-flacso
```

Después, en VS Code: `Ctrl+Shift+P` (o `⇧⌘P` en Mac) → **Python: Create Environment** → **Venv** → marcar `requirements.txt` para instalar las dependencias del curso. Equivalente por terminal:

```bash
# 2. Crear y activar el entorno virtual
python -m venv .venv
# Windows (PowerShell):
.venv\Scripts\Activate.ps1
# macOS / Linux:
source .venv/bin/activate

# 3. Instalar las dependencias del curso
python -m pip install -r requirements.txt
```

### Actualizar los materiales

Los materiales nuevos se publican en este mismo repositorio a medida que avanza el curso. Con el repositorio abierto, basta:

```bash
git pull
```

---

## Estructura del repositorio

```
propedeutico-flacso/
├── clases/                        # Notebooks del curso, por tema (patrón «Yo hago / Tú haces»)
│   ├── fundamentos_matematicas/   # Conjuntos y producto cartesiano
│   │   └── conjuntos_producto_cartesiano.ipynb
│   ├── fundamentos_python/        # Taller de fundamentos de programación
│   │   └── fundamentos_python_01.ipynb
│   ├── matrices/                  # Álgebra lineal con NumPy y regresión (datos junto al notebook)
│   │   ├── numpy_para_economistas.ipynb
│   │   ├── numpy_para_economistas_02.ipynb
│   │   ├── regresion_consumo.ipynb
│   │   ├── matrices_ejemplo.xlsx
│   │   ├── datos_consumo.csv
│   │   └── datos_salarios.csv
│   └── calculo_simbolico/         # Cálculo simbólico con SymPy
│       ├── intro_sympy_algebra.ipynb
│       ├── reglas_derivacion_sympy.ipynb
│       └── sympy_optimizacion.ipynb
├── manuales/                      # Guías paso a paso para preparar tu equipo
│   ├── manual_instalacion_vscode.html
│   ├── manual_github_primer_entorno.html
│   ├── manual_tu_propio_repositorio.html
│   └── manual_mapa_herramientas.html
├── aplicaciones/                  # Índice de aplicaciones web interactivas del curso
│   └── README.md
├── silabo_propedeutico_2026.pdf   # Sílabo oficial (temario completo y calendario)
├── requirements.txt               # Dependencias del curso, con versiones fijadas
├── LICENSE                        # Licencia MIT
└── README.md
```

---

## Contenido del curso

El material se organiza **por tema**, siguiendo las subcarpetas de [`clases/`](clases/). Este índice recoge únicamente el material ya publicado; el curso cubre más temas de los que aparecen aquí — el temario completo, con su calendario, está en el [sílabo (PDF)](silabo_propedeutico_2026.pdf).

### Fundamentos de matemáticas

| Notebook | Qué cubre |
|----------|-----------|
| [`conjuntos_producto_cartesiano.ipynb`](clases/fundamentos_matematicas/conjuntos_producto_cartesiano.ipynb) | **Conjuntos y producto cartesiano:** sistemas numéricos, operaciones fundamentales entre conjuntos y producto cartesiano — y, en paralelo, Python y Google Colab desde cero |

*Aplicaciones relacionadas:* [Tablas de Verdad](https://true-table-prope-1--true-table-prope.us-east4.hosted.app/) (lógica proposicional) · [Función lineal y cuadrática](https://www.wolframcloud.com/obj/faperezfl/MisParabolas) (funciones).

### Fundamentos de programación en Python

| Notebook | Qué cubre |
|----------|-----------|
| [`fundamentos_python_01.ipynb`](clases/fundamentos_python/fundamentos_python_01.ipynb) | **Taller de fundamentos:** algoritmos, variables y tipos de datos, operadores, listas, tuplas y diccionarios, estructuras de control (`if`, `for`, `while`) y funciones, con un ejercicio integrador de cierre |

### Álgebra lineal y matrices

La serie de notebooks de matrices — *NumPy para economistas* (partes 1 y 2) y la regresión de la función de consumo por MCO — usa la librería del curso y está documentada, con sus datos, en la sección [Librería del curso](#librería-del-curso-algebra-lineal-sheets).

*Aplicación relacionada:* [Transformaciones lineales](https://www.wolframcloud.com/obj/faperezfl/Transformaciones%20Lineales) (aplicaciones lineales).

### Cálculo simbólico y optimización

| Notebook | Qué cubre |
|----------|-----------|
| [`intro_sympy_algebra.ipynb`](clases/calculo_simbolico/intro_sympy_algebra.ipynb) | **Introducción a SymPy — símbolos y álgebra:** declarar símbolos sobre los reales, sustituir valores, conservar resultados exactos y resolver ecuaciones, con aplicaciones al equilibrio de mercado |
| [`reglas_derivacion_sympy.ipynb`](clases/calculo_simbolico/reglas_derivacion_sympy.ipynb) | **Límites, derivadas y series de Taylor:** las reglas de derivación comprobadas paso a paso con SymPy y la aproximación ln(1+r) ≈ r para tasas pequeñas |
| [`sympy_optimizacion.ipynb`](clases/calculo_simbolico/sympy_optimizacion.ipynb) | **Optimización analítica y métodos numéricos:** condiciones de primer y segundo orden, Hessianas y formas cuadráticas, con SymPy, NumPy y Matplotlib |

*Aplicaciones relacionadas:* [Derivada como límite](https://www.wolframcloud.com/obj/faperezfl/LimiteDerivada) · [Función y derivada](https://www.wolframcloud.com/obj/faperezfl/Funcion%20y%20Derivada) · [Series de Taylor](https://www.wolframcloud.com/obj/faperezfl/TaylorSeries).

---

## Librería del curso: `algebra-lineal-sheets`

Para este curso desarrollamos una librería de Python que permite hacer **álgebra lineal con matrices definidas en Google Sheets, Excel o CSV**: escribes tus matrices en una hoja de cálculo y las cargas como arreglos de NumPy listos para operar. Se instala con:

```bash
pip install algebra-lineal-sheets
```

En Google Colab no se necesita nada más.

- **Página en PyPI:** https://pypi.org/project/algebra-lineal-sheets/
- **Documentación completa:** https://github.com/franperezec/algebra-lineal-sheets

La librería se usa en la serie de notebooks de matrices de este repositorio:

| Notebook | Qué cubre | Datos que usa |
|----------|-----------|---------------|
| [`numpy_para_economistas.ipynb`](clases/matrices/numpy_para_economistas.ipynb) | **NumPy para economistas — parte 1:** arreglos y operaciones matriciales, con las matrices leídas desde una hoja de cálculo | [`matrices_ejemplo.xlsx`](clases/matrices/matrices_ejemplo.xlsx) — matrices `A`, `B`, `v1`, `v2` y `b0` |
| [`numpy_para_economistas_02.ipynb`](clases/matrices/numpy_para_economistas_02.ipynb) | **NumPy para economistas — parte 2:** vectorización, broadcasting, sistemas $Ax=b$ y descomposición espectral | — |
| [`regresion_consumo.ipynb`](clases/matrices/regresion_consumo.ipynb) | **Regresión lineal con matrices:** la función de consumo estimada por MCO con álgebra matricial, verificada con `statsmodels` | [`datos_consumo.csv`](clases/matrices/datos_consumo.csv) · [`datos_salarios.csv`](clases/matrices/datos_salarios.csv) |

---

## Aplicaciones interactivas

Herramientas web del curso, sin instalación — se abren en el navegador. El índice completo está en [`aplicaciones/`](aplicaciones/).

| Aplicación | Qué hace | Enlace |
|------------|----------|--------|
| **Tablas de Verdad** | Genera la tabla de verdad de una expresión lógica (AND, OR, NOT, `->`, `<->`) — lógica proposicional | [Abrir aplicación](https://true-table-prope-1--true-table-prope.us-east4.hosted.app/) |
| **Función lineal y cuadrática** | Mueve los coeficientes de una recta y de una parábola y observa cómo cambian la pendiente, el vértice y los cortes con los ejes — funciones | [Abrir aplicación](https://www.wolframcloud.com/obj/faperezfl/MisParabolas) |
| **Transformaciones lineales** | Aplica una matriz 2×2 a una figura del plano y visualiza el efecto geométrico de la transformación: rotaciones, escalamientos y reflexiones — álgebra lineal | [Abrir aplicación](https://www.wolframcloud.com/obj/faperezfl/Transformaciones%20Lineales) |
| **Derivada como límite** | Muestra la recta secante convirtiéndose en tangente: la derivada como límite del cociente incremental cuando h → 0 — cálculo diferencial | [Abrir aplicación](https://www.wolframcloud.com/obj/faperezfl/LimiteDerivada) |
| **Función y derivada** | Grafica una función junto a su derivada para conectar el signo de f′ con el crecimiento y los puntos críticos — derivadas y optimización | [Abrir aplicación](https://www.wolframcloud.com/obj/faperezfl/Funcion%20y%20Derivada) |
| **Series de Taylor** | Compara una función con su polinomio de Taylor: elige el punto de expansión y el número de términos, y observa la gráfica y el error absoluto — series de Taylor | [Abrir aplicación](https://www.wolframcloud.com/obj/faperezfl/TaylorSeries) |

---

## Metodología

Cada notebook sigue el patrón **«Yo hago / Tú haces»**: primero el docente ejecuta y explica; luego el estudiante resuelve un ejercicio análogo con solución oculta en celdas colapsables, para intentar antes de mirar. Todos los notebooks están escritos íntegramente en español (código, comentarios y texto), usan semillas deterministas cuando hay componentes aleatorios y se validan mediante **ejecución completa** antes de publicarse. La notación matemática acompaña siempre al código: la sintaxis de Python se presenta como traducción casi literal del lenguaje de la pizarra.

## Requisitos previos

Ninguno de programación. Para la Vía A basta una cuenta de Google (Gmail); para la Vía B, seguir el [Manual de instalación](https://franperezec.github.io/propedeutico-flacso/manuales/manual_instalacion_vscode.html) y tener una cuenta de GitHub verificada. Cualquier Python **3.12 o superior** sirve.

---

## Docentes

**Francisco Pérez M.** — FLACSO Ecuador
Sitio web: [franciscoperezm.com](https://franciscoperezm.com) · GitHub: [@franperezec](https://github.com/franperezec) · Correo: [fperezfl@flacso.edu.ec](mailto:fperezfl@flacso.edu.ec)

**David Villamar C.** — FLACSO Ecuador
Correo: [davillamarfl@flacso.edu.ec](mailto:davillamarfl@flacso.edu.ec)

Dudas del curso: usa el aula virtual ([Blackboard](https://flacsosaas.blackboard.com/)) o el canal indicado en clase, no los *issues* de este repositorio.

## Cómo citar

Si reutilizas estos materiales:

> Pérez M., F. y Villamar, D. (2026). *Propedéutico de Matemáticas y Programación en Python* [Materiales de curso]. FLACSO Ecuador. https://github.com/franperezec/propedeutico-flacso

## Licencia

Este repositorio se distribuye bajo la licencia [MIT](LICENSE): puedes usar, copiar, modificar y redistribuir los materiales, siempre que conserves el aviso de copyright y la licencia.
