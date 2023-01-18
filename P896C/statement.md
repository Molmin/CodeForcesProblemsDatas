## Description

<div><div class="epigraph"><div class="epigraph-text"><span class="tex-font-style-it"><p>— Willem...</p><p>— What's the matter?</p><p>— It seems that there's something wrong with Seniorious...</p><p>— I'll have a look...</p></span></div></div><center><p><img class="tex-graphics" src="file://zn6lZe6b.png" style="max-width: 100.0%;max-height: 100.0%;"></p></center><p>Seniorious is made by linking special talismans in particular order.</p><p>After over 500 years, the carillon is now in bad condition, so Willem decides to examine it thoroughly.</p><p>Seniorious has <span class="tex-span"><i>n</i></span> pieces of talisman. Willem puts them in a line, the <span class="tex-span"><i>i</i></span>-th of which is an integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>In order to maintain it, Willem needs to perform <span class="tex-span"><i>m</i></span> operations.</p><p>There are four types of operations:</p><ul><li> <span class="tex-span">1 <i>l</i> <i>r</i> <i>x</i></span>: For each <span class="tex-span"><i>i</i></span> such that <span class="tex-span"><i>l</i> ≤ <i>i</i> ≤ <i>r</i></span>, assign <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> + <i>x</i></span> to <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</li><li> <span class="tex-span">2 <i>l</i> <i>r</i> <i>x</i></span>: For each <span class="tex-span"><i>i</i></span> such that <span class="tex-span"><i>l</i> ≤ <i>i</i> ≤ <i>r</i></span>, assign <span class="tex-span"><i>x</i></span> to <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</li><li> <span class="tex-span">3 <i>l</i> <i>r</i> <i>x</i></span>: Print the <span class="tex-span"><i>x</i></span>-th smallest number in the index range <span class="tex-span">[<i>l</i>, <i>r</i>]</span>, i.e. the element at the <span class="tex-span"><i>x</i></span>-th position if all the elements <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> such that <span class="tex-span"><i>l</i> ≤ <i>i</i> ≤ <i>r</i></span> are taken and sorted into an array of non-decreasing integers. It's guaranteed that <span class="tex-span">1 ≤ <i>x</i> ≤ <i>r</i> - <i>l</i> + 1</span>.</li><li> <span class="tex-span">4 <i>l</i> <i>r</i> <i>x</i> <i>y</i></span>: Print the sum of the <span class="tex-span"><i>x</i></span>-th power of <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> such that <span class="tex-span"><i>l</i> ≤ <i>i</i> ≤ <i>r</i></span>, modulo <span class="tex-span"><i>y</i></span>, i.e. <img align="middle" class="tex-formula" src="file://UDfpxBfu.png" style="max-width: 100.0%;max-height: 100.0%;">.</li></ul></div><div class="input-specification"><p>The only line contains four integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>seed</i>, <i>v</i><sub class="lower-index"><i>max</i></sub></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>, 0 ≤ <i>seed</i> &lt; 10<sup class="upper-index">9</sup> + 7, 1 ≤ <i>vmax</i> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>The initial values and operations are generated using following pseudo code:</p><pre class="verbatim"><br>def rnd():<br><br>    ret = seed<br>    seed = (seed * 7 + 13) mod 1000000007<br>    return ret<br><br>for i = 1 to n:<br><br>    a[i] = (rnd() mod vmax) + 1<br><br>for i = 1 to m:<br><br>    op = (rnd() mod 4) + 1<br>    l = (rnd() mod n) + 1<br>    r = (rnd() mod n) + 1<br><br>    if (l &gt; r): <br>         swap(l, r)<br><br>    if (op == 3):<br>        x = (rnd() mod (r - l + 1)) + 1<br>    else:<br>        x = (rnd() mod vmax) + 1<br><br>    if (op == 4):<br>        y = (rnd() mod vmax) + 1<br><br></pre><p>Here <span class="tex-span"><i>op</i></span> is the type of the operation mentioned in the legend.</p></div><div class="output-specification"><p>For each operation of types <span class="tex-span">3</span> or <span class="tex-span">4</span>, output a line containing the answer.</p></div>

## Input

<p>The only line contains four integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>seed</i>, <i>v</i><sub class="lower-index"><i>max</i></sub></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>, 0 ≤ <i>seed</i> &lt; 10<sup class="upper-index">9</sup> + 7, 1 ≤ <i>vmax</i> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>The initial values and operations are generated using following pseudo code:</p><pre class="verbatim"><br>def rnd():<br><br>    ret = seed<br>    seed = (seed * 7 + 13) mod 1000000007<br>    return ret<br><br>for i = 1 to n:<br><br>    a[i] = (rnd() mod vmax) + 1<br><br>for i = 1 to m:<br><br>    op = (rnd() mod 4) + 1<br>    l = (rnd() mod n) + 1<br>    r = (rnd() mod n) + 1<br><br>    if (l &gt; r): <br>         swap(l, r)<br><br>    if (op == 3):<br>        x = (rnd() mod (r - l + 1)) + 1<br>    else:<br>        x = (rnd() mod vmax) + 1<br><br>    if (op == 4):<br>        y = (rnd() mod vmax) + 1<br><br></pre><p>Here <span class="tex-span"><i>op</i></span> is the type of the operation mentioned in the legend.</p>

## Output

<p>For each operation of types <span class="tex-span">3</span> or <span class="tex-span">4</span>, output a line containing the answer.</p>





```input1
10 10 7 9

```




```input2
10 10 9 9

```




```output1
2
1
0
3

```




```output2
1
1
3
3

```



## Note

<p>In the first example, the initial array is <span class="tex-span">{8, 9, 7, 2, 3, 1, 5, 6, 4, 8}</span>.</p><p>The operations are:</p><ul> <li> <span class="tex-span">2 6 7 9</span> </li><li> <span class="tex-span">1 3 10 8</span> </li><li> <span class="tex-span">4 4 6 2 4</span> </li><li> <span class="tex-span">1 4 5 8</span> </li><li> <span class="tex-span">2 1 7 1</span> </li><li> <span class="tex-span">4 7 9 4 4</span> </li><li> <span class="tex-span">1 2 7 9</span> </li><li> <span class="tex-span">4 5 8 1 1</span> </li><li> <span class="tex-span">2 5 7 5</span> </li><li> <span class="tex-span">4 3 10 8 5</span> </li></ul>
