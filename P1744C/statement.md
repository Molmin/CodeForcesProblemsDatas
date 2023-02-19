## Description

<div><p>You find yourself on an unusual crossroad with a weird traffic light. That traffic light has three possible colors: red (<span class="tex-font-style-tt">r</span>), yellow (<span class="tex-font-style-tt">y</span>), green (<span class="tex-font-style-tt">g</span>). It is known that the traffic light repeats its colors every $n$ seconds and at the $i$-th second the color $s_i$ is on.</p><p>That way, the order of the colors is described by a string. For example, if $s=$"<span class="tex-font-style-tt">rggry</span>", then the traffic light works as the following: red-green-green-red-yellow-red-green-green-red-yellow- ... and so on.</p><p>More formally, you are given a string $s_1, s_2, \ldots, s_n$ of length $n$. At the first second the color $s_1$ is on, at the second — $s_2$, ..., at the $n$-th second the color $s_n$ is on, at the $n + 1$-st second the color $s_1$ is on and so on.</p><p>You need to cross the road and that can only be done when the green color is on. </p><p>You know which color is on the traffic light at the moment, but you don't know the current moment of time. You need to find the minimum amount of time in which you are guaranteed to cross the road.</p><p>You can assume that you cross the road immediately. </p><p>For example, with $s=$"<span class="tex-font-style-tt">rggry</span>" and the current color <span class="tex-font-style-tt">r</span> there are two options: either the green color will be on after $1$ second, or after $3$. That way, the answer is equal to $3$ — that is the number of seconds that we are guaranteed to cross the road, if the current color is <span class="tex-font-style-tt">r</span>.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ $(1 \leq t \leq 10^4$) — the number of test cases.</p><p>Then the description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ and a symbol $c$ ($1 \leq n \leq 2 \cdot 10^5$, $c$ is one of allowed traffic light colors <span class="tex-font-style-tt">r</span>, <span class="tex-font-style-tt">y</span> or <span class="tex-font-style-tt">g</span>)— the length of the string $s$ and the current color of the traffic light. </p><p>The second line of each test case contains a string $s$ of the length $n$, consisting of the letters <span class="tex-font-style-tt">r</span>, <span class="tex-font-style-tt">y</span> and <span class="tex-font-style-tt">g</span>.</p><p>It is guaranteed that the symbol <span class="tex-font-style-tt">g</span> is in the string $s$ and the symbol $c$ is in the string $s$. </p><p>It is guaranteed, that the sum of $n$ over all test cases does not exceed $2\cdot10^5$.</p></div><div class="output-specification"><p>For each test case output the minimal number of second in which you are guaranteed to cross the road.</p></div>

## Input

<p>The first line contains a single integer $t$ $(1 \leq t \leq 10^4$) — the number of test cases.</p><p>Then the description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ and a symbol $c$ ($1 \leq n \leq 2 \cdot 10^5$, $c$ is one of allowed traffic light colors <span class="tex-font-style-tt">r</span>, <span class="tex-font-style-tt">y</span> or <span class="tex-font-style-tt">g</span>)— the length of the string $s$ and the current color of the traffic light. </p><p>The second line of each test case contains a string $s$ of the length $n$, consisting of the letters <span class="tex-font-style-tt">r</span>, <span class="tex-font-style-tt">y</span> and <span class="tex-font-style-tt">g</span>.</p><p>It is guaranteed that the symbol <span class="tex-font-style-tt">g</span> is in the string $s$ and the symbol $c$ is in the string $s$. </p><p>It is guaranteed, that the sum of $n$ over all test cases does not exceed $2\cdot10^5$.</p>

## Output

<p>For each test case output the minimal number of second in which you are guaranteed to cross the road.</p>





```input1|2,3,6,7,10,11
6
5 r
rggry
1 g
g
3 r
rrg
5 y
yrrgy
7 r
rgrgyrg
9 y
rrrgyyygy
```




```output1
3
0
2
4
1
4
```



## Note

<p>The first test case is explained in the statement.</p><p>In the second test case the green color is on so you can cross the road immediately. </p><p>In the third test case, if the red color was on at the second second, then we would wait for the green color for one second, and if the red light was on at the first second, then we would wait for the green light for two seconds.</p><p>In the fourth test case the longest we would wait for the green color is if we wait for it starting from the fifth second.</p>
