## Description

<div><p>The DNA sequence for every living creature in Berland can be represented as a non-empty line consisting of lowercase Latin letters. Berland scientists found out that all the creatures evolve by stages. During one stage exactly one symbol of the DNA line is replaced by exactly two other ones. At that overall there are <span class="tex-span"><i>n</i></span> permissible substitutions. The substitution <span class="tex-font-style-tt"><span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>-&gt;<span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub><i>c</i><sub class="lower-index"><i>i</i></sub></span></span> means that any <span class="tex-font-style-bf">one</span> symbol <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> can be replaced with two symbols <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub><i>c</i><sub class="lower-index"><i>i</i></sub></span>. Every substitution could happen an unlimited number of times.</p><p>They say that two creatures with DNA sequences <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> can have a common ancestor if there exists such a DNA sequence <span class="tex-span"><i>s</i><sub class="lower-index">3</sub></span> that throughout evolution it can result in <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span>, perhaps after a different number of stages. Your task is to find out by the given <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> whether the creatures possessing such DNA sequences can have a common ancestor. If the answer is positive, you have to find the length of the shortest sequence of the common ancestor’s DNA.</p></div><div class="input-specification"><p>The first line contains a non-empty DNA sequence <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span>, the second line contains a non-empty DNA sequence <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span>. The lengths of these lines do not exceed 50, the lines contain only lowercase Latin letters. The third line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 50</span>) — the number of permissible substitutions. Then follow <span class="tex-span"><i>n</i></span> lines each of which describes a substitution in the format <span class="tex-font-style-tt"><span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>-&gt;<span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub><i>c</i><sub class="lower-index"><i>i</i></sub></span></span>. The characters <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> are lowercase Latin letters. Lines <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> can coincide, the list of substitutions can contain similar substitutions.</p></div><div class="output-specification"><p>If <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> cannot have a common ancestor, print -1. Otherwise print the length of the shortest sequence <span class="tex-span"><i>s</i><sub class="lower-index">3</sub></span>, from which <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> could have evolved.</p></div>

## Input

<p>The first line contains a non-empty DNA sequence <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span>, the second line contains a non-empty DNA sequence <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span>. The lengths of these lines do not exceed 50, the lines contain only lowercase Latin letters. The third line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 50</span>) — the number of permissible substitutions. Then follow <span class="tex-span"><i>n</i></span> lines each of which describes a substitution in the format <span class="tex-font-style-tt"><span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>-&gt;<span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub><i>c</i><sub class="lower-index"><i>i</i></sub></span></span>. The characters <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> are lowercase Latin letters. Lines <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> can coincide, the list of substitutions can contain similar substitutions.</p>

## Output

<p>If <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> cannot have a common ancestor, print -1. Otherwise print the length of the shortest sequence <span class="tex-span"><i>s</i><sub class="lower-index">3</sub></span>, from which <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> could have evolved.</p>





```input1
ababa
aba
2
c-&gt;ba
c-&gt;cc

```




```input2
ababa
aba
7
c-&gt;ba
c-&gt;cc
e-&gt;ab
z-&gt;ea
b-&gt;ba
d-&gt;dd
d-&gt;ab

```




```input3
ababa
aba
1
c-&gt;ba

```




```output1
2

```




```output2
1

```




```output3
-1

```


