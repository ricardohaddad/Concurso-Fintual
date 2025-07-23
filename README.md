# Concurso Fintual: Analizador de Números

Este proyecto contiene un script de Python para analizar una lista de números y encontrar los faltantes, diseñado originalmente para el concurso "Hasta Pronto Jefe" de Fintual.

El script está preparado para procesar una lista de números, identificar cuáles faltan en una secuencia consecutiva desde el 1, y calcular la suma total de dichos números ausentes. La salida se presenta de forma clara y con colores en la terminal para una fácil visualización.

## Requisitos

- Python 3.6 o superior
- pip (el gestor de paquetes de Python)

## Instalación

Sigue estos pasos para configurar el entorno y poder ejecutar el script.

1.  **Clona el repositorio:**

    ```bash
    git clone https://github.com/TU_USUARIO/Concurso-Fintual.git
    cd Concurso-Fintual
    ```

2.  **Crea y activa un entorno virtual:**

    Es una buena práctica utilizar un entorno virtual para aislar las dependencias del proyecto.

    ```bash
    # Crear el entorno virtual
    python3 -m venv venv

    # Activarlo (en Linux/macOS)
    source venv/bin/activate

    # Activarlo (en Windows)
    .\\venv\\Scripts\\activate
    ```

3.  **Instala las dependencias:**

    El proyecto utiliza la librería `colorama`. Puedes instalarla fácilmente usando el archivo `requirements.txt` que he creado.

    ```bash
    pip install -r requirements.txt
    ```

## Uso

1.  **Agrega tus números:**

    Abre el archivo `concurso.py` y modifica la función `get_numbers()` para que devuelva la lista de números que quieres analizar. Puedes descomentar los números de ejemplo o añadir los tuyos.

    ```python
    def get_numbers():
        """Returns the array of numbers to process."""
        # Descomenta o añade aquí tu lista de números
        numeros = [
            1, 2, 3, 4, 5, 8, 10,
            # ... y así sucesivamente
        ]
        return numeros
    ```

2.  **Ejecuta el script:**

    Una vez que hayas guardado los cambios con tus números, ejecuta el script desde la terminal (asegúrate de que tu entorno virtual esté activado):

    ```bash
    python concurso.py
    ```

### ¿Qué hace el script?

Al ejecutarlo, el script realizará lo siguiente:

- **Leerá** los números que has proporcionado.
- **Mostrará un resumen** con la cantidad total de números, el número más bajo y el más alto.
- **Encontrará los primeros 100 números que faltan** en la secuencia.
- **Imprimirá** la lista de números faltantes en columnas.
- **Calculará y mostrará la "inversión total"**, que es la suma de todos los números faltantes encontrados.
