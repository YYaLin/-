$$\overrightarrow{x_i} = [x_1^i, x_2^i, \ldots, x_m^i]$$  

$$\vec{\beta} = [\beta_0, \beta_1, \ldots, \beta_m]$$

$$y_i \approx \beta_0 + \sum_{j=1}^m \beta_j \times x_j^i.$$

$$\overrightarrow{x_i} = [1, x_1^i, x_2^i, \ldots, x_m^i]$$

$$y_i \approx \sum_{j=0}^m \beta_j \times x_j^i = \vec{\beta} \cdot \overrightarrow{x_i}.$$

$$\vec{\hat{\beta}} = \arg\min_{\vec{\beta}} L\left(D, \vec{\beta}\right) = \arg\min_{\vec{\beta}} \sum_{i=1}^{n} \left(\vec{\beta} \cdot \vec{x}_i - y_i\right)^2$$

$$\begin{align*}
L\left(D, \vec{\beta}\right) &= ||X\vec{\beta} - Y||^2 \\
&= \left(X\vec{\beta} - Y\right)^T \left(X\vec{\beta} - Y\right) \\
&= Y^TY - Y^TX\vec{\beta} - \vec{\beta}^T X^TY + \vec{\beta}^T X^TX\vec{\beta}
\end{align*}$$

$$\begin{aligned}
\frac{\partial L\left(D, \vec{\beta}\right)}{\partial \vec{\beta}} 
&= \frac{\partial \left(Y^TY - Y^TX\vec{\beta} - \vec{\beta}^T X^TY + \vec{\beta}^T X^TX\vec{\beta}\right)}{\partial \vec{\beta}} \\
&= -2X^TY + 2X^TX\vec{\beta}
\end{aligned}$$

$$\begin{align*}
-2X^TY + 2X^TX\vec{\beta} = 0 
\Rightarrow X^TX\vec{\beta} = X^TY 
\Rightarrow\vec{\hat{\beta}} = \left(X^TX\right)^{-1}X^TY
\end{align*}$$

