# Examen intermedio - Reconocimiento de Patrones

Este repositorio contiene la solución de dos problemas del examen intermedio:

- `problema-1/`: análisis de equidad y toma de decisiones con clientes bancarios.
- `problema-2/`: modelado de series temporales para predecir la demanda de bicicletas.

El proyecto ya incluye el archivo `requirements.txt` en la raíz para instalar todas las dependencias necesarias.

## Estructura del repositorio

```text
examen-intermedio/
├── requirements.txt
├── README.md
├── problema-1/
│   ├── README.md
│   ├── problema-1.ipynb
│   ├── data/
│   └── resultados/
├── problema-2/
│   ├── README.md
│   ├── problema-2.ipynb
│   ├── data/
│   └── resultados/
└── parte-teorica.pdf
```

## Requisitos

- Python 3.10 o superior
- Entorno virtual recomendado

## Instalación

Desde la raíz del proyecto, ejecuta:

### macOS / Linux

```bash
python3 -m venv .venv
source .venv/bin/activate
python -m pip install --upgrade pip
pip install -r requirements.txt
```

### Windows (PowerShell)

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
pip install -r requirements.txt
```

## Ejecución de los notebooks

### Problema 1

```bash
jupyter nbconvert --to notebook --execute --inplace problema-1/problema-1.ipynb
```

### Problema 2

```bash
jupyter nbconvert --to notebook --execute --inplace problema-2/problema-2.ipynb
```

También puedes abrir cada notebook directamente en VS Code o Jupyter y ejecutarlo manualmente.

## Datos

Los notebooks descargan automáticamente los datasets si no existen en `data/`:

- `problema-1` usa el dataset de Default of Credit Card Clients de UCI.
- `problema-2` usa el dataset de Bike Sharing Dataset de UCI.

## Resultados

Cada problema genera archivos en su carpeta `resultados/`, incluyendo:

- tablas CSV
- gráficos
- comparaciones de modelos
- métricas de validación y prueba

## Documentación adicional

Cada problema tiene un README específico con detalles del análisis y la metodología:

- `problema-1/README.md`
- `problema-2/README.md`

## Descripción breve de los problemas

### Problema 1

Se trabaja con un conjunto de clientes bancarios para estudiar la relación entre riesgo de impago, decisiones de crédito y equidad entre grupos. El análisis incluye modelos predictivos, calibración, validación de hipótesis y evaluación de diferencias por grupos.

### Problema 2

Se trabaja con un problema de regresión temporal sobre el número de bicicletas alquiladas por hora. Se comparan distintas representaciones del tiempo, modelos de referencia y una solución basada en kernels circulares.

## Recomendación de uso

La forma más sencilla de reproducir el proyecto es activar el entorno virtual desde la raíz y luego ejecutar cada notebook por separado desde Jupyter o desde la terminal.

