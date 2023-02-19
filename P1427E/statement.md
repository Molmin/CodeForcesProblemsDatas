## Description

<div><p>You have a blackboard and initially only an <span class="tex-font-style-bf">odd</span> number $x$ is written on it. Your goal is to write the number $1$ on the blackboard.</p><p>You may write new numbers on the blackboard with the following two operations. </p><ul> <li> You may take two numbers (not necessarily distinct) already on the blackboard and write their sum on the blackboard. The two numbers you have chosen remain on the blackboard. </li><li> You may take two numbers (not necessarily distinct) already on the blackboard and write their <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR</a> on the blackboard. The two numbers you have chosen remain on the blackboard. </li></ul> Perform a sequence of operations such that at the end the number $1$ is on the blackboard.</div><div class="input-specification"><p>The single line of the input contains the odd integer $x$ ($3 \le x \le 999,999$).</p></div><div class="output-specification"><p>Print on the first line the number $q$ of operations you perform. Then $q$ lines should follow, each describing one operation. </p><ul> <li> The "sum" operation is described by the line "$a$ + $b$", where $a, b$ must be integers already present on the blackboard. </li><li> The "xor" operation is described by the line "$a$ ^ $b$", where $a, b$ must be integers already present on the blackboard. </li></ul> <span class="tex-font-style-bf">The operation symbol (+ or ^) must be separated from $a, b$ by a whitespace.</span><p>You can perform at most $100,000$ operations (that is, $q\le 100,000$) and all numbers written on the blackboard must be in the range $[0, 5\cdot10^{18}]$. It can be proven that under such restrictions the required sequence of operations exists. You can output any suitable sequence of operations.</p></div>

## Input

<p>The single line of the input contains the odd integer $x$ ($3 \le x \le 999,999$).</p>

## Output

<p>Print on the first line the number $q$ of operations you perform. Then $q$ lines should follow, each describing one operation. </p><ul> <li> The "sum" operation is described by the line "$a$ + $b$", where $a, b$ must be integers already present on the blackboard. </li><li> The "xor" operation is described by the line "$a$ ^ $b$", where $a, b$ must be integers already present on the blackboard. </li></ul> <span class="tex-font-style-bf">The operation symbol (+ or ^) must be separated from $a, b$ by a whitespace.</span><p>You can perform at most $100,000$ operations (that is, $q\le 100,000$) and all numbers written on the blackboard must be in the range $[0, 5\cdot10^{18}]$. It can be proven that under such restrictions the required sequence of operations exists. You can output any suitable sequence of operations.</p>





```input1
3
```




```input2
123
```




```output1
5
3 + 3
3 ^ 6
3 + 5
3 + 6
8 ^ 9
```




```output2
10
123 + 123
123 ^ 246
141 + 123
246 + 123
264 ^ 369
121 + 246
367 ^ 369
30 + 30
60 + 60
120 ^ 121
```


