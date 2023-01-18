## Description

<div><p>Bogdan has a birthday today and mom gave him a tree consisting of <span class="tex-span"><i>n</i></span> vertecies. For every edge of the tree <span class="tex-span"><i>i</i></span>, some number <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> was written on it. In case you forget, a tree is a connected non-directed graph without cycles. After the present was granted, <span class="tex-span"><i>m</i></span> guests consecutively come to Bogdan's party. When the <span class="tex-span"><i>i</i></span>-th guest comes, he performs exactly one of the two possible operations: </p><ol> <li> Chooses some number <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, and two vertecies <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. After that, he moves along the edges of the tree from vertex <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to vertex <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> using the shortest path (of course, such a path is unique in the tree). Every time he moves along some edge <span class="tex-span"><i>j</i></span>, he replaces his current number <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> by <img align="middle" class="tex-formula" src="file://5YH5Y4Zy.png" style="max-width: 100.0%;max-height: 100.0%;">, that is, by the result of integer division <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> div <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub></span>. </li><li> Chooses some edge <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and replaces the value written in it <span class="tex-span"><i>x</i><sub class="lower-index"><i>p</i><sub class="lower-index"><i>i</i></sub></sub></span> by some positive integer <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub> &lt; <i>x</i><sub class="lower-index"><i>p</i><sub class="lower-index"><i>i</i></sub></sub></span>. </li></ol><p>As Bogdan cares about his guests, he decided to ease the process. Write a program that performs all the operations requested by guests and outputs the resulting value <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> for each <span class="tex-span"><i>i</i></span> of the first type.</p></div><div class="input-specification"><p>The first line of the input contains integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200 000</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 200 000</span>)&nbsp;— the number of vertecies in the tree granted to Bogdan by his mom and the number of guests that came to the party respectively.</p><p>Next <span class="tex-span"><i>n</i> - 1</span> lines contain the description of the edges. The <span class="tex-span"><i>i</i></span>-th of these lines contains three integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">18</sup></span>), denoting an edge that connects vertecies <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, with the number <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> initially written on it.</p><p>The following <span class="tex-span"><i>m</i></span> lines describe operations, requested by Bogdan's guests. Each description contains three or four integers and has one of the two possible forms: </p><ul> <li> <span class="tex-span">1</span> <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> corresponds to a guest, who chooses the operation of the first type. </li><li> <span class="tex-span">2</span> <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> corresponds to a guests, who chooses the operation of the second type. </li></ul> It is guaranteed that all the queries are correct, namely <span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> - 1</span>, <span class="tex-span">1 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">18</sup></span> and <span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> &lt; <i>x</i><sub class="lower-index"><i>p</i><sub class="lower-index"><i>i</i></sub></sub></span>, where <span class="tex-span"><i>x</i><sub class="lower-index"><i>p</i><sub class="lower-index"><i>i</i></sub></sub></span> represents a number written on edge <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> at this particular moment of time that is not necessarily equal to the initial value <span class="tex-span"><i>x</i><sub class="lower-index"><i>p</i><sub class="lower-index"><i>i</i></sub></sub></span>, as some decreases may have already been applied to it. The edges are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i> - 1</span> in the order they appear in the input.</div><div class="output-specification"><p>For each guest who chooses the operation of the first type, print the result of processing the value <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> through the path from <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>.</p></div>

## Input

<p>The first line of the input contains integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200 000</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 200 000</span>)&nbsp;— the number of vertecies in the tree granted to Bogdan by his mom and the number of guests that came to the party respectively.</p><p>Next <span class="tex-span"><i>n</i> - 1</span> lines contain the description of the edges. The <span class="tex-span"><i>i</i></span>-th of these lines contains three integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">18</sup></span>), denoting an edge that connects vertecies <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, with the number <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> initially written on it.</p><p>The following <span class="tex-span"><i>m</i></span> lines describe operations, requested by Bogdan's guests. Each description contains three or four integers and has one of the two possible forms: </p><ul> <li> <span class="tex-span">1</span> <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> corresponds to a guest, who chooses the operation of the first type. </li><li> <span class="tex-span">2</span> <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> corresponds to a guests, who chooses the operation of the second type. </li></ul> It is guaranteed that all the queries are correct, namely <span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> - 1</span>, <span class="tex-span">1 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">18</sup></span> and <span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> &lt; <i>x</i><sub class="lower-index"><i>p</i><sub class="lower-index"><i>i</i></sub></sub></span>, where <span class="tex-span"><i>x</i><sub class="lower-index"><i>p</i><sub class="lower-index"><i>i</i></sub></sub></span> represents a number written on edge <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> at this particular moment of time that is not necessarily equal to the initial value <span class="tex-span"><i>x</i><sub class="lower-index"><i>p</i><sub class="lower-index"><i>i</i></sub></sub></span>, as some decreases may have already been applied to it. The edges are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i> - 1</span> in the order they appear in the input.

## Output

<p>For each guest who chooses the operation of the first type, print the result of processing the value <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> through the path from <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>.</p>





```input1
6 6
1 2 1
1 3 7
1 4 4
2 5 5
2 6 2
1 4 6 17
2 3 2
1 4 6 17
1 5 5 20
2 4 1
1 5 1 3

```




```input2
5 4
1 2 7
1 3 3
3 4 2
3 5 5
1 4 2 100
1 5 4 1
2 2 2
1 1 3 4

```




```output1
2
4
20
3

```




```output2
2
0
2

```



## Note

<center><p>Initially the tree looks like this: </p><center> <img class="tex-graphics" src="file://4mJOXU3q.png" style="max-width: 100.0%;max-height: 100.0%;"> <p>The response to the first query is: <img align="middle" class="tex-formula" src="file://Wo9VcCVc.png" style="max-width: 100.0%;max-height: 100.0%;"> = 2</p><p>After the third edge is changed, the tree looks like this: </p><center> <img class="tex-graphics" src="file://Nwx7Mnbp.png" style="max-width: 100.0%;max-height: 100.0%;"> <p>The response to the second query is: <img align="middle" class="tex-formula" src="file://EJCan1oW.png" style="max-width: 100.0%;max-height: 100.0%;"> = 4</p><p>In the third query the initial and final vertex coincide, that is, the answer will be the initial number 20.</p><p>After the change in the fourth edge the tree looks like this: </p><center> <img class="tex-graphics" src="file://ZDcvPMs9.png" style="max-width: 100.0%;max-height: 100.0%;"> <p>In the last query the answer will be: <img align="middle" class="tex-formula" src="file://6Mz0vL9N.png" style="max-width: 100.0%;max-height: 100.0%;"> = 3</p></center></center></center></center>
