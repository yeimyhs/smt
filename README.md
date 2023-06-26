# smt

El método de Galerkin y el método de Gauss son dos técnicas numéricas para resolver ecuaciones diferenciales parciales. Ambos métodos se basan en la idea de aproximar la solución mediante una combinación lineal de funciones de prueba o base, y luego minimizar el error entre la solución aproximada y la solución exacta. La diferencia entre los dos métodos radica en la forma de definir el error y el criterio de minimización.

El método de Galerkin define el error como la proyección ortogonal del residuo de la ecuación diferencial sobre el espacio generado por las funciones de prueba. El criterio de minimización es que el error sea cero para todas las funciones de prueba, lo que conduce a un sistema de ecuaciones lineales para los coeficientes de la combinación lineal. La fórmula general del método de Galerkin es:

$$\int_\Omega R(u) \phi_i d\Omega = 0 \quad \forall i = 1, ..., N$$

donde $R(u)$ es el residuo de la ecuación diferencial, $\phi_i$ son las funciones de prueba y $N$ es el número de funciones de prueba.

El método de Gauss define el error como la diferencia al cuadrado entre la solución aproximada y la solución exacta. El criterio de minimización es que el error sea mínimo en un conjunto de puntos llamados puntos de Gauss, que se eligen según una distribución de probabilidad. La fórmula general del método de Gauss es:

$$\sum_{i=1}^N w_i (u(x_i) - u_e(x_i))^2 = \min$$

donde $w_i$ son los pesos asociados a los puntos de Gauss, $u(x_i)$ es la solución aproximada, $u_e(x_i)$ es la solución exacta y $N$ es el número de puntos de Gauss.
