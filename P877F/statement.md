## Description

<div><p>In Ann's favorite book shop are as many as <span class="tex-span"><i>n</i></span> books on math and economics. Books are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Each of them contains non-negative number of problems.</p><p>Today there is a sale: any subsegment of a segment from <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span> can be bought at a fixed price. </p><p>Ann decided that she wants to buy such non-empty subsegment that the sale operates on it and the number of math problems is greater than the number of economics problems <span class="tex-font-style-bf">exactly</span> by <span class="tex-span"><i>k</i></span>. Note that <span class="tex-span"><i>k</i></span> may be positive, negative or zero.</p><p>Unfortunately, Ann is not sure on which segment the sale operates, but she has <span class="tex-span"><i>q</i></span> assumptions. For each of them she wants to know the number of options to buy a subsegment satisfying the condition (because the time she spends on choosing depends on that).</p><p>Currently Ann is too busy solving other problems, she asks you for help. For each her assumption determine the number of subsegments of the given segment such that the number of math problems is greaten than the number of economics problems on that subsegment exactly by <span class="tex-span"><i>k</i></span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>) — the number of books and the needed difference between the number of math problems and the number of economics problems.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>), where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> is <span class="tex-span">1</span> if the <span class="tex-span"><i>i</i></span>-th book is on math or <span class="tex-span">2</span> if the <span class="tex-span"><i>i</i></span>-th is on economics.</p><p>The third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of problems in the <span class="tex-span"><i>i</i></span>-th book.</p><p>The fourth line contains a single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 100 000</span>) — the number of assumptions.</p><p>Each of the next <span class="tex-span"><i>q</i></span> lines contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) describing the <span class="tex-span"><i>i</i></span>-th Ann's assumption.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>q</i></span> lines, in the <span class="tex-span"><i>i</i></span>-th of them print the number of subsegments for the <span class="tex-span"><i>i</i></span>-th Ann's assumption.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>) — the number of books and the needed difference between the number of math problems and the number of economics problems.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>), where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> is <span class="tex-span">1</span> if the <span class="tex-span"><i>i</i></span>-th book is on math or <span class="tex-span">2</span> if the <span class="tex-span"><i>i</i></span>-th is on economics.</p><p>The third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of problems in the <span class="tex-span"><i>i</i></span>-th book.</p><p>The fourth line contains a single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 100 000</span>) — the number of assumptions.</p><p>Each of the next <span class="tex-span"><i>q</i></span> lines contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) describing the <span class="tex-span"><i>i</i></span>-th Ann's assumption.</p>

## Output

<p>Print <span class="tex-span"><i>q</i></span> lines, in the <span class="tex-span"><i>i</i></span>-th of them print the number of subsegments for the <span class="tex-span"><i>i</i></span>-th Ann's assumption.</p>





```input1
4 1
1 1 1 2
1 1 1 1
4
1 2
1 3
1 4
3 4

```




```input2
4 0
1 2 1 2
0 0 0 0
1
1 4

```




```output1
2
3
4
1

```




```output2
10

```



## Note

<p>In the first sample Ann can buy subsegments <span class="tex-span">[1;1], [2;2], [3;3], [2;4]</span> if they fall into the sales segment, because the number of math problems is greater by <span class="tex-span">1</span> on them that the number of economics problems. So we should count for each assumption the number of these subsegments that are subsegments of the given segment.</p><p>Segments <span class="tex-span">[1;1]</span> and <span class="tex-span">[2;2]</span> are subsegments of <span class="tex-span">[1;2]</span>.</p><p>Segments <span class="tex-span">[1;1], [2;2]</span> and <span class="tex-span">[3;3]</span> are subsegments of <span class="tex-span">[1;3]</span>.</p><p>Segments <span class="tex-span">[1;1], [2;2], [3;3], [2;4]</span> are subsegments of <span class="tex-span">[1;4]</span>.</p><p>Segment <span class="tex-span">[3;3]</span> is subsegment of <span class="tex-span">[3;4]</span>.</p>
