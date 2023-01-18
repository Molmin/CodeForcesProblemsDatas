## Description

<div><p>This time you should help a team of researchers on an island in the Pacific Ocean. They research the culture of the ancient tribes that used to inhabit the island many years ago.</p><p>Overall they've dug out <span class="tex-span"><i>n</i></span> villages. Some pairs of villages were connected by roads. People could go on the roads in both directions. Overall there were exactly <span class="tex-span"><i>n</i> - 1</span> roads, and from any village one could get to any other one.</p><p>The tribes were not peaceful and they had many wars. As a result of the wars, some villages were destroyed completely. During more peaceful years some of the villages were restored.</p><p>At each moment of time people <span class="tex-font-style-underline">used</span> only those roads that belonged to some shortest way between two villages <span class="tex-font-style-underline">that existed at the given moment</span>. In other words, people used the minimum subset of roads in such a way, that it was possible to get from any existing village to any other existing one. Note that throughout the island's whole history, there existed exactly <span class="tex-span"><i>n</i> - 1</span> roads that have been found by the researchers. There never were any other roads.</p><p>The researchers think that observing the total sum of used roads’ lengths at different moments of time can help to better understand the tribes' culture and answer several historical questions.</p><p>You will be given the full history of the tribes' existence. Your task is to determine the total length of used roads at some moments of time.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of villages. The next <span class="tex-span"><i>n</i> - 1</span> lines describe the roads. The <span class="tex-span"><i>i</i></span>-th of these lines contains three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>i</i> &lt; <i>n</i></span>) — the numbers of villages that are connected by the <span class="tex-span"><i>i</i></span>-th road and the road's length. The numbers in the lines are separated by a space.</p><p>The next line contains an integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of queries. Then follow <span class="tex-span"><i>q</i></span> queries, one per line, ordered by time. Each query belongs to one of three types:</p><ul><li> "<span class="tex-font-style-tt">+ </span><span class="tex-span"><i>x</i></span>" — village number <span class="tex-span"><i>x</i></span> is restored (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i></span>). </li><li> "<span class="tex-font-style-tt">- </span><span class="tex-span"><i>x</i></span>" — village number <span class="tex-span"><i>x</i></span> is destroyed (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i></span>). </li><li> "<span class="tex-font-style-tt">?</span>" — the archaeologists want to know the total length of the roads which were used for that time period.</li></ul><p>It is guaranteed that the queries do not contradict each other, that is, there won't be queries to destroy non-existing villages or restore the already existing ones. It is guaranteed that we have at least one query of type "<span class="tex-font-style-tt">?</span>". It is also guaranteed that one can get from any village to any other one by the given roads.</p><p>At the initial moment of time no village is considered to exist.</p></div><div class="output-specification"><p>For each query of type "<span class="tex-font-style-tt">?</span>" print the total length of used roads on a single line. You should print the answers to the queries in the order, in which they are given in the input.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of villages. The next <span class="tex-span"><i>n</i> - 1</span> lines describe the roads. The <span class="tex-span"><i>i</i></span>-th of these lines contains three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>i</i> &lt; <i>n</i></span>) — the numbers of villages that are connected by the <span class="tex-span"><i>i</i></span>-th road and the road's length. The numbers in the lines are separated by a space.</p><p>The next line contains an integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of queries. Then follow <span class="tex-span"><i>q</i></span> queries, one per line, ordered by time. Each query belongs to one of three types:</p><ul><li> "<span class="tex-font-style-tt">+ </span><span class="tex-span"><i>x</i></span>" — village number <span class="tex-span"><i>x</i></span> is restored (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i></span>). </li><li> "<span class="tex-font-style-tt">- </span><span class="tex-span"><i>x</i></span>" — village number <span class="tex-span"><i>x</i></span> is destroyed (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i></span>). </li><li> "<span class="tex-font-style-tt">?</span>" — the archaeologists want to know the total length of the roads which were used for that time period.</li></ul><p>It is guaranteed that the queries do not contradict each other, that is, there won't be queries to destroy non-existing villages or restore the already existing ones. It is guaranteed that we have at least one query of type "<span class="tex-font-style-tt">?</span>". It is also guaranteed that one can get from any village to any other one by the given roads.</p><p>At the initial moment of time no village is considered to exist.</p>

## Output

<p>For each query of type "<span class="tex-font-style-tt">?</span>" print the total length of used roads on a single line. You should print the answers to the queries in the order, in which they are given in the input.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
6
1 2 1
1 3 5
4 1 7
4 5 3
6 4 2
10
+ 3
+ 1
?
+ 6
?
+ 5
?
- 6
- 3
?

```




```output1
5
14
17
10

```


