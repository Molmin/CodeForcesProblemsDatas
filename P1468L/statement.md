## Description

<div><p>Suppose you have a sequence of $k$ integers $A = [a_1, a_2, \dots , a_k]$ where each $a_i \geq 2$. A sequence of <span class="tex-font-style-bf">prime</span> integers $P = [p_1, p_2, \dots, p_k]$ is called <span class="tex-font-style-it">suitable</span> for the sequence $A$ if $a_1$ is divisible by $p_1$, $a_2$ is divisible by $p_2$ and so on. </p><p>A sequence of <span class="tex-font-style-bf">prime</span> integers $P$ is called <span class="tex-font-style-it">friendly</span> if there are no unique integers in this sequence. </p><p>A sequence $A$ is called <span class="tex-font-style-it">ideal</span>, if each sequence $P$ that is <span class="tex-font-style-it">suitable</span> for $A$ is <span class="tex-font-style-it">friendly</span> as well (i. e. there is no sequence $P$ that is <span class="tex-font-style-it">suitable</span> for $A$, but not <span class="tex-font-style-it">friendly</span>). For example, the sequence $[2, 4, 16]$ is <span class="tex-font-style-it">ideal</span>, while the sequence $[2, 4, 6]$ is not <span class="tex-font-style-it">ideal</span> (there exists a sequence $P = [2, 2, 3]$ which is <span class="tex-font-style-it">suitable</span> for $A$, but not <span class="tex-font-style-it">friendly</span>).</p><p>You are given $n$ different integers $x_1$, $x_2$, ..., $x_n$. You have to choose <span class="tex-font-style-bf">exactly</span> $k$ of them in such a way that they form an <span class="tex-font-style-it">ideal</span> sequence, or report that it is impossible. Note that no integer can be chosen more than once.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ ($1 \leq k \leq n \leq 1000$). </p><p>The second line contains $n$ pairwise distinct integers $x_1$, $x_2$, ..., $x_n$ ($2 \leq x_i \leq 10^{18}$).</p></div><div class="output-specification"><p>If it is impossible to choose exactly $k$ integers from $x_1$, $x_2$, ..., $x_n$ in such a way that the chosen integers form an <span class="tex-font-style-it">ideal</span> sequence, print $0$.</p><p>Otherwise, print $k$ pairwise distinct integers — the elements of the chosen <span class="tex-font-style-it">ideal</span> sequence. If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line contains two integers $n$ and $k$ ($1 \leq k \leq n \leq 1000$). </p><p>The second line contains $n$ pairwise distinct integers $x_1$, $x_2$, ..., $x_n$ ($2 \leq x_i \leq 10^{18}$).</p>

## Output

<p>If it is impossible to choose exactly $k$ integers from $x_1$, $x_2$, ..., $x_n$ in such a way that the chosen integers form an <span class="tex-font-style-it">ideal</span> sequence, print $0$.</p><p>Otherwise, print $k$ pairwise distinct integers — the elements of the chosen <span class="tex-font-style-it">ideal</span> sequence. If there are multiple answers, print any of them.</p>





```input1
3 3
2 4 6

```




```input2
3 3
2 4 16

```




```input3
4 3
2 4 6 16

```




```output1
0

```




```output2
2 4 16 

```




```output3
2 4 16 

```


