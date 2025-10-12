# Mátrixok

## Mátrix műveletek

$$ A = \begin{bmatrix} a_{11} & a_{12} \\ a_{21} & a_{22} \end{bmatrix} \quad B = \begin{bmatrix} b_{11} & b_{12} \\ b_{21} & b_{22} \end{bmatrix} $$

$$ A + B = \begin{bmatrix} a_{11} + b_{11} & a_{12} + b_{12} \\ a_{21} + b_{21} & a_{22} + b_{22} \end{bmatrix} $$

$$ A - B = \begin{bmatrix} a_{11} - b_{11} & a_{12} - b_{12} \\ a_{21} - b_{21} & a_{22} - b_{22} \end{bmatrix} $$

$$ A \times B = \begin{bmatrix} a_{11}b_{11} + a_{12}b_{21} & a_{11}b_{12} + a_{12}b_{22} \\ a_{21}b_{11} + a_{22}b_{21} & a_{21}b_{12} + a_{22}b_{22} \end{bmatrix} $$

## Gauss-Jordan elimináció

Elvégezhető műveletek
- Megszorozahtunk egy sort egy konstansal (nem 0)
- Felcserélhetünk 2 sort
- Egy sor konstans szorosát hozzá adhatjuk egy másik sorhoz

$$
\begin{cases}
x + 2y = 5 \\
3x + y = 5
\end{cases}
$$

$$
\left[
\begin{array}{cc|c}
1 & 2 & 5 \\
3 & 1 & 5
\end{array}
\right]
$$

$$
R_2 \leftarrow R_2 - 3R_1
$$

$$
\left[
\begin{array}{cc|c}
1 & 2 & 5 \\
0 & -5 & -10
\end{array}
\right]
$$

$$
R_2 \leftarrow \frac{1}{-5}R_2
$$

$$
\left[
\begin{array}{cc|c}
1 & 2 & 5 \\
0 & 1 & 2
\end{array}
\right]
$$

$$
R_1 \leftarrow R_1 - 2R_2
$$

$$
\left[
\begin{array}{cc|c}
1 & 0 & 1 \\
0 & 1 & 2
\end{array}
\right]
$$