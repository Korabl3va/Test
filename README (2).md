# PINN. Исследование эффективности различных методов оптимизации при обучении PINN.

## Формулировка задачи

### Уравнение теплопроводности:
$\frac{\partial^2 u}{\partial x^2}$

Тут описать про нашу задачу ... На Ане

• Импуль Нестерова (optim.SGD)  
Определяет скорость затухания накапливаемых элементов.

• RMSprop — Running Mean Square (optim.RMSprop)  
SGD + RMSprop

• Adam — Adaptive Momentum (optim.Adam)  
SGD + Adam

• L-BFGS  
...
