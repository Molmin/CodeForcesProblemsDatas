## Description

<div><p>In the country there are <span class="tex-span"><i>n</i></span> cities and <span class="tex-span"><i>m</i></span> bidirectional roads between them. Each city has an army. Army of the <span class="tex-span"><i>i</i></span>-th city consists of <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> soldiers. Now soldiers roam. After roaming each soldier has to either stay in his city or to go to the one of neighboring cities by at <span class="tex-font-style-bf">moving along at most one road</span>.</p><p>Check if is it possible that after roaming there will be exactly <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> soldiers in the <span class="tex-span"><i>i</i></span>-th city.</p></div><div class="input-specification"><p>First line of input consists of two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 200</span>).</p><p>Next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>).</p><p>Next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>).</p><p>Then <span class="tex-span"><i>m</i></span> lines follow, each of them consists of two integers <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>p</i>, <i>q</i> ≤ <i>n</i></span>, <span class="tex-span"><i>p</i> ≠ <i>q</i></span>) denoting that there is an undirected road between cities <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>q</i></span>. </p><p>It is guaranteed that there is at most one road between each pair of cities.</p></div><div class="output-specification"><p>If the conditions can not be met output single word "<span class="tex-font-style-tt">NO</span>".</p><p>Otherwise output word "<span class="tex-font-style-tt">YES</span>" and then <span class="tex-span"><i>n</i></span> lines, each of them consisting of <span class="tex-span"><i>n</i></span> integers. Number in the <span class="tex-span"><i>i</i></span>-th line in the <span class="tex-span"><i>j</i></span>-th column should denote how many soldiers should road from city <span class="tex-span"><i>i</i></span> to city <span class="tex-span"><i>j</i></span> (if <span class="tex-span"><i>i</i> ≠ <i>j</i></span>) or how many soldiers should stay in city <span class="tex-span"><i>i</i></span> (if <span class="tex-span"><i>i</i> = <i>j</i></span>).</p><p>If there are several possible answers you may output any of them.</p></div>

## Input

<p>First line of input consists of two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 200</span>).</p><p>Next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>).</p><p>Next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>).</p><p>Then <span class="tex-span"><i>m</i></span> lines follow, each of them consists of two integers <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>p</i>, <i>q</i> ≤ <i>n</i></span>, <span class="tex-span"><i>p</i> ≠ <i>q</i></span>) denoting that there is an undirected road between cities <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>q</i></span>. </p><p>It is guaranteed that there is at most one road between each pair of cities.</p>

## Output

<p>If the conditions can not be met output single word "<span class="tex-font-style-tt">NO</span>".</p><p>Otherwise output word "<span class="tex-font-style-tt">YES</span>" and then <span class="tex-span"><i>n</i></span> lines, each of them consisting of <span class="tex-span"><i>n</i></span> integers. Number in the <span class="tex-span"><i>i</i></span>-th line in the <span class="tex-span"><i>j</i></span>-th column should denote how many soldiers should road from city <span class="tex-span"><i>i</i></span> to city <span class="tex-span"><i>j</i></span> (if <span class="tex-span"><i>i</i> ≠ <i>j</i></span>) or how many soldiers should stay in city <span class="tex-span"><i>i</i></span> (if <span class="tex-span"><i>i</i> = <i>j</i></span>).</p><p>If there are several possible answers you may output any of them.</p>





```input1
4 4
1 2 6 3
3 5 3 1
1 2
2 3
3 4
4 2

```




```input2
2 0
1 2
2 1

```




```output1
YES
1 0 0 0 
2 0 0 0 
0 5 1 0 
0 0 2 1 

```




```output2
NO
```


