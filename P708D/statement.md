## Description

<div><p>At the entrance examination for the magistracy of the MSU Cyber-Mechanics Department Sasha got the question about Ford-Fulkerson algorithm. He knew the topic perfectly as he worked with it many times on programming competition. As the task for the question he was given a network with partially build flow that he had to use in order to demonstrate the workflow of the algorithm. He quickly finished to write the text and took a look at the problem only to understand that the given network is incorrect!</p><p>Suppose you are given a directed graph <span class="tex-span"><i>G</i>(<i>V</i>, <i>E</i>)</span> with two special nodes <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> called source and sink. We denote as <span class="tex-span"><i>n</i></span> the number of nodes in the graph, i.e. <span class="tex-span"><i>n</i> = |<i>V</i>|</span> and <span class="tex-span"><i>m</i></span> stands for the number of directed edges in the graph, i.e. <span class="tex-span"><i>m</i> = |<i>E</i>|</span>. For the purpose of this problem we always consider node <span class="tex-span">1</span> to be the source and node <span class="tex-span"><i>n</i></span> to be the sink. In addition, for each edge of the graph <span class="tex-span"><i>e</i></span> we define the capacity function <span class="tex-span"><i>c</i>(<i>e</i>)</span> and flow function <span class="tex-span"><i>f</i>(<i>e</i>)</span>. Function <span class="tex-span"><i>f</i>(<i>e</i>)</span> represents the correct flow if the following conditions are satisfied:</p><ol> <li> For each edge <img align="middle" class="tex-formula" src="file://6jjOssJ2.png" style="max-width: 100.0%;max-height: 100.0%;"> the flow is non-negative and does not exceed capacity <span class="tex-span"><i>c</i>(<i>e</i>)</span>, i.e. <span class="tex-span">0 ≤ <i>f</i>(<i>e</i>) ≤ <i>c</i>(<i>e</i>)</span>. </li><li> For each node <img align="middle" class="tex-formula" src="file://JF95CMIc.png" style="max-width: 100.0%;max-height: 100.0%;">, that is not source or sink (<span class="tex-span"><i>v</i> ≠ <i>s</i></span> and <span class="tex-span"><i>v</i> ≠ <i>t</i></span>) the sum of flows of all edges going in <span class="tex-span"><i>v</i></span> is equal to the sum of the flows among all edges going out from <span class="tex-span"><i>v</i></span>. In other words, there is no flow stuck in <span class="tex-span"><i>v</i></span>. </li></ol><p>It was clear that as the exam was prepared last night and there are plenty of mistakes in the tasks. Sasha asked one of the professors to fix the network or give the correct task, but the reply was that the magistrate student should be able to fix the network himself. As the professor doesn't want the task to become easier, he asks Sasha to fix the network in a such way that the total number of changes is minimum possible. Sasha is not allowed to remove edges, add new ones or reverse the direction of existing edges. The only thing he is able to do is to change capacity function <span class="tex-span"><i>c</i>(<i>e</i>)</span> and flow function <span class="tex-span"><i>f</i>(<i>e</i>)</span>. Moreover, all the values should remain non-negative integers. There is no requirement on the flow to be maximum in any sense.</p><p>Find the minimum possible total change of the functions <span class="tex-span"><i>f</i>(<i>e</i>)</span> and <span class="tex-span"><i>c</i>(<i>e</i>)</span> that Sasha has to make in order to make the flow correct. The total change is defined as the sum of absolute differences, i.e. if new functions are <span class="tex-span"><i>f</i><sup class="upper-index"> * </sup>(<i>e</i>)</span> and <span class="tex-span"><i>c</i><sup class="upper-index"> * </sup>(<i>e</i>)</span>, then the total change is <img align="middle" class="tex-formula" src="file://ikg5EDy6.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 100</span>)&nbsp;— the number of nodes and edges in the graph respectively. Each of the following <span class="tex-span"><i>m</i></span> lines contains the description of the edges, consisting of four integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>f</i><sub class="lower-index"><i>i</i></sub> ≤ 1 000 000</span>)&nbsp;— index of the node the edges starts from, the index of the node the edge goes to, current capacity and flow value.</p><p>Node number <span class="tex-span">1</span> is the source, and node number <span class="tex-span"><i>n</i></span> is the sink. It's guaranteed that no edge goes to the source, and no edges starts in the sink.</p><p>Given graph contains no self-loops but may contain multiple edges.</p></div><div class="output-specification"><p>Print one integer&nbsp;— the minimum total sum of changes that Sasha has to do in order to get the correct flow description.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 100</span>)&nbsp;— the number of nodes and edges in the graph respectively. Each of the following <span class="tex-span"><i>m</i></span> lines contains the description of the edges, consisting of four integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>f</i><sub class="lower-index"><i>i</i></sub> ≤ 1 000 000</span>)&nbsp;— index of the node the edges starts from, the index of the node the edge goes to, current capacity and flow value.</p><p>Node number <span class="tex-span">1</span> is the source, and node number <span class="tex-span"><i>n</i></span> is the sink. It's guaranteed that no edge goes to the source, and no edges starts in the sink.</p><p>Given graph contains no self-loops but may contain multiple edges.</p>

## Output

<p>Print one integer&nbsp;— the minimum total sum of changes that Sasha has to do in order to get the correct flow description.</p>





```input1
2 1
1 2 2 1

```




```input2
2 1
1 2 1 2

```




```input3
3 3
1 2 1 1
2 3 2 2
1 3 3 3

```




```input4
4 2
2 3 1 1
3 2 1 1

```




```output1
0

```




```output2
1

```




```output3
1

```




```output4
0

```



## Note

<p>In the first sample, the flow is initially correct. Note, that the flow is not maximum, but this is not required.</p><p>In the second sample, the flow value of the only edge is greater than its capacity. There are two ways to fix this: either increase the capacity up to <span class="tex-span">2</span> or reduce the flow down to <span class="tex-span">1</span>.</p><p>In the third sample, there is only <span class="tex-span">1</span> unit of flow coming to vertex <span class="tex-span">2</span>, but there are <span class="tex-span">2</span> units going out of it. One of the possible solutions is to reduce the value of the flow on the second edge by <span class="tex-span">1</span>.</p><p>In the fourth sample, there is isolated circulation of flow, but this description is correct by definition.</p>
