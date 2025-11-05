Aquí tienes el archivo `README.md` (Markdown) que resume los scripts de instalación y las dependencias de los lenguajes para todas las soluciones que hemos implementado.

Puedes guardar este texto en un archivo llamado `README.md` en tu carpeta de proyectos.

-----

-----

# 🚀 Guía de Instalación de Dependencias

Este documento describe los componentes y pasos de configuración necesarios para compilar y ejecutar las soluciones de software desarrolladas en Python, Java y C.

## 🐍 Python

Se requiere Python para ejecutar los siguientes scripts:

  * `fen_validator.py`
  * `pascal_polynomial.py`
  * `string_recognizer.py`

### 1\. Instalación

1.  **Descargar:** Ve al sitio web oficial [python.org/downloads](https://www.python.org/downloads/) y descarga la última versión estable para Windows.
2.  **Instalador:** Ejecuta el instalador.
      * **¡MUY IMPORTANTE\!** En la primera pantalla de la instalación, asegúrate de marcar la casilla que dice **"Add Python to PATH"**.

### 2\. Verificación

Para confirmar que Python está instalado y reconocido por el sistema, abre una terminal (`cmd` o `PowerShell`) y ejecuta el siguiente comando:

```bash
python --version
```

Deberías ver la versión de Python que acabas de instalar.

### 3\. Dependencias (Librerías)

**No se requieren librerías externas.**

Todos los scripts de Python utilizan módulos que vienen incluidos en la biblioteca estándar de Python:

  * `re` (para expresiones regulares)
  * `time` (para medir el tiempo de ejecución)

-----

## ☕ Java

Se requiere Java para compilar y ejecutar los siguientes archivos:

  * `FenValidator.java`
  * `PascalPolynomial.java`

### 1\. Instalación (JDK)

Necesitas el **Kit de Desarrollo de Java (JDK)** para poder compilar (`javac`).

1.  **Descargar:** Recomendamos una distribución moderna y estándar de OpenJDK, como [Eclipse Temurin (Adoptium)](https://adoptium.net/). Descarga la última versión LTS (ej. JDK 17, 21).
2.  **Instalador:** El instalador `.msi` para Windows es la opción más sencilla, ya que configurará automáticamente las variables de entorno (`JAVA_HOME` y el `PATH`).

### 2\. Verificación

Abre una nueva terminal y ejecuta ambos comandos para verificar tanto el compilador como el entorno de ejecución:

```bash
# Verifica el compilador
javac --version

# Verifica el entorno de ejecución
java --version
```

### 3\. Dependencias

**No se requieren librerías externas.**

Todas las clases utilizadas son parte del JDK estándar:

  * `java.util.regex.Pattern` (para expresiones regulares)
  * `java.math.BigInteger` (para los números grandes del polinomio)
  * `java.util.ArrayList`, `java.io.FileWriter`, etc.

-----

## ⚙️ C (Usando el IDE Dev-C++)

Se utiliza C para la solución `traductor.c`. La forma más sencilla de compilar en Windows (evitando los problemas de `PATH` que encontramos) es usar un IDE que incluya su propio compilador.

### 1\. Instalación

1.  **Descargar:** Descarga una versión moderna de Dev-C++, como [Embarcadero Dev-C++](https://www.embarcadero.com/free-tools/dev-cpp) o la versión mantenida en [SourceForge](https://sourceforge.net/projects/orwelldevcpp/).
2.  **Instalar:** Ejecuta el instalador. Este IDE **ya incluye** una versión del compilador MinGW (`gcc`), por lo que no es necesario instalar `gcc` por separado.

### 2\. "Script" de Configuración (Pasos Manuales)

El único "script" o paso de configuración necesario es indicarle a Dev-C++ que use un estándar de C moderno (C99 o C11) para permitir la sintaxis de bucle `for` moderna.

1.  Dentro de Dev-C++, ve al menú **Herramientas (Tools) \> Opciones del Compilador (Compiler Options)**.
2.  Ve a la pestaña **Generación de Código (Code Generation)**.
3.  Busca la opción **Estándar del Lenguaje (-std)**.
4.  Selecciona **`ISO C11`** (recomendado) o **`ISO C99`**.
5.  Haz clic en **Aceptar**.

### 3\. Dependencias

**Ninguna.** El código usa únicamente las bibliotecas estándar de C que vienen incluidas con el compilador:

  * `stdio.h`
  * `stdlib.h`
  * `string.h`
  * `ctype.h`
