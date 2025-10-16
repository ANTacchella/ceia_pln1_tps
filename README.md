# Desafíos - Procesamiento del Lenguaje Natural (PLN) 1

**Carrera de Especialización en Inteligencia Artificial (CEIA) - Universidad de Buenos Aires (UBA)**

Este repositorio contiene los cuatro desafíos desarrollados para la materia de Procesamiento del Lenguaje Natural 1 de la Carrera de Especialización en Inteligencia Artificial de la Universidad de Buenos Aires.

## Contenido

### [Desafío 1: Vectorización de Documentos y Clasificación](./TP1/)
**Archivo:** `tp1.ipynb`

**Dataset:**

- Se utilizó el dataset fetch_20newsgroups, que contiene aproximadamente 18.000 documentos de texto divididos en 20 categorías (noticias). El dataset se dividió en conjuntos de entrenamiento (train) y prueba (test).

**Objetivos:**

- Vectorizar documentos utilizando TF-IDF y medir la similaridad entre ellos. Estudiar los documentos más similares a 5 documentos elegidos al azar.
- Construir un modelo de clasificación por prototipos (zero-shot) para clasificar documentos del conjunto de test basado en la similaridad con documentos del conjunto de entrenamiento.
- Entrenar modelos de clasificación Naïve Bayes (MultinomialNB y ComplementNB) para maximizar el f1-score macro en el conjunto de test, experimentando con parámetros del vectorizador y los modelos.
- Transponer la matriz documento-término para obtener una matriz término-documento (vectorización de palabras) y estudiar la similaridad entre palabras elegidas manualmente.

### [Desafío 2: Word Embeddings con Gensim](./TP2/)
**Archivo:** `tp2.ipynb`

**Dataset:** 

- El dataset utilizado en este trabajo son letras de canciones de bandas de habla inglesa, específicamente se cargaron las canciones de Michael Jackson (michael-jackson.txt). Cada línea del archivo se considera un "documento" o verso.

**Objetivos:**

- Crear y entrenar un modelo Word2Vec (Skipgram) utilizando Gensim para generar embeddings de palabras a partir del dataset.
- Explorar las relaciones semánticas entre palabras calculando la similitud entre sus vectores de embeddings.
- Identificar palabras más y menos relacionadas con términos de interés como "billie", "bad", "beat", "thriller" y "black".
- Visualizar los embeddings en 2D y 3D para comprender las relaciones espaciales entre las palabras.

### [Desafío 3: Predicción de Próxima Palabra](./TP3/)
**Archivo:** `tp3.ipynb`

**Dataset:**

- El dataset utilizado en este trabajo son letras de canciones de bandas de habla inglesa, específicamente se cargaron las canciones de Michael Jackson (michael-jackson.txt). Cada línea del archivo se considera un "documento" o verso.

**Objetivos:**

- Preparación de datos: Cargar y preprocesar las letras de las canciones, incluyendo la tokenización y la determinación de un tamaño de contexto máximo para las secuencias.
- Modelado: Definir y entrenar un modelo de red neuronal (en este caso, una red LSTM) para predecir la siguiente palabra en una secuencia.
- Evaluación: Medir la calidad de la generación de secuencias utilizando métricas como la perplejidad sobre un conjunto de validación.
- Generación de secuencias: Implementar y ensayar diferentes estrategias de generación de secuencias, como la predicción de la próxima palabra y la búsqueda Beam Search, para generar texto coherente a partir de una semilla inicial.

### [Desafío 4: Traductor Secuencia a Secuencia](./TP4/)
**Archivo:** `tp4.ipynb`

**Dataset:**
- El dataset empleado para este trabajo es el de pares de oraciones en inglés y español (`spa-eng.zip`), descargado de los recursos de TensorFlow. Se utilizaron 7000 pares de oraciones de este dataset para entrenar los modelos de traducción.

**Objetivos:**
- El objetivo principal de este trabajo es implementar y entrenar un modelo de traducción automática basado en una arquitectura Sequence-to-Sequence (Seq2Seq) utilizando PyTorch. Específicamente, se busca:
    - Preprocesar los datos de texto para convertirlos en secuencias numéricas y realizar el padding adecuado.
    - Utilizar embeddings pre-entrenados (GloVe) para representar las palabras de entrada.
    - Construir y entrenar modelos Seq2Seq con diferentes tamaños de capas LSTM para comparar su rendimiento.
    - Evaluar la capacidad de los modelos entrenados para traducir frases de inglés a español.

## Tecnologías Utilizadas

### Bibliotecas principales:
- **scikit-learn** - Vectorización, clasificación y métricas
- **gensim** - Word embeddings y Word2Vec
- **tensorflow/keras** - Redes neuronales y procesamiento de secuencias
- **pytorch** - Implementación de modelos seq2seq
- **plotly** - Visualizaciones interactivas
- **gradio** - Interfaces de usuario interactivas
- **numpy, pandas** - Manipulación de datos
- **matplotlib, seaborn** - Visualizaciones estáticas

## Instrucciones de Uso

**Ejecutar notebooks:**
- Abrir cualquier archivo `.ipynb` en GoogleColab
- Ejecutar las celdas secuencialmente

## Contexto Académico

**Materia:** Procesamiento del Lenguaje Natural 1

**Carrera:** Carrea de Especialización en Inteligencia Artificial (CEIA)

**Universidad:** Universidad de Buenos Aires (UBA)

**Autor:** Ing. Alejandro Nicolás Tacchella

**Proferores:** Dr. Rodrigo Cardenas Szigety, Dr. Mauro Bringas

## Licencia

Este proyecto está bajo la Licencia Apache 2.0 - ver el archivo [LICENSE](LICENSE) para más detalles.

## Contribuciones

Este repositorio es parte de un proyecto académico. Las sugerencias y mejoras son bienvenidas.
