# PyTorch desde cero

Curso de PyTorch en español, en notebooks. Cada notebook explica un tema paso a paso, con el código ejecutado y los gráficos a la vista, y termina con un resumen y ejercicios.

La idea es entender qué hace cada línea y por qué: primero se usa una herramienta, después se abre para ver cómo funciona, y al final se justifica con su matemática.

## Contenido

| Módulo | Notebook | Qué cubre |
|---|---|---|
| **00 · Fundamentos** | [Tensores, autograd y una neurona](00-fundamentos/01_tensores_autograd_y_una_neurona.ipynb) | Tensores, formas, broadcasting, producto matricial, autograd, una neurona entrenada de tres formas |
| **01 · Red neuronal simple** | [Una red neuronal simple](01-red-neuronal-simple/01_red_neuronal_simple.ipynb) | El flujo completo: datos, modelo, pérdida, optimizador, entrenamiento y predicción. De una neurona a una red con capa oculta y ReLU |
| **02 · Descenso de gradiente** | [Descenso de gradiente](02-descenso-de-gradiente/01_descenso_de_gradiente.ipynb) | Qué hace `optimizer.step()`, tasa de aprendizaje, superficie de pérdida, por qué normalizar |
| | [SGD y mini-batches](02-descenso-de-gradiente/02_sgd_y_minibatches.ipynb) | Gradiente estocástico, tamaño de lote, ruido, tasa decreciente, `DataLoader` |
| **03 · Optimalidad** | [Mínimos, convexidad y puntos silla](03-optimalidad/01_optimalidad.ipynb) | Condiciones de optimalidad, hessiano, convexidad, ecuaciones normales, número de condición, por qué la pérdida de una red no es convexa |
| **04 · Matemática de PyTorch** | [Autograd y regla de la cadena](04-matematica-de-pytorch/01_autograd_y_regla_de_la_cadena.ipynb) | Jacobianos, productos vector-jacobiano, retropropagación a mano |
| | [Capas y activaciones](04-matematica-de-pytorch/02_capas_y_activaciones.ipynb) | `nn.Linear`, inicialización, `ReLU`, `Sigmoid`, `Tanh`, `Softmax`, estabilidad numérica |
| | [Funciones de pérdida](04-matematica-de-pytorch/03_funciones_de_perdida.ipynb) | Máxima verosimilitud, `MSELoss`, `L1Loss`, `HuberLoss`, `BCELoss`, `BCEWithLogitsLoss`, `CrossEntropyLoss` |
| | [Optimizadores](04-matematica-de-pytorch/04_optimizadores.ipynb) | `SGD`, `weight_decay`, momento, Nesterov, `RMSprop`, `Adam`, `AdamW` |

En el módulo 04 cada función de PyTorch se trata igual: su fórmula, de dónde sale, una implementación a mano y una comprobación con `torch.allclose` de que coincide con la de PyTorch.

## Orden sugerido

Los módulos 00 a 03 están pensados para leerse en orden. El módulo 04 es más formal y se puede leer al final o ir consultando a medida que aparecen las funciones en los módulos anteriores.

Conocimientos previos: Python básico. Para los módulos 03 y 04 ayuda haber visto derivadas y matrices, aunque todo lo que se usa se explica en el momento.

## Cómo ejecutarlos

**En tu computador**

```bash
git clone https://github.com/B3njjaman/pytorch-desde-cero.git
cd pytorch-desde-cero
pip install -r requirements.txt
jupyter lab
```

También se pueden abrir directamente en VS Code con la extensión de Jupyter.

**En Google Colab**

Abre `https://colab.research.google.com/github/B3njjaman/pytorch-desde-cero` y elige el notebook. Colab ya trae PyTorch instalado.

Todos los notebooks corren en CPU en pocos segundos. No hace falta GPU.

## Próximos módulos

- Clasificación de imágenes con una red densa (MNIST), con conjuntos de entrenamiento y validación.
- Sobreajuste y regularización: dropout, parada temprana, decaimiento de pesos.
- Redes convolucionales.
- Programación de la tasa de aprendizaje y normalización por lotes.

## Créditos

El escenario del repartidor del módulo 01 está inspirado en el primer laboratorio del curso de PyTorch de DeepLearning.AI en Coursera. Los datos, el código y las explicaciones de este repositorio son propios.
