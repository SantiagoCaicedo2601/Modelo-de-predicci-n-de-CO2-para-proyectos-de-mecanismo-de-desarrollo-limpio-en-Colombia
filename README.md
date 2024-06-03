# Modelo-de-prediccion-de-CO2-para-proyectos-de-mecanismo-de-desarrollo-limpio-en-Colombia
Se esquematiza el modelo a utilizar con inspiración de diversos modelos de redes neuronales para predecir la contaminación del aire en diferentes ciudades, utiliza datos simulados para demostrar el proceso de entrenamiento del modelo, la generación de gráficas y el cálculo del factor de emisión.
# Importar librerías necesarias
numpy: Biblioteca fundamental para realizar operaciones numéricas en Python, como la creación y manipulación de arreglos multidimensionales.
pandas: Utilizada para la manipulación y el análisis de datos, proporciona estructuras de datos y operaciones para manipular tablas numéricas y series temporales.
MinMaxScaler de sklearn.preprocessing: Herramienta para escalar o normalizar los datos, ajustando todos los valores en un rango específico, generalmente [0, 1].
Sequential, LSTM y Dense de tensorflow.keras: Herramientas para construir redes neuronales. Sequential facilita la creación de modelos lineales, LSTM es una capa de red neuronal recurrente adecuada para series temporales, y Dense es una capa completamente conectada.
matplotlib.pyplot: Biblioteca para crear visualizaciones de datos, como gráficos de líneas, barras, dispersión, etc.
make_interp_spline de scipy.interpolate: Utilizada para suavizar curvas en gráficos, creando una interpolación spline suave a partir de un conjunto de puntos de datos.
import numpy as np
import pandas as pd
from sklearn.preprocessing import MinMaxScaler
from tensorflow.keras.models import Sequential
from tensorflow.keras.layers import LSTM, Dense
import matplotlib.pyplot as plt
from scipy.interpolate import make_interp_spline
# Introduccion de funciones basicas
