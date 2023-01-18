## Description

<div><p>Little X has met the following problem recently. </p><p>Let's define <span class="tex-span"><i>f</i>(<i>x</i>)</span> as the sum of digits in decimal representation of number <span class="tex-span"><i>x</i></span> (for example, <span class="tex-span"><i>f</i>(1234) = 1 + 2 + 3 + 4</span>). You are to calculate <img align="middle" class="tex-formula" src="file://ijts8N9W.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>Of course Little X has solved this problem quickly, has locked it, and then has tried to hack others. He has seen the following C++ code: </p><pre class="verbatim"><br>    ans = solve(l, r) % a;<br>    if (ans &lt;= 0)<br>      ans += a;<br><br></pre> This code will fail only on the test with <img align="middle" class="tex-formula" src="file://kkhImd80.png" style="max-width: 100.0%;max-height: 100.0%;">. You are given number <span class="tex-span"><i>a</i></span>, help Little X to find a proper test for hack.</div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>a</i>&nbsp;(1 ≤ <i>a</i> ≤ 10<sup class="upper-index">18</sup>)</span>.</p></div><div class="output-specification"><p>Print two integers: <span class="tex-span"><i>l</i>, <i>r</i>&nbsp;(1 ≤ <i>l</i> ≤ <i>r</i> &lt; 10<sup class="upper-index">200</sup>)</span> — the required test data. Leading zeros aren't allowed. It's guaranteed that the solution exists.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>a</i>&nbsp;(1 ≤ <i>a</i> ≤ 10<sup class="upper-index">18</sup>)</span>.</p>

## Output

<p>Print two integers: <span class="tex-span"><i>l</i>, <i>r</i>&nbsp;(1 ≤ <i>l</i> ≤ <i>r</i> &lt; 10<sup class="upper-index">200</sup>)</span> — the required test data. Leading zeros aren't allowed. It's guaranteed that the solution exists.</p>





```input1
46

```




```input2
126444381000032

```




```output1
1 10

```




```output2
2333333 2333333333333

```


