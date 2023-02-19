## Description

<div><p>The grasshopper is located on the numeric axis at the point with coordinate $x_0$.</p><p>Having nothing else to do he starts jumping between integer points on the axis. Making a jump from a point with coordinate $x$ with a distance $d$ to the left moves the grasshopper to a point with a coordinate $x - d$, while jumping to the right moves him to a point with a coordinate $x + d$.</p><p>The grasshopper is very fond of positive integers, so for each integer $i$ starting with $1$ the following holds: exactly $i$ minutes after the start he makes a jump with a distance of exactly $i$. So, in the first minutes he jumps by $1$, then by $2$, and so on.</p><p>The direction of a jump is determined as follows: if the point where the grasshopper was before the jump has an <span class="tex-font-style-bf">even</span> coordinate, the grasshopper jumps to the <span class="tex-font-style-bf">left</span>, <span class="tex-font-style-bf">otherwise</span> he jumps to the <span class="tex-font-style-bf">right</span>.</p><p>For example, if after $18$ consecutive jumps he arrives at the point with a coordinate $7$, he will jump by a distance of $19$ to the right, since $7$ is an odd number, and will end up at a point $7 + 19 = 26$. Since $26$ is an even number, the next jump the grasshopper will make to the left by a distance of $20$, and it will move him to the point $26 - 20 = 6$.</p><p>Find exactly which point the grasshopper will be at after exactly $n$ jumps.</p></div><div class="input-specification"><p>The first line of input contains an integer $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases.</p><p>Each of the following $t$ lines contains two integers $x_0$ ($-10^{14} \leq x_0 \leq 10^{14}$) and $n$ ($0 \leq n \leq 10^{14}$)&nbsp;— the coordinate of the grasshopper's initial position and the number of jumps.</p></div><div class="output-specification"><p>Print exactly $t$ lines. On the $i$-th line print one integer&nbsp;— the answer to the $i$-th test case&nbsp;— the coordinate of the point the grasshopper will be at after making $n$ jumps from the point $x_0$.</p></div>

## Input

<p>The first line of input contains an integer $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases.</p><p>Each of the following $t$ lines contains two integers $x_0$ ($-10^{14} \leq x_0 \leq 10^{14}$) and $n$ ($0 \leq n \leq 10^{14}$)&nbsp;— the coordinate of the grasshopper's initial position and the number of jumps.</p>

## Output

<p>Print exactly $t$ lines. On the $i$-th line print one integer&nbsp;— the answer to the $i$-th test case&nbsp;— the coordinate of the point the grasshopper will be at after making $n$ jumps from the point $x_0$.</p>





```input1
9
0 1
0 2
10 10
10 99
177 13
10000000000 987654321
-433494437 87178291199
1 0
-1 1
```




```output1
-1
1
11
110
190
9012345679
-87611785637
1
0
```



## Note

<p>The first two test cases in the example correspond to the first two jumps from the point $x_0 = 0$. </p><p>Since $0$ is an even number, the first jump of length $1$ is made to the left, and the grasshopper ends up at the point $0 - 1 = -1$.</p><p>Then, since $-1$ is an odd number, a jump of length $2$ is made to the right, bringing the grasshopper to the point with coordinate $-1 + 2 = 1$.</p>
