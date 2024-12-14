
# Análisis de Sentimientos con Google Cloud NLP

Este proyecto implementa un sistema de análisis de sentimientos utilizando la API de Google Cloud Natural Language Processing (NLP). Se clasifica el sentimiento de textos en **positivo**, **negativo** o **neutral** basado en el contenido de las columnas de un archivo Excel contenido de Titulo y su Resumen.

---

## Descripción

### Características principales:
- **Uso de Google Cloud NLP:** Análisis preciso de sentimientos utilizando la tecnología de Google.
- **Procesamiento directo del texto:** Sin limpieza previa para respetar el contexto y significado completo del contenido.
- **Visualización de resultados:** Generación de tablas y gráficos que resumen el análisis.
- **Resultados exportados:** Resultados clasificados exportados a un archivo Excel.

### Entrada y Salida:
- **Entrada:** Archivo Excel con dos columnas: `Titular` y `Resumen`.
- **Salida:** Archivo Excel con columnas adicionales:
  - `Sentimiento_Titular`: Clasificación del sentimiento del titular (Positivo, Negativo o Neutral).
  - `Sentimiento_Resumen`: Clasificación del sentimiento del resumen (Positivo, Negativo o Neutral).

---

## Estructura del Proyecto

La estructura del proyecto es la siguiente:

![Estructura Proyecto](./estructura_proyecto.jpeg "Analisis de Sentimiento")


## Instalación y Configuración

### Prerrequisitos
- **Python:** Versión 3.8 o superior.
- **Google Cloud Account:** Con credenciales configuradas para acceder a la API de NLP.
- **Entorno virtual recomendado:** Para evitar conflictos de dependencias.

### Pasos de Instalación

1. **Crear y activar un entorno virtual:**
   ```bash
   conda create -n analisis_sentimiento_env python=3.8
   conda activate analisis_sentimiento_env
2. **Activa el entorno virtual (Windows):**
	```bash
	 analisis_sentimiento_env\Scripts\activate
3. **Instalar las dependencias:**
   ```bash
	 pip install -r requirements.txt
4. **Ejecutar el análisis de sentimientos:**
   ```bash
	 python -m src.main
5. **Visualizar los resultados:**
	```bash
	 python -m src.visualization	
## Muestra de los resultados
  
### Tabla:

| **Categoría** | **Titulares** | **Resúmenes** |
|---------------|---------------|---------------|
| **Positivos** | 528           | 542           |
| **Negativos** | 20            | 8             |
| **Neutrales** | 74            | 72            |
	
### Graficos:
![Estructura Proyecto](./grafico_barra.jpeg "GraficoBarra")

![Estructura Proyecto](./grafico_circular.jpeg "GraficoCircular")
