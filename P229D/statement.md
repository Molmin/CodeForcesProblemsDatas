## Description

<div><p>The city of D consists of <span class="tex-span"><i>n</i></span> towers, built consecutively on a straight line. The height of the tower that goes <span class="tex-span"><i>i</i></span>-th (from left to right) in the sequence equals <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span>. The city mayor decided to rebuild the city to make it <span class="tex-font-style-underline">beautiful</span>. In a <span class="tex-font-style-underline">beautiful</span> city all towers are are arranged in non-descending order of their height from left to right.</p><p>The rebuilding consists of performing several (perhaps zero) operations. An operation constitutes using a crane to take any tower and put it altogether on the top of some other neighboring tower. In other words, we can take the tower that stands <span class="tex-span"><i>i</i></span>-th and put it on the top of either the <span class="tex-span">(<i>i</i> - 1)</span>-th tower (if it exists), or the <span class="tex-span">(<i>i</i> + 1)</span>-th tower (of it exists). The height of the resulting tower equals the sum of heights of the two towers that were put together. After that the two towers can't be split by any means, but more similar operations can be performed on the resulting tower. Note that after each operation the total number of towers on the straight line decreases by 1.</p><p>Help the mayor determine the minimum number of operations required to make the city beautiful.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>)&nbsp;— the number of towers in the city. The next line contains <span class="tex-span"><i>n</i></span> space-separated integers: the <span class="tex-span"><i>i</i></span>-th number <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>) determines the height of the tower that is <span class="tex-span"><i>i</i></span>-th (from left to right) in the initial tower sequence.</p></div><div class="output-specification"><p>Print a single integer — the minimum number of operations needed to make the city beautiful.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>)&nbsp;— the number of towers in the city. The next line contains <span class="tex-span"><i>n</i></span> space-separated integers: the <span class="tex-span"><i>i</i></span>-th number <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>) determines the height of the tower that is <span class="tex-span"><i>i</i></span>-th (from left to right) in the initial tower sequence.</p>

## Output

<p>Print a single integer — the minimum number of operations needed to make the city beautiful.</p>





```input1
5
8 2 7 3 1

```




```input2
3
5 2 1

```




```output1
3

```




```output2
2

```


