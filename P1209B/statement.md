## Description

<div><p>It is a holiday season, and Koala is decorating his house with cool lights! He owns $n$ lights, all of which flash periodically.</p><p>After taking a quick glance at them, Koala realizes that each of his lights can be described with two parameters $a_i$ and $b_i$. Light with parameters $a_i$ and $b_i$ will toggle (on to off, or off to on) every $a_i$ seconds starting from the $b_i$-th second. In other words, it will toggle at the moments $b_i$, $b_i + a_i$, $b_i + 2 \cdot a_i$ and so on.</p><p>You know for each light whether it's initially on or off and its corresponding parameters $a_i$ and $b_i$. Koala is wondering what is the maximum number of lights that will ever be on at the same time. So you need to find that out.</p><center> <img class="tex-graphics" height="302px" src="file://dninz0dC.png" style="max-width: 100.0%;max-height: 100.0%;" width="643px">   <span class="tex-font-size-small">Here is a graphic for the first example.</span> </center></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 100$), the number of lights.</p><p>The next line contains a string $s$ of $n$ characters. The $i$-th character is "<span class="tex-font-style-tt">1</span>", if the $i$-th lamp is initially on. Otherwise, $i$-th character is "<span class="tex-font-style-tt">0</span>".</p><p>The $i$-th of the following $n$ lines contains two integers $a_i$ and $b_i$ ($1 \le a_i, b_i \le 5$) &nbsp;— the parameters of the $i$-th light.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the maximum number of lights that will ever be on at the same time.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 100$), the number of lights.</p><p>The next line contains a string $s$ of $n$ characters. The $i$-th character is "<span class="tex-font-style-tt">1</span>", if the $i$-th lamp is initially on. Otherwise, $i$-th character is "<span class="tex-font-style-tt">0</span>".</p><p>The $i$-th of the following $n$ lines contains two integers $a_i$ and $b_i$ ($1 \le a_i, b_i \le 5$) &nbsp;— the parameters of the $i$-th light.</p>

## Output

<p>Print a single integer&nbsp;— the maximum number of lights that will ever be on at the same time.</p>





```input1
3
101
3 3
3 2
3 1
```




```input2
4
1111
3 4
5 2
3 1
3 2
```




```input3
6
011100
5 3
5 5
2 4
3 5
4 2
1 5
```




```output1
2
```




```output2
4
```




```output3
6
```



## Note

<p>For first example, the lamps' states are shown in the picture above. The largest number of simultaneously on lamps is $2$ (e.g. at the moment $2$).</p><p>In the second example, all lights are initially on. So the answer is $4$.</p>
