## Description

<div><p>For some experiments little Petya needs a synchrophasotron. He has already got the device, all that's left is to set the fuel supply. Fuel comes through a system of nodes numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> and connected by pipes. Pipes go from every node with smaller number to every node with greater number. Fuel can only flow through pipes in direction from node with smaller number to node with greater number. Any amount of fuel can enter through the first node and the last node is connected directly to the synchrophasotron. It is known that every pipe has three attributes: the minimum amount of fuel that should go through it, the maximum amount of fuel that can possibly go through it and the cost of pipe activation. If <span class="tex-span"><i>c</i><sub class="lower-index"><i>ij</i></sub></span> units of fuel (<span class="tex-span"><i>c</i><sub class="lower-index"><i>ij</i></sub> &gt; 0</span>) flow from node <span class="tex-span"><i>i</i></span> to node <span class="tex-span"><i>j</i></span>, it will cost <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub> + <i>c</i><sub class="lower-index"><i>ij</i></sub><sup class="upper-index">2</sup></span> tugriks (<span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> is the cost of pipe activation), and if fuel doesn't flow through the pipe, it doesn't cost anything. Only integer number of units of fuel can flow through each pipe.</p><p>Constraints on the minimal and the maximal fuel capacity of a pipe take place <span class="tex-font-style-bf">always</span>, not only if it is active. You may assume that the pipe is active if and only if the flow through it is strictly greater than zero.</p><p>Petya doesn't want the pipe system to be overloaded, so he wants to find the minimal amount of fuel, that, having entered the first node, can reach the synchrophasotron. Besides that he wants to impress the sponsors, so the sum of money needed to be paid for fuel to go through each pipe, must be as big as possible.</p></div><div class="input-specification"><p>First line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 6</span>), which represents the number of nodes. Each of the next <span class="tex-span"><i>n</i>(<i>n</i> - 1) / 2</span> lines contains five integers <span class="tex-span"><i>s</i>, <i>f</i>, <i>l</i>, <i>h</i>, <i>a</i></span> that describe pipes — the first node of the pipe, the second node of the pipe, the minimum and the maximum amount of fuel that can flow through the pipe and the the activation cost, respectively. (<span class="tex-span">1 ≤ <i>s</i> &lt; <i>f</i> ≤ <i>n</i>, 0 ≤ <i>l</i> ≤ <i>h</i> ≤ 5, 0 ≤ <i>a</i> ≤ 6</span>). It is guaranteed that for each pair of nodes with distinct numbers there will be exactly one pipe between them described in the input.</p></div><div class="output-specification"><p>Output in the first line two space-separated numbers: the minimum possible amount of fuel that can flow into the synchrophasotron, and the maximum possible sum that needs to be paid in order for that amount of fuel to reach synchrophasotron. If there is no amount of fuel that can reach synchrophasotron, output "<span class="tex-font-style-tt">-1 -1</span>".</p><p>The amount of fuel which will flow into synchrophasotron is not neccessary positive. It could be equal to zero if the minimum constraint of every pipe is equal to zero.</p></div>

## Input

<p>First line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 6</span>), which represents the number of nodes. Each of the next <span class="tex-span"><i>n</i>(<i>n</i> - 1) / 2</span> lines contains five integers <span class="tex-span"><i>s</i>, <i>f</i>, <i>l</i>, <i>h</i>, <i>a</i></span> that describe pipes — the first node of the pipe, the second node of the pipe, the minimum and the maximum amount of fuel that can flow through the pipe and the the activation cost, respectively. (<span class="tex-span">1 ≤ <i>s</i> &lt; <i>f</i> ≤ <i>n</i>, 0 ≤ <i>l</i> ≤ <i>h</i> ≤ 5, 0 ≤ <i>a</i> ≤ 6</span>). It is guaranteed that for each pair of nodes with distinct numbers there will be exactly one pipe between them described in the input.</p>

## Output

<p>Output in the first line two space-separated numbers: the minimum possible amount of fuel that can flow into the synchrophasotron, and the maximum possible sum that needs to be paid in order for that amount of fuel to reach synchrophasotron. If there is no amount of fuel that can reach synchrophasotron, output "<span class="tex-font-style-tt">-1 -1</span>".</p><p>The amount of fuel which will flow into synchrophasotron is not neccessary positive. It could be equal to zero if the minimum constraint of every pipe is equal to zero.</p>





```input1
2
1 2 1 2 3

```




```input2
3
1 2 1 2 3
1 3 0 0 0
2 3 3 4 5

```




```input3
4
1 2 0 2 1
2 3 0 2 1
1 3 0 2 6
1 4 0 0 1
2 4 0 0 0
3 4 2 3 0

```




```input4
3
1 2 0 2 1
1 3 1 2 1
2 3 1 2 1

```




```output1
1 4

```




```output2
-1 -1

```




```output3
2 15

```




```output4
2 6

```



## Note

<p>In the first test, we can either pass 1 or 2 units of fuel from node 1 to node 2. The minimum possible amount is 1, it costs <span class="tex-span"><i>a</i><sub class="lower-index">12</sub> + 1<sup class="upper-index">2</sup> = 4</span>.</p><p>In the second test, you can pass at most 2 units from node 1 to node 2, and at you have to pass at least 3 units from node 2 to node 3. It is impossible.</p><p>In the third test, the minimum possible amount is 2. You can pass each unit of fuel through two different paths: either 1-&gt;2-&gt;3-&gt;4 or 1-&gt;3-&gt;4. If you use the first path twice, it will cost <span class="tex-span"><i>a</i><sub class="lower-index">12</sub> + 2<sup class="upper-index">2</sup> + <i>a</i><sub class="lower-index">23</sub> + 2<sup class="upper-index">2</sup> + <i>a</i><sub class="lower-index">34</sub> + 2<sup class="upper-index">2</sup></span>=14. If you use the second path twice, it will cost <span class="tex-span"><i>a</i><sub class="lower-index">13</sub> + 2<sup class="upper-index">2</sup> + <i>a</i><sub class="lower-index">34</sub> + 2<sup class="upper-index">2</sup></span>=14. However, if you use each path (allowing one unit of fuel go through pipes 1-&gt;2, 2-&gt;3, 1-&gt;3, and two units go through 3-&gt;4) it will cost <span class="tex-span"><i>a</i><sub class="lower-index">12</sub> + 1<sup class="upper-index">2</sup> + <i>a</i><sub class="lower-index">23</sub> + 1<sup class="upper-index">2</sup> + <i>a</i><sub class="lower-index">13</sub> + 1<sup class="upper-index">2</sup> + <i>a</i><sub class="lower-index">34</sub> + 2<sup class="upper-index">2</sup></span>=15 and it is the maximum possible cost.</p><p>Also note that since no fuel flows from node 1 to node 4, activation cost for that pipe is not added to the answer.</p>
