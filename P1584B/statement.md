## Description

<div><p>David was given a <span class="tex-font-style-bf">red</span> checkered rectangle of size $n \times m$. But he doesn't like it. So David cuts the original or any other rectangle piece obtained during the cutting into two new pieces along the grid lines. He can do this operation as many times as he wants.</p><p>As a result, he will get a set of rectangles. Rectangles $1 \times 1$ are <span class="tex-font-style-bf">forbidden</span>.</p><p>David also knows how to paint the cells <span class="tex-font-style-bf">blue</span>. He wants each rectangle from the resulting set of pieces to be colored such that any pair of adjacent cells by side (from the same piece) have different colors.</p><p>What is the minimum number of cells David will have to paint?</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 10^3$)&nbsp;— the number of test cases. The next lines contain descriptions of test cases.</p><p>The only line of each test case contains two integers $n$, $m$ ($1 \leq n, m \leq 3 \cdot 10^4$, $n \cdot m \geq 2$).</p></div><div class="output-specification"><p>For each test case print a single integer — the minimum number of cells David will have to paint blue.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 10^3$)&nbsp;— the number of test cases. The next lines contain descriptions of test cases.</p><p>The only line of each test case contains two integers $n$, $m$ ($1 \leq n, m \leq 3 \cdot 10^4$, $n \cdot m \geq 2$).</p>

## Output

<p>For each test case print a single integer — the minimum number of cells David will have to paint blue.</p>





```input1
4
1 3
2 2
2 5
3 5
```




```output1
1
2
4
5
```



## Note

<p>The following pictures show how the initial rectangle can be split and cells colored blue.</p><p>In the first test case:</p><center> <img class="tex-graphics" src="file://0FN0NfMb.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the second test case:</p><center> <img class="tex-graphics" src="file://t11pyPwL.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the third test case:</p><center> <img class="tex-graphics" src="file://DURf1TTk.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the fourth test case:</p><center> <img class="tex-graphics" src="file://pov6n0NC.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
