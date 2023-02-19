## Description

<div><p><span class="tex-font-style-bf">This is an interactive problem.</span></p><p>There are $n$ words in a text editor. The $i$-th word has length $l_i$ ($1 \leq l_i \leq 2000$). The array $l$ is hidden and only known by the grader. </p><p>The text editor displays words in lines, splitting each two words in a line with at least one space. Note that a line does not have to end with a space. Let the height of the text editor refer to the number of lines used. For the given <span class="tex-font-style-bf">width</span>, the text editor will display words in such a way that the height is minimized.</p><p>More formally, suppose that the text editor has <span class="tex-font-style-bf">width</span> $w$. Let $a$ be an array of length $k+1$ where $1=a_1 &lt; a_2 &lt; \ldots &lt; a_{k+1}=n+1$. $a$ is a <span class="tex-font-style-bf">valid</span> array if for all $1 \leq i \leq k$, $l_{a_i}+1+l_{a_i+1}+1+\ldots+1+l_{a_{i+1}-1} \leq w$. Then the <span class="tex-font-style-bf">height</span> of the text editor is the minimum $k$ over all valid arrays.</p><p>Note that if $w &lt; \max(l_i)$, the text editor cannot display all the words properly and will crash, and the height of the text editor will be $0$ instead.</p><p>You can ask $n+30$ queries. In one query, you provide a width $w$. Then, the grader will return the height $h_w$ of the text editor when its width is $w$.</p><p>Find the minimum area of the text editor, which is the minimum value of $w \cdot h_w$ over all $w$ for which $h_w \neq 0$.</p><p>The lengths are fixed in advance. In other words, <span class="tex-font-style-bf">the interactor is not adaptive</span>.</p></div><div class="input-specification"><p>The first and only line of input contains a single integer $n$ ($1 \leq n \leq 2000$) &nbsp;— the number of words on the text editor.</p><p>It is guaranteed that the hidden lengths $l_i$ satisfy $1 \leq l_i \leq 2000$.</p></div><div><h2>Interaction</h2><p>Begin the interaction by reading $n$.</p><p>To make a query, print "<span class="tex-font-style-tt">?</span> $w$" (without quotes, $1 \leq w \leq 10^9$). Then you should read our response from standard input, that is, $h_w$.</p><p>If your program has made an invalid query or has run out of tries, the interactor will terminate immediately and your program will get a verdict <span class="tex-font-style-tt">Wrong answer</span>. </p><p>To give the final answer, print "<span class="tex-font-style-tt">!</span> $area$" (without the quotes). Note that giving this answer is not counted towards the limit of $n+30$ queries.</p><p>After printing a query do not forget to output end of line and flush the output. Otherwise, you will get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use:</p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> see documentation for other languages. </li></ul> <p><span class="tex-font-style-bf">Hacks</span></p><p>The first line of input must contain a single integer $n$ ($1 \leq n \leq 2000$) — the number of words in the text editor.</p><p>The second line of input must contain exactly $n$ space-separated integers $l_1,l_2,\ldots,l_n$ ($1 \leq l_i \leq 2000$).</p></div>

## Input

<p>The first and only line of input contains a single integer $n$ ($1 \leq n \leq 2000$) &nbsp;— the number of words on the text editor.</p><p>It is guaranteed that the hidden lengths $l_i$ satisfy $1 \leq l_i \leq 2000$.</p>





```input1
6

0

4

2
```




```output1
? 1

? 9

? 16

! 32
```



## Note

<p>In the first test case, the words are $\{\texttt{glory},\texttt{to},\texttt{ukraine},\texttt{and},\texttt{anton},\texttt{trygub}\}$, so $l=\{5,2,7,3,5,6\}$. </p><p>If $w=1$, then the text editor is not able to display all words properly and will crash. The height of the text editor is $h_1=0$, so the grader will return $0$.</p><p>If $w=9$, then a possible way that the words will be displayed on the text editor is: </p><ul> <li> $\texttt{glory__to}$ </li><li> $\texttt{ukraine__}$ </li><li> $\texttt{and_anton}$ </li><li> $\texttt{__trygub_}$ </li></ul><p>The height of the text editor is $h_{9}=4$, so the grader will return $4$.</p><p>If $w=16$, then a possible way that the words will be displayed on the text editor is: </p><ul> <li> $\texttt{glory_to_ukraine}$ </li><li> $\texttt{and_anton_trygub}$ </li></ul><p>The height of the text editor is $h_{16}=2$, so the grader will return $2$.</p><p>We have somehow figured out that the minimum area of the text editor is $32$, so we answer it.</p>
