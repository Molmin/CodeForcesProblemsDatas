## Description

<div><p><span class="tex-font-style-it">This is an interactive problem.</span></p><p>A legendary tree rests deep in the forest. Legend has it that individuals who realize this tree would eternally become a Legendary Grandmaster.</p><p>To help you determine the tree, Mikaela the Goddess has revealed to you that the tree contains $n$ vertices, enumerated from $1$ through $n$. She also allows you to ask her some questions as follows. For each question, you should tell Mikaela some two <span class="tex-font-style-bf">disjoint</span> non-empty sets of vertices $S$ and $T$, along with any vertex $v$ that you like. Then, Mikaela will count and give you the number of pairs of vertices $(s, t)$ where $s \in S$ and $t \in T$ such that the simple path from $s$ to $t$ contains $v$.</p><p>Mikaela the Goddess is busy and will be available to answer at most $11\,111$ questions.</p><p>This is your only chance. Your task is to determine the tree and report its edges.</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($2 \leq n \leq 500$) — the number of vertices in the tree.</p></div><div class="output-specification"><p>When program has realized the tree and is ready to report the edges, print "<span class="tex-font-style-tt">ANSWER</span>" in a separate line. Make sure that all letters are capitalized.</p><p>Then, print $n-1$ lines, each containing two space-separated integers, denoting the vertices that are the endpoints of a certain edge. Each edge should be reported exactly once. Your program should then immediately terminate.</p></div><div><h2>Interaction</h2><p>For each question that you wish to ask, interact as follows.</p><ol> <li> First, print the size of $S$ in its own line. In the following line, print $|S|$ space-separated distinct integers, denoting the vertices in $S$. </li><li> Similarly, print the size of $T$ in its own line. In the following line, print $|T|$ space-separated distinct integers, denoting the vertices in $T$. </li><li> Then, in the final line, print $v$ — the vertex that you choose for this question. </li><li> Read Mikaela's answer from input. </li></ol><p>Be reminded that $S$ and $T$ must be disjoint and non-empty.</p><p>After printing a query do not forget to output end of line and flush the output. Otherwise you will get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use:</p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> see documentation for other languages. </li></ul><p>If your program asks too many questions, asks an invalid question or does not correctly follow the interaction guideline above, it may receive an arbitrary verdict. Otherwise, your program will receive the <span class="tex-font-style-tt">Wrong Answer</span> verdict if it reports an incorrect tree.</p><p>Note that the tree is fixed beforehand and does not depend on your queries.</p><p><span class="tex-font-style-bf">Hacks</span></p><p>Hacks should be formatted as follows.</p><p>The first line should contain a single integer $n$ ($2 \leq n \leq 500$)&nbsp;— the number of vertices in the tree.</p><p>The following $n-1$ lines should each contain two space-separated integers $u$ and $v$, denoting the existence of an undirected edge $(u, v)$ ($1 \leq u, v \leq n$).</p></div>

## Input

<p>The first line contains an integer $n$ ($2 \leq n \leq 500$) — the number of vertices in the tree.</p>

## Output

<p>When program has realized the tree and is ready to report the edges, print "<span class="tex-font-style-tt">ANSWER</span>" in a separate line. Make sure that all letters are capitalized.</p><p>Then, print $n-1$ lines, each containing two space-separated integers, denoting the vertices that are the endpoints of a certain edge. Each edge should be reported exactly once. Your program should then immediately terminate.</p>





```input1
5
5

```




```output1
3
1 2 3
2
4 5
2
ANSWER
1 2
2 3
3 4
2 5

```



## Note

<p>In the sample, the tree is as follows.</p><center> <img class="tex-graphics" src="file://Ule24QIz.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>$n = 5$ is given to the program. The program then asks Mikaela a question where $S = \{1, 2, 3\}$, $T = \{4, 5\}$, and $v = 2$, to which she replies with $5$ (the pairs $(s, t)$ are $(1, 4)$, $(1, 5)$, $(2, 4)$, $(2, 5)$, and $(3, 5)$).</p>
