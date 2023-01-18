## Description

<div><p>Niwel is a little golden bear. As everyone knows, bears live in forests, but Niwel got tired of seeing all the trees so he decided to move to the city.</p><p>In the city, Niwel took on a job managing bears to deliver goods. The city that he lives in can be represented as a directed graph with <span class="tex-span"><i>n</i></span> nodes and <span class="tex-span"><i>m</i></span> edges. Each edge has a weight capacity. A delivery consists of a bear carrying weights with their bear hands on a simple path from node <span class="tex-span">1</span> to node <span class="tex-span"><i>n</i></span>. The total weight that travels across a particular edge must not exceed the weight capacity of that edge.</p><p>Niwel has <span class="tex-font-style-bf">exactly</span> <span class="tex-span"><i>x</i></span> bears. In the interest of fairness, no bear can rest, and the weight that each bear carries must be exactly the same. However, each bear may take different paths if they like.</p><p>Niwel would like to determine, what is the maximum amount of weight he can deliver (it's the sum of weights carried by bears). Find the maximum weight.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>x</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 50</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 500</span>, <span class="tex-span">1 ≤ <i>x</i> ≤ 100 000</span>)&nbsp;— the number of nodes, the number of directed edges and the number of bears, respectively.</p><p>Each of the following <span class="tex-span"><i>m</i></span> lines contains three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 1 000 000</span>). This represents a directed edge from node <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> with weight capacity <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>. There are no self loops and no multiple edges from one city to the other city. More formally, for each <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> that <span class="tex-span"><i>i</i> ≠ <i>j</i></span> it's guaranteed that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>a</i><sub class="lower-index"><i>j</i></sub></span> or <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>j</i></sub></span>. It is also guaranteed that there is at least one path from node 1 to node <span class="tex-span"><i>n</i></span>.</p></div><div class="output-specification"><p>Print one real value on a single line&nbsp;— the maximum amount of weight Niwel can deliver if he uses exactly <span class="tex-span"><i>x</i></span> bears. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct if <img align="middle" class="tex-formula" src="file://b944V8Zu.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>x</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 50</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 500</span>, <span class="tex-span">1 ≤ <i>x</i> ≤ 100 000</span>)&nbsp;— the number of nodes, the number of directed edges and the number of bears, respectively.</p><p>Each of the following <span class="tex-span"><i>m</i></span> lines contains three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 1 000 000</span>). This represents a directed edge from node <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> with weight capacity <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>. There are no self loops and no multiple edges from one city to the other city. More formally, for each <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> that <span class="tex-span"><i>i</i> ≠ <i>j</i></span> it's guaranteed that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>a</i><sub class="lower-index"><i>j</i></sub></span> or <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>j</i></sub></span>. It is also guaranteed that there is at least one path from node 1 to node <span class="tex-span"><i>n</i></span>.</p>

## Output

<p>Print one real value on a single line&nbsp;— the maximum amount of weight Niwel can deliver if he uses exactly <span class="tex-span"><i>x</i></span> bears. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct if <img align="middle" class="tex-formula" src="file://b944V8Zu.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
4 4 3
1 2 2
2 4 1
1 3 1
3 4 2

```




```input2
5 11 23
1 2 3
2 3 4
3 4 5
4 5 6
1 3 4
2 4 5
3 5 6
1 4 2
2 5 3
1 5 2
3 2 30

```




```output1
1.5000000000

```




```output2
10.2222222222

```



## Note

<p>In the first sample, Niwel has three bears. Two bears can choose the path <img align="middle" class="tex-formula" src="file://MwrmwhRf.png" style="max-width: 100.0%;max-height: 100.0%;">, while one bear can choose the path <img align="middle" class="tex-formula" src="file://GBYLckQ3.png" style="max-width: 100.0%;max-height: 100.0%;">. Even though the bear that goes on the path <img align="middle" class="tex-formula" src="file://WeWIwEyO.png" style="max-width: 100.0%;max-height: 100.0%;"> can carry one unit of weight, in the interest of fairness, he is restricted to carry 0.5 units of weight. Thus, the total weight is 1.5 units overall. Note that even though Niwel can deliver more weight with just 2 bears, he must use exactly 3 bears on this day.</p>
