# Trabajo-Practico-1-Entregable
Este repositorio tiene los archivos usados para obtener los resultados plasmados en el trabajo práctico entregable de la materia Matemática IV 

Enlace a Informe: Solo lectura: https://docs.google.com/document/d/19_s9WNMZ7e8Kqd9NeYb0sgfenqQmfLDYQ_MI0JzCiIc/edit?usp=sharing

## Tutorial: clonar y ejecutar los notebooks

### 1. Requisitos previos
- Git instalado.
- Python 3.12 (o compatible) instalado.
- Conexión a internet para descargar las dependencias.

### 2. Clonar el repositorio
Elegí una de las dos opciones según cómo tengas configurado GitHub.

Con HTTPS:
```bash
git clone https://github.com/Damian-Bicocchi/Trabajo-Practico-1-Entregable.git
```

Con SSH (requiere tener una clave SSH cargada en GitHub):
```bash
git clone git@github.com:Damian-Bicocchi/Trabajo-Practico-1-Entregable.git
```

Luego ingresá a la carpeta del proyecto:
```bash
cd Trabajo-Practico-1-Entregable
```

### 3. Crear y activar un entorno virtual
En Linux/macOS:
```bash
python3 -m venv .venv
source .venv/bin/activate
```

En Windows (PowerShell):
```powershell
python -m venv .venv
.venv\Scripts\Activate.ps1
```

### 4. Instalar las dependencias
Con el entorno virtual activado:
```bash
pip install --upgrade pip
pip install -r requirements.txt
```

### 5. Iniciar Jupyter
Desde la raíz del repositorio ejecutá:
```bash
jupyter lab
```

O, si preferís la interfaz clásica:
```bash
jupyter notebook
```

Se abrirá el navegador con el explorador de archivos del proyecto. Si no se abre automáticamente, copiá y pegá en el navegador la URL que muestra la terminal (por ejemplo, `http://localhost:8888/...`).

### 6. Abrir y ejecutar los notebooks
En el explorador de Jupyter entrá a la carpeta correspondiente y abrí el notebook que quieras ejecutar:

- `parte-A/a1_derivacion.ipynb`
- `parte-A/a2_comparacion.ipynb`
- `parte-B/b2_cuadro.ipynb`

Una vez abierto, podés ejecutar todas las celdas desde el menú **Run > Run All Cells** (o **Cell > Run All** según la versión). El kernel debe ser el del entorno virtual `.venv`; si no aparece seleccionado, elegilo en **Kernel > Change Kernel**.

> **Nota:** los notebooks cargan el dataset con la ruta relativa `../dataset/airfoil_self_noise.dat`. Por eso es importante abrirlos desde Jupyter manteniendo la estructura de carpetas del repositorio (no muevas los notebooks ni el archivo `.dat`).

### 7. Cerrar el entorno
Cuando termines, detené Jupyter con `Ctrl+C` en la terminal y desactivá el entorno virtual con:
```bash
deactivate
```

