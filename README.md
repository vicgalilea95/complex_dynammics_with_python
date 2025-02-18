# complex_dynammics_with_python
Este repositorio contiene principqalmente código python para dibujar tanto cuencas de atracción como planos de pará,etros en el plano complejo


# Cuenca de Atracción en el Plano Complejo usando el Método de Newton

## Definición de Cuenca de Atracción

En el **plano complejo**, una **cuenca de atracción** de un punto fijo \( z^* \) de una función \( f(z) \) es el conjunto de todos los puntos iniciales \( z_0 \) que, bajo iteraciones sucesivas de \( f \), convergen a \( z^* \).

En otras palabras, si \( z_n \) es la sucesión definida por:

\[
z_{n+1} = f(z_n)
\]

entonces la **cuenca de atracción** de \( z^* \) es el conjunto de todos los \( z_0 \) tales que:

\[
\lim_{n \to \infty} z_n = z^*
\]

## Cuenca de Atracción y el Método de Newton

El **método de Newton** es un algoritmo iterativo para encontrar raíces de una función \( f(z) \). En el **plano complejo**, este método se expresa como:

\[
z_{n+1} = z_n - \frac{f(z_n)}{f'(z_n)}
\]

Si aplicamos este método a una función polinómica \( f(z) \), típicamente encontramos varias **raíces** \( r_1, r_2, \dots, r_m \) en el plano complejo.

Cada una de estas raíces tiene su **cuenca de atracción**, es decir, el conjunto de puntos \( z_0 \) que, al iterar el método de Newton, convergen a esa raíz específica.

## Ejemplo: Aplicación a \( f(z) = z^3 - 1 \)

Consideremos la función:

\[
f(z) = z^3 - 1
\]

Sus raíces son las **tres raíces cúbicas de la unidad**:

\[
r_1 = 1, \quad r_2 = e^{2\pi i / 3}, \quad r_3 = e^{-2\pi i / 3}
\]

El método de Newton para esta función es:

\[
z_{n+1} = z_n - \frac{z_n^3 - 1}{3z_n^2}
\]

Dependiendo del punto de partida \( z_0 \), la iteración convergerá a una de las tres raíces. El **plano complejo** se divide en tres regiones, cada una correspondiente a la **cuenca de atracción** de una de las raíces.

## Fronteras Fractales

Un aspecto fascinante es que las fronteras entre estas cuencas de atracción pueden ser **fractalmente intrincadas**. Esto significa que incluso puntos muy cercanos pueden pertenecer a cuencas de atracción diferentes, mostrando estructuras altamente complejas y autosimilares.

Esta propiedad hace que la visualización de cuencas de atracción en el **método de Newton** sea un ejemplo popular en la teoría del caos y sistemas dinámicos.

## Conclusión

Las **cuencas de atracción** en el plano complejo representan conjuntos de puntos iniciales que convergen a una solución particular de una función bajo iteración. En el **método de Newton**, estas cuencas dividen el plano complejo en regiones correspondientes a diferentes soluciones, y sus fronteras pueden formar patrones fractales espectaculares.

