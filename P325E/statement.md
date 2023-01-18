## Description

<div><p>Piegirl found the red button. You have one last chance to change the inevitable end.</p><p>The circuit under the button consists of <span class="tex-span"><i>n</i></span> nodes, numbered from 0 to <span class="tex-span"><i>n</i></span> - 1. In order to deactivate the button, the <span class="tex-span"><i>n</i></span> nodes must be disarmed in a particular order. Node 0 must be disarmed first. After disarming node <span class="tex-span"><i>i</i></span>, the next node to be disarmed must be either node <span class="tex-span">(2·<i>i</i>)</span> modulo <span class="tex-span"><i>n</i></span> or node <span class="tex-span">(2·<i>i</i>) + 1</span> modulo <span class="tex-span"><i>n</i></span>. The last node to be disarmed must be node 0. Node 0 must be disarmed twice, but all other nodes must be disarmed exactly once. </p><p>Your task is to find any such order and print it. If there is no such order, print <span class="tex-font-style-tt">-1</span>.</p></div><div class="input-specification"><p>Input consists of a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p></div><div class="output-specification"><p>Print an order in which you can to disarm all nodes. If it is impossible, print <span class="tex-font-style-tt">-1</span> instead. If there are multiple orders, print any one of them.</p></div>

## Input

<p>Input consists of a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p>

## Output

<p>Print an order in which you can to disarm all nodes. If it is impossible, print <span class="tex-font-style-tt">-1</span> instead. If there are multiple orders, print any one of them.</p>





```input1
2

```




```input2
3

```




```input3
4

```




```input4
16

```




```output1
0 1 0

```




```output2
-1
```




```output3
0 1 3 2 0

```




```output4
0 1 2 4 9 3 6 13 10 5 11 7 15 14 12 8 0

```


