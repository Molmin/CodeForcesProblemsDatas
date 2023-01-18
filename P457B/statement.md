## Description

<div><p>Piegirl was asked to implement two table join operation for distributed database system, minimizing the network traffic.</p><p>Suppose she wants to join two tables, <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span>. Each of them has certain number of rows which are distributed on different number of partitions. Table <span class="tex-span"><i>A</i></span> is distributed on the first cluster consisting of <span class="tex-span"><i>m</i></span> partitions. Partition with index <span class="tex-span"><i>i</i></span> has <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> rows from <span class="tex-span"><i>A</i></span>. Similarly, second cluster containing table <span class="tex-span"><i>B</i></span> has <span class="tex-span"><i>n</i></span> partitions, <span class="tex-span"><i>i</i></span>-th one having <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> rows from <span class="tex-span"><i>B</i></span>. </p><p>In one network operation she can copy one row from any partition to any other partition. At the end, for each row from <span class="tex-span"><i>A</i></span> and each row from <span class="tex-span"><i>B</i></span> there should be a partition that has both rows. Determine the minimal number of network operations to achieve this.</p></div><div class="input-specification"><p>First line contains two integer numbers, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>m</i>, <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). Second line contains description of the first cluster with <span class="tex-span"><i>m</i></span> space separated integers, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>. Similarly, third line describes second cluster with <span class="tex-span"><i>n</i></span> space separated integers, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p></div><div class="output-specification"><p>Print one integer — minimal number of copy operations.</p></div>

## Input

<p>First line contains two integer numbers, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>m</i>, <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). Second line contains description of the first cluster with <span class="tex-span"><i>m</i></span> space separated integers, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>. Similarly, third line describes second cluster with <span class="tex-span"><i>n</i></span> space separated integers, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p>

## Output

<p>Print one integer — minimal number of copy operations.</p>





```input1
2 2
2 6
3 100

```




```input2
2 3
10 10
1 1 1

```




```output1
11

```




```output2
6

```



## Note

<p>In the first example it makes sense to move all the rows to the second partition of the second cluster which is achieved in <span class="tex-span">2 + 6 + 3 = 11</span> operations</p><p>In the second example Piegirl can copy each row from <span class="tex-span"><i>B</i></span> to the both partitions of the first cluster which needs <span class="tex-span">2·3 = 6</span> copy operations.</p>
