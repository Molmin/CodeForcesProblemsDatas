## Description

<div><p>A string is called <span class="tex-font-style-it">bracket sequence</span> if it does not contain any characters other than "<span class="tex-font-style-tt">(</span>" and "<span class="tex-font-style-tt">)</span>". A bracket sequence is called <span class="tex-font-style-it">regular</span> (shortly, RBS) if it is possible to obtain correct arithmetic expression by inserting characters "<span class="tex-font-style-tt">+</span>" and "<span class="tex-font-style-tt">1</span>" into this sequence. For example, "<span class="tex-font-style-tt"></span>", "<span class="tex-font-style-tt">(())</span>" and "<span class="tex-font-style-tt">()()</span>" are RBS and "<span class="tex-font-style-tt">)(</span>" and "<span class="tex-font-style-tt">(()</span>" are not.</p><p>We can see that each opening bracket in RBS is paired with some closing bracket, and, using this fact, we can define <span class="tex-font-style-bf">nesting depth</span> of the RBS as maximum number of bracket pairs, such that the $2$-nd pair lies inside the $1$-st one, the $3$-rd one — inside the $2$-nd one and so on. For example, nesting depth of "<span class="tex-font-style-tt"></span>" is $0$, "<span class="tex-font-style-tt">()()()</span>" is $1$ and "<span class="tex-font-style-tt">()((())())</span>" is $3$.</p><p>Now, you are given RBS $s$ of even length $n$. You should color each bracket of $s$ into one of two colors: red or blue. Bracket sequence $r$, consisting only of red brackets, should be RBS, and bracket sequence, consisting only of blue brackets $b$, should be RBS. Any of them can be empty. You are not allowed to reorder characters in $s$, $r$ or $b$. No brackets can be left uncolored.</p><p>Among all possible variants you should choose one that <span class="tex-font-style-bf">minimizes maximum</span> of $r$'s and $b$'s nesting depth. If there are multiple solutions you can print any of them.</p></div><div class="input-specification"><p>The first line contains an even integer $n$ ($2 \le n \le 2 \cdot 10^5$) — the length of RBS $s$.</p><p>The second line contains regular bracket sequence $s$ ($|s| = n$, $s_i \in \{$"<span class="tex-font-style-tt">(</span>", "<span class="tex-font-style-tt">)</span>"$\}$).</p></div><div class="output-specification"><p>Print single string $t$ of length $n$ consisting of "<span class="tex-font-style-tt">0</span>"-s and "<span class="tex-font-style-tt">1</span>"-s. If $t_i$ is equal to <span class="tex-font-style-tt">0</span> then character $s_i$ belongs to RBS $r$, otherwise $s_i$ belongs to $b$.</p></div>

## Input

<p>The first line contains an even integer $n$ ($2 \le n \le 2 \cdot 10^5$) — the length of RBS $s$.</p><p>The second line contains regular bracket sequence $s$ ($|s| = n$, $s_i \in \{$"<span class="tex-font-style-tt">(</span>", "<span class="tex-font-style-tt">)</span>"$\}$).</p>

## Output

<p>Print single string $t$ of length $n$ consisting of "<span class="tex-font-style-tt">0</span>"-s and "<span class="tex-font-style-tt">1</span>"-s. If $t_i$ is equal to <span class="tex-font-style-tt">0</span> then character $s_i$ belongs to RBS $r$, otherwise $s_i$ belongs to $b$.</p>





```input1
2
()
```




```input2
4
(())
```




```input3
10
((()())())
```




```output1
11
```




```output2
0101
```




```output3
0110001111
```



## Note

<p>In the first example one of optimal solutions is $s = $ "$\color{blue}{()}$". $r$ is empty and $b = $ "$()$". The answer is $\max(0, 1) = 1$.</p><p>In the second example it's optimal to make $s = $ "$\color{red}{(}\color{blue}{(}\color{red}{)}\color{blue}{)}$". $r = b = $ "$()$" and the answer is $1$.</p><p>In the third example we can make $s = $ "$\color{red}{(}\color{blue}{((}\color{red}{)()}\color{blue}{)())}$". $r = $ "$()()$" and $b = $ "$(()())$" and the answer is $2$.</p>
