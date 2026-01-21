# Predictive_analysis_Advanced_stats_assignment1

## Methodology

### Roll-Number-Parameterized Transformation

The original feature $x$ is mapped to a transformed variable $z$ via a non-linear function $T_r(x)$.

**Transformation Equation:**
$$z = T_r(x) = x + a_r \cdot \arcsin(b_r x)$$

The parameters $a_r$ and $b_r$ are derived from the university roll number $r$ as follows: $a_r = 0.05 \times (r \bmod 7)$ $b_r = 0.3 \times (r \bmod 5 + 1)$
For my roll no 102303736: $a_r = 0.1$ $b_r = 0.9$

**For Roll No 102303736, Resulting Equation:**
$z = x + 0.1 \cdot \arcsin(0.9x)$

---

### PDF Modeling & Estimation

$z$ is: $$\hat{p}(z) = c \cdot e^{-\lambda (z - \mu)^2}$$


**Parameters Calculation:**

Mean ($\mu$): $\mathbb{E}[z]$ Lambda ($\lambda$): $\frac{1}{2\sigma^2}$ Normalization Constant ($c$): $\sqrt{\frac{\lambda}{\pi}}$


---

## Results

| Parameter | Value |
| --- | --- |
| $\mu$ | 25.8114462144 |
| $\lambda$ | 0.001460551916 |
| $c$ | 0.0215617279952 |


