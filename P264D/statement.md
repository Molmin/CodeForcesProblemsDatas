## Description

<div><p>There are two sequences of colorful stones. The color of each stone is one of red, green, or blue. You are given two strings <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span>. The <span class="tex-span"><i>i</i></span>-th (1-based) character of <span class="tex-span"><i>s</i></span> represents the color of the <span class="tex-span"><i>i</i></span>-th stone of the first sequence. Similarly, the <span class="tex-span"><i>i</i></span>-th (1-based) character of <span class="tex-span"><i>t</i></span> represents the color of the <span class="tex-span"><i>i</i></span>-th stone of the second sequence. If the character is "<span class="tex-font-style-tt">R</span>", "<span class="tex-font-style-tt">G</span>", or "<span class="tex-font-style-tt">B</span>", the color of the corresponding stone is red, green, or blue, respectively.</p><p>Initially Squirrel Liss is standing on the first stone of the first sequence and Cat Vasya is standing on the first stone of the second sequence. You can perform the following instructions zero or more times.</p><p>Each instruction is one of the three types: "<span class="tex-font-style-tt">RED</span>", "<span class="tex-font-style-tt">GREEN</span>", or "<span class="tex-font-style-tt">BLUE</span>". After an instruction <span class="tex-span"><i>c</i></span>, the animals standing on stones whose colors are <span class="tex-span"><i>c</i></span> will move one stone forward. For example, if you perform an instruction «<span class="tex-font-style-tt">RED</span>», the animals standing on red stones will move one stone forward. You are not allowed to perform instructions that lead some animals out of the sequences. In other words, if some animals are standing on the last stones, you can't perform the instructions of the colors of those stones.</p><p>A pair of positions (position of Liss, position of Vasya) is called a state. A state is called <span class="tex-font-style-it">reachable</span> if the state is reachable by performing instructions zero or more times from the initial state (1, 1). Calculate the number of distinct reachable states.</p></div><div class="input-specification"><p>The input contains two lines. The first line contains the string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 10<sup class="upper-index">6</sup></span>). The second line contains the string <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ |<i>t</i>| ≤ 10<sup class="upper-index">6</sup></span>). The characters of each string will be one of "<span class="tex-font-style-tt">R</span>", "<span class="tex-font-style-tt">G</span>", or "<span class="tex-font-style-tt">B</span>".</p></div><div class="output-specification"><p>Print the number of distinct reachable states in a single line.</p><p>Please, do not write the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The input contains two lines. The first line contains the string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 10<sup class="upper-index">6</sup></span>). The second line contains the string <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ |<i>t</i>| ≤ 10<sup class="upper-index">6</sup></span>). The characters of each string will be one of "<span class="tex-font-style-tt">R</span>", "<span class="tex-font-style-tt">G</span>", or "<span class="tex-font-style-tt">B</span>".</p>

## Output

<p>Print the number of distinct reachable states in a single line.</p><p>Please, do not write the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
RBR
RGG

```




```input2
RGBB
BRRBRR

```




```input3
RRRRRRRRRR
RRRRRRRR

```




```output1
5

```




```output2
19

```




```output3
8

```



## Note

<p>In the first example, there are five reachable states: (1, 1), (2, 2), (2, 3), (3, 2), and (3, 3). For example, the state (3, 3) is reachable because if you perform instructions "<span class="tex-font-style-tt">RED</span>", "<span class="tex-font-style-tt">GREEN</span>", and "<span class="tex-font-style-tt">BLUE</span>" in this order from the initial state, the state will be (3, 3). The following picture shows how the instructions work in this case.</p><center> <img class="tex-graphics" src="file://LOM07TrP.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
