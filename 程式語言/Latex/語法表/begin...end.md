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
- - -
3. matrix：用於創建矩陣
我有做一個專門介紹矩陣的筆記，詳細使用方法可以點[這裡](obsidian://open?vault=kuku_s_database&file=%E7%A8%8B%E5%BC%8F%E8%AA%9E%E8%A8%80%2FLatex%2F%E8%AA%9E%E6%B3%95%E8%A1%A8%2F%E7%9F%A9%E9%99%A3)。這邊我就簡單帶過。
```
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
