## Description

<div><center> <img class="tex-graphics" src="file://ohfy20bt.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Ela needs to send a large package from machine $1$ to machine $n$ through a network of machines. Currently, with the network condition, she complains that the network is too slow and the package can't arrive in time. Luckily, a Wiring Wizard offered her a helping hand.</p><p>The network can be represented as an <span class="tex-font-style-bf">undirected connected graph</span> with $n$ nodes, each node representing a machine. $m$ wires are used to connect them. Wire $i$ is used to connect machines $u_i$ and $v_i$, and has a weight $w_i$. The aforementioned large package, if going through wire $i$, will move from machine $u_i$ to machine $v_i$ (or vice versa) in exactly $w_i$ microseconds. The Wiring Wizard can use his spell an arbitrary number of times. For each spell, he will choose the wire of index $i$, connecting machine $u_i$ and $v_i$, and rewire it following these steps:</p><ul> <li> Choose one machine that is connected by this wire. Without loss of generality, let's choose $v_i$. </li><li> Choose a machine that is currently connecting to $v_i$ (including $u_i$), call it $t_i$. Disconnect the wire indexed $i$ from $v_i$, then using it to connect $u_i$ and $t_i$. </li></ul><p>The rewiring of wire $i$ will takes $w_i$ microseconds, and the weight of the wire will not change after this operation. After a rewiring, a machine might have some wire connect it with itself. Also, the Wiring Wizard has warned Ela that rewiring might cause temporary disconnections between some machines, but Ela just ignores it anyway. Her mission is to send the large package from machine $1$ to machine $n$ as fast as possible. Note that the Wizard can use his spell on a wire <span class="tex-font-style-it">zero, one, or many</span> times. To make sure the network works seamlessly while transferring the large package, <span class="tex-font-style-bf">once the package starts transferring from machine $1$, the Wiring Wizard cannot use his spell to move wires around anymore.</span></p><p>Ela wonders, with the help of the Wiring Wizard, what is the least amount of time needed to transfer the large package from machine $1$ to $n$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). The description of the test cases follows.</p><p>The first line contains $n$ and $m$ ($2 \le n \le 500$, $n - 1 \le m \le 250 000$), the number of nodes and number of wires, respectively.</p><p>For the next $m$ lines, $i$-th line will contains $u_i$, $v_i$ and $w_i$ ($1 \le u_i, v_i \le n$, $1 \le w_i \le 10^9$) - the indices 2 machines that are connected by the $i$-th edge and the weight of it.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $500$ and the sum of $m$ over all test cases does not exceed $250 000$. The graph in each test case is guaranteed to be <span class="tex-font-style-it">connected, no self-loops</span>, but it <span class="tex-font-style-bf">can contain multiple edges</span>.</p></div><div class="output-specification"><p>For each test case, output one integer denotes the least amount of time needed to transfer the large package from machine $1$ to $n$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). The description of the test cases follows.</p><p>The first line contains $n$ and $m$ ($2 \le n \le 500$, $n - 1 \le m \le 250 000$), the number of nodes and number of wires, respectively.</p><p>For the next $m$ lines, $i$-th line will contains $u_i$, $v_i$ and $w_i$ ($1 \le u_i, v_i \le n$, $1 \le w_i \le 10^9$) - the indices 2 machines that are connected by the $i$-th edge and the weight of it.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $500$ and the sum of $m$ over all test cases does not exceed $250 000$. The graph in each test case is guaranteed to be <span class="tex-font-style-it">connected, no self-loops</span>, but it <span class="tex-font-style-bf">can contain multiple edges</span>.</p>

## Output

<p>For each test case, output one integer denotes the least amount of time needed to transfer the large package from machine $1$ to $n$.</p>





```input1|2,3,4,5,6,7,8,9,10,11,18,19,20,21,22,23,24,25,26
3
8 9
1 2 3
6 4 5
3 5 6
6 1 3
7 4 4
3 8 4
2 3 3
7 8 5
4 5 2
4 5
1 2 1
2 4 1
3 4 1
3 1 1
1 3 2
8 8
4 6 92
7 1 65
6 5 43
6 7 96
4 3 74
4 8 54
7 4 99
2 5 22
```




```output1
9
2
154
```



## Note

<p>Here is the graph in the first test case in the sample input:</p><center> <img class="tex-graphics" src="file://JgTQJCop.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Ela can ask the Wiring Wizard to use his spell on wire with the index of $7$, which is connecting machines $2$ and $3$. Then, since the machine $8$ is connected to machine $3$, the Wiring Wizard can disconnect wire $7$ from machine $3$ and connect it to machine $8$ in $3$ microseconds (weight of wire $3$).</p><p>After that, the package can be sent from machine $1$ to machine $8$ in $6$ microseconds. Therefore, the answer is $3 + 6 = 9$ microseconds.</p><p>Here is the graph in the third test case in the sample input:</p><center> <img class="tex-graphics" src="file://7HhR68vv.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
