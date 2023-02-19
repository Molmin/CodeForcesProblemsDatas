## Description

<div><div class="epigraph"><div class="epigraph-text">Even if it's a really easy question, she won't be able to answer it</div><div class="epigraph-source">— <span class="tex-font-style-it">Perfect Memento in Strict Sense</span></div></div><p>Cirno's perfect bitmasks classroom has just started!</p><p>Cirno gave her students a positive integer $x$. As an assignment, her students need to find the <span class="tex-font-style-bf">minimum positive</span> integer $y$, which satisfies the following two conditions:</p><p>$$x\ \texttt{and}\ y &gt; 0$$ $$x\ \texttt{xor}\ y &gt; 0$$</p><p>Where $\texttt{and}$ is the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#AND">bitwise AND operation</a>, and $\texttt{xor}$ is the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR operation</a>.</p><p>Among the students was Mystia, who was truly baffled by all these new operators. Please help her!</p></div><div class="input-specification"><p>The first line of input contains a single integer $t$ ($1 \leq t \leq 10^3$) — the number of input test cases.</p><p>For each test case, the only line of input contains one integer $x$ ($1 \leq x \leq 2^{30}$).</p></div><div class="output-specification"><p>For each test case, print a single integer — the minimum number of $y$.</p></div>

## Input

<p>The first line of input contains a single integer $t$ ($1 \leq t \leq 10^3$) — the number of input test cases.</p><p>For each test case, the only line of input contains one integer $x$ ($1 \leq x \leq 2^{30}$).</p>

## Output

<p>For each test case, print a single integer — the minimum number of $y$.</p>





```input1
7
1
2
5
9
16
114514
1000000
```




```output1
3
3
1
1
17
2
64
```



## Note

<p>Test case 1: </p><p>$1\; \texttt{and}\; 3=1&gt;0$, $1\; \texttt{xor}\; 3=2&gt;0$.</p><p>Test case 2: </p><p>$2\; \texttt{and}\; 3=2&gt;0$, $2\; \texttt{xor}\; 3=1&gt;0$.</p>
