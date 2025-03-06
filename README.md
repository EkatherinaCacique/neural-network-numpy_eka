# Red Neuronal con Retropropagación en Python (by Ekatherina Cacique)

Este proyecto implementa una red neuronal artificial desde cero en Python para la clasificación de datos generados de manera sintética. Utiliza NumPy para los cálculos matriciales y Matplotlib para la visualización de resultados.

## Características
- Implementación manual de una red neuronal con tres capas ocultas.
- Uso de funciones de activación **ReLU** y **sigmoide**.
- Implementación de la función de pérdida **MSE (Error Cuadrático Medio)**.
- Inicialización de pesos aleatoria.
- Entrenamiento utilizando gradiente descendente.
- Generación y visualización de los datos de clasificación.

## Requisitos
Asegúrate de tener instaladas las siguientes bibliotecas antes de ejecutar el código:

```sh
pip install numpy matplotlib scikit-learn
```

## Estructura del Código
El código está dividido en las siguientes funciones:

### 1. Creación del Dataset
```python
def create_dataset(N=1000):
```
Genera un conjunto de datos de clasificación binaria con distribución gaussiana.

### 2. Funciones de Activación
```python
def sigmoid(x, derivate=False):
def relu(x, derivate=False):
```
- **Sigmoide:** Se usa en la capa de salida para producir probabilidades.
- **ReLU:** Se usa en capas ocultas para mejorar la convergencia.

### 3. Inicialización de Pesos
```python
def initialize_parameters_deep(layers_dims):
```
Inicializa los pesos y sesgos de la red de manera aleatoria.

### 4. Entrenamiento de la Red
```python
def train(x_data, y_data, learning_rate, params, training=True):
```
Ejecuta la propagación hacia adelante y el entrenamiento mediante retropropagación si está habilitado.

### 5. Entrenamiento y Visualización
```python
train_neural_network()
```
Ejecuta el entrenamiento y muestra la clasificación de los datos en un gráfico.

## Ejecución
Para ejecutar el código, simplemente corre el script en Python:

```sh
python main.py
```