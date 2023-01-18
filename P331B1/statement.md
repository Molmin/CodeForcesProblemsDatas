## Description

<div><p>The Smart Beaver has recently designed and built an innovative nanotechnologic all-purpose beaver mass shaving machine, "Beavershave 5000". Beavershave 5000 can shave beavers by families! How does it work? Very easily!</p><p>There are <span class="tex-span"><i>n</i></span> beavers, each of them has a unique id from 1 to <span class="tex-span"><i>n</i></span>. Consider a permutation <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> of <span class="tex-span"><i>n</i></span> these beavers. Beavershave 5000 needs one session to shave beavers with ids from <span class="tex-span"><i>x</i></span> to <span class="tex-span"><i>y</i></span> (inclusive) if and only if there are such indices <span class="tex-span"><i>i</i><sub class="lower-index">1</sub> &lt; <i>i</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>i</i><sub class="lower-index"><i>k</i></sub></span>, that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i><sub class="lower-index">1</sub></sub> = <i>x</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i><sub class="lower-index">2</sub></sub> = <i>x</i> + 1</span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i><sub class="lower-index"><i>k</i> - 1</sub></sub> = <i>y</i> - 1</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i><sub class="lower-index"><i>k</i></sub></sub> = <i>y</i></span>. And that is really convenient. For example, it needs one session to shave a permutation of beavers <span class="tex-span">1, 2, 3, ..., <i>n</i></span>.</p><p>If we can't shave beavers from <span class="tex-span"><i>x</i></span> to <span class="tex-span"><i>y</i></span> in one session, then we can split these beavers into groups <span class="tex-span">[<i>x</i>, <i>p</i><sub class="lower-index">1</sub>]</span>, <span class="tex-span">[<i>p</i><sub class="lower-index">1</sub> + 1, <i>p</i><sub class="lower-index">2</sub>]</span>, ..., <span class="tex-span">[<i>p</i><sub class="lower-index"><i>m</i></sub> + 1, <i>y</i>]</span> <span class="tex-span">(<i>x</i> ≤ <i>p</i><sub class="lower-index">1</sub> &lt; <i>p</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>p</i><sub class="lower-index"><i>m</i></sub> &lt; <i>y</i>)</span>, in such a way that the machine can shave beavers in each group in one session. But then Beavershave 5000 needs <span class="tex-span"><i>m</i> + 1</span> working sessions to shave beavers from <span class="tex-span"><i>x</i></span> to <span class="tex-span"><i>y</i></span>.</p><p>All beavers are restless and they keep trying to swap. So if we consider the problem more formally, we can consider queries of two types: </p><ul> <li> what is the minimum number of sessions that Beavershave 5000 needs to shave beavers with ids from <span class="tex-span"><i>x</i></span> to <span class="tex-span"><i>y</i></span>, inclusive? </li><li> two beavers on positions <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (the beavers <span class="tex-span"><i>a</i><sub class="lower-index"><i>x</i></sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>y</i></sub></span>) swapped. </li></ul><p>You can assume that any beaver can be shaved any number of times.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> — the total number of beavers, <span class="tex-span">2 ≤ <i>n</i></span>. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers — the initial beaver permutation.</p><p>The third line contains integer <span class="tex-span"><i>q</i></span> — the number of queries, <span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>. The next <span class="tex-span"><i>q</i></span> lines contain the queries. Each query <span class="tex-span"><i>i</i></span> looks as <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, where <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> is the query type (<span class="tex-span">1</span> is to shave beavers from <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, inclusive, <span class="tex-span">2</span> is to swap beavers on positions <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>). All queries meet the condition: <span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> &lt; <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>.</p><ul> <li> to get 30 points, you need to solve the problem with constraints: <span class="tex-span"><i>n</i> ≤ 100</span> (subproblem B1); </li><li> to get 100 points, you need to solve the problem with constraints: <span class="tex-span"><i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span> (subproblems B1+B2). </li></ul><p>Note that the number of queries <span class="tex-span"><i>q</i></span> is limited <span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span> in both subproblem B1 and subproblem B2.</p></div><div class="output-specification"><p>For each query with <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> = 1</span>, print the minimum number of Beavershave 5000 sessions.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> — the total number of beavers, <span class="tex-span">2 ≤ <i>n</i></span>. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers — the initial beaver permutation.</p><p>The third line contains integer <span class="tex-span"><i>q</i></span> — the number of queries, <span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>. The next <span class="tex-span"><i>q</i></span> lines contain the queries. Each query <span class="tex-span"><i>i</i></span> looks as <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, where <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> is the query type (<span class="tex-span">1</span> is to shave beavers from <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, inclusive, <span class="tex-span">2</span> is to swap beavers on positions <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>). All queries meet the condition: <span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> &lt; <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>.</p><ul> <li> to get 30 points, you need to solve the problem with constraints: <span class="tex-span"><i>n</i> ≤ 100</span> (subproblem B1); </li><li> to get 100 points, you need to solve the problem with constraints: <span class="tex-span"><i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span> (subproblems B1+B2). </li></ul><p>Note that the number of queries <span class="tex-span"><i>q</i></span> is limited <span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span> in both subproblem B1 and subproblem B2.</p>

## Output

<p>For each query with <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> = 1</span>, print the minimum number of Beavershave 5000 sessions.</p>





```input1
5
1 3 4 2 5
6
1 1 5
1 3 4
2 2 3
1 1 5
2 1 5
1 1 5

```




```output1
2
1
3
5

```


