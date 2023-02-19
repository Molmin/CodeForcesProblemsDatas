## Description

<div><p>Polycarp remembered the $2020$-th year, and he is happy with the arrival of the new $2021$-th year. To remember such a wonderful moment, Polycarp wants to represent the number $n$ as the sum of a certain number of $2020$ and a certain number of $2021$.</p><p>For example, if: </p><ul> <li> $n=4041$, then the number $n$ can be represented as the sum $2020 + 2021$; </li><li> $n=4042$, then the number $n$ can be represented as the sum $2021 + 2021$; </li><li> $n=8081$, then the number $n$ can be represented as the sum $2020 + 2020 + 2020 + 2021$; </li><li> $n=8079$, then the number $n$ cannot be represented as the sum of the numbers $2020$ and $2021$. </li></ul><p>Help Polycarp to find out whether the number $n$ can be represented as the sum of a certain number of numbers $2020$ and a certain number of numbers $2021$.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases. Then $t$ test cases follow.</p><p>Each test case contains one integer $n$ ($1 \leq n \leq 10^6$)&nbsp;— the number that Polycarp wants to represent as the sum of the numbers $2020$ and $2021$.</p></div><div class="output-specification"><p>For each test case, output on a separate line: </p><ul> <li> "<span class="tex-font-style-tt">YES</span>" if the number $n$ is representable as the sum of a certain number of $2020$ and a certain number of $2021$; </li><li> "<span class="tex-font-style-tt">NO</span>" otherwise. </li></ul><p>You can output "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case (for example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> will be recognized as positive).</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases. Then $t$ test cases follow.</p><p>Each test case contains one integer $n$ ($1 \leq n \leq 10^6$)&nbsp;— the number that Polycarp wants to represent as the sum of the numbers $2020$ and $2021$.</p>

## Output

<p>For each test case, output on a separate line: </p><ul> <li> "<span class="tex-font-style-tt">YES</span>" if the number $n$ is representable as the sum of a certain number of $2020$ and a certain number of $2021$; </li><li> "<span class="tex-font-style-tt">NO</span>" otherwise. </li></ul><p>You can output "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case (for example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> will be recognized as positive).</p>





```input1
5
1
4041
4042
8081
8079
```




```output1
NO
YES
YES
YES
NO
```


