## Description

<div><p>Limak is a little polar bear. He likes <span class="tex-font-style-bf">nice</span> strings — strings of length <span class="tex-span"><i>n</i></span>, consisting of lowercase English letters only.</p><p>The distance between two letters is defined as the difference between their positions in the alphabet. For example, <img align="middle" class="tex-formula" src="file://NjDkXXT1.png" style="max-width: 100.0%;max-height: 100.0%;">, and <img align="middle" class="tex-formula" src="file://qHxQR1xl.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>Also, the distance between two nice strings is defined as the sum of distances of corresponding letters. For example, <img align="middle" class="tex-formula" src="file://axdpgYyO.png" style="max-width: 100.0%;max-height: 100.0%;">, and <img align="middle" class="tex-formula" src="file://YOYtSrjj.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>Limak gives you a nice string <span class="tex-span"><i>s</i></span> and an integer <span class="tex-span"><i>k</i></span>. He challenges you to find any nice string <span class="tex-span"><i>s</i>'</span> that <img align="middle" class="tex-formula" src="file://b2WmBWuQ.png" style="max-width: 100.0%;max-height: 100.0%;">. Find any <span class="tex-span"><i>s</i>'</span> satisfying the given conditions, or print "<span class="tex-font-style-tt">-1</span>" if it's impossible to do so.</p><p>As input/output can reach huge size it is recommended to use fast input/output methods: for example, prefer to use <span class="tex-font-style-tt">gets/scanf/printf</span> instead of <span class="tex-font-style-tt">getline/cin/cout</span> in C++, prefer to use <span class="tex-font-style-tt">BufferedReader/PrintWriter</span> instead of <span class="tex-font-style-tt">Scanner/System.out</span> in <span class="tex-font-style-tt">Java</span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 10<sup class="upper-index">6</sup></span>).</p><p>The second line contains a string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span>, consisting of lowercase English letters.</p></div><div class="output-specification"><p>If there is no string satisfying the given conditions then print "<span class="tex-font-style-tt">-1</span>" (without the quotes).</p><p>Otherwise, print any nice string <span class="tex-span"><i>s</i>'</span> that <img align="middle" class="tex-formula" src="file://QecCemOu.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 10<sup class="upper-index">6</sup></span>).</p><p>The second line contains a string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span>, consisting of lowercase English letters.</p>

## Output

<p>If there is no string satisfying the given conditions then print "<span class="tex-font-style-tt">-1</span>" (without the quotes).</p><p>Otherwise, print any nice string <span class="tex-span"><i>s</i>'</span> that <img align="middle" class="tex-formula" src="file://QecCemOu.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
4 26
bear

```




```input2
2 7
af

```




```input3
3 1000
hey

```




```output1
roar
```




```output2
db

```




```output3
-1

```


