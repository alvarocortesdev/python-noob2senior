Copyright (c) 2025 [Alvaro Cortés Opazo(https://alvarocortes.cl/)]

Este material es parte del curso de Python publicado en [https://github.com/alvarocortesdev/python-noob2senior](https://github.com/alvarocortesdev/python-noob2senior).
Distribuido bajo la licencia CC BY-NC 4.0.
Para más detalles, consulta el archivo LICENSE en el repositorio.

---

# Roadmap 🐍 Python 2025 🐍

Este roadmap fue generado con el afán de robustecer mis conocimientos y partir desde cero, derribando todo conocimiento y seguridad sobre lo que sabía de Python. La finalidad es re-aprender, desde lo más básico e intentando construir una forma de aprender como me hubiese gustado que me enseñaran en la universidad.
Este camino está estructurado para llevarte desde los conceptos más básicos hasta los más avanzados, culminando en áreas de especialización. 

La clave es la práctica constante: intenta construir algo pequeño con cada nuevo concepto que aprendas.

## ¿Estás listo?
---

### 🎓 **Fase 0: Preparación del Entorno y Fundamentos de la Programación**

Antes de escribir una línea de Python, es crucial preparar tu entorno y entender los conceptos universales de la programación.

* [ ] **Configuración del Entorno**

  * [ ] Entender la diferencia entre Python 2 y Python 3 (y por qué usar siempre Python 3).
  * [ ] Instalar Python en tu sistema operativo (Windows, macOS, Linux).
  * [ ] Verificar la instalación en la terminal (`python --version` o `python3 --version`).
  * [ ] Aprender a usar el intérprete interactivo de Python.
* [ ] **Instalación y Uso de un Editor de Código / IDE**

  * [ ] Diferencia entre un editor de texto (Sublime Text, Atom) y un IDE (Integrated Development Environment).
  * [ ] Instalar y configurar un editor popular como **VS Code** con extensiones recomendadas (Python, Pylance).
  * [ ] Alternativa: Instalar y configurar un IDE robusto como **PyCharm** (Community o Professional).
* [ ] &#x20;**Gestión de Versiones de Python**

  * [ ] Pyenv para gestionar múltiples versiones de Python
  * [ ] Python Launcher para Windows (py.exe)
  * [ ] Entender cuándo y por qué necesitarías diferentes versiones
* [ ] **Fundamentos de la Terminal/Línea de Comandos**

  * [ ] Navegar entre directorios (`cd`).
  * [ ] Listar archivos (`ls` / `dir`).
  * [ ] Crear y eliminar directorios (`mkdir`, `rmdir`).
  * [ ] Ejecutar un script de Python (`python nombre_del_archivo.py`).
* [ ] **Shell scripting básico**

  * [ ] Variables de entorno
  * [ ] Redirección de outputs (>, |)
  * [ ] Scripts bash simples
* [ ] **Conceptos Básicos de Programación**

  * [ ] ¿Qué es un algoritmo?
  * [ ] ¿Qué es una variable?
  * [ ] ¿Qué es el pseudocódigo?
  * [ ] Entender el flujo de un programa (secuencial, condicional, iterativo).
* [ ] **Logging básico desde el inicio**

  * [ ] Configuración de `logging`: niveles (`DEBUG`, `INFO`, `WARNING`, `ERROR`, `CRITICAL`), handlers, formateadores.
  * [ ] Registro a archivo y a consola; por qué evitar `print()` para logs de aplicación.

---

### 🐍 **Fase 1: Python Básico - El Núcleo del Lenguaje**

Aquí aprenderás la sintaxis y los bloques de construcción fundamentales de Python.

* [ ] **Sintaxis y Variables**

  * [ ] Comentarios (`#`).

  * [ ] Variables: asignación y reglas de nombramiento (snake\_case).

  * [ ] Tipos de datos primitivos:

    * [ ] `int` (enteros).
    * [ ] `float` (decimales).
    * [ ] `str` (cadenas de texto).
    * [ ] `bool` (booleanos: `True`, `False`).
    * [ ] `NoneType` (`None`).

  * [ ] La función `type()` para verificar el tipo de una variable.
* [ ] **Operadores**

  * [ ] Aritméticos: `+`, `-`, `*`, `/`, `//` (división entera), `%` (módulo), `**` (potencia).
  * [ ] De asignación: `=`, `+=`, `-=`, `*=`, `/=`.
  * [ ] De comparación: `==`, `!=`, `>`, `<`, `>=`, `<=`.
  * [ ] Lógicos: `and`, `or`, `not`.
  * [ ] Operadores de identidad: is, is not
  * [ ] Operadores de membresía: in, not in
  * [ ] Operador walrus := (Python 3.8+)
  * [ ] Operador ternario: x if cond else y
* [ ] **Manejo de Cadenas de Texto (Strings)**

  * [ ] Concatenación (`+`).
  * [ ] Métodos comunes: `.upper()`, `.lower()`, `.strip()`, `.replace()`, `.split()`.
  * [ ] Indexación y Slicing (`mi_string[0]`, `mi_string[1:5]`).
  * [ ] F-strings (formateo moderno de cadenas): `f"Hola, {nombre}"`.
  * [ ] **Unicode y codificación**

    * [ ] `str.encode()` / `bytes.decode()`; errores comunes (mojibake).
    * [ ] `codecs`, UTF-8 por defecto, BOM, manejo de archivos con codificación.
* [ ] **Fecha y zona horaria**

  * [ ] `datetime` vs `date`, formatos ISO-8601.
  * [ ] `timezone`/`zoneinfo`: zonas horarias, aware vs naive datetimes.
* [ ] **Entrada y Salida Básica**

  * [ ] `print()`: Mostrar datos en la consola.
  * [ ] `input()`: Recibir datos del usuario.
  * [ ] Conversión de tipos (casting): `int()`, `str()`, `float()`.
* [ ] **Control de Flujo: Condicionales**

  * [ ] `if`.
  * [ ] `if-else`.
  * [ ] `if-elif-else`.
* [ ] **Control de Flujo: Bucles**

  * [ ] Bucle `for` (para iterar sobre secuencias).

    * [ ] La función `range()`.
  * [ ] Bucle `while` (para repetir mientras una condición sea verdadera).
  * [ ] Sentencias `break` (para salir de un bucle) y `continue` (para saltar a la siguiente iteración).
  * [ ] Else en bucles
  * [ ] for...else y while...else
  * [ ] Cuándo se ejecuta el else en bucles
  * [ ] match/case (Python 3.10+)
* [ ] **Módulos “fundamentales ocultos”**

  * [ ] `itertools`
  * [ ] `functools` (`lru_cache`, `partial`)
  * [ ] `operator`
  * [ ] `collections` (`Counter`, `defaultdict`, `namedtuple`)
* [ ] **Mini-proyecto**

  * [ ] **CLI** que parsea CSV (Unicode) y genera un resumen por fecha con **logging** a archivo.

---

### 🗃️ **Fase 2: Estructuras de Datos Fundamentales**

Cómo organizar y almacenar colecciones de datos de manera eficiente.

* [ ] **Listas (`list`)**

  * [ ] Creación de listas `[]`.
  * [ ] Mutabilidad (pueden ser modificadas).
  * [ ] Indexación y slicing.
  * [ ] Métodos principales: `.append()`, `.insert()`, `.pop()`, `.remove()`, `.sort()`, `.reverse()`.
  * [ ] Listas anidadas (matrices).
  * [ ] Shallow copy vs deep copy
  * [ ] collections.deque para operaciones eficientes
* [ ] **Tuplas (`tuple`)**

  * [ ] Creación de tuplas `()`.
  * [ ] Inmutabilidad (no pueden ser modificadas después de su creación).
  * [ ] Casos de uso: cuando los datos no deben cambiar (coordenadas, constantes).
  * [ ] Desempaquetado de tuplas: `x, y = (10, 20)`.
* [ ] **Diccionarios (`dict`)**

  * [ ] Creación de diccionarios `{}` (pares clave-valor).
  * [ ] Acceso a valores mediante claves (`mi_diccionario['clave']`).
  * [ ] Métodos principales: `.keys()`, `.values()`, `.items()`, `.get()`, `.pop()`.
  * [ ] Iterar sobre diccionarios.
* [ ] **Conjuntos (`set`)**

  * [ ] Creación de conjuntos `{}` o `set()`.
  * [ ] Elementos únicos y desordenados.
  * [ ] Operaciones de conjuntos: unión (`|`), intersección (`&`), diferencia (`-`).
* [ ] &#x20;**Iterables e Iteradores**

  * [ ] Protocolo de iteración en Python
  * [ ] Diferencia entre iterable e iterador
  * [ ] La función iter() y next()
  * [ ] StopIteration exception
* [ ] **Complejidad Algorítmica**

  * [ ] Notación Big-O básica
  * [ ] Complejidad de operaciones comunes
* [ ] **Comprensiones (Comprehensions)**

  * [ ] Una forma "Pythonica" y concisa de crear estructuras de datos.
  * [ ] List Comprehensions: `[x*x for x in range(10)]`.
  * [ ] Dictionary Comprehensions: `{k: v for k, v in una_lista_de_tuplas}`.
  * [ ] Set Comprehensions.
  * [ ] Generator expressions y su eficiencia en memoria
  * [ ] Cuándo NO usar comprehensions (legibilidad vs concisión)
  * [ ] Comprehensions anidadas y sus límites
  * [ ] Generadores asíncronos (async comprehensions)
* [ ] &#x20;**Mutabilidad vs Inmutabilidad**

  * [ ] Concepto fundamental que afecta todo el código Python
  * [ ] Comportamiento de variables con objetos mutables vs inmutables
  * [ ] El problema de las listas como argumentos por defecto
* [ ] **Validación de datos**

  * [ ] `pydantic` / `pydantic-settings` para validar inputs y configuración.
* [ ] **Persistencia simple**

  * [ ] `csv`, `json` y **Parquet** con `pyarrow` (intro).
* [ ] **Mini-proyecto**

  * [ ] **Transformador de datos**: lee CSV/JSON, valida con **Pydantic** y exporta a **Parquet**.

---

### 🏛️ **Fase 3: Funciones y Programación Orientada a Objetos (POO)**

Abstraer y organizar tu código para que sea reutilizable y escalable.

* [ ] **Funciones**

  * [ ] Definición de funciones con `def`.
  * [ ] Parámetros y argumentos.
  * [ ] Sentencia `return` para devolver valores.
  * [ ] Argumentos por defecto.
  * [ ] Argumentos posicionales y de palabra clave (keyword arguments).
  * [ ] `*args` y `**kwargs` para un número variable de argumentos.
  * [ ] Alcance (Scope) de las variables: Local vs. Global.
  * [ ] Funciones Lambda (funciones anónimas).
  * [ ] Function annotations
* [ ] &#x20;**Closures y Funciones de Orden Superior**

  * [ ] Funciones que retornan funciones
  * [ ] Closures y el concepto de "captured variables"
  * [ ] Aplicaciones prácticas en el mundo real
* [ ] **Programación Orientada a Objetos (POO)**

  * [ ] Concepto de **Clases** y **Objetos**.
  * [ ] Definición de una clase con `class`.
  * [ ] El método constructor `__init__()`.
  * [ ] **Atributos**: de instancia y de clase.
  * [ ] **Métodos**: de instancia, de clase (`@classmethod`) y estáticos (`@staticmethod`).
  * [ ] Los 4 Pilares de la POO:

    * [ ] **Encapsulamiento**: Atributos públicos, protegidos (`_`) y privados (`__`).
    * [ ] **Herencia**: Crear subclases que heredan de una clase padre. Uso de `super()`.
    * [ ] **Polimorfismo**: Sobreescritura de métodos (Method Overriding).
    * [ ] **Abstracción**: Clases base abstractas (`abc` module).
  * [ ] Patrones de Diseño

    * [ ] Singleton, Factory, Observer
    * [ ] Patrones específicos Python (Context Manager, State)
  * [ ] Métodos Mágicos (Dunder Methods): `__str__`, `__repr__`, `__len__`, etc.
  * [ ] Mixins
  * [ ] Protocolos estructurales (typing.Protocol)
  * [ ] Dataclasses (Python 3.7+)
* [ ] &#x20;**Protocolos de Python**

  * [ ] Protocolo de secuencia
  * [ ] Protocolo de contexto
  * [ ] Protocolo descriptor
* [ ] **Typing moderno**

  * [ ] `TypedDict`, `Literal`, `Final`, `Annotated`, `Protocol` (polimorfismo estructural).
* [ ] **Slots & dataclasses**

  * [ ] `@dataclass(slots=True)` para menor uso de memoria.
* [ ] **Diseño**

  * [ ] Principios **SOLID** aplicados con ejemplos en Python.
* [ ] **Mini-proyecto**

  * [ ] **Pequeña librería** con interfaces vía `Protocol`, `dataclasses` y **tests unitarios**.

---

### ⚙️ **Fase 4: Python Intermedio - Herramientas y Módulos**

Conceptos que te permitirán construir aplicaciones más complejas y robustas.

* [ ] **Manejo de Errores y Excepciones**

  * [ ] Bloques `try`, `except`, `else`, `finally`.
  * [ ] Capturar excepciones específicas (`ValueError`, `TypeError`).
  * [ ] Lanzar excepciones con `raise`.
* [ ] &#x20;**Creación de Excepciones Personalizadas**

  * [ ] Cuándo y cómo crear tus propias excepciones
  * [ ] Jerarquía de excepciones
  * [ ] Best practices para mensajes de error
* [ ] **Manejo de Archivos**

  * [ ] Abrir y cerrar archivos con `open()`.
  * [ ] El gestor de contexto `with open(...) as ...:` (la forma correcta de hacerlo).
  * [ ] Modos de apertura: `'r'` (lectura), `'w'` (escritura), `'a'` (añadir), `'b'` (binario).
  * [ ] Trabajar con rutas de archivo: módulo `os` y `pathlib`.
  * [ ] Archivos temporales (tempfile module)
* [ ] **Módulos y Paquetes**

  * [ ] Cómo importar módulos: `import modulo`, `from modulo import funcion`.
  * [ ] Creación de tus propios módulos (archivos `.py`).
  * [ ] Creación de paquetes (directorios con un archivo `__init__.py`).
  * [ ] &#x20;El sistema de importación de Python en profundidad
  * [ ] Imports circulares y cómo evitarlos
  * [ ] **all** y su propósito
  * [ ] Imports relativos vs absolutos
  * [ ] Namespace packages
  * [ ] Relative imports
* [ ] **Packaging moderno**

  * [ ] **PEP 621**: `pyproject.toml` con `build`/`hatch`/`poetry`.
  * [ ] `entry_points` para CLIs.
* [ ] **Gestión de Entornos y Dependencias**

  * [ ] Entornos Virtuales Básicos

    * [ ] ¿Por qué son esenciales? (Aislar dependencias de proyectos)
    * [ ] Crear y activar un entorno con el módulo venv
    * [ ] Estructura de un entorno virtual
  * [ ] Gestión Moderna de Dependencias

    * [ ] **Poetry**: El gestor de dependencias moderno

      * [ ] Instalación y configuración inicial
      * [ ] pyproject.toml vs requirements.txt
      * [ ] Comandos esenciales: poetry add, poetry install, poetry update
      * [ ] Gestión de dependencias de desarrollo vs producción
      * [ ] Lock files y reproducibilidad
    * [ ] **Pipenv**: Alternativa a Poetry

      * [ ] Pipfile y Pipfile.lock
      * [ ] Ventajas y desventajas vs Poetry
    * [ ] **pip-tools**: Para proyectos que prefieren pip

      * [ ] pip-compile y pip-sync
      * [ ] requirements.in vs requirements.txt
    * [ ] **uv** (opcional) para instalación/resolución ultrarrápida.
* [ ] **Resolución de Conflictos de Dependencias**

  * [ ] Entender el dependency hell
  * [ ] Estrategias para resolver conflictos
  * [ ] Uso de **constraints files**.
* [ ] **Clientes HTTP**

  * [ ] `httpx` (sync/async) además de `requests`.
* [ ] **Serialización de Datos**

  * [ ] pickle, JSON, YAML, msgpack
  * [ ] Consideraciones de seguridad
  * [ ] **Evitar `pickle`** en límites de confianza; preferir **JSON/MessagePack**.
* [ ] **Type Hints y Tipado Estático**

  * [ ] Anotaciones de tipo básicas
  * [ ] typing module: List, Dict, Optional, Union, etc.
  * [ ] Generics y TypeVar
  * [ ] Mypy para verificación estática
* [ ] **Mini-proyecto**

  * [ ] **Empaquetar tu librería** en `pyproject.toml` y publicar en **TestPyPI**.

---

### 🛠️ **Fase 5: Buenas Prácticas y Herramientas Profesionales**

Escribir código no es suficiente. Hay que escribirlo bien y colaborar eficazmente.

* [ ] **Control de Versiones con Git**

  * [ ] Conceptos básicos: repositorio, commit, branch, merge, pull, push.
  * [ ] Flujo de trabajo básico: `git add`, `git commit`, `git push`.
  * [ ] Usar plataformas como GitHub, GitLab o Bitbucket para alojar tus repositorios.
* [ ] **Estilo de Código y Linting**

  * [ ] **PEP 8**: La guía de estilo oficial para el código Python.
  * [ ] **Linters** para verificar el estilo automáticamente: `Flake8`, `Pylint`.
  * [ ] **Formatters** para ordenar el código automáticamente: `Black`, `isort`.
  * [ ] **Ruff** (linter+formatter ultrarrápido) junto a Black/isort.
* [ ] &#x20;**Pre-commit Hooks y Automatización de Calidad**

  * [ ] Instalación y configuración de pre-commit

    * [ ] El archivo .pre-commit-config.yaml
    * [ ] Hooks esenciales: black, flake8, mypy, isort
    * [ ] Security linters (**Bandit**, **Safety**)
    * [ ] **Secret scanning** con **detect-secrets**
  * [ ] Hooks personalizados

    * [ ] Verificación de secrets
    * [ ] Validación de archivos JSON/YAML
    * [ ] Tests automáticos antes del commit
  * [ ] Integración con CI/CD

    * [ ] pre-commit.ci
    * [ ] Ejecución en pipelines
* [ ] **Testing (Pruebas)**

  * [ ] La importancia de las pruebas de software.
  * [ ] Pruebas unitarias con el módulo `unittest`.
  * [ ] Framework de pruebas **`pytest`** (estándar de la industria).
  * [ ] Conceptos: aserciones, fixtures, mocks.
  * [ ] Test parametrizados
  * [ ] Property-based testing (Hypothesis)
  * [ ] Fuzzing básico
  * [ ] **Testing Avanzado**

    * [ ] Mocking Avanzado

      * [ ] unittest.mock en profundidad
      * [ ] Mock, MagicMock, patch
      * [ ] Mocking de side effects y excepciones
      * [ ] Context managers para mocking
      * [ ] pytest-mock para mejor integración
    * [ ] Testing de APIs

      * [ ] pytest + requests para APIs externas
      * [ ] httpx para testing asíncrono
      * [ ] responses y requests-mock para mockear HTTP
      * [ ] Testing de endpoints con FastAPI TestClient
      * [ ] Testing con Django REST Framework APIClient
      * [ ] Validación de schemas con jsonschema
    * [ ] Property-based Testing

      * [ ] Hypothesis framework
      * [ ] Generación automática de casos de prueba
* [ ] &#x20;**Test Coverage**

  * [ ] Coverage.py
  * [ ] Qué porcentaje de coverage es realista
  * [ ] Integration tests vs unit tests
  * [ ] **Umbral mínimo >85%** en el pipeline.
* [ ] **Depuración (Debugging)**

  * [ ] Uso de `print()` para depuración simple (y por qué no es ideal).
  * [ ] Uso del depurador de Python (`pdb`).
  * [ ] Usar las herramientas de depuración integradas en VS Code o PyCharm.
* [ ] **Refactoring**

  * [ ] Técnicas básicas (extract method, rename)
  * [ ] Herramientas (Rope, Redbaron)
* [ ] &#x20;**Profiling y Optimización**

  * [ ] cProfile y profile
  * [ ] line\_profiler para análisis línea por línea
  * [ ] memory\_profiler
  * [ ] Cuándo optimizar (y cuándo no)
* [ ] &#x20;**Documentación**

  * [ ] Docstrings: Google Style vs NumPy Style
  * [ ] Sphinx para documentación automática
  * [ ] README.md efectivos
  * [ ] Type annotations en docstrings
* [ ] **Observabilidad**

  * [ ] **OpenTelemetry**: nociones básicas de traces/metrics/logs.
* [ ] **Mini-proyecto**

  * [ ] **Pipeline de CI (GitHub Actions)** que ejecuta linters, tests, coverage y safeties.

---

### 🚀 **Fase 6: Python Avanzado - Dominando el Lenguaje**

Características potentes que te diferenciarán como un desarrollador senior.

* [ ] **Programación Funcional**

  * [ ] Funciones como ciudadanos de primera clase.
  * [ ] `map()`, `filter()`, `reduce()`.
* [ ] **Decoradores (`Decorators`)**

  * [ ] Entender qué son y para qué sirven (extender la funcionalidad de una función).
  * [ ] Sintaxis con `@`.
  * [ ] Crear tus propios decoradores.
  * [ ] Decoradores con Parámetros
  * [ ] Decoradores de Clase
  * [ ] Property Decorators en Profundidad
* [ ] **Generadores (`Generators`)**

  * [ ] La palabra clave `yield`.
  * [ ] Creación de iteradores eficientes en memoria.
  * [ ] Expresiones generadoras.
* [ ] **Gestores de Contexto (`Context Managers`)**

  * [ ] Entender cómo funciona la sentencia `with`.
  * [ ] Crear tus propios gestores de contexto con `__enter__` y `__exit__`.
  * [ ] **Avanzado**: `contextlib` (`contextmanager`, `suppress`, `ExitStack`).
* [ ] **Concurrencia y Paralelismo**

  * [ ] Diferencia entre concurrencia y paralelismo.
  * [ ] **`threading`**: Para operaciones de I/O-bound.
  * [ ] **`multiprocessing`**: Para operaciones de CPU-bound y el GIL (Global Interpreter Lock).
  * [ ] El GIL (Global Interpreter Lock) en Profundidad

    * [ ] ¿Qué es exactamente el GIL?

      * [ ] Historia y razón de su existencia
      * [ ] Cómo funciona internamente
    * [ ] Implicaciones del GIL

      * [ ] Por qué Python no puede usar múltiples cores efectivamente con threads
      * [ ] Diferencia entre CPU-bound y I/O-bound tasks
      * [ ] Cuándo el GIL no es un problema
    * [ ] Estrategias para superar el GIL

      * [ ] Multiprocessing como solución
      * [ ] Usar extensiones en C (Cython, ctypes)
      * [ ] Alternativas: Jython, IronPython, PyPy
    * [ ] El futuro del GIL

      * [ ] PEP 703 y Python sin GIL
      * [ ] Subinterpreters (PEP 554)
  * [ ] **`asyncio`**: Programación asíncrona con `async` y `await` para I/O concurrente de alto rendimiento.
  * [ ] **Async I/O real**: `asyncio` + `aiofiles`/`httpx`; patrones (fan-out, timeouts, backoff).
  * [ ] AsyncIO avanzado (task groups, queues)
  * [ ] Trio como alternativa a asyncio
  * [ ] concurrent.futures (ThreadPoolExecutor, ProcessPoolExecutor)
  * [ ] Queue y comunicación entre threads/procesos
  * [ ] Locks, Semaphores, Events
  * [ ] El problema de race conditions
  * [ ] **Concurrencia & CPU**: `ProcessPoolExecutor` + **diseño idempotente**.
* [ ] &#x20;**Metaprogramación**

  * [ ] getattr, setattr, hasattr dinámicos
  * [ ] **getattribute** vs **getattr**
  * [ ] Descriptors en profundidad
  * [ ] **Metaclases**

    * [ ] Qué son y cuándo usarlas (spoiler: casi nunca)
    * [ ] El patrón Singleton con metaclases
* [ ] **Gestión de Memoria**

  * [ ] Garbage collection en Python
  * [ ] Reference counting
  * [ ] Weak references
* [ ] **C Extensions**

  * [ ] CFFI
  * [ ] Cython básico
* [ ] **Paralelismo científico**

  * [ ] **Numba/Cython** cuando la vectorización con NumPy no basta.
* [ ] **Mini-proyecto**

  * [ ] **Descargador asíncrono** con rate-limit y reintentos exponenciales; **profiling** con `cProfile`.

---

### 🌐 **Fase 7: Especialización y Ecosistema Python**

Python es un universo. Elige tu camino y profundiza en sus librerías más populares.

* [ ] **Desarrollo Web (Backend)**

  * [ ] Fundamentos de HTTP (request/response, métodos, status codes).
  * [ ] **Frameworks Web**:

    * [ ] **Flask**: Micro-framework, ideal para empezar y para APIs pequeñas.
    * [ ] **Django**: Framework "con baterías incluidas", para aplicaciones grandes y complejas.
  * [ ] **APIs REST**:

    * [ ] **Django REST Framework (DRF)**.
    * [ ] **FastAPI**: Moderno, rápido, basado en `asyncio` y tipado estático.
  * [ ] **ORM (Object-Relational Mapping)**: `SQLAlchemy`, Django ORM.
  * [ ] **Bases de Datos**: PostgreSQL, MySQL, SQLite.
  * [ ] **Seguridad Web**

    * [ ] OWASP Top 10
    * [ ] SQL Injection, XSS, CSRF
    * [ ] Autenticación vs Autorización
    * [ ] JWT tokens
  * [ ] **GraphQL (Strawberry/Ariadne)**
  * [ ] **WebSockets**
  * [ ] **FastAPI/Starlette (prod)**

    * [ ] Validación con Pydantic, **rate limiting**, **CORS**, **JWT**.
  * [ ] **Seguridad aplicada**

    * [ ] Cabeceras seguras, CSRF en formularios, **OWASP Top 10** aplicado.
* [ ] **Ciencia de Datos y Machine Learning** 🔬

  * [ ] **Análisis de Datos**:

    * [ ] **NumPy**: Computación numérica y arrays multidimensionales.
    * [ ] **Pandas**: Manipulación y análisis de datos con DataFrames.
  * [ ] **Visualización de Datos**:

    * [ ] **Matplotlib**: La base para crear gráficos.
    * [ ] **Seaborn**: Gráficos estadísticos de alto nivel.
    * [ ] **Plotly**: Gráficos interactivos.
  * [ ] **Machine Learning**:

    * [ ] **Scikit-learn**: El kit de herramientas fundamental para modelos de ML (regresión, clasificación, clustering).
    * [ ] **Deep Learning**: **TensorFlow** o **PyTorch**.
  * [ ] **Entornos de Trabajo**: **Jupyter Notebooks** / **JupyterLab**.
  * [ ] **Dask para procesamiento distribuido**
  * [ ] **Evaluación de modelos**

    * [ ] Leakage, validación cruzada estratificada, métricas apropiadas.
  * [ ] **Pipelines**

    * [ ] `sklearn.pipeline`, `ColumnTransformer`, persistencia con **joblib**.
  * [ ] **RAG (vista previa)**

    * [ ] Chunking, embeddings, re-ranking, límites de contexto.
* [ ] **Automatización y Scripting** 🤖

  * [ ] **Interacción con el Sistema Operativo**: `os`, `sys`, `shutil`.
  * [ ] **Web Scraping**:

    * [ ] **Requests**: Para hacer peticiones HTTP.
    * [ ] **Beautiful Soup 4**: Para parsear HTML y XML.
    * [ ] **Selenium**: Para automatizar navegadores web.
  * [ ] **Automatización de Tareas**: `schedule`, `cron`.
* [ ] &#x20;**DevOps y Cloud**

  * [ ] Docker y containerización
  * [ ] CI/CD pipelines
  * [ ] AWS/GCP/Azure SDK para Python
  * [ ] Infrastructure as Code con Python
* [ ] \*\*Deployment y Producción 🚀

  * [ ] Preparación para Producción

    * [ ] Configuración por entorno (development, staging, production)
    * [ ] Variables de entorno y secrets management
    * [ ] python-dotenv y configuración segura
  * [ ] Empaquetado y Distribución

    * [ ] setup.py vs setup.cfg vs pyproject.toml
    * [ ] Crear wheels y source distributions
    * [ ] Publicar en PyPI (twine)
    * [ ] Versionado semántico
  * [ ] Containerización con Docker

    * [ ] Dockerfile optimizado para Python
    * [ ] Multi-stage builds
    * [ ] Reducción del tamaño de imágenes
    * [ ] Docker Compose para desarrollo local
  * [ ] Servidores de Aplicación

    * [ ] WSGI: Gunicorn, uWSGI
    * [ ] ASGI: Uvicorn, Hypercorn
    * [ ] Configuración de workers y threads
  * [ ] Reverse Proxy y Load Balancing

    * [ ] Nginx como reverse proxy
    * [ ] Configuración SSL/TLS
    * [ ] Load balancing strategies
  * [ ] Monitoring y Logging en Producción

    * [ ] Structured logging con structlog
    * [ ] Centralización de logs (ELK stack)
    * [ ] APM tools: New Relic, DataDog, AppDynamics
    * [ ] Prometheus y Grafana para métricas
  * [ ] CI/CD Pipelines

    * [ ] GitHub Actions para Python
    * [ ] GitLab CI/CD
    * [ ] Jenkins pipelines
    * [ ] Estrategias de deployment: Blue-Green, Canary
  * [ ] Gestión de Procesos

    * [ ] Supervisor
    * [ ] systemd services
    * [ ] Process managers en cloud
  * [ ] Serverless (AWS Lambda, Google Functions)
  * [ ] Service meshes (Istio, Linkerd)
* [ ] **Seguridad Aplicada**

  * [ ] Hardening de aplicaciones
  * [ ] OWASP Top 10 implementación práctica
  * [ ] Auditoría de dependencias (SBOM)

---

### 🏠 **Arquitectura y Sistemas**

* [ ] **Patrones arquitectónicos**
* [ ] **Diseño de APIs**
* [ ] **Estrategias de cache**
* [ ] **Sistemas distribuidos**

---

### 🌱 **Fase 8: Aprendizaje Continuo y Proyectos**

El viaje nunca termina. La tecnología evoluciona, y tú también debes hacerlo.

* [ ] **Capstone “real”**

  * [ ] **API FastAPI** que expone búsqueda semántica (**FAISS/Chroma** o **Azure AI Search**) con **trazas OpenTelemetry**, **Docker**, **CI/CD** y **tests end-to-end**.
* [ ] **Construye un Portfolio de Proyectos**

  * [ ] Crea al menos un proyecto significativo para cada área de especialización que te interese.
  * [ ] Súbelos a tu GitHub.
* [ ] **Contribuye a Proyectos Open Source**

  * [ ] Empieza por corregir documentación o bugs sencillos.
* [ ] **Mantente Actualizado**

  * [ ] Lee la documentación oficial de Python y sus librerías.
  * [ ] Sigue blogs, newsletters (Pycoder's Weekly) y conferencias (PyCon).
  * [ ] Participa en comunidades online (Stack Overflow, Reddit r/Python).
* [ ] **Explora Tópicos Adicionales**

  * [ ] Empaquetado y distribución de software con `PyPI`.
  * [ ] Desarrollo de Interfaces Gráficas (GUI) con `Tkinter`, `PyQt`, `Kivy`.
  * [ ] Microservicios y contenedores (`Docker`).
  * [ ] Sistemas Distribuidos

    * [ ] Patrones de resiliencia (circuit breaker, retries)
    * [ ] Message brokers (RabbitMQ, Kafka)
* [ ] **Soft Skills para Desarrolladores Senior**

  * [ ] Code reviews efectivos
  * [ ] Mentoría a juniors
  * [ ] Comunicación técnica
  * [ ] Estimación de proyectos
  * [ ] Priorización técnica (Tech Debt vs Features)
  * [ ] Mentoring estructurado
* [ ] **Arquitectura de Software**

  * [ ] Design Patterns en Python
  * [ ] SOLID principles
  * [ ] Clean Architecture
  * [ ] Domain-Driven Design
  * [ ] Event Sourcing/CQRS
* [ ] **Performance en Producción**

  * [ ] APM (Application Performance Monitoring)
  * [ ] Logging estructurado
  * [ ] Métricas y observabilidad
* [ ] &#x20;**Prácticas de Producción Avanzadas**

  * [ ] Feature Flags y A/B Testing

    * [ ] Implementación de feature toggles
    * [ ] Rollout progresivo de features
  * [ ] Caching Strategies

    * [ ] Redis/Memcached
    * [ ] Cache invalidation patterns
    * [ ] CDN integration
  * [ ] Database Migrations

    * [ ] Alembic para SQLAlchemy
    * [ ] Django migrations
    * [ ] Zero-downtime migrations
  * [ ] Health Checks y Readiness Probes

    * [ ] Implementación de endpoints de salud
    * [ ] Integración con Kubernetes
  * [ ] Disaster Recovery

    * [ ] Backup strategies
    * [ ] Rollback procedimientos
    * [ ] Incident response
