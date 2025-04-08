---
jupytext:
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
    format_version: 0.13
    jupytext_version: 1.11.5
kernelspec:
  display_name: Python 3
  language: python
  name: python3
---

# Nonlinear Properties of Material

A nonlinear polarization term is introduced explicitly as follows:

$$ P_i = \varepsilon_0 \chi^{(1)}_{ii} E_i + \varepsilon _0 \chi^{(2)}_{iii} E^2_i+ \varepsilon _0 \chi^{(3)}_{iiii} E^3_i \,\,\, (i\in\{x,y,z\}) $$

And
$\bar D$ is then defined as: $\bar D=\varepsilon_{0} \bar E + \bar P$.

```{note}
$ \varrho ^{(k)}_{i}$ is then defined as: $ \varrho^{(k)}_{i} = P^{(k)}_{i} / \varepsilon _0$ for $ k = 2,3 $.
```

## Full Tensorial $\chi^{(1)}$

$$ 
\begin{bmatrix}
\varrho ^{(1)}_{x} \\
\varrho ^{(1)}_{y} \\
\varrho ^{(1)}_{z}
\end{bmatrix}
=\begin{bmatrix}
\chi^{(1)}_{11} & \chi^{(1)}_{12} & \chi^{(1)}_{13} \\
\chi^{(1)}_{21} & \chi^{(1)}_{22} & \chi^{(1)}_{23} \\ 
\chi^{(1)}_{31} & \chi^{(1)}_{32} & \chi^{(1)}_{33} 
\end{bmatrix} 
\begin{bmatrix}
E_{x} \\
E_{y} \\
E_{z} 
\end{bmatrix} 
$$ 

## Full Tensorial $\chi^{(2)}$


$$ 
\begin{bmatrix}
\varrho ^{(2)}_{x} \\
\varrho ^{(2)}_{y} \\
\varrho ^{(2)}_{z}
\end{bmatrix}
=2\begin{bmatrix}
d_{11} & d_{12} & d_{13} & d_{14} & d_{15} & d_{16} \\
d_{21} & d_{22} & d_{23} & d_{24} & d_{25} & d_{26} \\ 
d_{31} & d_{32} & d_{33} & d_{34} & d_{35} & d_{36}
\end{bmatrix} 
\begin{bmatrix}
E^{2}_{x} \\
E^{2}_{y} \\
E^{2}_{z} \\
2E_{y}E_{z} \\
2E_{x}E_{z} \\
2E_{x}E_{y} 
\end{bmatrix} 
$$ 


## Full Tensorial $\chi^{(3)}$


$$ 
\begin{bmatrix}
\varrho ^{(3)}_{x} \\
\varrho ^{(3)}_{y} \\
\varrho ^{(3)}_{z}
\end{bmatrix}
=2\begin{bmatrix}
T_{11} & T_{12} & T_{13} & T_{14} & T_{15} & T_{16} & T_{17} & T_{18} & T_{19} & T_{110} \\
T_{21} & T_{22} & T_{23} & T_{24} & T_{25} & T_{26} & T_{27} & T_{28} & T_{29} & T_{210} \\ 
T_{31} & T_{32} & T_{33} & T_{34} & T_{35} & T_{36} & T_{37} & T_{38} & T_{39} & T_{310}
\end{bmatrix} \begin{bmatrix}
E^{3}_{x} \\
E^{3}_{y} \\
E^{3}_{z} \\
3E^{2}_{z}E_{x} \\
3E^{2}_{z}E_{y} \\
3E^{2}_{y}E_{z} \\
3E^{2}_{y}E_{x} \\
3E^{2}_{x}E_{y} \\
3E^{2}_{x}E_{z} \\
6E_{x}E_{y}E_{z}
\end{bmatrix}
$$

## Different Materials

### Isotropic $\chi^{(3)}$ 

$$
\chi^{(3)}
\begin{bmatrix}
3 & 0 & 0 & 1 & 0 & 0 & 1 & 0 & 0 & 0 \\
0 & 3 & 0 & 0 & 1 & 0 & 0 & 1 & 0 & 0 \\
0 & 0 & 3 & 0 & 0 & 1 & 0 & 0 & 1 & 0
\end{bmatrix}
$$

### Calcite (Calcium Carbonate $CaCO_{3}$ )

$$
\chi^{(3)}_{iiii}
=
\begin{bmatrix}
{\chi}_{11} & 0 & 0 & {\chi}_{14} & 0 & 0 & \frac{1}{3}{\chi}_{11} & 0 & 0 & {\chi}_{110} \\
0 & {\chi}_{11} & 0 & 0 & {\chi}_{14} & -{\chi}_{110} & 0 & \frac{1}{3}{\chi}_{11} & {\chi}_{110} & 0 \\ 
0 & -{\chi}_{38} & {\chi}_{33} & 0 & 0 & {\chi}_{36} & 0 & {\chi}_{38} & {\chi}_{36} & 0
\end{bmatrix}
$$