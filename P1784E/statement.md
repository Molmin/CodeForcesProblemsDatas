## Description

<div><p>Alice and Bob are playing an infinite game consisting of <span class="tex-font-style-it">sets</span>. Each set consists of <span class="tex-font-style-it">rounds</span>. In each round, one of the players wins. The first player to win two rounds in a set wins this set. Thus, a set always ends with the score of $2:0$ or $2:1$ in favor of one of the players.</p><p>Let's call a <span class="tex-font-style-it">game scenario</span> a finite string $s$ consisting of characters '<span class="tex-font-style-tt">a</span>' and '<span class="tex-font-style-tt">b</span>'. Consider an infinite string formed with repetitions of string $s$: $sss \ldots$ Suppose that Alice and Bob play rounds according to this infinite string, left to right. If a character of the string $sss \ldots$ is '<span class="tex-font-style-tt">a</span>', then Alice wins the round; if it's '<span class="tex-font-style-tt">b</span>', Bob wins the round. As soon as one of the players wins two rounds, the set ends in their favor, and a new set starts from the next round.</p><p>Let's define $a_i$ as the number of sets won by Alice among the first $i$ sets while playing according to the given scenario. Let's also define $r$ as the limit of ratio $\frac{a_i}{i}$ as $i \rightarrow \infty$. If $r &gt; \frac{1}{2}$, we'll say that scenario $s$ is <span class="tex-font-style-it">winning for Alice</span>. If $r = \frac{1}{2}$, we'll say that scenario $s$ is <span class="tex-font-style-it">tied</span>. If $r &lt; \frac{1}{2}$, we'll say that scenario $s$ is <span class="tex-font-style-it">winning for Bob</span>.</p><p>You are given a string $s$ consisting of characters '<span class="tex-font-style-tt">a</span>', '<span class="tex-font-style-tt">b</span>', and '<span class="tex-font-style-tt">?</span>'. Consider all possible ways of replacing every '<span class="tex-font-style-tt">?</span>' with '<span class="tex-font-style-tt">a</span>' or '<span class="tex-font-style-tt">b</span>' to obtain a string consisting only of characters '<span class="tex-font-style-tt">a</span>' and '<span class="tex-font-style-tt">b</span>'. Count how many of them result in a scenario winning for Alice, how many result in a tied scenario, and how many result in a scenario winning for Bob. Print these three numbers modulo $998\,244\,353$.</p></div><div class="input-specification"><p>The only line contains a single string $s$&nbsp;($1 \le |s| \le 200$), consisting of characters '<span class="tex-font-style-tt">a</span>', '<span class="tex-font-style-tt">b</span>', and '<span class="tex-font-style-tt">?</span>'.</p></div><div class="output-specification"><p>Print three integers: how many ways result in a scenario winning for Alice, how many result in a tied scenario, and how many result in a scenario winning for Bob, modulo $998\,244\,353$.</p></div>

## Input

<p>The only line contains a single string $s$&nbsp;($1 \le |s| \le 200$), consisting of characters '<span class="tex-font-style-tt">a</span>', '<span class="tex-font-style-tt">b</span>', and '<span class="tex-font-style-tt">?</span>'.</p>

## Output

<p>Print three integers: how many ways result in a scenario winning for Alice, how many result in a tied scenario, and how many result in a scenario winning for Bob, modulo $998\,244\,353$.</p>





```input1
??
```




```input2
?aa?b
```




```input3
a???ba
```




```input4
????????
```




```input5
ba????a?a???abbb?
```




```input6
a????a??????b??abbababbbb?a?aaa????bb
```




```input7
??????????????a????????????????b?????
```




```output1
1
2
1
```




```output2
1
3
0
```




```output3
4
3
1
```




```output4
121
14
121
```




```output5
216
57
239
```




```output6
97833
28387
135924
```




```output7
484121060
448940322
484613337
```



## Note

<p>In the first example, there are four ways to replace the question marks: </p><ul> <li> $s = \mathtt{aa}$: Alice wins every set $2:0$&nbsp;— the scenario is winning for Alice; </li><li> $s = \mathtt{ab}$: Alice and Bob win sets in turns, with the score of $2:1$ each&nbsp;— the scenario is tied; </li><li> $s = \mathtt{ba}$: Bob and Alice win sets in turns, with the score of $2:1$ each&nbsp;— the scenario is tied; </li><li> $s = \mathtt{bb}$: Bob wins every set $2:0$&nbsp;— the scenario is winning for Bob. </li></ul>
