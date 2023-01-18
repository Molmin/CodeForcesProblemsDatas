## Description

<div><p>A super computer has been built in the Turtle Academy of Sciences. The computer consists of <span class="tex-span"><i>n</i>·<i>m</i>·<i>k</i></span> CPUs. The architecture was the paralellepiped of size <span class="tex-span"><i>n</i> × <i>m</i> × <i>k</i></span>, split into <span class="tex-span">1 × 1 × 1</span> cells, each cell contains exactly one CPU. Thus, each CPU can be simultaneously identified as a group of three numbers from the layer number from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, the line number from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> and the column number from <span class="tex-span">1</span> to <span class="tex-span"><i>k</i></span>.</p><p>In the process of the Super Computer's work the CPUs can send each other messages by the famous turtle scheme: CPU <span class="tex-span">(<i>x</i>, <i>y</i>, <i>z</i>)</span> can send messages to CPUs <span class="tex-span">(<i>x</i> + 1, <i>y</i>, <i>z</i>)</span>, <span class="tex-span">(<i>x</i>, <i>y</i> + 1, <i>z</i>)</span> and <span class="tex-span">(<i>x</i>, <i>y</i>, <i>z</i> + 1)</span> (of course, if they exist), there is no feedback, that is, CPUs <span class="tex-span">(<i>x</i> + 1, <i>y</i>, <i>z</i>)</span>, <span class="tex-span">(<i>x</i>, <i>y</i> + 1, <i>z</i>)</span> and <span class="tex-span">(<i>x</i>, <i>y</i>, <i>z</i> + 1)</span> cannot send messages to CPU <span class="tex-span">(<i>x</i>, <i>y</i>, <i>z</i>)</span>.</p><p>Over time some CPUs broke down and stopped working. Such CPUs cannot send messages, receive messages or serve as intermediates in transmitting messages. We will say that CPU <span class="tex-span">(<i>a</i>, <i>b</i>, <i>c</i>)</span> <span class="tex-font-style-it">controls</span> CPU <span class="tex-span">(<i>d</i>, <i>e</i>, <i>f</i>)</span> , if there is a chain of CPUs <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>, <i>z</i><sub class="lower-index"><i>i</i></sub>)</span>, such that <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub> = <i>a</i>, <i>y</i><sub class="lower-index">1</sub> = <i>b</i>, <i>z</i><sub class="lower-index">1</sub> = <i>c</i>)</span>, <span class="tex-span">(<i>x</i><sub class="lower-index"><i>p</i></sub> = <i>d</i>, <i>y</i><sub class="lower-index"><i>p</i></sub> = <i>e</i>, <i>z</i><sub class="lower-index"><i>p</i></sub> = <i>f</i>)</span> (here and below <span class="tex-span"><i>p</i></span> is the length of the chain) and the CPU in the chain with number <span class="tex-span"><i>i</i></span> (<span class="tex-span"><i>i</i> &lt; <i>p</i></span>) can send messages to CPU <span class="tex-span"><i>i</i> + 1</span>.</p><p>Turtles are quite concerned about the denial-proofness of the system of communication between the remaining CPUs. For that they want to know the number of critical CPUs. A CPU <span class="tex-span">(<i>x</i>, <i>y</i>, <i>z</i>)</span> is <span class="tex-font-style-it">critical</span>, if turning it off will disrupt some control, that is, if there are two distinctive from <span class="tex-span">(<i>x</i>, <i>y</i>, <i>z</i>)</span> CPUs: <span class="tex-span">(<i>a</i>, <i>b</i>, <i>c</i>)</span> and <span class="tex-span">(<i>d</i>, <i>e</i>, <i>f</i>)</span>, such that <span class="tex-span">(<i>a</i>, <i>b</i>, <i>c</i>)</span> controls <span class="tex-span">(<i>d</i>, <i>e</i>, <i>f</i>)</span> before <span class="tex-span">(<i>x</i>, <i>y</i>, <i>z</i>)</span> is turned off and stopped controlling it after the turning off.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i>, <i>k</i> ≤ 100</span>)&nbsp;— the dimensions of the Super Computer. </p><p>Then <span class="tex-span"><i>n</i></span> blocks follow, describing the current state of the processes. The blocks correspond to the layers of the Super Computer in the order from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Each block consists of <span class="tex-span"><i>m</i></span> lines, <span class="tex-span"><i>k</i></span> characters in each — the description of a layer in the format of an <span class="tex-span"><i>m</i> × <i>k</i></span> table. Thus, the state of the CPU <span class="tex-span">(<i>x</i>, <i>y</i>, <i>z</i>)</span> is corresponded to the <span class="tex-span"><i>z</i></span>-th character of the <span class="tex-span"><i>y</i></span>-th line of the block number <span class="tex-span"><i>x</i></span>. Character "<span class="tex-font-style-tt">1</span>" corresponds to a working CPU and character "<span class="tex-font-style-tt">0</span>" corresponds to a malfunctioning one. The blocks are separated by exactly one empty line.</p></div><div class="output-specification"><p>Print a single integer — the number of critical CPUs, that is, such that turning only this CPU off will disrupt some control.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i>, <i>k</i> ≤ 100</span>)&nbsp;— the dimensions of the Super Computer. </p><p>Then <span class="tex-span"><i>n</i></span> blocks follow, describing the current state of the processes. The blocks correspond to the layers of the Super Computer in the order from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Each block consists of <span class="tex-span"><i>m</i></span> lines, <span class="tex-span"><i>k</i></span> characters in each — the description of a layer in the format of an <span class="tex-span"><i>m</i> × <i>k</i></span> table. Thus, the state of the CPU <span class="tex-span">(<i>x</i>, <i>y</i>, <i>z</i>)</span> is corresponded to the <span class="tex-span"><i>z</i></span>-th character of the <span class="tex-span"><i>y</i></span>-th line of the block number <span class="tex-span"><i>x</i></span>. Character "<span class="tex-font-style-tt">1</span>" corresponds to a working CPU and character "<span class="tex-font-style-tt">0</span>" corresponds to a malfunctioning one. The blocks are separated by exactly one empty line.</p>

## Output

<p>Print a single integer — the number of critical CPUs, that is, such that turning only this CPU off will disrupt some control.</p>





```input1
2 2 3
000
000

111
111

```




```input2
3 3 3
111
111
111

111
111
111

111
111
111

```




```input3
1 1 10
0101010101

```




```output1
2

```




```output2
19

```




```output3
0

```



## Note

<p>In the first sample the whole first layer of CPUs is malfunctional. In the second layer when CPU <span class="tex-span">(2, 1, 2)</span> turns off, it disrupts the control by CPU <span class="tex-span">(2, 1, 3)</span> over CPU <span class="tex-span">(2, 1, 1)</span>, and when CPU <span class="tex-span">(2, 2, 2)</span> is turned off, it disrupts the control over CPU <span class="tex-span">(2, 2, 3)</span> by CPU <span class="tex-span">(2, 2, 1)</span>.</p><p>In the second sample all processors except for the corner ones are critical.</p><p>In the third sample there is not a single processor controlling another processor, so the answer is <span class="tex-span">0</span>.</p>
