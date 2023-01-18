## Description

<div><p>Fox Ciel has a robot on a 2D plane. Initially it is located in (0, 0). Fox Ciel code a command to it. The command was represented by string <span class="tex-span"><i>s</i></span>. Each character of <span class="tex-span"><i>s</i></span> is one move operation. There are four move operations at all:</p><ul> <li> '<span class="tex-font-style-tt">U</span>': go up, (x, y) <span class="tex-span"> → </span> (x, y+1); </li><li> '<span class="tex-font-style-tt">D</span>': go down, (x, y) <span class="tex-span"> → </span> (x, y-1); </li><li> '<span class="tex-font-style-tt">L</span>': go left, (x, y) <span class="tex-span"> → </span> (x-1, y); </li><li> '<span class="tex-font-style-tt">R</span>': go right, (x, y) <span class="tex-span"> → </span> (x+1, y). </li></ul><p>The robot will do the operations in <span class="tex-span"><i>s</i></span> from left to right, and repeat it infinite times. Help Fox Ciel to determine if after some steps the robot will located in <span class="tex-span">(<i>a</i>, <i>b</i>)</span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>, (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">9</sup></span>). The second line contains a string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 100</span>, <span class="tex-span"><i>s</i></span> only contains characters '<span class="tex-font-style-tt">U</span>', '<span class="tex-font-style-tt">D</span>', '<span class="tex-font-style-tt">L</span>', '<span class="tex-font-style-tt">R</span>') — the command.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">Yes</span>" if the robot will be located at <span class="tex-span">(<i>a</i>, <i>b</i>)</span>, and "<span class="tex-font-style-tt">No</span>" otherwise.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>, (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">9</sup></span>). The second line contains a string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 100</span>, <span class="tex-span"><i>s</i></span> only contains characters '<span class="tex-font-style-tt">U</span>', '<span class="tex-font-style-tt">D</span>', '<span class="tex-font-style-tt">L</span>', '<span class="tex-font-style-tt">R</span>') — the command.</p>

## Output

<p>Print "<span class="tex-font-style-tt">Yes</span>" if the robot will be located at <span class="tex-span">(<i>a</i>, <i>b</i>)</span>, and "<span class="tex-font-style-tt">No</span>" otherwise.</p>





```input1
2 2
RU

```




```input2
1 2
RU

```




```input3
-1 1000000000
LRRLU

```




```input4
0 0
D

```




```output1
Yes

```




```output2
No

```




```output3
Yes

```




```output4
Yes

```



## Note

<p>In the first and second test case, command string is "<span class="tex-font-style-tt">RU</span>", so the robot will go right, then go up, then right, and then up and so on.</p><p>The locations of its moves are (0, 0) <span class="tex-span"> → </span> (1, 0) <span class="tex-span"> → </span> (1, 1) <span class="tex-span"> → </span> (2, 1) <span class="tex-span"> → </span> (2, 2) <span class="tex-span"> → </span> <span class="tex-span">...</span></p><p>So it can reach (2, 2) but not (1, 2).</p>
