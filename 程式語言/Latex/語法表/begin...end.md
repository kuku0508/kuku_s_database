在某一些情況下，需要用到\\begin{}...\\end{}的指令，例如在寫聯立方程式的時候、矩陣、或是你希望方程式可以換行的狀況。
這時候可以用\\begin{環境名稱}\\end{環境名稱}來切換環境
這邊提供幾個常用環境
- - -
1. equation：用於創建單行方程式
```Latex
\begin{equation}
y = mx + b 
\end{equation}
```
$$
\begin{equation}
y=mx+b
\end{equation}
$$
- - -
2. align：用於創建多行的對其方程式
```
\begin{align}
y &= mx + b \\
&= \frac{d}{dx} (mx) + b \\
&= m
\end{align}
```
$$
\begin{align}
y &= mx + b \\
&= \frac{d}{dx} (mx) + b \\
&= m
\end{align}
$$
