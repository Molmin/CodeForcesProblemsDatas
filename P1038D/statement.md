## Description

<div><p>There are $n$ slimes in a row. Each slime has an integer value (possibly negative or zero) associated with it.</p><p>Any slime can eat its adjacent slime (the closest slime to its left or to its right, assuming that this slime exists). </p><p>When a slime with a value $x$ eats a slime with a value $y$, the eaten slime disappears, and the value of the remaining slime changes to $x - y$.</p><p>The slimes will eat each other until there is only one slime left. </p><p>Find the maximum possible value of the last slime.</p></div><div class="input-specification"><p>The first line of the input contains an integer $n$ ($1 \le n \le 500\,000$) denoting the number of slimes.</p><p>The next line contains $n$ integers $a_i$ ($-10^9 \le a_i \le 10^9$), where $a_i$ is the value of $i$-th slime.</p></div><div class="output-specification"><p>Print an only integer&nbsp;— the maximum possible value of the last slime.</p></div>

## Input

<p>The first line of the input contains an integer $n$ ($1 \le n \le 500\,000$) denoting the number of slimes.</p><p>The next line contains $n$ integers $a_i$ ($-10^9 \le a_i \le 10^9$), where $a_i$ is the value of $i$-th slime.</p>

## Output

<p>Print an only integer&nbsp;— the maximum possible value of the last slime.</p>





```input1
4
2 1 2 1

```




```input2
5
0 -1 -1 -1 -1

```




```output1
4
```




```output2
4
```



## Note

<p>In the first example, a possible way of getting the last slime with value $4$ is:</p><ul> <li> Second slime eats the third slime, the row now contains slimes $2, -1, 1$</li><li> Second slime eats the third slime, the row now contains slimes $2, -2$</li><li> First slime eats the second slime, the row now contains $4$ </li></ul><p>In the second example, the first slime can keep eating slimes to its right to end up with a value of $4$.</p>
