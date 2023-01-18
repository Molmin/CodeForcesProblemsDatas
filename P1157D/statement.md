## Description

<div><p>Polycarp has to solve exactly $n$ problems to improve his programming skill before an important programming competition. But this competition will be held very soon, most precisely, it will start in $k$ days. It means that Polycarp has exactly $k$ days for training!</p><p>Polycarp doesn't want to procrastinate, so he wants to solve at least one problem during each of $k$ days. He also doesn't want to overwork, so if he solves $x$ problems during some day, he should solve no more than $2x$ problems during the next day. And, at last, he wants to improve his skill, so if he solves $x$ problems during some day, he should solve at least $x+1$ problem during the next day.</p><p>More formally: let $[a_1, a_2, \dots, a_k]$ be the array of numbers of problems solved by Polycarp. The $i$-th element of this array is the number of problems Polycarp solves during the $i$-th day of his training. Then the following conditions must be satisfied: </p><ul> <li> sum of all $a_i$ for $i$ from $1$ to $k$ should be $n$; </li><li> $a_i$ should be <span class="tex-font-style-bf">greater than zero</span> for each $i$ from $1$ to $k$; </li><li> the condition $a_i &lt; a_{i + 1} \le 2 a_i$ should be satisfied for each $i$ from $1$ to $k-1$. </li></ul><p>Your problem is to find <span class="tex-font-style-bf">any</span> array $a$ of length $k$ satisfying the conditions above or say that it is impossible to do it.</p></div><div class="input-specification"><p>The first line of the input contains two integers $n$ and $k$ ($1 \le n \le 10^9, 1 \le k \le 10^5$) — the number of problems Polycarp wants to solve and the number of days Polycarp wants to train.</p></div><div class="output-specification"><p>If it is impossible to find any array $a$ of length $k$ satisfying Polycarp's rules of training, print "<span class="tex-font-style-tt">NO</span>" in the first line.</p><p>Otherwise print "<span class="tex-font-style-tt">YES</span>" in the first line, then print $k$ integers $a_1, a_2, \dots, a_k$ in the second line, where $a_i$ should be the number of problems Polycarp should solve during the $i$-th day. If there are multiple answers, you can print any.</p></div>

## Input

<p>The first line of the input contains two integers $n$ and $k$ ($1 \le n \le 10^9, 1 \le k \le 10^5$) — the number of problems Polycarp wants to solve and the number of days Polycarp wants to train.</p>

## Output

<p>If it is impossible to find any array $a$ of length $k$ satisfying Polycarp's rules of training, print "<span class="tex-font-style-tt">NO</span>" in the first line.</p><p>Otherwise print "<span class="tex-font-style-tt">YES</span>" in the first line, then print $k$ integers $a_1, a_2, \dots, a_k$ in the second line, where $a_i$ should be the number of problems Polycarp should solve during the $i$-th day. If there are multiple answers, you can print any.</p>





```input1
26 6
```




```input2
8 3
```




```input3
1 1
```




```input4
9 4
```




```output1
YES
1 2 4 5 6 8
```




```output2
NO
```




```output3
YES
1
```




```output4
NO
```


