## Description

<div><p>On his free time, Chouti likes doing some housework. He has got one new task, paint some bricks in the yard.</p><p>There are $n$ bricks lined in a row on the ground. Chouti has got $m$ paint buckets of different colors at hand, so he painted each brick in one of those $m$ colors.</p><p>Having finished painting all bricks, Chouti was satisfied. He stood back and decided to find something fun with these bricks. After some counting, he found there are $k$ bricks with a color different from the color of the brick on its left (the first brick is not counted, for sure).</p><p>So as usual, he needs your help in counting how many ways could he paint the bricks. Two ways of painting bricks are different if there is at least one brick painted in different colors in these two ways. Because the answer might be quite big, you only need to output the number of ways modulo $998\,244\,353$.</p></div><div class="input-specification"><p>The first and only line contains three integers $n$, $m$ and $k$ ($1 \leq n,m \leq 2000, 0 \leq k \leq n-1$)&nbsp;— the number of bricks, the number of colors, and the number of bricks, such that its color differs from the color of brick to the left of it.</p></div><div class="output-specification"><p>Print one integer&nbsp;— the number of ways to color bricks modulo $998\,244\,353$.</p></div>

## Input

<p>The first and only line contains three integers $n$, $m$ and $k$ ($1 \leq n,m \leq 2000, 0 \leq k \leq n-1$)&nbsp;— the number of bricks, the number of colors, and the number of bricks, such that its color differs from the color of brick to the left of it.</p>

## Output

<p>Print one integer&nbsp;— the number of ways to color bricks modulo $998\,244\,353$.</p>





```input1
3 3 0
```




```input2
3 2 1
```




```output1
3
```




```output2
4
```



## Note

<p>In the first example, since $k=0$, the color of every brick should be the same, so there will be exactly $m=3$ ways to color the bricks.</p><p>In the second example, suppose the two colors in the buckets are yellow and lime, the following image shows all $4$ possible colorings.</p><center> <img class="tex-graphics" src="file://8GMgYxYX.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
