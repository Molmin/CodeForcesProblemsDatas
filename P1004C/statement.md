## Description

<div><p>Since Sonya is interested in robotics too, she decided to construct robots that will read and recognize numbers.</p><p>Sonya has drawn $n$ numbers in a row, $a_i$ is located in the $i$-th position. She also has put a robot at each end of the row (to the left of the first number and to the right of the last number). Sonya will give a number to each robot (they can be either same or different) and run them. When a robot is running, it is moving toward to another robot, reading numbers in the row. When a robot is reading a number that is equal to the number that was given to that robot, it will turn off and stay in the same position.</p><p>Sonya does not want robots to break, so she will give such numbers that robots will stop before they meet. That is, the girl wants them to stop at different positions so that the first robot is to the left of the second one.</p><p>For example, if the numbers $[1, 5, 4, 1, 3]$ are written, and Sonya gives the number $1$ to the first robot and the number $4$ to the second one, the first robot will stop in the $1$-st position while the second one in the $3$-rd position. In that case, robots will not meet each other. As a result, robots will not be broken. But if Sonya gives the number $4$ to the first robot and the number $5$ to the second one, they will meet since the first robot will stop in the $3$-rd position while the second one is in the $2$-nd position.</p><p>Sonya understands that it does not make sense to give a number that is not written in the row because a robot will not find this number and will meet the other robot.</p><p>Sonya is now interested in finding the number of different pairs that she can give to robots so that they will not meet. In other words, she wants to know the number of pairs ($p$, $q$), where she will give $p$ to the first robot and $q$ to the second one. Pairs ($p_i$, $q_i$) and ($p_j$, $q_j$) are different if $p_i\neq p_j$ or $q_i\neq q_j$.</p><p>Unfortunately, Sonya is busy fixing robots that broke after a failed launch. That is why she is asking you to find the number of pairs that she can give to robots so that they will not meet.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1\leq n\leq 10^5$)&nbsp;— the number of numbers in a row.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1\leq a_i\leq 10^5$)&nbsp;— the numbers in a row.</p></div><div class="output-specification"><p>Print one number&nbsp;— the number of possible pairs that Sonya can give to robots so that they will not meet.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1\leq n\leq 10^5$)&nbsp;— the number of numbers in a row.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1\leq a_i\leq 10^5$)&nbsp;— the numbers in a row.</p>

## Output

<p>Print one number&nbsp;— the number of possible pairs that Sonya can give to robots so that they will not meet.</p>





```input1
5
1 5 4 1 3

```




```input2
7
1 2 1 1 1 3 2

```




```output1
9

```




```output2
7

```



## Note

<p>In the first example, Sonya can give pairs ($1$, $1$), ($1$, $3$), ($1$, $4$), ($1$, $5$), ($4$, $1$), ($4$, $3$), ($5$, $1$), ($5$, $3$), and ($5$, $4$).</p><p>In the second example, Sonya can give pairs ($1$, $1$), ($1$, $2$), ($1$, $3$), ($2$, $1$), ($2$, $2$), ($2$, $3$), and ($3$, $2$).</p>
