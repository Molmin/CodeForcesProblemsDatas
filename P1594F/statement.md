## Description

<div><p>Theofanis decided to visit his uncle's farm. There are $s$ animals and $n$ animal pens on the farm. For utility purpose, animal pens are constructed in one row.</p><p>Uncle told Theofanis that a farm is <span class="tex-font-style-it">lucky</span> if you can distribute all animals in all pens in such a way that there are no empty pens and there is at least one continuous segment of pens that has exactly $k$ animals in total.</p><p>Moreover, a farm is <span class="tex-font-style-it">ideal</span> if it's lucky for any distribution without empty pens.</p><p>Neither Theofanis nor his uncle knows if their farm is ideal or not. Can you help them to figure it out?</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^5$)&nbsp;— the number of test cases.</p><p>The first and only line of each test case contains three integers $s$, $n$, and $k$ ($1 \le s, n, k \le 10^{18}$; $n \le s$).</p></div><div class="output-specification"><p>For each test case, print <span class="tex-font-style-tt">YES</span> (case-insensitive), if the farm is ideal, or <span class="tex-font-style-tt">NO</span> (case-insensitive) otherwise.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^5$)&nbsp;— the number of test cases.</p><p>The first and only line of each test case contains three integers $s$, $n$, and $k$ ($1 \le s, n, k \le 10^{18}$; $n \le s$).</p>

## Output

<p>For each test case, print <span class="tex-font-style-tt">YES</span> (case-insensitive), if the farm is ideal, or <span class="tex-font-style-tt">NO</span> (case-insensitive) otherwise.</p>





```input1
4
1 1 1
1 1 2
100 50 200
56220 47258 14497
```




```output1
YES
NO
NO
YES
```



## Note

<p>For the first and the second test case, the only possible combination is $[1]$ so there always will be a subsegment with $1$ animal but not with $2$ animals.</p>
