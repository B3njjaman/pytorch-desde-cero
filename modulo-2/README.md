# Módulo 2: el flujo de trabajo de PyTorch

Este módulo sigue el segundo módulo del curso de PyTorch de DeepLearning.AI en Coursera. Arma el flujo con el que se entrena cualquier modelo en PyTorch (datos, modelo, pérdida, optimizador, dispositivo, entrenamiento y evaluación) y lo usa para clasificar los dígitos escritos a mano de MNIST.

## Contenido

| Parte | Notebooks |
|---|---|
| [00 · Datos](00-datos) | [Transforms, Dataset y DataLoader](00-datos/01_transforms_dataset_y_dataloader.ipynb) |
| [01 · Modelos](01-modelos) | [De `Sequential` a `nn.Module`](01-modelos/01_nn_module.ipynb) |
| [02 · Entrenamiento](02-entrenamiento) | [MSE y entropía cruzada en la práctica](02-entrenamiento/01_funciones_de_perdida_en_la_practica.ipynb) · [Gradientes y optimizadores](02-entrenamiento/02_gradientes_y_optimizadores.ipynb) |
| [03 · Dispositivos](03-dispositivos) | [CPU, GPU y dónde vive cada tensor](03-dispositivos/01_cpu_gpu_y_dispositivos.ipynb) |
| [04 · Clasificación de imágenes](04-clasificacion-de-imagenes) | [MNIST de punta a punta](04-clasificacion-de-imagenes/01_mnist_de_punta_a_punta.ipynb) · [Experimentos con MNIST](04-clasificacion-de-imagenes/02_experimentos_con_mnist.ipynb) |

La descripción de cada notebook está en el [README principal](../README.md).

## Los datos

Los notebooks descargan MNIST la primera vez que se ejecutan, en la carpeta `modulo-2/data`, que comparten todos. Son unos 12 MB comprimidos y unos 64 MB en disco una vez descomprimidos. La carpeta no se sube al repositorio.
