# Erwen Li

## Education

- Ph.D's Degree in Electrical and Computer Engineering, Oregon State University, 2014 - 2020
- Ph.D Canditate in Condensed Matter and Material Physics, Fudan University (transferred to OSU), 2011 - 2014
- BS's Degree in Physics, Fudan University, 2007 - 2011

## Academic Experience

### Ph.D, Oregon State University

- Developed TCO-gated Si micro-resonators platform for advanced photonic applications
    - Defined the entire workflow from scratch, including 
        - material modeling
        - optical simulation 
        - semiconductor process and device simulation
        - RF simulation
        - script-based layout drawing
        - semiconductor fabrication
        - high-speed electro-optical characterization
- Designed and demonestrated various Si-TCO hybrid electro-optical modulators:
    - Ultra-compact high-speed energy efficient EO modulator based on 1d photonic crystal nanocavity driven by a Si/TCO MOS capacitor (sub-fJ/bit, >23 GHz).
    - Microring modulator (design BW up to 50 GHz) and tunable filter (271 pm/V tunability)
    - Ultra-compact broadband EA modulator based on hybrid plasmonic-Si waeguide driven by an epsilon-near-zero (ENZ) TCO capacitor
- Collabrated on developing optical technologies for bio and gas sensing applications
- Published 20 journals, delieverd 12 conference oral presentations, and applied 1 US patent.
    - [publication list](https://scholar.google.com/citations?view_op=list_works&hl=zh-CN&user=FXwjSWQAAAAJ)

![[Ph.D achievements in OSU.canvas]]


### Reseach Associate, Hewlett Packard Enterprise

- Conducted theoretical modeling and experimental charaterization of an optical injection locking (OIL) transmitter based on a quantum dot microring laser and an external comb laser, which achieves high speed direct laser modulation (20 Gbps)
- Performed comprehensive design optimization for the IIIV-Si hetergeneous MOS microring modulator

## Work Experience at Siluxtek

### Comprehensive design and optimzation for MZM based EO link

- Led the design of high-speed MZM (50GBaud, 100GBaud) for use in DR4, DR8, FR4 and coherent transcievers


![[Comprehensive MZM design|1000]]

### Passive devices based on mode evolution

- refine design methodologies

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

Calculate device shap
- minimize coupling $c_{ij}$
- maximize propagation $\kappa_{ii}$

### Multiparameter-device optimization

- MZI based MUX/DeMUX
    - improve optimization speed by enable parallel computing
    
### Software tools

**Cadence SKILL VSCode pulgins**

**Database for organizing device pools and data**

**python based photonic network solver**

**python based RF circuits solver**

