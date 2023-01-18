## Description

<div><p>Little Chris is having a nightmare. Even in dreams all he thinks about is math.</p><p>Chris dreams about <span class="tex-span"><i>m</i></span> binary strings of length <span class="tex-span"><i>n</i></span>, indexed with numbers from 1 to <span class="tex-span"><i>m</i></span>. The most horrifying part is that the bits of each string are ordered in either ascending or descending order. For example, Chris could be dreaming about the following 4 strings of length 5:</p><center> <img class="tex-graphics" src="file://Cgf8BpMP.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The <span class="tex-font-style-underline">Hamming distance</span> <span class="tex-span"><i>H</i>(<i>a</i>, <i>b</i>)</span> between two strings <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> of length <span class="tex-span"><i>n</i></span> is the number of positions at which the corresponding symbols are different. </p><p>Сhris thinks that each three strings with different indices constitute a single triple. Chris's delusion is that he will wake up only if he counts the number of such string triples <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span> that the sum <span class="tex-span"><i>H</i>(<i>a</i>, <i>b</i>) + <i>H</i>(<i>b</i>, <i>c</i>) + <i>H</i>(<i>c</i>, <i>a</i>)</span> is maximal among all the string triples constructed from the dreamed strings.</p><p>Help Chris wake up from this nightmare!</p></div><div class="input-specification"><p>The first line of input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>; <span class="tex-span">3 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>), the length and the number of strings. The next <span class="tex-span"><i>m</i></span> lines contain the description of the strings. The <span class="tex-span"><i>i</i></span>-th line contains two space-separated integers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 1</span>; <span class="tex-span">1 ≤ <i>f</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), the description of the string with index <span class="tex-span"><i>i</i></span>; that means that the first <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span> bits of the <span class="tex-span"><i>i</i></span>-th string are equal to <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>, and the remaining <span class="tex-span"><i>n</i> - <i>f</i><sub class="lower-index"><i>i</i></sub></span> bits are equal to <span class="tex-span">1 - <i>s</i><sub class="lower-index"><i>i</i></sub></span>. There can be multiple equal strings in Chris's dream.</p></div><div class="output-specification"><p>Output a single integer, the number of such string triples among the given that the sum of the Hamming distances between the strings of the triple is maximal.</p></div>

## Input

<p>The first line of input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>; <span class="tex-span">3 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>), the length and the number of strings. The next <span class="tex-span"><i>m</i></span> lines contain the description of the strings. The <span class="tex-span"><i>i</i></span>-th line contains two space-separated integers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 1</span>; <span class="tex-span">1 ≤ <i>f</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), the description of the string with index <span class="tex-span"><i>i</i></span>; that means that the first <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span> bits of the <span class="tex-span"><i>i</i></span>-th string are equal to <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>, and the remaining <span class="tex-span"><i>n</i> - <i>f</i><sub class="lower-index"><i>i</i></sub></span> bits are equal to <span class="tex-span">1 - <i>s</i><sub class="lower-index"><i>i</i></sub></span>. There can be multiple equal strings in Chris's dream.</p>

## Output

<p>Output a single integer, the number of such string triples among the given that the sum of the Hamming distances between the strings of the triple is maximal.</p>





```input1
5 4
0 3
0 5
1 4
1 5

```




```input2
10 4
1 5
0 5
0 5
1 5

```




```output1
3

```




```output2
4

```


