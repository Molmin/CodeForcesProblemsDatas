## Description

<div><p>You are given three integers $a$, $b$ and $x$. Your task is to construct a binary string $s$ of length $n = a + b$ such that there are exactly $a$ zeroes, exactly $b$ ones and exactly $x$ indices $i$ (where $1 \le i &lt; n$) such that $s_i \ne s_{i + 1}$. It is guaranteed that the answer always exists.</p><p>For example, for the string "<span class="tex-font-style-tt">01010</span>" there are four indices $i$ such that $1 \le i &lt; n$ and $s_i \ne s_{i + 1}$ ($i = 1, 2, 3, 4$). For the string "<span class="tex-font-style-tt">111001</span>" there are two such indices $i$ ($i = 3, 5$).</p><p>Recall that binary string is a non-empty sequence of characters where each character is either <span class="tex-font-style-tt">0</span> or <span class="tex-font-style-tt">1</span>.</p></div><div class="input-specification"><p>The first line of the input contains three integers $a$, $b$ and $x$ ($1 \le a, b \le 100, 1 \le x &lt; a + b)$.</p></div><div class="output-specification"><p>Print only one string $s$, where $s$ is <span class="tex-font-style-bf">any</span> binary string satisfying conditions described above. It is guaranteed that the answer always exists.</p></div>

## Input

<p>The first line of the input contains three integers $a$, $b$ and $x$ ($1 \le a, b \le 100, 1 \le x &lt; a + b)$.</p>

## Output

<p>Print only one string $s$, where $s$ is <span class="tex-font-style-bf">any</span> binary string satisfying conditions described above. It is guaranteed that the answer always exists.</p>





```input1
2 2 1

```




```input2
3 3 3

```




```input3
5 3 6

```




```output1
1100

```




```output2
101100

```




```output3
01010100

```



## Note

<p>All possible answers for the first example: </p><ul> <li> <span class="tex-font-style-tt">1100</span>; </li><li> <span class="tex-font-style-tt">0011</span>. </li></ul><p>All possible answers for the second example: </p><ul> <li> <span class="tex-font-style-tt">110100</span>; </li><li> <span class="tex-font-style-tt">101100</span>; </li><li> <span class="tex-font-style-tt">110010</span>; </li><li> <span class="tex-font-style-tt">100110</span>; </li><li> <span class="tex-font-style-tt">011001</span>; </li><li> <span class="tex-font-style-tt">001101</span>; </li><li> <span class="tex-font-style-tt">010011</span>; </li><li> <span class="tex-font-style-tt">001011</span>. </li></ul>
