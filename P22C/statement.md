## Description

<div><p>Bob got a job as a system administrator in X corporation. His first task was to connect <span class="tex-span"><i>n</i></span> servers with the help of <span class="tex-span"><i>m</i></span> two-way direct connection so that it becomes possible to transmit data from one server to any other server via these connections. Each direct connection has to link two different servers, each pair of servers should have at most one direct connection. Y corporation, a business rival of X corporation, made Bob an offer that he couldn't refuse: Bob was asked to connect the servers in such a way, that when server with index <span class="tex-span"><i>v</i></span> fails, the transmission of data between some other two servers becomes impossible, i.e. the system stops being connected. Help Bob connect the servers.</p></div><div class="input-specification"><p>The first input line contains 3 space-separated integer numbers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>v</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 0 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>v</i> ≤ <i>n</i></span>), <span class="tex-span"><i>n</i></span> — amount of servers, <span class="tex-span"><i>m</i></span> — amount of direct connections, <span class="tex-span"><i>v</i></span> — index of the server that fails and leads to the failure of the whole system.</p></div><div class="output-specification"><p>If it is impossible to connect the servers in the required way, output <span class="tex-font-style-tt">-1</span>. Otherwise output <span class="tex-span"><i>m</i></span> lines with 2 numbers each — description of all the direct connections in the system. Each direct connection is described by two numbers — indexes of two servers, linked by this direct connection. The servers are numbered from 1. If the answer is not unique, output any.</p></div>

## Input

<p>The first input line contains 3 space-separated integer numbers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>v</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 0 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>v</i> ≤ <i>n</i></span>), <span class="tex-span"><i>n</i></span> — amount of servers, <span class="tex-span"><i>m</i></span> — amount of direct connections, <span class="tex-span"><i>v</i></span> — index of the server that fails and leads to the failure of the whole system.</p>

## Output

<p>If it is impossible to connect the servers in the required way, output <span class="tex-font-style-tt">-1</span>. Otherwise output <span class="tex-span"><i>m</i></span> lines with 2 numbers each — description of all the direct connections in the system. Each direct connection is described by two numbers — indexes of two servers, linked by this direct connection. The servers are numbered from 1. If the answer is not unique, output any.</p>





```input1
5 6 3

```




```input2
6 100 1

```




```output1
1 2
2 3
3 4
4 5
1 3
3 5

```




```output2
-1

```


