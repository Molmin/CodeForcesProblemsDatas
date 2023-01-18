## Description

<div><p>Ivan has a robot which is situated on an infinite grid. Initially the robot is standing in the starting cell <span class="tex-span">(0, 0)</span>. The robot can process commands. There are four types of commands it can perform:</p><ul> <li> <span class="tex-font-style-tt">U</span> — move from the cell <span class="tex-span">(<i>x</i>, <i>y</i>)</span> to <span class="tex-span">(<i>x</i>, <i>y</i> + 1)</span>; </li><li> <span class="tex-font-style-tt">D</span> — move from <span class="tex-span">(<i>x</i>, <i>y</i>)</span> to <span class="tex-span">(<i>x</i>, <i>y</i> - 1)</span>; </li><li> <span class="tex-font-style-tt">L</span> — move from <span class="tex-span">(<i>x</i>, <i>y</i>)</span> to <span class="tex-span">(<i>x</i> - 1, <i>y</i>)</span>; </li><li> <span class="tex-font-style-tt">R</span> — move from <span class="tex-span">(<i>x</i>, <i>y</i>)</span> to <span class="tex-span">(<i>x</i> + 1, <i>y</i>)</span>. </li></ul><p>Ivan entered a sequence of <span class="tex-span"><i>n</i></span> commands, and the robot processed it. After this sequence the robot ended up in the starting cell <span class="tex-span">(0, 0)</span>, but Ivan doubts that the sequence is such that after performing it correctly the robot ends up in the same cell. He thinks that some commands were ignored by robot. To acknowledge whether the robot is severely bugged, he needs to calculate the maximum possible number of commands that were performed correctly. Help Ivan to do the calculations!</p></div><div class="input-specification"><p>The first line contains one number <span class="tex-span"><i>n</i></span> — the length of sequence of commands entered by Ivan (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>).</p><p>The second line contains the sequence itself — a string consisting of <span class="tex-span"><i>n</i></span> characters. Each character can be <span class="tex-font-style-tt">U</span>, <span class="tex-font-style-tt">D</span>, <span class="tex-font-style-tt">L</span> or <span class="tex-font-style-tt">R</span>.</p></div><div class="output-specification"><p>Print the maximum possible number of commands from the sequence the robot could perform to end up in the starting cell.</p></div>

## Input

<p>The first line contains one number <span class="tex-span"><i>n</i></span> — the length of sequence of commands entered by Ivan (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>).</p><p>The second line contains the sequence itself — a string consisting of <span class="tex-span"><i>n</i></span> characters. Each character can be <span class="tex-font-style-tt">U</span>, <span class="tex-font-style-tt">D</span>, <span class="tex-font-style-tt">L</span> or <span class="tex-font-style-tt">R</span>.</p>

## Output

<p>Print the maximum possible number of commands from the sequence the robot could perform to end up in the starting cell.</p>





```input1
4
LDUR

```




```input2
5
RRRUU

```




```input3
6
LLRRRR

```




```output1
4

```




```output2
0

```




```output3
4

```


