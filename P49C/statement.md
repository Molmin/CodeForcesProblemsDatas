## Description

<div><p>Vasya bought the collected works of a well-known Berland poet Petya in <span class="tex-span"><i>n</i></span> volumes. The volumes are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. He thinks that it does not do to arrange the book simply according to their order. Vasya wants to minimize the number of the disposition’s <span class="tex-font-style-underline">divisors</span> — the positive integers <span class="tex-span"><i>i</i></span> such that for at least one <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>j</i> ≤ <i>n</i></span>) is true both: <span class="tex-span"><i>j</i></span> <span class="tex-span"><i>mod</i></span> <span class="tex-span"><i>i</i> = 0</span> and at the same time <span class="tex-span"><i>p</i>(<i>j</i>)</span> <span class="tex-span"><i>mod</i></span> <span class="tex-span"><i>i</i> = 0</span>, where <span class="tex-span"><i>p</i>(<i>j</i>)</span> is the number of the tome that stands on the <span class="tex-span"><i>j</i></span>-th place and <span class="tex-span"><i>mod</i></span> is the operation of taking the division remainder. Naturally, one volume can occupy exactly one place and in one place can stand exactly one volume.</p><p>Help Vasya — find the volume disposition with the minimum number of divisors.</p></div><div class="input-specification"><p>The first line contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100000</span>) which represents the number of volumes and free places.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> numbers — the sought disposition with the minimum divisor number. The <span class="tex-span"><i>j</i></span>-th number (<span class="tex-span">1 ≤ <i>j</i> ≤ <i>n</i></span>) should be equal to <span class="tex-span"><i>p</i>(<i>j</i>)</span> — the number of tome that stands on the <span class="tex-span"><i>j</i></span>-th place. If there are several solutions, print any of them.</p></div>

## Input

<p>The first line contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100000</span>) which represents the number of volumes and free places.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> numbers — the sought disposition with the minimum divisor number. The <span class="tex-span"><i>j</i></span>-th number (<span class="tex-span">1 ≤ <i>j</i> ≤ <i>n</i></span>) should be equal to <span class="tex-span"><i>p</i>(<i>j</i>)</span> — the number of tome that stands on the <span class="tex-span"><i>j</i></span>-th place. If there are several solutions, print any of them.</p>





```input1
2

```




```input2
3

```




```output1
2 1 

```




```output2
1 3 2 

```


