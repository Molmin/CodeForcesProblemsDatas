## Description

<div><p>The city Valera lives in is going to hold elections to the city Parliament.</p><p>The city has <span class="tex-span"><i>n</i></span> districts and <span class="tex-span"><i>n</i> - 1</span> bidirectional roads. We know that from any district there is a path along the roads to any other district. Let's enumerate all districts in some way by integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, inclusive. Furthermore, for each road the residents decided if it is the problem road or not. <span class="tex-font-style-it">A problem road</span> is a road that needs to be repaired.</p><p>There are <span class="tex-span"><i>n</i></span> candidates running the elections. Let's enumerate all candidates in some way by integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, inclusive. If the candidate number <span class="tex-span"><i>i</i></span> will be elected in the city Parliament, he will perform exactly one promise — to repair all problem roads on the way from the <span class="tex-span"><i>i</i></span>-th district to the district <span class="tex-span">1</span>, where the city Parliament is located.</p><p>Help Valera and determine the subset of candidates such that if all candidates from the subset will be elected to the city Parliament, all problem roads in the city will be repaired. If there are several such subsets, you should choose the subset consisting of the minimum number of candidates.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of districts in the city.</p><p>Then <span class="tex-span"><i>n</i> - 1</span> lines follow. Each line contains the description of a city road as three positive integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>) — the districts connected by the <span class="tex-span"><i>i</i></span>-th bidirectional road and the road type. If <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> equals to one, then the <span class="tex-span"><i>i</i></span>-th road isn't the problem road; if <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> equals to two, then the <span class="tex-span"><i>i</i></span>-th road is the problem road.</p><p>It's guaranteed that the graph structure of the city is a tree.</p></div><div class="output-specification"><p>In the first line print a single non-negative number <span class="tex-span"><i>k</i></span> — the minimum size of the required subset of candidates. Then on the second line print <span class="tex-span"><i>k</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... <i>a</i><sub class="lower-index"><i>k</i></sub></span> — the numbers of the candidates that form the required subset. If there are multiple solutions, you are allowed to print any of them.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of districts in the city.</p><p>Then <span class="tex-span"><i>n</i> - 1</span> lines follow. Each line contains the description of a city road as three positive integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>) — the districts connected by the <span class="tex-span"><i>i</i></span>-th bidirectional road and the road type. If <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> equals to one, then the <span class="tex-span"><i>i</i></span>-th road isn't the problem road; if <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> equals to two, then the <span class="tex-span"><i>i</i></span>-th road is the problem road.</p><p>It's guaranteed that the graph structure of the city is a tree.</p>

## Output

<p>In the first line print a single non-negative number <span class="tex-span"><i>k</i></span> — the minimum size of the required subset of candidates. Then on the second line print <span class="tex-span"><i>k</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... <i>a</i><sub class="lower-index"><i>k</i></sub></span> — the numbers of the candidates that form the required subset. If there are multiple solutions, you are allowed to print any of them.</p>





```input1
5
1 2 2
2 3 2
3 4 2
4 5 2

```




```input2
5
1 2 1
2 3 2
2 4 1
4 5 1

```




```input3
5
1 2 2
1 3 2
1 4 2
1 5 2

```




```output1
1
5 

```




```output2
1
3 

```




```output3
4
5 4 3 2 

```


