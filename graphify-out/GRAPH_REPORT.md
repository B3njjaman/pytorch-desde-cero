# Graph Report - corpus  (2026-10-14)

## Corpus Check
- Corpus is ~30,065 words - fits in a single context window. You may not need a graph.

## Summary
- 116 nodes · 152 edges · 9 communities (8 shown, 1 thin omitted)
- Extraction: 89% EXTRACTED · 11% INFERRED · 0% AMBIGUOUS · INFERRED: 16 edges (avg confidence: 0.83)
- Token cost: 273,001 input · 0 output

## Community Hubs (Navigation)
- Ciclo de entrenamiento y descenso
- Optimalidad y retropropagación
- Estructura del curso y tensores
- Activaciones y funciones de pérdida
- Neurona y red con capa oculta
- Normalización y SGD estocástico
- Optimizadores y condicionamiento
- Autograd y regla de la cadena
- Notebook de pérdidas

## God Nodes (most connected - your core abstractions)
1. `Regla de actualizacion w <- w - eta * grad` - 6 edges
2. `Curso PyTorch desde cero` - 6 edges
3. `Hessiano y sus autovalores` - 6 edges
4. `Momento (SGD momentum)` - 6 edges
5. `Notebook: Tensores, autograd y una neurona` - 5 edges
6. `Autograd` - 5 edges
7. `Entrenamiento a mano con descenso de gradiente (y = 2x + 1)` - 5 edges
8. `Notebook: Descenso de gradiente` - 5 edges
9. `Convexidad` - 5 edges
10. `Regla de la cadena` - 5 edges

## Surprising Connections (you probably didn't know these)
- `Punto silla` --semantically_similar_to--> `Gradiente que se desvanece`  [INFERRED] [semantically similar]
  03-optimalidad__01_optimalidad.md → 04-matematica-de-pytorch__02_capas_y_activaciones.md
- `descenso(x, y, lr, pasos)` --semantically_similar_to--> `Entrenamiento a mano con descenso de gradiente (y = 2x + 1)`  [INFERRED] [semantically similar]
  02-descenso-de-gradiente__01_descenso_de_gradiente.md → 00-fundamentos__01_tensores_autograd_y_una_neurona.md
- `Tasa de aprendizaje` --semantically_similar_to--> `Tasa de aprendizaje (lr)`  [INFERRED] [semantically similar]
  02-descenso-de-gradiente__01_descenso_de_gradiente.md → 00-fundamentos__01_tensores_autograd_y_una_neurona.md
- `Ciclo de entrenamiento en 5 pasos` --semantically_similar_to--> `Ciclo de entrenamiento (prediccion, perdida, zero_grad, backward, step)`  [INFERRED] [semantically similar]
  01-red-neuronal-simple__01_red_neuronal_simple.md → 00-fundamentos__01_tensores_autograd_y_una_neurona.md
- `entrenar(x, y, tam_lote, lr, epocas)` --semantically_similar_to--> `entrenar(modelo, X, y, lr, epocas)`  [INFERRED] [semantically similar]
  02-descenso-de-gradiente__02_sgd_y_minibatches.md → 01-red-neuronal-simple__01_red_neuronal_simple.md

## Import Cycles
- None detected.

## Hyperedges (group relationships)
- **Ciclo de entrenamiento PyTorch (prediccion, perdida, zero_grad, backward, step)** — 00_fundamentos__01_tensores_autograd_y_una_neurona_ciclo_de_entrenamiento, 00_fundamentos__01_tensores_autograd_y_una_neurona_autograd, 00_fundamentos__01_tensores_autograd_y_una_neurona_acumulacion_de_gradientes, 00_fundamentos__01_tensores_autograd_y_una_neurona_torch_optim_sgd, 00_fundamentos__01_tensores_autograd_y_una_neurona_mse, 01_red_neuronal_simple__01_red_neuronal_simple_ciclo_de_entrenamiento [EXTRACTED 1.00]
- **Normalizacion, curvatura y tasa de aprendizaje maxima** — 01_red_neuronal_simple__01_red_neuronal_simple_normalizacion, 02_descenso_de_gradiente__01_descenso_de_gradiente_por_que_normalizar, 02_descenso_de_gradiente__01_descenso_de_gradiente_valle_angosto, 02_descenso_de_gradiente__01_descenso_de_gradiente_curvatura, 02_descenso_de_gradiente__01_descenso_de_gradiente_tasa_de_aprendizaje [INFERRED 0.85]
- **Control del ruido en SGD (lote, tasa decreciente, Robbins-Monro, scheduler)** — 02_descenso_de_gradiente__02_sgd_y_minibatches_ruido_sgd, 02_descenso_de_gradiente__02_sgd_y_minibatches_estimacion_gradiente_lote, 02_descenso_de_gradiente__02_sgd_y_minibatches_tasa_decreciente, 02_descenso_de_gradiente__02_sgd_y_minibatches_robbins_monro, 02_descenso_de_gradiente__02_sgd_y_minibatches_lr_scheduler [EXTRACTED 1.00]
- **Pérdidas derivadas de máxima verosimilitud** — 04_matematica_de_pytorch__03_funciones_de_perdida_maxima_verosimilitud, 04_matematica_de_pytorch__03_funciones_de_perdida_mseloss, 04_matematica_de_pytorch__03_funciones_de_perdida_l1loss, 04_matematica_de_pytorch__03_funciones_de_perdida_bceloss, 04_matematica_de_pytorch__03_funciones_de_perdida_crossentropyloss [EXTRACTED 1.00]
- **Familia de optimizadores de torch.optim (SGD → momento → RMSprop → Adam → AdamW)** — 04_matematica_de_pytorch__04_optimizadores_sgd, 04_matematica_de_pytorch__04_optimizadores_momento, 04_matematica_de_pytorch__04_optimizadores_nesterov, 04_matematica_de_pytorch__04_optimizadores_rmsprop, 04_matematica_de_pytorch__04_optimizadores_adam, 04_matematica_de_pytorch__04_optimizadores_adamw [EXTRACTED 1.00]
- **Mecanismo de backward(): regla de la cadena, grafo, VJP y reglas locales** — 04_matematica_de_pytorch__01_autograd_y_regla_de_la_cadena_regla_de_la_cadena, 04_matematica_de_pytorch__01_autograd_y_regla_de_la_cadena_grafo_computacional, 04_matematica_de_pytorch__01_autograd_y_regla_de_la_cadena_producto_vector_jacobiano, 04_matematica_de_pytorch__01_autograd_y_regla_de_la_cadena_reglas_locales, 04_matematica_de_pytorch__01_autograd_y_regla_de_la_cadena_retropropagacion [EXTRACTED 1.00]

## Communities (9 total, 1 thin omitted)

### Community 0 - "Ciclo de entrenamiento y descenso"
Cohesion: 0.11
Nodes (20): Autograd, Ciclo de entrenamiento (prediccion, perdida, zero_grad, backward, step), Entrenamiento a mano con descenso de gradiente (y = 2x + 1), Error cuadratico medio (MSE / nn.MSELoss), Tasa de aprendizaje (lr), torch.optim.SGD, Ciclo de entrenamiento en 5 pasos, entrenar(modelo, X, y, lr, epocas) (+12 more)

### Community 1 - "Optimalidad y retropropagación"
Cohesion: 0.13
Nodes (17): clasificar() (punto crítico vía autovalores del hessiano), Convexidad, Cuenca de atracción (dependencia de la inicialización), Ecuaciones normales (AᵀA θ = Aᵀy), Hessiano y sus autovalores, Mínimo global vs mínimo local, Optimalidad: mínimos, convexidad y puntos silla, Punto silla (+9 more)

### Community 2 - "Estructura del curso y tensores"
Cohesion: 0.18
Nodes (14): Atributos shape, dtype, device, Broadcasting, Notebook: Tensores, autograd y una neurona, Puente con NumPy, Tensor, Notebook: Una red neuronal simple, Problema del repartidor (7 millas, 30 minutos), Entrenar es minimizar la perdida (+6 more)

### Community 3 - "Activaciones y funciones de pérdida"
Cohesion: 0.20
Nodes (13): Cota de tasa de aprendizaje η < 2/λmax, La pérdida MSE de una neurona es convexa (H = 2/N AᵀA), Gradiente que se desvanece, Sigmoid σ(z), Softmax (jacobiano diag(p) - ppᵀ), Tanh (tanh(z) = 2σ(2z) - 1), BCELoss (Bernoulli, entropía cruzada binaria), BCEWithLogitsLoss (+5 more)

### Community 4 - "Neurona y red con capa oculta"
Cohesion: 0.17
Nodes (11): Entropia cruzada binaria (nn.BCELoss), Compuerta logica AND, Neurona (nn.Module), Neurona artificial (w·x + b, activacion), nn.Linear, Producto matricial (@), Activacion sigmoide, state_dict (guardar y cargar modelo) (+3 more)

### Community 5 - "Normalización y SGD estocástico"
Cohesion: 0.17
Nodes (8): predecir_minutos(modelo, millas), superficie(x, y, rango_w, rango_b), Superficie de perdida L(w, b), Estimacion del gradiente con un lote (sin sesgo, ruido 1/sqrt(B)), torch.optim.lr_scheduler, Condiciones de Robbins-Monro, Descenso de gradiente estocastico (SGD), tasa_decreciente (eta0 / (1 + t/tau))

### Community 6 - "Optimizadores y condicionamiento"
Cohesion: 0.22
Nodes (9): Número de condición κ = λmax/λmin, Adam (adaptive moment estimation), AdamW: decaimiento de pesos desacoplado, Momento (SGD momentum), Momento de Nesterov, Polyak (1964): parámetros óptimos del momento, RMSprop: una tasa por parámetro, Comparación de optimizadores en un valle angosto (κ = 88) (+1 more)

### Community 7 - "Autograd y regla de la cadena"
Cohesion: 0.31
Nodes (7): detach() y no_grad(): cortar el grafo, Grafo computacional (grad_fn, AccumulateGrad), Derivada, gradiente y jacobiano, La matemática de autograd: regla de la cadena y retropropagación, Regla de la cadena, La matemática de las capas y las activaciones, SGD (θ ← θ - ηg)

## Knowledge Gaps
- **29 isolated node(s):** `Atributos shape, dtype, device`, `Broadcasting`, `Producto matricial (@)`, `Puente con NumPy`, `Error cuadratico medio (MSE / nn.MSELoss)` (+24 more)
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 33 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)
- **1 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `Notebook: Tensores, autograd y una neurona` connect `Estructura del curso y tensores` to `Ciclo de entrenamiento y descenso`, `Neurona y red con capa oculta`?**
  _High betweenness centrality (0.144) - this node is a cross-community bridge._
- **What connects `Atributos shape, dtype, device`, `Broadcasting`, `Producto matricial (@)` to the rest of the system?**
  _29 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Should `Ciclo de entrenamiento y descenso` be split into smaller, more focused modules?**
  _Cohesion score 0.11067193675889328 - nodes in this community are weakly interconnected._
- **Why does `Neurona artificial (w·x + b, activacion)` connect `Neurona y red con capa oculta` to `Estructura del curso y tensores`?**
  _High betweenness centrality (0.094) - this node is a cross-community bridge._
- **Should `Optimalidad y retropropagación` be split into smaller, more focused modules?**
  _Cohesion score 0.13071895424836602 - nodes in this community are weakly interconnected._
- **Why does `Autograd` connect `Ciclo de entrenamiento y descenso` to `Estructura del curso y tensores`?**
  _High betweenness centrality (0.091) - this node is a cross-community bridge._