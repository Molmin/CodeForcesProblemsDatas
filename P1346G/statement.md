## Description

<div><p>You have two IP cameras of the same model. Each camera can take photos starting from some moment of time with a fixed period. You can freely choose the starting moment but you can choose the period only as one of $k$ values $p_1, p_2, \dots, p_k$ which are chosen by the camera's manufacturer.</p><p>You have $n$ moments of interest $x_1, x_2, \dots, x_n$. You'd like to configure both cameras in such a way that at least one camera will take a photo in each of these moments. Configuring the camera means setting the moment when it takes the first photo and the gap between two consecutive photos (which should be one of the values $p_1, p_2, \dots, p_k$). It's not a problem for you that cameras can take photos at other moments of time&nbsp;— you only care about moments of interest.</p></div><div class="input-specification"><p>The first line contains two integers $k$ and $n$ ($1 \le k \le 10^5$; $2 \le n \le 10^5$)&nbsp;— the number of periods to choose and the number of moments of interest.</p><p>The second line contains $k$ integers $p_1, p_2, \dots, p_k$ ($1 \le p_1 &lt; p_2 &lt; \dots &lt; p_k \le 10^6$)&nbsp;— the periods to choose in the ascending order.</p><p>The third line contains $n$ integers $x_1, x_2, \dots, x_n$ ($1 \le x_1 &lt; x_2 &lt; \dots &lt; x_n \le 10^6$)&nbsp;— the moments of interest in the ascending order.</p></div><div class="output-specification"><p>Print <span class="tex-font-style-tt">YES</span> (case insensitive) in the first line if there is a way to configure cameras.</p><p>In the second line, print two integers $s_1$ and $cp_1$ ($1 \le s_1 \le 10^6$; $1 \le cp_1 \le 10^6$; $cp_1 \in \{p_1, \dots, p_k\}$)&nbsp;— the starting moment and the period for the first camera. The period should be one of the given periods.</p><p>In the third line, print two integers $s_2$ and $cp_2$ ($1 \le s_2 \le 10^6$; $1 \le cp_2 \le 10^6$; $cp_2 \in \{p_1, \dots, p_k\}$)&nbsp;— the starting moment and the period for the second camera. The period should be one of the given periods.</p><p>If there is no way to configure cameras, print <span class="tex-font-style-tt">NO</span> (case insensitive). If there are multiple ways, you may print any of them.</p></div>

## Input

<p>The first line contains two integers $k$ and $n$ ($1 \le k \le 10^5$; $2 \le n \le 10^5$)&nbsp;— the number of periods to choose and the number of moments of interest.</p><p>The second line contains $k$ integers $p_1, p_2, \dots, p_k$ ($1 \le p_1 &lt; p_2 &lt; \dots &lt; p_k \le 10^6$)&nbsp;— the periods to choose in the ascending order.</p><p>The third line contains $n$ integers $x_1, x_2, \dots, x_n$ ($1 \le x_1 &lt; x_2 &lt; \dots &lt; x_n \le 10^6$)&nbsp;— the moments of interest in the ascending order.</p>

## Output

<p>Print <span class="tex-font-style-tt">YES</span> (case insensitive) in the first line if there is a way to configure cameras.</p><p>In the second line, print two integers $s_1$ and $cp_1$ ($1 \le s_1 \le 10^6$; $1 \le cp_1 \le 10^6$; $cp_1 \in \{p_1, \dots, p_k\}$)&nbsp;— the starting moment and the period for the first camera. The period should be one of the given periods.</p><p>In the third line, print two integers $s_2$ and $cp_2$ ($1 \le s_2 \le 10^6$; $1 \le cp_2 \le 10^6$; $cp_2 \in \{p_1, \dots, p_k\}$)&nbsp;— the starting moment and the period for the second camera. The period should be one of the given periods.</p><p>If there is no way to configure cameras, print <span class="tex-font-style-tt">NO</span> (case insensitive). If there are multiple ways, you may print any of them.</p>





```input1
3 5
3 5 7
1 4 5 7 12
```




```input2
3 2
1 2 3
1 10
```




```input3
3 4
1 2 3
5 7 9 11
```




```input4
3 4
10 20 100
2 3 4 7
```




```output1
YES
1 3
5 7
```




```output2
YES
1 1
10 1
```




```output3
YES
5 1
5 1
```




```output4
NO
```


