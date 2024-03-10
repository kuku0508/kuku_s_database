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
2. align：用於創建多行的對齊方程式
然後下面的&的作用在於「決定對齊點」
\\\\的作用在於換行
```Latex
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
- - -
3. matrix：用於創建矩陣
我有做一個專門介紹矩陣的筆記，詳細使用方法可以點[這裡](obsidian://open?vault=kuku_s_database&file=%E7%A8%8B%E5%BC%8F%E8%AA%9E%E8%A8%80%2FLatex%2F%E8%AA%9E%E6%B3%95%E8%A1%A8%2F%E7%9F%A9%E9%99%A3)。這邊我就簡單帶過。
```Latex
\begin{matrix}
    1 & 2 \\
    3 & 4
\end{matrix}
```
$$
\begin{matrix}
	1 & 2 \\
	3 & 4 
\end{matrix}
$$
- - -
4. cases：用於創建帶有分段函數的方程式(聯立方程式)
而下面的\\\\跟&分別功能是換行還有「決定對齊點」，值得注意的是，對齊線其實可以有數個，每一行的每一個「&」都會去對應下一行的「&」。
```Latex
\begin{cases}
    \text{條件1} & \text{結果1a} & \text{結果1b} \\
    \text{條件2} & \text{結果2a} & \text{結果2b} \\
    \text{條件3} & \text{結果3a} & \text{結果3b}
\end{cases}

f(x) =
\begin{cases}
    x^2, & \text{if } x > 0 \\
    -x^2, & \text{if } x < 0 \\
    0, & \text{if } x = 0
\end{cases}
```
$$
\begin{cases}
    \text{條件1} & \text{結果1a} & \text{結果1b} \\
    \text{條件2} & \text{結果2a} & \text{結果2b} \\
    \text{條件3} & \text{結果3a} & \text{結果3b}
\end{cases}
$$
$$
f(x) =
\begin{cases}
    x^2, & \text{if } x > 0 \\
    -x^2, & \text{if } x < 0 \\
    0, & \text{if } x = 0
\end{cases}
$$
- - -
5. alignat：用於創建多行的對齊方程式，提供更靈活地對齊控制。
我其實有點看不懂他跟align的差別在哪。
```
\begin{alignat}{2}
    y &= mx &+& b \\
    &= \frac{d}{dx} (mx) &+& b \\
    &= m
\end{alignat}
```
$$
\begin{alignat}{2}
    y &= mx &+& b \\
    &= \frac{d}{dx} (mx) &+& b \\
    &= m
\end{alignat}
$$