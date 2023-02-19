## Description

<div><p>Bash has set out on a journey to become the greatest Pokemon master. To get his first Pokemon, he went to Professor Zulu's Lab. Since Bash is Professor Zulu's favourite student, Zulu allows him to take as many Pokemon from his lab as he pleases.</p><p>But Zulu warns him that a group of <span class="tex-span"><i>k</i> &gt; 1</span> Pokemon with strengths <span class="tex-span">{<i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, <i>s</i><sub class="lower-index">3</sub>, ..., <i>s</i><sub class="lower-index"><i>k</i></sub>}</span> tend to fight among each other if <span class="tex-span"><i>gcd</i>(<i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, <i>s</i><sub class="lower-index">3</sub>, ..., <i>s</i><sub class="lower-index"><i>k</i></sub>) = 1</span> (see notes for <span class="tex-span"><i>gcd</i></span> definition).</p><p>Bash, being smart, does not want his Pokemon to fight among each other. However, he also wants to maximize the number of Pokemon he takes from the lab. Can you help Bash find out the maximum number of Pokemon he can take? </p><p><span class="tex-font-style-bf">Note</span>: A Pokemon cannot fight with itself.</p></div><div class="input-specification"><p>The input consists of two lines.</p><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), the number of Pokemon in the lab.</p><p>The next line contains <span class="tex-span"><i>n</i></span> space separated integers, where the <span class="tex-span"><i>i</i></span>-th of them denotes <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>), the strength of the <span class="tex-span"><i>i</i></span>-th Pokemon.</p></div><div class="output-specification"><p>Print single integer&nbsp;— the maximum number of Pokemons Bash can take.</p></div>

## Input

<p>The input consists of two lines.</p><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), the number of Pokemon in the lab.</p><p>The next line contains <span class="tex-span"><i>n</i></span> space separated integers, where the <span class="tex-span"><i>i</i></span>-th of them denotes <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>), the strength of the <span class="tex-span"><i>i</i></span>-th Pokemon.</p>

## Output

<p>Print single integer&nbsp;— the maximum number of Pokemons Bash can take.</p>





```input1
3
2 3 4

```




```input2
5
2 3 4 6 7

```




```output1
2

```




```output2
3

```



## Note

<p><span class="tex-span"><i>gcd</i></span> (greatest common divisor) of positive integers set <span class="tex-span">{<i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub>}</span> is the maximum positive integer that divides all the integers <span class="tex-span">{<i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub>}</span>.</p><p>In the first sample, we can take Pokemons with strengths <span class="tex-span">{2, 4}</span> since <span class="tex-span"><i>gcd</i>(2, 4) = 2</span>.</p><p>In the second sample, we can take Pokemons with strengths <span class="tex-span">{2, 4, 6}</span>, and there is no larger group with <span class="tex-span"><i>gcd</i> ≠ 1</span>.</p>
