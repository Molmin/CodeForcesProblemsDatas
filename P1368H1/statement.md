## Description

<div><p><span class="tex-font-style-it">This is an easier version of the problem H without modification queries.</span></p><p>Lester and Delbert work at an electronics company. They are currently working on a microchip component serving to connect two independent parts of a large supercomputer.</p><p>The component is built on top of a <span class="tex-font-style-it">breadboard</span>&nbsp;— a grid-like base for a microchip. The breadboard has $n$ rows and $m$ columns, and each row-column intersection contains a node. Also, on each side of the breadboard there are ports that can be attached to adjacent nodes. Left and right side have $n$ ports each, and top and bottom side have $m$ ports each. Each of the ports is connected on the outside to one of the parts bridged by the breadboard, and is colored red or blue respectively.</p><center> <img class="tex-graphics" src="file://G5seYle5.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Ports can be connected by wires going inside the breadboard. However, there are a few rules to follow:</p><ul><li> Each wire should connect a red port with a blue port, and each port should be connected to at most one wire.</li><li> Each part of the wire should be horizontal or vertical, and turns are only possible at one of the nodes.</li><li> To avoid interference, wires can not have common parts of non-zero length (but may have common nodes). Also, a wire can not cover the same segment of non-zero length twice.</li></ul><p>The <span class="tex-font-style-it">capacity</span> of the breadboard is the largest number of red-blue wire connections that can be made subject to the rules above. For example, the breadboard above has capacity $7$, and one way to make seven connections is pictured below.</p><center> <img class="tex-graphics" src="file://3AVn0kd9.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p><span class="tex-font-style-it">Up to this point statements of both versions are identical. Differences follow below.</span></p><p>Given the current breadboard configuration, help Lester and Delbert find its capacity efficiently.</p></div><div class="input-specification"><p>The first line contains three integers $n, m, q$ ($1 \leq n, m \leq 10^5$, $\pmb{q = 0}$). $n$ and $m$ are the number of rows and columns of the breadboard respectively. <span class="tex-font-style-it">In this version $q$ is always zero, and is only present for consistency with the harder version.</span></p><p>The next four lines describe initial coloring of the ports. Each character in these lines is either <span class="tex-font-style-tt">R</span> or <span class="tex-font-style-tt">B</span>, depending on the coloring of the respective port. The first two of these lines contain $n$ characters each, and describe ports on the left and right sides respectively from top to bottom. The last two lines contain $m$ characters each, and describe ports on the top and bottom sides respectively from left to right.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the given breadboard capacity.</p></div>

## Input

<p>The first line contains three integers $n, m, q$ ($1 \leq n, m \leq 10^5$, $\pmb{q = 0}$). $n$ and $m$ are the number of rows and columns of the breadboard respectively. <span class="tex-font-style-it">In this version $q$ is always zero, and is only present for consistency with the harder version.</span></p><p>The next four lines describe initial coloring of the ports. Each character in these lines is either <span class="tex-font-style-tt">R</span> or <span class="tex-font-style-tt">B</span>, depending on the coloring of the respective port. The first two of these lines contain $n$ characters each, and describe ports on the left and right sides respectively from top to bottom. The last two lines contain $m$ characters each, and describe ports on the top and bottom sides respectively from left to right.</p>

## Output

<p>Print a single integer&nbsp;— the given breadboard capacity.</p>





```input1
4 5 0
BBRR
RBBR
BBBBB
RRRRR
```




```output1
7
```


