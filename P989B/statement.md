## Description

<div><div class="epigraph"><div class="epigraph-text"><span class="tex-font-style-it"> Walking along a riverside, Mino silently takes a note of something.<p>"Time," Mino thinks aloud.</p><p>"What?"</p><p>"Time and tide wait for no man," explains Mino. "My name, taken from the river, always reminds me of this."</p><p>"And what are you recording?"</p><p>"You see it, tide. Everything has its own period, and I think I've figured out this one," says Mino with confidence.</p><p>Doubtfully, Kanno peeks at Mino's records. </p></span></div></div><p>The records are expressed as a string $s$ of characters '<span class="tex-font-style-tt">0</span>', '<span class="tex-font-style-tt">1</span>' and '<span class="tex-font-style-tt">.</span>', where '<span class="tex-font-style-tt">0</span>' denotes a low tide, '<span class="tex-font-style-tt">1</span>' denotes a high tide, and '<span class="tex-font-style-tt">.</span>' denotes an unknown one (either high or low).</p><p>You are to help Mino determine whether it's possible that after replacing each '<span class="tex-font-style-tt">.</span>' independently with '<span class="tex-font-style-tt">0</span>' or '<span class="tex-font-style-tt">1</span>', a given integer $p$ is <span class="tex-font-style-bf">not</span> a period of the resulting string. In case the answer is yes, please also show such a replacement to Mino.</p><p>In this problem, a positive integer $p$ is considered a period of string $s$, if for all $1 \leq i \leq \lvert s \rvert - p$, the $i$-th and $(i + p)$-th characters of $s$ are the same. Here $\lvert s \rvert$ is the length of $s$.</p></div><div class="input-specification"><p>The first line contains two space-separated integers $n$ and $p$ ($1 \leq p \leq n \leq 2000$)&nbsp;— the length of the given string and the supposed period, respectively.</p><p>The second line contains a string $s$ of $n$ characters&nbsp;— Mino's records. $s$ only contains characters '<span class="tex-font-style-tt">0</span>', '<span class="tex-font-style-tt">1</span>' and '<span class="tex-font-style-tt">.</span>', and contains at least one '<span class="tex-font-style-tt">.</span>' character.</p></div><div class="output-specification"><p>Output one line&nbsp;— if it's possible that $p$ is <span class="tex-font-style-bf">not</span> a period of the resulting string, output any one of such strings; otherwise output "<span class="tex-font-style-tt">No</span>" (without quotes, you can print letters in any case (upper or lower)).</p></div>

## Input

<p>The first line contains two space-separated integers $n$ and $p$ ($1 \leq p \leq n \leq 2000$)&nbsp;— the length of the given string and the supposed period, respectively.</p><p>The second line contains a string $s$ of $n$ characters&nbsp;— Mino's records. $s$ only contains characters '<span class="tex-font-style-tt">0</span>', '<span class="tex-font-style-tt">1</span>' and '<span class="tex-font-style-tt">.</span>', and contains at least one '<span class="tex-font-style-tt">.</span>' character.</p>

## Output

<p>Output one line&nbsp;— if it's possible that $p$ is <span class="tex-font-style-bf">not</span> a period of the resulting string, output any one of such strings; otherwise output "<span class="tex-font-style-tt">No</span>" (without quotes, you can print letters in any case (upper or lower)).</p>





```input1
10 7
1.0.1.0.1.

```




```input2
10 6
1.0.1.1000

```




```input3
10 9
1........1

```




```output1
1000100010

```




```output2
1001101000

```




```output3
No

```



## Note

<p>In the first example, $7$ is not a period of the resulting string because the $1$-st and $8$-th characters of it are different.</p><p>In the second example, $6$ is not a period of the resulting string because the $4$-th and $10$-th characters of it are different.</p><p>In the third example, $9$ is always a period because the only constraint that the first and last characters are the same is already satisfied.</p><p>Note that there are multiple acceptable answers for the first two examples, you can print any of them.</p>
