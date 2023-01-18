## Description

<div><p>Bob is a competitive programmer. He wants to become red, and for that he needs a strict training regime. He went to the annual meeting of grandmasters and asked $n$ of them how much effort they needed to reach red.</p><p>"Oh, I just spent $x_i$ <span class="tex-font-style-bf">hours</span> solving problems", said the $i$-th of them. </p><p>Bob wants to train his math skills, so for each answer he wrote down the number of <span class="tex-font-style-bf">minutes</span> ($60 \cdot x_i$), thanked the grandmasters and went home. Bob could write numbers with leading zeroes — for example, if some grandmaster answered that he had spent $2$ hours, Bob could write $000120$ instead of $120$.</p><p>Alice wanted to tease Bob and so she took the numbers Bob wrote down, and for each of them she did one of the following independently: </p><ul> <li> rearranged its digits, or </li><li> wrote a random number. </li></ul><p>This way, Alice generated $n$ numbers, denoted $y_1$, ..., $y_n$.</p><p>For each of the numbers, help Bob determine whether $y_i$ can be a permutation of a number divisible by $60$ (possibly with leading zeroes).</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \leq n \leq 418$)&nbsp;— the number of grandmasters Bob asked.</p><p>Then $n$ lines follow, the $i$-th of which contains a single integer $y_i$&nbsp;— the number that Alice wrote down.</p><p>Each of these numbers has between $2$ and $100$ digits '0' through '9'. They can contain leading zeroes.</p></div><div class="output-specification"><p>Output $n$ lines.</p><p>For each $i$, output the following. If it is possible to rearrange the digits of $y_i$ such that the resulting number is divisible by $60$, output "<span class="tex-font-style-tt">red</span>" (quotes for clarity). Otherwise, output "<span class="tex-font-style-tt">cyan</span>".</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \leq n \leq 418$)&nbsp;— the number of grandmasters Bob asked.</p><p>Then $n$ lines follow, the $i$-th of which contains a single integer $y_i$&nbsp;— the number that Alice wrote down.</p><p>Each of these numbers has between $2$ and $100$ digits '0' through '9'. They can contain leading zeroes.</p>

## Output

<p>Output $n$ lines.</p><p>For each $i$, output the following. If it is possible to rearrange the digits of $y_i$ such that the resulting number is divisible by $60$, output "<span class="tex-font-style-tt">red</span>" (quotes for clarity). Otherwise, output "<span class="tex-font-style-tt">cyan</span>".</p>





```input1
6
603
006
205
228
1053
0000000000000000000000000000000000000000000000
```




```output1
red
red
cyan
cyan
cyan
red
```



## Note

<p>In the first example, there is one rearrangement that yields a number divisible by $60$, and that is $360$.</p><p>In the second example, there are two solutions. One is $060$ and the second is $600$.</p><p>In the third example, there are $6$ possible rearrangments: $025$, $052$, $205$, $250$, $502$, $520$. None of these numbers is divisible by $60$.</p><p>In the fourth example, there are $3$ rearrangements: $228$, $282$, $822$.</p><p>In the fifth example, none of the $24$ rearrangements result in a number divisible by $60$.</p><p>In the sixth example, note that $000\dots0$ is a valid solution.</p>
