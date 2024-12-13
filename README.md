# PINN. Исследование эффективности различных методов оптимизации при обучении PINN.

## Точная постановка задачи

### *Уравнение теплопроводности:*

$$
\frac{\partial u}{\partial t} = \alpha \frac{\partial^2 u}{\partial x^2}, \quad x \in (0, L), \quad t > 0
$$

### *Начальные и граничные условия:*

$$
\begin{cases}
u(x, 0) = f(x), & x \in [0, L] \\
u(0, t) = u(L, t) = 0, & t > 0
\end{cases}
$$

### *Задача:*
Реализовать PINN метод решения начально-краевой задачи для уравнения теплопроводности. Сравнить эффективность различных оптимизаторов (SGD, Adam, RMSprop, L-BFGS).

## Испльзуемые методы:

- **Импульс Нестерова (optim.SGD)**
  Определяет скорость затухания накапливаемых элементов.

- **RMSprop — Running Mean Square (optim.RMSprop)**
  *SGD + RMSprop*

- **Adam — Adaptive Momentum (optim.Adam)**
  *SGD + Adam*

- **L-BFGS**
