## Description

<div><p>Polycarp is an experienced participant in Codehorses programming contests. Now he wants to become a problemsetter.</p><p>He sent to the coordinator a set of <span class="tex-span"><i>n</i></span> problems. Each problem has it's quality, the quality of the <span class="tex-span"><i>i</i></span>-th problem is <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> can be positive, negative or equal to zero). The problems are ordered by expected difficulty, but the difficulty is not related to the quality in any way. The easiest problem has index <span class="tex-span">1</span>, the hardest problem has index <span class="tex-span"><i>n</i></span>.</p><p>The coordinator's mood is equal to <span class="tex-span"><i>q</i></span> now. After reading a problem, the mood changes by it's quality. It means that after the coordinator reads a problem with quality <span class="tex-span"><i>b</i></span>, the value <span class="tex-span"><i>b</i></span> is added to his mood. The coordinator always reads problems one by one from the easiest to the hardest, it's impossible to change the order of the problems.</p><p>If after reading some problem the coordinator's mood becomes negative, he immediately stops reading and rejects the problemset.</p><p>Polycarp wants to remove the minimum number of problems from his problemset to make the coordinator's mood non-negative at any moment of time. Polycarp is not sure about the current coordinator's mood, but he has <span class="tex-span"><i>m</i></span> guesses "the current coordinator's mood <span class="tex-span"><i>q</i> = <i>b</i><sub class="lower-index"><i>i</i></sub></span>".</p><p>For each of <span class="tex-span"><i>m</i></span> guesses, find the minimum number of problems Polycarp needs to remove so that the coordinator's mood will always be greater or equal to <span class="tex-span">0</span> while he reads problems from the easiest of the remaining problems to the hardest.</p></div><div class="input-specification"><p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 750</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 200 000</span>)&nbsp;— the number of problems in the problemset and the number of guesses about the current coordinator's mood.</p><p>The second line of input contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the qualities of the problems in order of increasing difficulty.</p><p>The third line of input contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">0 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">15</sup></span>)&nbsp;— the guesses of the current coordinator's mood <span class="tex-span"><i>q</i></span>.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> lines, in <span class="tex-span"><i>i</i></span>-th line print single integer&nbsp;— the answer to the problem with <span class="tex-span"><i>q</i> = <i>b</i><sub class="lower-index"><i>i</i></sub></span>.</p></div>

## Input

<p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 750</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 200 000</span>)&nbsp;— the number of problems in the problemset and the number of guesses about the current coordinator's mood.</p><p>The second line of input contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the qualities of the problems in order of increasing difficulty.</p><p>The third line of input contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">0 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">15</sup></span>)&nbsp;— the guesses of the current coordinator's mood <span class="tex-span"><i>q</i></span>.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> lines, in <span class="tex-span"><i>i</i></span>-th line print single integer&nbsp;— the answer to the problem with <span class="tex-span"><i>q</i> = <i>b</i><sub class="lower-index"><i>i</i></sub></span>.</p>





```input1
6 3
8 -5 -4 1 -7 4
0 7 3

```




```output1
2
0
1

```


