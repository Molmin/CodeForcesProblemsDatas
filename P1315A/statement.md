## Description

<div><p>Screen resolution of Polycarp's monitor is $a \times b$ pixels. Unfortunately, there is one dead pixel at his screen. It has coordinates $(x, y)$ ($0 \le x &lt; a, 0 \le y &lt; b$). You can consider columns of pixels to be numbered from $0$ to $a-1$, and rows&nbsp;— from $0$ to $b-1$.</p><p>Polycarp wants to open a rectangular window of maximal size, which doesn't contain the dead pixel. The boundaries of the window should be parallel to the sides of the screen.</p><p>Print the maximal area (in pixels) of a window that doesn't contain the dead pixel inside itself.</p></div><div class="input-specification"><p>In the first line you are given an integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases in the test. In the next lines you are given descriptions of $t$ test cases.</p><p>Each test case contains a single line which consists of $4$ integers $a, b, x$ and $y$ ($1 \le a, b \le 10^4$; $0 \le x &lt; a$; $0 \le y &lt; b$)&nbsp;— the resolution of the screen and the coordinates of a dead pixel. It is guaranteed that $a+b&gt;2$ (e.g. $a=b=1$ is impossible).</p></div><div class="output-specification"><p>Print $t$ integers&nbsp;— the answers for each test case. Each answer should contain an integer equal to the maximal possible area (in pixels) of a rectangular window, that doesn't contain the dead pixel.</p></div>

## Input

<p>In the first line you are given an integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases in the test. In the next lines you are given descriptions of $t$ test cases.</p><p>Each test case contains a single line which consists of $4$ integers $a, b, x$ and $y$ ($1 \le a, b \le 10^4$; $0 \le x &lt; a$; $0 \le y &lt; b$)&nbsp;— the resolution of the screen and the coordinates of a dead pixel. It is guaranteed that $a+b&gt;2$ (e.g. $a=b=1$ is impossible).</p>

## Output

<p>Print $t$ integers&nbsp;— the answers for each test case. Each answer should contain an integer equal to the maximal possible area (in pixels) of a rectangular window, that doesn't contain the dead pixel.</p>





```input1
6
8 8 0 0
1 10 0 3
17 31 10 4
2 1 0 0
5 10 3 9
10 10 4 8
```




```output1
56
6
442
1
45
80
```



## Note

<p>In the first test case, the screen resolution is $8 \times 8$, and the upper left pixel is a dead pixel. Here you can see one of two possible layouts of the maximal window.</p><center> <img class="tex-graphics" src="file://A7hyCT9S.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
