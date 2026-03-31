| Dataset | (i) Missing Complementary Classes | (ii) Empirical Sum $\sum_k p(\bar{Y} = k \mid Y = k)$ |
| :--- | :--- | :--- |
| **BCLCIFAR-10** | 0 | 0.0226 |
| **BCLCIFAR-20** | 1/20 | 0.1600 |
| **BCLCIFAR-100** | 1/100 | 0.0260 |
| **BCLTinyImageNet-200** | 93/200 | 0.1100 |

**(iii) Precise formula:**
$$\text{noise rate} = \frac{1}{C} \sum_{i=1}^{C} P(\bar{y} = i \mid y = i)$$