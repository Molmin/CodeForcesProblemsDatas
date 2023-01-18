## Description

<div><p>Yash loves playing with trees and gets especially excited when they have something to do with prime numbers. On his 20th birthday he was granted with a rooted tree of <span class="tex-span"><i>n</i></span> nodes to answer queries on. Hearing of prime numbers on trees, Yash gets too intoxicated with excitement and asks you to help out and answer queries on trees for him. Tree is rooted at node <span class="tex-span">1</span>. Each node <span class="tex-span"><i>i</i></span> has some value <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> associated with it. Also, integer <span class="tex-span"><i>m</i></span> is given.</p><p>There are queries of two types:</p><ol> <li> for given node <span class="tex-span"><i>v</i></span> and integer value <span class="tex-span"><i>x</i></span>, increase all <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> in the subtree of node <span class="tex-span"><i>v</i></span> by value <span class="tex-span"><i>x</i></span> </li><li> for given node <span class="tex-span"><i>v</i></span>, find the number of prime numbers <span class="tex-span"><i>p</i></span> less than <span class="tex-span"><i>m</i></span>, for which there exists a node <span class="tex-span"><i>u</i></span> in the subtree of <span class="tex-span"><i>v</i></span> and a non-negative integer value <span class="tex-span"><i>k</i></span>, such that <span class="tex-span"><i>a</i><sub class="lower-index"><i>u</i></sub> = <i>p</i> + <i>m</i>·<i>k</i></span>.</li></ol></div><div class="input-specification"><p>The first of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000, 1 ≤ <i>m</i> ≤ 1000</span>)&nbsp;— the number of nodes in the tree and value <span class="tex-span"><i>m</i></span> from the problem statement, respectively.</p><p>The second line consists of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— initial values of the nodes.</p><p>Then follow <span class="tex-span"><i>n</i> - 1</span> lines that describe the tree. Each of them contains two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— indices of nodes connected by the <span class="tex-span"><i>i</i></span>-th edge.</p><p>Next line contains a single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 100 000</span>)&nbsp;— the number of queries to proceed.</p><p>Each of the last <span class="tex-span"><i>q</i></span> lines is either <span class="tex-font-style-tt">1 v x</span> or <span class="tex-font-style-tt">2 v</span> (<span class="tex-span">1 ≤ <i>v</i> ≤ <i>n</i>, 0 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup></span>), giving the query of the first or the second type, respectively. It's guaranteed that there will be at least one query of the second type.</p></div><div class="output-specification"><p>For each of the queries of the second type print the number of suitable prime numbers.</p></div>

## Input

<p>The first of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000, 1 ≤ <i>m</i> ≤ 1000</span>)&nbsp;— the number of nodes in the tree and value <span class="tex-span"><i>m</i></span> from the problem statement, respectively.</p><p>The second line consists of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— initial values of the nodes.</p><p>Then follow <span class="tex-span"><i>n</i> - 1</span> lines that describe the tree. Each of them contains two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— indices of nodes connected by the <span class="tex-span"><i>i</i></span>-th edge.</p><p>Next line contains a single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 100 000</span>)&nbsp;— the number of queries to proceed.</p><p>Each of the last <span class="tex-span"><i>q</i></span> lines is either <span class="tex-font-style-tt">1 v x</span> or <span class="tex-font-style-tt">2 v</span> (<span class="tex-span">1 ≤ <i>v</i> ≤ <i>n</i>, 0 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup></span>), giving the query of the first or the second type, respectively. It's guaranteed that there will be at least one query of the second type.</p>

## Output

<p>For each of the queries of the second type print the number of suitable prime numbers.</p>





```input1
8 20
3 7 9 8 4 11 7 3
1 2
1 3
3 4
4 5
4 6
4 7
5 8
4
2 1
1 1 1
2 5
2 4

```




```input2
5 10
8 7 5 1 0
1 2
2 3
1 5
2 4
3
1 1 0
1 1 2
2 2

```




```output1
3
1
1

```




```output2
2

```


