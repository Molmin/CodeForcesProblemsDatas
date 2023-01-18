## Description

<div><p>One day Sasha visited the farmer 2D and his famous magnetic farm. On this farm, the crop grows due to the influence of a special magnetic field. Maintaining of the magnetic field is provided by $n$ machines, and the power of the $i$-th machine is $a_i$. </p><p>This year 2D decided to cultivate a new culture, but what exactly he didn't say. For the successful growth of the new culture, it is necessary to slightly change the powers of the machines. 2D can <span class="tex-font-style-bf">at most once</span> choose an arbitrary integer $x$, then choose one machine and reduce the power of its machine by $x$ times, and at the same time increase the power of one another machine by $x$ times (powers of all the machines must stay <span class="tex-font-style-bf">positive integers</span>). Note that he may not do that if he wants. More formally, 2D can choose two such indices $i$ and $j$, and one integer $x$ such that $x$ is a divisor of $a_i$, and change powers as following: $a_i = \frac{a_i}{x}$, $a_j = a_j \cdot x$</p><p>Sasha is very curious, that's why he wants to calculate the <span class="tex-font-style-bf">minimum</span> total power the farmer can reach. There are too many machines, and Sasha can't cope with computations, help him!</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($2 \le n \le 5 \cdot 10^4$)&nbsp;— the number of machines.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 100$)&nbsp;— the powers of the machines.</p></div><div class="output-specification"><p>Print one integer&nbsp;— minimum total power.</p></div>

## Input

<p>The first line contains one integer $n$ ($2 \le n \le 5 \cdot 10^4$)&nbsp;— the number of machines.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 100$)&nbsp;— the powers of the machines.</p>

## Output

<p>Print one integer&nbsp;— minimum total power.</p>





```input1
5
1 2 3 4 5
```




```input2
4
4 2 4 4
```




```input3
5
2 4 2 3 7
```




```output1
14
```




```output2
14
```




```output3
18
```



## Note

<p>In the first example, the farmer can reduce the power of the $4$-th machine by $2$ times, and increase the power of the $1$-st machine by $2$ times, then the powers will be: $[2, 2, 3, 2, 5]$.</p><p>In the second example, the farmer can reduce the power of the $3$-rd machine by $2$ times, and increase the power of the $2$-nd machine by $2$ times. At the same time, the farmer can leave is be as it is and the total power won't change.</p><p>In the third example, it is optimal to leave it be as it is.</p>
