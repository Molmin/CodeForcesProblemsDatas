## Description

<div><p>Sereja has an array <span class="tex-span"><i>a</i></span>, consisting of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span>. The boy cannot sit and do nothing, he decided to study an array. Sereja took a piece of paper and wrote out <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>l</i><sub class="lower-index">1</sub>, <i>l</i><sub class="lower-index">2</sub>, ..., <i>l</i><sub class="lower-index"><i>m</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>. For each number <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> he wants to know how many distinct numbers are staying on the positions <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub> + 1</span>, ..., <span class="tex-span"><i>n</i></span>. Formally, he want to find the number of distinct numbers among <span class="tex-span"><i>a</i><sub class="lower-index"><i>l</i><sub class="lower-index"><i>i</i></sub></sub>, <i>a</i><sub class="lower-index"><i>l</i><sub class="lower-index"><i>i</i></sub> + 1</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>.?</p><p>Sereja wrote out the necessary array elements but the array was so large and the boy was so pressed for time. Help him, find the answer for the described question for each <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span> — the array elements.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain integers <span class="tex-span"><i>l</i><sub class="lower-index">1</sub>, <i>l</i><sub class="lower-index">2</sub>, ..., <i>l</i><sub class="lower-index"><i>m</i></sub></span>. The <span class="tex-span"><i>i</i></span>-th line contains integer <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> lines — on the <span class="tex-span"><i>i</i></span>-th line print the answer to the number <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span> — the array elements.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain integers <span class="tex-span"><i>l</i><sub class="lower-index">1</sub>, <i>l</i><sub class="lower-index">2</sub>, ..., <i>l</i><sub class="lower-index"><i>m</i></sub></span>. The <span class="tex-span"><i>i</i></span>-th line contains integer <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> lines — on the <span class="tex-span"><i>i</i></span>-th line print the answer to the number <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>.</p>





```input1
10 10
1 2 3 4 1 2 3 4 100000 99999
1
2
3
4
5
6
7
8
9
10

```




```output1
6
6
6
6
6
5
4
3
2
1

```


