## Description

<div><p>You are given an array of <span class="tex-span"><i>n</i></span> integer numbers. Let <span class="tex-span"><i>sum</i>(<i>l</i>, <i>r</i>)</span> be the sum of all numbers on positions from <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span> non-inclusive (<span class="tex-span"><i>l</i></span>-th element is counted, <span class="tex-span"><i>r</i></span>-th element is not counted). For indices <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> holds <span class="tex-span">0 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>. Indices in array are numbered from <span class="tex-span">0</span>. </p><p>For example, if <span class="tex-span"><i>a</i> = [ - 5, 3, 9, 4]</span>, then <span class="tex-span"><i>sum</i>(0, 1) =  - 5</span>, <span class="tex-span"><i>sum</i>(0, 2) =  - 2</span>, <span class="tex-span"><i>sum</i>(1, 4) = 16</span> and <span class="tex-span"><i>sum</i>(<i>i</i>, <i>i</i>) = 0</span> for each <span class="tex-span"><i>i</i></span> from <span class="tex-span">0</span> to <span class="tex-span">4</span>.</p><p>Choose the indices of three delimiters <span class="tex-span"><i>delim</i><sub class="lower-index">0</sub></span>, <span class="tex-span"><i>delim</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>delim</i><sub class="lower-index">2</sub></span> (<span class="tex-span">0 ≤ <i>delim</i><sub class="lower-index">0</sub> ≤ <i>delim</i><sub class="lower-index">1</sub> ≤ <i>delim</i><sub class="lower-index">2</sub> ≤ <i>n</i></span>) and divide the array in such a way that the value of <span class="tex-span"><i>res</i> = <i>sum</i>(0, <i>delim</i><sub class="lower-index">0</sub>)</span> - <span class="tex-span"><i>sum</i>(<i>delim</i><sub class="lower-index">0</sub>, <i>delim</i><sub class="lower-index">1</sub>)</span> + <span class="tex-span"><i>sum</i>(<i>delim</i><sub class="lower-index">1</sub>, <i>delim</i><sub class="lower-index">2</sub>)</span> - <span class="tex-span"><i>sum</i>(<i>delim</i><sub class="lower-index">2</sub>, <i>n</i>)</span> is maximal. </p><p>Note that some of the expressions <span class="tex-span"><i>sum</i>(<i>l</i>, <i>r</i>)</span> can correspond to empty segments (if <span class="tex-span"><i>l</i> = <i>r</i></span> for some segment).</p></div><div class="input-specification"><p>The first line contains one integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>a</i><sub class="lower-index">0</sub>, <i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i> - 1</sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Choose three indices so that the value of <span class="tex-span"><i>res</i></span> is maximal. If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line contains one integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>a</i><sub class="lower-index">0</sub>, <i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i> - 1</sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Choose three indices so that the value of <span class="tex-span"><i>res</i></span> is maximal. If there are multiple answers, print any of them.</p>





```input1
3
-1 2 3

```




```input2
4
0 0 -1 0

```




```input3
1
10000

```




```output1
0 1 3

```




```output2
0 0 0

```




```output3
1 1 1

```


