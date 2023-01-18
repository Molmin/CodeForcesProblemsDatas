## Description

<div><p>The Elements of Harmony are six supernatural artifacts representing subjective aspects of harmony. They are arguably the most powerful force in Equestria. The inside of Elements of Harmony can be seen as a complete graph with <span class="tex-span"><i>n</i></span> vertices labeled from 0 to <span class="tex-span"><i>n</i> - 1</span>, where <span class="tex-span"><i>n</i></span> is a power of two, equal to <span class="tex-span">2<sup class="upper-index"><i>m</i></sup></span>.</p><center> <img class="tex-graphics" src="file://OobINk16.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The energy in Elements of Harmony is in constant movement. According to the ancient book, the energy of vertex <span class="tex-span"><i>u</i></span> in time <span class="tex-span"><i>i</i></span> <span class="tex-span">(<i>e</i><sub class="lower-index"><i>i</i></sub>[<i>u</i>])</span> equals to: </p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://ijXuqrue.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>Here <span class="tex-span"><i>b</i>[]</span> is the transformation coefficient — an array of <span class="tex-span"><i>m</i> + 1</span> integers and <span class="tex-span"><i>f</i>(<i>u</i>, <i>v</i>)</span> is the number of ones in the binary representation of number <span class="tex-span">(<i>u</i>&nbsp;<i>xor</i>&nbsp;<i>v</i>)</span>.</p><p>Given the transformation coefficient and the energy distribution at time 0 <span class="tex-span">(<i>e</i><sub class="lower-index">0</sub>[])</span>. Help Twilight Sparkle predict the energy distribution at time <span class="tex-span"><i>t</i></span> <span class="tex-span">(<i>e</i><sub class="lower-index"><i>t</i></sub>[])</span>. The answer can be quite large, so output it modulo <span class="tex-span"><i>p</i></span>.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>t</i></span> and <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 20;&nbsp;0 ≤ <i>t</i> ≤ 10<sup class="upper-index">18</sup>;&nbsp;2 ≤ <i>p</i> ≤ 10<sup class="upper-index">9</sup></span>). The following line contains <span class="tex-span"><i>n</i></span> (<span class="tex-span"><i>n</i> = 2<sup class="upper-index"><i>m</i></sup></span>) integers <span class="tex-span"><i>e</i><sub class="lower-index">0</sub>[<i>i</i>]</span> (<span class="tex-span">1 ≤ <i>e</i><sub class="lower-index">0</sub>[<i>i</i>] ≤ 10<sup class="upper-index">9</sup>;&nbsp;0 ≤ <i>i</i> &lt; <i>n</i></span>). The next line contains <span class="tex-span"><i>m</i> + 1</span> integers <span class="tex-span"><i>b</i>[<i>i</i>]</span> (<span class="tex-span">0 ≤ <i>b</i>[<i>i</i>] ≤ 10<sup class="upper-index">9</sup>;&nbsp;0 ≤ <i>i</i> ≤ <i>m</i></span>).</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>n</i></span> lines, the <span class="tex-span"><i>i</i></span>-th line must contain a single integer <span class="tex-span"><i>e</i><sub class="lower-index"><i>t</i></sub>[<i>i</i>]</span> modulo <span class="tex-span"><i>p</i></span>.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>t</i></span> and <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 20;&nbsp;0 ≤ <i>t</i> ≤ 10<sup class="upper-index">18</sup>;&nbsp;2 ≤ <i>p</i> ≤ 10<sup class="upper-index">9</sup></span>). The following line contains <span class="tex-span"><i>n</i></span> (<span class="tex-span"><i>n</i> = 2<sup class="upper-index"><i>m</i></sup></span>) integers <span class="tex-span"><i>e</i><sub class="lower-index">0</sub>[<i>i</i>]</span> (<span class="tex-span">1 ≤ <i>e</i><sub class="lower-index">0</sub>[<i>i</i>] ≤ 10<sup class="upper-index">9</sup>;&nbsp;0 ≤ <i>i</i> &lt; <i>n</i></span>). The next line contains <span class="tex-span"><i>m</i> + 1</span> integers <span class="tex-span"><i>b</i>[<i>i</i>]</span> (<span class="tex-span">0 ≤ <i>b</i>[<i>i</i>] ≤ 10<sup class="upper-index">9</sup>;&nbsp;0 ≤ <i>i</i> ≤ <i>m</i></span>).</p>

## Output

<p>Output <span class="tex-span"><i>n</i></span> lines, the <span class="tex-span"><i>i</i></span>-th line must contain a single integer <span class="tex-span"><i>e</i><sub class="lower-index"><i>t</i></sub>[<i>i</i>]</span> modulo <span class="tex-span"><i>p</i></span>.</p>





```input1
2 2 10000
4 1 2 3
0 1 0

```




```output1
14
6
6
14

```


