
Eigenmode expansion (EME)

$$
\begin{align}
P_z &= \frac{1}{4}\int\int (E^*_{i,x} H_{j,y} -E^*_{i,y} H_{j,x}+E_{j,x} H^*_{i,y} -E_{j,y} H^*_{i,x}) dx dy = \delta_{ij}\\
\end{align}
$$

$$
\begin{align}
\begin{pmatrix}
i\kappa_{ii} A_i+  &\color{red}\textrm{change of propagation constant}\\
\sum_{i\ne j} i\kappa_{ij} A_j+ &\color{red}\textrm{mode coupling}\\
\delta_{ii}\partial_zA_i+ &\color{red}\textrm{eigenmode amplitude derivative}\\
\sum_{i\ne j}\delta_{ij}\partial_zA_j &\color{red}\textrm{butt coupling}\\
\end{pmatrix}
&= 0\\
\end{align}
$$
$$
\begin{align}
\partial_zA_i 
&= -i\kappa_{ii}A_i - \sum_{i\ne j}i\kappa_{ij}A_j\\
&= \sum_{i\ne j}c_{ij}A_j - i\kappa_{ii}A_i
\end{align}
$$

coupling coefficient

$$
\begin{align}
\kappa_{ij} 
&= \frac{i\omega\epsilon_0}{4}\frac{1}{\beta_j-\beta_i}(e^{-i (\beta_j-\beta_i)z}-1)
\int\int \partial_z\epsilon_r(x, y)E_i(x, y) \cdot E_j(x, y)  dx dy \\
&= ic_{ij} \\

\kappa_{ii} 
&= \frac{i\omega\epsilon_0}{4}\frac{1}{\beta_i-\beta_i}(e^{-i (\beta_i-\beta_i)z}-1)
\int\int \partial_z\epsilon_r(x, y)E_i(x, y) \cdot E_i(x, y)  dx dy \\
&= \frac{\omega\epsilon_0z}{4} \int\int \partial_z\epsilon_r(x, y)E_i(x, y) \cdot E_i(x, y)  dx dy

\end{align}
$$
