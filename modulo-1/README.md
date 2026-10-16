# Módulo 1: de los tensores a una red neuronal

Este módulo sigue el primer módulo del curso de PyTorch de DeepLearning.AI en Coursera. Parte de los tensores y llega a una red con capas ocultas entrenada con descenso de gradiente, y después abre cada pieza para ver su matemática.

## Contenido

| Parte | Notebooks |
|---|---|
| [00 · Fundamentos](00-fundamentos) | [Tensores, autograd y una neurona](00-fundamentos/01_tensores_autograd_y_una_neurona.ipynb) · [Tensores a fondo](00-fundamentos/02_tensores_a_fondo.ipynb) |
| [01 · Red neuronal simple](01-red-neuronal-simple) | [Una red neuronal simple](01-red-neuronal-simple/01_red_neuronal_simple.ipynb) |
| [02 · Descenso de gradiente](02-descenso-de-gradiente) | [Descenso de gradiente](02-descenso-de-gradiente/01_descenso_de_gradiente.ipynb) · [SGD y mini-batches](02-descenso-de-gradiente/02_sgd_y_minibatches.ipynb) |
| [03 · Optimalidad](03-optimalidad) | [Mínimos, convexidad y puntos silla](03-optimalidad/01_optimalidad.ipynb) |
| [04 · Matemática de PyTorch](04-matematica-de-pytorch) | [Autograd y regla de la cadena](04-matematica-de-pytorch/01_autograd_y_regla_de_la_cadena.ipynb) · [Capas y activaciones](04-matematica-de-pytorch/02_capas_y_activaciones.ipynb) · [Funciones de pérdida](04-matematica-de-pytorch/03_funciones_de_perdida.ipynb) · [Optimizadores](04-matematica-de-pytorch/04_optimizadores.ipynb) |
| [05 · Profundización](05-profundizacion) | [El perceptrón de Rosenblatt](05-profundizacion/01_perceptron.ipynb) · [XOR y redes feedforward](05-profundizacion/02_xor_y_redes_feedforward.ipynb) |

La descripción de cada notebook está en el [README principal](../README.md).

## Recursos para profundizar

Esta es la lista de lecturas que el curso recomienda para el módulo 1, ordenada por tema. Donde un recurso calza con una parte de este repositorio, se indica cuál. Los que tienen un notebook propio en `05-profundizacion` lo indican con **En código**. Las diapositivas de las clases están en la [comunidad de DeepLearning.AI](https://community.deeplearning.ai/) y hace falta una cuenta para verlas.

### Fundamentos

- **[PyTorch: Deep Learning with PyTorch, A 60 Minute Blitz](https://docs.pytorch.org/tutorials/beginner/deep_learning_60min_blitz.html)** (tutorial oficial, gratis). Un recorrido rápido y práctico por tensores, autograd y el entrenamiento de una red pequeña. Va bien junto a `00-fundamentos`.
- **[3Blue1Brown: Neural networks](https://www.youtube.com/playlist?list=PLZHQObOWTQDNU6R1_67000Dx_ZCJB-3pi)** (videos, gratis). Los capítulos 1 y 2 explican con animaciones qué es una neurona, qué son los pesos y cómo funciona el descenso de gradiente. Los capítulos siguientes, sobre retropropagación, acompañan a `04-matematica-de-pytorch/01_autograd_y_regla_de_la_cadena`. **En código:** [XOR y redes feedforward](05-profundizacion/02_xor_y_redes_feedforward.ipynb).
- **[Goodfellow, Bengio y Courville: Deep Learning](https://www.deeplearningbook.org/)** (libro, gratis en línea). El texto de referencia de la teoría. Los capítulos 1 a 6 cubren álgebra lineal, probabilidad, cálculo numérico (con optimización por gradiente), fundamentos de machine learning y redes feedforward, y conectan con `03-optimalidad` y `04-matematica-de-pytorch`. Los capítulos posteriores tratan regularización, optimización avanzada y redes convolucionales. **En código:** [XOR y redes feedforward](05-profundizacion/02_xor_y_redes_feedforward.ipynb).

### IA: historia y contexto

- **[Melanie Mitchell: Artificial Intelligence: A Guide for Thinking Humans](https://melaniemitchell.me/aibook/)** (libro). Un panorama accesible y equilibrado de lo que la IA puede y no puede hacer, y por qué importa. **En código:** [el perceptrón de Rosenblatt](05-profundizacion/01_perceptron.ipynb).
- **[Nils J. Nilsson: The Quest for Artificial Intelligence](https://ai.stanford.edu/~nilsson/QAI/qai.pdf)** (libro, PDF gratis). La historia completa de la IA, desde los sistemas simbólicos hasta el machine learning moderno. **En código:** [el perceptrón de Rosenblatt](05-profundizacion/01_perceptron.ipynb).

### Machine learning en general

- **[Bishop: Pattern Recognition and Machine Learning](https://www.microsoft.com/en-us/research/publication/pattern-recognition-machine-learning/)** (libro, PDF gratis en la página de Microsoft Research). El tratamiento matemático de referencia de los modelos probabilísticos y los algoritmos de aprendizaje. En los capítulos 1 a 4 deduce el error cuadrático y la entropía cruzada a partir de la máxima verosimilitud, lo mismo que hace `04-matematica-de-pytorch/03_funciones_de_perdida`.
- **[Aurélien Géron: Hands-On Machine Learning](https://github.com/ageron/handson-ml3)** (libro; los notebooks son gratis). Una guía práctica, basada en proyectos, para construir, evaluar y poner en producción sistemas de ML.
- **[DeepLearning.AI: Machine Learning Specialization](https://www.deeplearning.ai/courses/machine-learning-specialization/)** (curso). Sobre todo la semana 1: aprendizaje supervisado, métricas y el flujo de trabajo de un proyecto de ML.

### PyTorch

- **[Documentación de PyTorch](https://docs.pytorch.org/docs/stable/index.html)**. La referencia de cada función, con la filosofía de ejecución inmediata (*eager*) de PyTorch, sus APIs principales y las librerías del ecosistema.
- **[PyTorch 2.x](https://pytorch.org/get-started/pytorch-2-x/)**. Qué trae la serie 2.x: `torch.compile`, el compilador Inductor y las mejoras de rendimiento.
- **[Huang, Stevens, Antiga y Viehmann: Deep Learning with PyTorch, 2.ª edición](https://www.manning.com/books/deep-learning-with-pytorch-second-edition)** (libro, Manning). Patrones y recetas para construir, entrenar y desplegar modelos en PyTorch de principio a fin.
- **[fast.ai: Practical Deep Learning for Coders](https://course.fast.ai/)** (curso y libro, gratis). Enfoque de arriba hacia abajo: primero se entrenan modelos buenos en proyectos reales y después se estudia cómo funcionan.

### Deep learning: teoría

- **[Michael Nielsen: Neural Networks and Deep Learning](http://neuralnetworksanddeeplearning.com/)** (libro, gratis en línea). Una explicación paso a paso, con ejemplos interactivos, de la retropropagación y las ideas centrales del deep learning. El capítulo 2 es la mejor compañía para `04-matematica-de-pytorch/01_autograd_y_regla_de_la_cadena`.
- **[CS231n: Neural Networks Part 1](https://cs231n.github.io/neural-networks-1/)** (apuntes de Stanford, gratis). Perceptrones multicapa, activaciones, inicialización y consejos prácticos para entrenar. Acompaña a `04-matematica-de-pytorch/02_capas_y_activaciones`.
- **[DeepLearning.AI: Deep Learning Specialization](https://www.deeplearning.ai/courses/deep-learning-specialization/)** (curso). Redes neuronales, técnicas de optimización, redes convolucionales y recurrentes, y aplicaciones prácticas.

### El ciclo de vida de un proyecto de ML

- **[Google: Rules of Machine Learning](https://developers.google.com/machine-learning/guides/rules-of-ml)** (guía, gratis). Buenas prácticas para diseñar, iterar y mantener sistemas de ML en producción, de Martin Zinkevich.
- **[Google Cloud: MLOps, continuous delivery and automation pipelines in machine learning](https://cloud.google.com/architecture/mlops-continuous-delivery-and-automation-pipelines-in-machine-learning)** (guía, gratis). Integración, entrega y entrenamiento continuos, versionado de modelos y monitoreo en producción.

### Redes neuronales: intuición visual

- **[Welch Labs: Neural Networks Demystified](https://www.youtube.com/playlist?list=PLiaHhY2iBX9hdHaRr6b7XevZtgZRa1PoU)** (videos, gratis). Videos cortos que construyen la intuición sobre capas, activaciones y fronteras de decisión.
- **[MIT 6.S191: Introduction to Deep Learning](https://introtodeeplearning.com/)** (clases y diapositivas, gratis). Un complemento visual y conciso de los fundamentos del deep learning.
