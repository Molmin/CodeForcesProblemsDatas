## Description

<div><p>You are given a string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span> consisting of lowercase English letters.</p><p>For two given strings <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span>, say <span class="tex-span"><i>S</i></span> is the set of distinct characters of <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>T</i></span> is the set of distinct characters of <span class="tex-span"><i>t</i></span>. The strings <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> are <span class="tex-font-style-it">isomorphic</span> if their lengths are equal and there is a one-to-one mapping (bijection) <span class="tex-span"><i>f</i></span> between <span class="tex-span"><i>S</i></span> and <span class="tex-span"><i>T</i></span> for which <span class="tex-span"><i>f</i>(<i>s</i><sub class="lower-index"><i>i</i></sub>) = <i>t</i><sub class="lower-index"><i>i</i></sub></span>. Formally:</p><ol> <li> <span class="tex-span"><i>f</i>(<i>s</i><sub class="lower-index"><i>i</i></sub>) = <i>t</i><sub class="lower-index"><i>i</i></sub></span> for any index <span class="tex-span"><i>i</i></span>, </li><li> for any character <img align="middle" class="tex-formula" src="file://Eittsfpd.png" style="max-width: 100.0%;max-height: 100.0%;"> there is exactly one character <img align="middle" class="tex-formula" src="file://uy13MgcR.png" style="max-width: 100.0%;max-height: 100.0%;"> that <span class="tex-span"><i>f</i>(<i>x</i>) = <i>y</i></span>, </li><li> for any character <img align="middle" class="tex-formula" src="file://ceeoLM1L.png" style="max-width: 100.0%;max-height: 100.0%;"> there is exactly one character <img align="middle" class="tex-formula" src="file://lESIG0ti.png" style="max-width: 100.0%;max-height: 100.0%;"> that <span class="tex-span"><i>f</i>(<i>x</i>) = <i>y</i></span>. </li></ol><p>For example, the strings "<span class="tex-font-style-tt">aababc</span>" and "<span class="tex-font-style-tt">bbcbcz</span>" are isomorphic. Also the strings "<span class="tex-font-style-tt">aaaww</span>" and "<span class="tex-font-style-tt">wwwaa</span>" are isomorphic. The following pairs of strings are not isomorphic: "<span class="tex-font-style-tt">aab</span>" and "<span class="tex-font-style-tt">bbb</span>", "<span class="tex-font-style-tt">test</span>" and "<span class="tex-font-style-tt">best</span>".</p><p>You have to handle <span class="tex-span"><i>m</i></span> queries characterized by three integers <span class="tex-span"><i>x</i>, <i>y</i>, <i>len</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i> - <i>len</i> + 1</span>). For each query check if two substrings <span class="tex-span"><i>s</i>[<i>x</i>... <i>x</i> + <i>len</i> - 1]</span> and <span class="tex-span"><i>s</i>[<i>y</i>... <i>y</i> + <i>len</i> - 1]</span> are isomorphic.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the length of the string <span class="tex-span"><i>s</i></span> and the number of queries.</p><p>The second line contains string <span class="tex-span"><i>s</i></span> consisting of <span class="tex-span"><i>n</i></span> lowercase English letters.</p><p>The following <span class="tex-span"><i>m</i></span> lines contain a single query on each line: <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>len</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>len</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> - <i>max</i>(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>) + 1</span>) — the description of the pair of the substrings to check.</p></div><div class="output-specification"><p>For each query in a separate line print "<span class="tex-font-style-tt">YES</span>" if substrings <span class="tex-span"><i>s</i>[<i>x</i><sub class="lower-index"><i>i</i></sub>... <i>x</i><sub class="lower-index"><i>i</i></sub> + <i>len</i><sub class="lower-index"><i>i</i></sub> - 1]</span> and <span class="tex-span"><i>s</i>[<i>y</i><sub class="lower-index"><i>i</i></sub>... <i>y</i><sub class="lower-index"><i>i</i></sub> + <i>len</i><sub class="lower-index"><i>i</i></sub> - 1]</span> are isomorphic and "<span class="tex-font-style-tt">NO</span>" otherwise.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the length of the string <span class="tex-span"><i>s</i></span> and the number of queries.</p><p>The second line contains string <span class="tex-span"><i>s</i></span> consisting of <span class="tex-span"><i>n</i></span> lowercase English letters.</p><p>The following <span class="tex-span"><i>m</i></span> lines contain a single query on each line: <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>len</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>len</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> - <i>max</i>(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>) + 1</span>) — the description of the pair of the substrings to check.</p>

## Output

<p>For each query in a separate line print "<span class="tex-font-style-tt">YES</span>" if substrings <span class="tex-span"><i>s</i>[<i>x</i><sub class="lower-index"><i>i</i></sub>... <i>x</i><sub class="lower-index"><i>i</i></sub> + <i>len</i><sub class="lower-index"><i>i</i></sub> - 1]</span> and <span class="tex-span"><i>s</i>[<i>y</i><sub class="lower-index"><i>i</i></sub>... <i>y</i><sub class="lower-index"><i>i</i></sub> + <i>len</i><sub class="lower-index"><i>i</i></sub> - 1]</span> are isomorphic and "<span class="tex-font-style-tt">NO</span>" otherwise.</p>





```input1
7 4
abacaba
1 1 1
1 4 2
2 1 3
2 4 3

```




```output1
YES
YES
NO
YES

```



## Note

<p>The queries in the example are following: </p><ol> <li> substrings "<span class="tex-font-style-tt">a</span>" and "<span class="tex-font-style-tt">a</span>" are isomorphic: <span class="tex-span"><i>f</i>(<i>a</i>) = <i>a</i></span>; </li><li> substrings "<span class="tex-font-style-tt">ab</span>" and "<span class="tex-font-style-tt">ca</span>" are isomorphic: <span class="tex-span"><i>f</i>(<i>a</i>) = <i>c</i></span>, <span class="tex-span"><i>f</i>(<i>b</i>) = <i>a</i></span>; </li><li> substrings "<span class="tex-font-style-tt">bac</span>" and "<span class="tex-font-style-tt">aba</span>" are not isomorphic since <span class="tex-span"><i>f</i>(<i>b</i>)</span> and <span class="tex-span"><i>f</i>(<i>c</i>)</span> must be equal to <span class="tex-span"><i>a</i></span> at same time; </li><li> substrings "<span class="tex-font-style-tt">bac</span>" and "<span class="tex-font-style-tt">cab</span>" are isomorphic: <span class="tex-span"><i>f</i>(<i>b</i>) = <i>c</i></span>, <span class="tex-span"><i>f</i>(<i>a</i>) = <i>a</i></span>, <span class="tex-span"><i>f</i>(<i>c</i>) = <i>b</i></span>. </li></ol>
