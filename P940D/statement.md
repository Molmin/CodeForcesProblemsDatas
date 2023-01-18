## Description

<div><p><span class="tex-font-style-it">"We've tried solitary confinement, waterboarding and listening to Just In Beaver, to no avail. We need something extreme."</span></p><p><span class="tex-font-style-it">"Little Alena got an array as a birthday present<span class="tex-span">...</span>"</span></p><p>The array <span class="tex-span"><i>b</i></span> of length <span class="tex-span"><i>n</i></span> is obtained from the array <span class="tex-span"><i>a</i></span> of length <span class="tex-span"><i>n</i></span> and two integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span>&nbsp;(<span class="tex-span"><i>l</i> ≤ <i>r</i></span>) using the following procedure:</p><p><span class="tex-span"><i>b</i><sub class="lower-index">1</sub> = <i>b</i><sub class="lower-index">2</sub> = <i>b</i><sub class="lower-index">3</sub> = <i>b</i><sub class="lower-index">4</sub> = 0</span>.</p><p>For all <span class="tex-span">5 ≤ <i>i</i> ≤ <i>n</i></span>: </p><ul> <li> <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> = 0</span> if <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>a</i><sub class="lower-index"><i>i</i> - 1</sub>, <i>a</i><sub class="lower-index"><i>i</i> - 2</sub>, <i>a</i><sub class="lower-index"><i>i</i> - 3</sub>, <i>a</i><sub class="lower-index"><i>i</i> - 4</sub> &gt; <i>r</i></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i> - 1</sub> = <i>b</i><sub class="lower-index"><i>i</i> - 2</sub> = <i>b</i><sub class="lower-index"><i>i</i> - 3</sub> = <i>b</i><sub class="lower-index"><i>i</i> - 4</sub> = 1</span> </li><li> <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> = 1</span> if <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>a</i><sub class="lower-index"><i>i</i> - 1</sub>, <i>a</i><sub class="lower-index"><i>i</i> - 2</sub>, <i>a</i><sub class="lower-index"><i>i</i> - 3</sub>, <i>a</i><sub class="lower-index"><i>i</i> - 4</sub> &lt; <i>l</i></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i> - 1</sub> = <i>b</i><sub class="lower-index"><i>i</i> - 2</sub> = <i>b</i><sub class="lower-index"><i>i</i> - 3</sub> = <i>b</i><sub class="lower-index"><i>i</i> - 4</sub> = 0</span> </li><li> <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> = <i>b</i><sub class="lower-index"><i>i</i> - 1</sub></span> otherwise </li></ul><p>You are given arrays <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i>'</span> of the same length. Find two integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span>&nbsp;(<span class="tex-span"><i>l</i> ≤ <i>r</i></span>), such that applying the algorithm described above will yield an array <span class="tex-span"><i>b</i></span> equal to <span class="tex-span"><i>b</i>'</span>.</p><p>It's guaranteed that the answer exists.</p></div><div class="input-specification"><p>The first line of input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">5 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the length of <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i>'</span>.</p><p>The second line of input contains <span class="tex-span"><i>n</i></span> space separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the elements of <span class="tex-span"><i>a</i></span>.</p><p>The third line of input contains a string of <span class="tex-span"><i>n</i></span> characters, consisting of <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>&nbsp;— the elements of <span class="tex-span"><i>b</i>'</span>. Note that they are not separated by spaces.</p></div><div class="output-specification"><p>Output two integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span>&nbsp;(<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">9</sup></span>), conforming to the requirements described above.</p><p>If there are multiple solutions, output any of them.</p><p>It's guaranteed that the answer exists.</p></div>

## Input

<p>The first line of input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">5 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the length of <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i>'</span>.</p><p>The second line of input contains <span class="tex-span"><i>n</i></span> space separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the elements of <span class="tex-span"><i>a</i></span>.</p><p>The third line of input contains a string of <span class="tex-span"><i>n</i></span> characters, consisting of <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>&nbsp;— the elements of <span class="tex-span"><i>b</i>'</span>. Note that they are not separated by spaces.</p>

## Output

<p>Output two integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span>&nbsp;(<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">9</sup></span>), conforming to the requirements described above.</p><p>If there are multiple solutions, output any of them.</p><p>It's guaranteed that the answer exists.</p>





```input1
5
1 2 3 4 5
00001

```




```input2
10
-10 -9 -8 -7 -6 6 7 8 9 10
0000111110

```




```output1
6 15

```




```output2
-5 5

```



## Note

<p>In the first test case any pair of <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> pair is valid, if <span class="tex-span">6 ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">9</sup></span>, in that case <span class="tex-span"><i>b</i><sub class="lower-index">5</sub> = 1</span>, because <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index">5</sub> &lt; <i>l</i></span>.</p>
