# ant-algoritm
Пример реализации муравьиного алгоритма для задачи комивояжёра (python 3)
## Как этоработает:
### 1. Создаем объект класса AntSwarm(distance, n_ants, n_best, n_iterations, decay, alpha=1, beta=1):
  * **distance** - матрица граффа 
  * **n_ants** - колличество муравьев за итерацию
  * **n_best** - количество элитных муравьев
  * **n_iterations** - количество итераций для поиска кротчайшего пути
  * **decay** - количество испаряемого феромона
  * n_ants, n_best, n_iterations, decay, alpha, beta подбираются опытным путем

### 2. Муравей решает куда пойти с помощью
``row=pheromone ** self.alpha*((1.0/dist)**self.beta)``
  
  
