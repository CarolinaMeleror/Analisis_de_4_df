# Título del Proyecto: Análisis Inicial y Selección de Problema

  ## Descripción
  Este proyecto realiza un análisis exploratorio exhaustivo de cuatro conjuntos de datos diversos con el objetivo de identificar y seleccionar problemáticas específicas de
  machine learning. El proyecto busca demostrar competencias en análisis de datos, limpieza, preparación y selección estratégica de problemas de aprendizaje automático
  adaptados a las características únicas de cada dataset.

  ## Conjuntos de Datos Analizados

  ### 1. **Videojuegos - Ventas Globales**
  - Dataset con información de ventas de videojuegos por región, plataforma y género
  - Variables: nombre, plataforma, año, género, publisher, ventas por región
  - Tamaño: Miles de registros de videojuegos históricos

  ### 2. **Clientes de Telecomunicaciones**
  - Información demográfica y de servicios de clientes de una empresa de telecomunicaciones
  - Variables: demografía, servicios contratados, facturación, churn
  - Enfoque: Análisis de retención y comportamiento de clientes

  ### 3. **Clasificación de Precios de Celulares**
  - Especificaciones técnicas de teléfonos móviles con rangos de precio
  - Variables: 20+ características técnicas (RAM, batería, cámara, etc.)
  - Objetivo: Clasificación en 4 rangos de precio (0-3)

  ### 4. **Pokémon - Estadísticas de Combate**
  - Estadísticas completas de Pokémon de todas las generaciones
  - Variables: tipos, estadísticas de combate, generación, legendario
  - Aplicación: Análisis estratégico y balance del juego

  ## Resumen del EDA Inicial

  ### Hallazgos Principales:

  **Videojuegos:**
  - Datos con valores faltantes en ventas regionales (imputados con media)
  - Alta variabilidad en ventas entre plataformas y géneros
  - Distribución asimétrica de ventas globales

  **Telecomunicaciones:**
  - Dataset completo con mínimos valores faltantes
  - Variable objetivo clara: churn (abandono de clientes)
  - Múltiples servicios y características demográficas disponibles

  **Celulares:**
  - Dataset perfectamente balanceado sin valores nulos
  - 4 clases de precio equitativamente distribuidas
  - Características técnicas altamente correlacionadas con precio

  **Pokémon:**
  - Valores faltantes en columna 'moves' (imputados por tipo)
  - Gran diversidad en estadísticas indica múltiples arquetipos
  - Datos de 7+ generaciones con evolución clara en diseño

  ## Problema Seleccionado

  ### Por Dataset:

  1. **Videojuegos → REGRESIÓN**
     - **Problema**: Predecir ventas globales basándose en características del juego
     - **Justificación**: Permite a publishers estimar el potencial comercial
     - **Objetivo**: Modelo predictivo para forecasting de ventas

  2. **Telecomunicaciones → CLASIFICACIÓN BINARIA**
     - **Problema**: Predecir churn (abandono) de clientes
     - **Justificación**: Alto valor comercial en retención de clientes
     - **Objetivo**: Identificar clientes en riesgo para acciones preventivas

  3. **Celulares → CLASIFICACIÓN MULTICLASE**
     - **Problema**: Clasificar dispositivos en rangos de precio (0-3)
     - **Justificación**: Dataset balanceado ideal para clasificación
     - **Objetivo**: Modelo interpretable para estrategias de pricing

  4. **Pokémon → CLUSTERING**
     - **Problema**: Agrupar Pokémon por arquetipos de combate
     - **Justificación**: No requiere variable objetivo, revela patrones ocultos
     - **Objetivo**: Identificar roles (tanques, sweepers, soportes) para estrategias

  ## Instrucciones para Ejecutar

  ### Requisitos:
  ```bash
  - Python 3.7+
  - Jupyter Notebook o Google Colab
  - Librerías: pandas, numpy, matplotlib, seaborn

  Pasos:

  1. Clonar o descargar el proyecto
  git clone [URL_del_repositorio]
  cd proyecto2final
  2. Instalar dependencias
  pip install pandas numpy matplotlib seaborn
  3. Ejecutar los notebooks en orden:
    - EDA_videojuegos.ipynb
    - EDA_clientes_telecomunicaciones.ipynb
    - EDA_clasificacion_celulares.ipynb
    - EDA_pokemon.ipynb (o EDA_pokemon1.ipynb)
  4. Para Google Colab:
    - Subir los archivos CSV a Colab
    - Ejecutar todas las celdas en orden
    - Los datasets limpios se guardarán como *_limpio.csv

  Archivos de datos necesarios:

  - videos_juegos.csv
  - clientes_telecomunicaciones.csv
  - clasificacion_precio_celulares.csv
  - pokemon_data.csv

  Autores

  Carolina Melero
  - Rol: Análisis de Datos y Desarrollo
  - Responsabilidades: EDA completo, limpieza de datos, selección de problemas

  Licencia

  Este proyecto es desarrollado con fines educativos como parte del curso de Machine Learning.

  ---Proyecto desarrollado como parte del curso de Introducción al Machine Learning
