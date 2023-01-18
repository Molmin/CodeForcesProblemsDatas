## Description

<div><div class="epigraph"><div class="epigraph-text"><span class="tex-font-style-it">Are you going to Scarborough Fair?<p>Parsley, sage, rosemary and thyme.</p><p>Remember me to one who lives there.</p><p>He once was the true love of mine.</p></span></div></div><p>Willem is taking the girl to the highest building in island No.28, however, neither of them knows how to get there.</p><p>Willem asks his friend, Grick for directions, Grick helped them, and gave them a task.</p><p>Although the girl wants to help, Willem insists on doing it by himself.</p><p>Grick gave Willem a string of length <span class="tex-span"><i>n</i></span>.</p><p>Willem needs to do <span class="tex-span"><i>m</i></span> operations, each operation has four parameters <span class="tex-span"><i>l</i>, <i>r</i>, <i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub></span>, which means that all symbols <span class="tex-span"><i>c</i><sub class="lower-index">1</sub></span> in range <span class="tex-span">[<i>l</i>, <i>r</i>]</span> (from <span class="tex-span"><i>l</i></span>-th to <span class="tex-span"><i>r</i></span>-th, including <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span>) are changed into <span class="tex-span"><i>c</i><sub class="lower-index">2</sub></span>. String is 1-indexed.</p><p>Grick wants to know the final string after all the <span class="tex-span"><i>m</i></span> operations.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 100)</span>.</p><p>The second line contains a string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span>, consisting of lowercase English letters.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains four parameters <span class="tex-span"><i>l</i>, <i>r</i>, <i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>, <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub></span> are lowercase English letters), separated by space.</p></div><div class="output-specification"><p>Output string <span class="tex-span"><i>s</i></span> after performing <span class="tex-span"><i>m</i></span> operations described above.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 100)</span>.</p><p>The second line contains a string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span>, consisting of lowercase English letters.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains four parameters <span class="tex-span"><i>l</i>, <i>r</i>, <i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>, <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub></span> are lowercase English letters), separated by space.</p>

## Output

<p>Output string <span class="tex-span"><i>s</i></span> after performing <span class="tex-span"><i>m</i></span> operations described above.</p>





```input1
3 1
ioi
1 1 i n

```




```input2
5 3
wxhak
3 3 h x
1 5 x a
1 3 w g

```




```output1
noi
```




```output2
gaaak
```



## Note

<p>For the second example:</p><p>After the first operation, the string is <span class="tex-font-style-tt">wxxak</span>.</p><p>After the second operation, the string is <span class="tex-font-style-tt">waaak</span>.</p><p>After the third operation, the string is <span class="tex-font-style-tt">gaaak</span>.</p>
