## Description

<div><p>You're given a matrix <span class="tex-span"><i>A</i></span> of size <span class="tex-span"><i>n</i> × <i>n</i></span>.</p><p>Let's call the matrix with nonnegative elements magic if it is symmetric (so <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub> = <i>a</i><sub class="lower-index"><i>ji</i></sub></span>), <span class="tex-span"><i>a</i><sub class="lower-index"><i>ii</i></sub> = 0</span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub> ≤ <i>max</i>(<i>a</i><sub class="lower-index"><i>ik</i></sub>, <i>a</i><sub class="lower-index"><i>jk</i></sub>)</span> for all triples <span class="tex-span"><i>i</i>, <i>j</i>, <i>k</i></span>. Note that <span class="tex-span"><i>i</i>, <i>j</i>, <i>k</i></span> do not need to be distinct.</p><p>Determine if the matrix is magic.</p><p>As the input/output can reach very huge size it is recommended to use fast input/output methods: for example, prefer to use <span class="tex-font-style-tt">scanf/printf</span> instead of <span class="tex-font-style-tt">cin/cout</span> in C++, prefer to use <span class="tex-font-style-tt">BufferedReader/PrintWriter</span> instead of <span class="tex-font-style-tt">Scanner/System.out</span> in <span class="tex-font-style-tt">Java</span>.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2500</span>) — the size of the matrix <span class="tex-span"><i>A</i></span>.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>ij</i></sub> &lt; 10<sup class="upper-index">9</sup></span>) — the elements of the matrix <span class="tex-span"><i>A</i></span>.</p><p>Note that the given matrix not necessarily is symmetric and can be arbitrary.</p></div><div class="output-specification"><p>Print ''<span class="tex-font-style-tt">MAGIC</span>" (without quotes) if the given matrix <span class="tex-span"><i>A</i></span> is magic. Otherwise print ''<span class="tex-font-style-tt">NOT MAGIC</span>".</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2500</span>) — the size of the matrix <span class="tex-span"><i>A</i></span>.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>ij</i></sub> &lt; 10<sup class="upper-index">9</sup></span>) — the elements of the matrix <span class="tex-span"><i>A</i></span>.</p><p>Note that the given matrix not necessarily is symmetric and can be arbitrary.</p>

## Output

<p>Print ''<span class="tex-font-style-tt">MAGIC</span>" (without quotes) if the given matrix <span class="tex-span"><i>A</i></span> is magic. Otherwise print ''<span class="tex-font-style-tt">NOT MAGIC</span>".</p>





```input1
3
0 1 2
1 0 2
2 2 0

```




```input2
2
0 1
2 3

```




```input3
4
0 1 2 3
1 0 3 4
2 3 0 5
3 4 5 0

```




```output1
MAGIC

```




```output2
NOT MAGIC

```




```output3
NOT MAGIC

```


