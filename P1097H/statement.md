## Description

<div><p>A <span class="tex-font-style-it">Thue-Morse-Radecki-Mateusz sequence</span> (Thorse-Radewoosh sequence in short) is an infinite sequence constructed from a finite sequence $\mathrm{gen}$ of length $d$ and an integer $m$, obtained in the following sequence of steps:</p><ul> <li> In the beginning, we define the one-element sequence $M_0=(0)$.</li><li> In the $k$-th step, $k \geq 1$, we define the sequence $M_k$ to be the concatenation of the $d$ copies of $M_{k-1}$. However, each of them is altered slightly — in the $i$-th of them ($1 \leq i \leq d$), each element $x$ is changed to $(x+\mathrm{gen}_i) \pmod{m}$. </li></ul><p>For instance, if we pick $\mathrm{gen} = (0, \color{blue}{1}, \color{green}{2})$ and $m = 4$: </p><ul> <li> $M_0 = (0)$, </li><li> $M_1 = (0, \color{blue}{1}, \color{green}{2})$, </li><li> $M_2 = (0, 1, 2, \color{blue}{1, 2, 3}, \color{green}{2, 3, 0})$, </li><li> $M_3 = (0, 1, 2, 1, 2, 3, 2, 3, 0, \color{blue}{1, 2, 3, 2, 3, 0, 3, 0, 1}, \color{green}{2, 3, 0, 3, 0, 1, 0, 1, 2})$, and so on. </li></ul><p>As you can see, as long as the first element of $\mathrm{gen}$ is $0$, each consecutive step produces a sequence whose prefix is the sequence generated in the previous step. Therefore, we can define the infinite Thorse-Radewoosh sequence $M_\infty$ as the sequence obtained by applying the step above indefinitely. For the parameters above, $M_\infty = (0, 1, 2, 1, 2, 3, 2, 3, 0, 1, 2, 3, 2, 3, 0, 3, 0, 1, \dots)$.</p><p>Mateusz picked a sequence $\mathrm{gen}$ and an integer $m$, and used them to obtain a Thorse-Radewoosh sequence $M_\infty$. He then picked two integers $l$, $r$, and wrote down a subsequence of this sequence $A := ((M_\infty)_l, (M_\infty)_{l+1}, \dots, (M_\infty)_r)$.</p><p>Note that we use the $1$-based indexing both for $M_\infty$ and $A$.</p><p>Mateusz has his favorite sequence $B$ with length $n$, and would like to see how large it is compared to $A$. Let's say that $B$ majorizes sequence $X$ of length $n$ (let's denote it as $B \geq X$) if and only if for all $i \in \{1, 2, \dots, n\}$, we have $B_i \geq X_i$.</p><p>He now asks himself how many integers $x$ in the range $[1, |A| - n + 1]$ there are such that $B \geq (A_x, A_{x+1}, A_{x+2}, \dots, A_{x+n-1})$. As both sequences were huge, answering the question using only his pen and paper turned out to be too time-consuming. Can you help him automate his research?</p></div><div class="input-specification"><p>The first line contains two integers $d$ and $m$ ($2 \leq d \leq 20$, $2 \leq m \leq 60$) — the length of the sequence $\mathrm{gen}$ and an integer used to perform the modular operations. The second line contains $d$ integers $\mathrm{gen}_i$ ($0 \leq \mathrm{gen}_i &lt; m$). It's guaranteed that the first element of the sequence $\mathrm{gen}$ is equal to zero.</p><p>The third line contains one integer $n$ ($1 \leq n \leq 30000$) — the length of the sequence $B$. The fourth line contains $n$ integers $B_i$ ($0 \leq B_i &lt; m$). The fifth line contains two integers $l$ and $r$ ($1 \leq l \leq r \leq 10^{18}$, $r-l+1 \geq n$).</p></div><div class="output-specification"><p>Print a single integer — the answer to the problem.</p></div>

## Input

<p>The first line contains two integers $d$ and $m$ ($2 \leq d \leq 20$, $2 \leq m \leq 60$) — the length of the sequence $\mathrm{gen}$ and an integer used to perform the modular operations. The second line contains $d$ integers $\mathrm{gen}_i$ ($0 \leq \mathrm{gen}_i &lt; m$). It's guaranteed that the first element of the sequence $\mathrm{gen}$ is equal to zero.</p><p>The third line contains one integer $n$ ($1 \leq n \leq 30000$) — the length of the sequence $B$. The fourth line contains $n$ integers $B_i$ ($0 \leq B_i &lt; m$). The fifth line contains two integers $l$ and $r$ ($1 \leq l \leq r \leq 10^{18}$, $r-l+1 \geq n$).</p>

## Output

<p>Print a single integer — the answer to the problem.</p>





```input1
2 2
0 1
4
0 1 1 0
2 21
```




```input2
3 4
0 1 2
2
0 2
6 11
```




```output1
6
```




```output2
1
```



## Note

<p>Thorse-Radewoosh sequence in the first example is the standard Thue-Morse sequence, so the sequence $A$ is as follows: $11010011001011010010$. Here are the places where the sequence $B$ majorizes $A$:</p><center> <img class="tex-graphics" src="file://vpxM8dxq.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
