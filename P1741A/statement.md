## Description

<div><p>Two T-shirt sizes are given: $a$ and $b$. The T-shirt size is either a string <span class="tex-font-style-tt">M</span> or a string consisting of several (possibly zero) characters <span class="tex-font-style-tt">X</span> and one of the characters <span class="tex-font-style-tt">S</span> or <span class="tex-font-style-tt">L</span>.</p><p>For example, strings <span class="tex-font-style-tt">M</span>, <span class="tex-font-style-tt">XXL</span>, <span class="tex-font-style-tt">S</span>, <span class="tex-font-style-tt">XXXXXXXS</span> could be the size of some T-shirts. And the strings <span class="tex-font-style-tt">XM</span>, <span class="tex-font-style-tt">LL</span>, <span class="tex-font-style-tt">SX</span> are not sizes.</p><p>The letter <span class="tex-font-style-tt">M</span> stands for medium, <span class="tex-font-style-tt">S</span> for small, <span class="tex-font-style-tt">L</span> for large. The letter <span class="tex-font-style-tt">X</span> refers to the degree of size (from eXtra). For example, <span class="tex-font-style-tt">XXL</span> is extra-extra-large (bigger than <span class="tex-font-style-tt">XL</span>, and smaller than <span class="tex-font-style-tt">XXXL</span>).</p><p>You need to compare two given sizes of T-shirts $a$ and $b$.</p><p>The T-shirts are compared as follows: </p><ul> <li> any small size (no matter how many letters <span class="tex-font-style-tt">X</span>) is smaller than the medium size and any large size; </li><li> any large size (regardless of the number of letters <span class="tex-font-style-tt">X</span>) is larger than the medium size and any small size; </li><li> the more letters <span class="tex-font-style-tt">X</span> before <span class="tex-font-style-tt">S</span>, the smaller the size; </li><li> the more letters <span class="tex-font-style-tt">X</span> in front of <span class="tex-font-style-tt">L</span>, the larger the size. </li></ul><p>For example: </p><ul> <li> <span class="tex-font-style-tt">XXXS</span> &lt; <span class="tex-font-style-tt">XS</span> </li><li> <span class="tex-font-style-tt">XXXL</span> &gt; <span class="tex-font-style-tt">XL</span> </li><li> <span class="tex-font-style-tt">XL</span> &gt; <span class="tex-font-style-tt">M</span> </li><li> <span class="tex-font-style-tt">XXL</span> = <span class="tex-font-style-tt">XXL</span> </li><li> <span class="tex-font-style-tt">XXXXXS</span> &lt; <span class="tex-font-style-tt">M</span> </li><li> <span class="tex-font-style-tt">XL</span> &gt; <span class="tex-font-style-tt">XXXS</span> </li></ul></div><div class="input-specification"><p>The first line of the input contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>Each test case consists of one line, in which $a$ and $b$ T-shirt sizes are written. The lengths of the strings corresponding to the T-shirt sizes do not exceed $50$. It is guaranteed that all sizes are correct.</p></div><div class="output-specification"><p>For each test case, print on a separate line the result of comparing $a$ and $b$ T-shirt sizes (lines "<span class="tex-font-style-tt">&lt;</span>", "<span class="tex-font-style-tt">&gt;</span>" or "<span class="tex-font-style-tt">=</span>" without quotes).</p></div>

## Input

<p>The first line of the input contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>Each test case consists of one line, in which $a$ and $b$ T-shirt sizes are written. The lengths of the strings corresponding to the T-shirt sizes do not exceed $50$. It is guaranteed that all sizes are correct.</p>

## Output

<p>For each test case, print on a separate line the result of comparing $a$ and $b$ T-shirt sizes (lines "<span class="tex-font-style-tt">&lt;</span>", "<span class="tex-font-style-tt">&gt;</span>" or "<span class="tex-font-style-tt">=</span>" without quotes).</p>





```input1|2,4,6
6
XXXS XS
XXXL XL
XL M
XXL XXL
XXXXXS M
L M
```




```output1
&lt;
&gt;
&gt;
=
&lt;
&gt;
```


