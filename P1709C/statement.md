## Description

<div><p>A bracket sequence is a string containing only characters "<span class="tex-font-style-tt">(</span>" and "<span class="tex-font-style-tt">)</span>". A regular bracket sequence (or, shortly, an RBS) is a bracket sequence that can be transformed into a correct arithmetic expression by inserting characters "<span class="tex-font-style-tt">1</span>" and "<span class="tex-font-style-tt">+</span>" between the original characters of the sequence. For example:</p><ul> <li> bracket sequences "<span class="tex-font-style-tt">()()</span>" and "<span class="tex-font-style-tt">(())</span>" are regular (the resulting expressions are: "<span class="tex-font-style-tt">(1)+(1)</span>" and "<span class="tex-font-style-tt">((1+1)+1)</span>"); </li><li> bracket sequences "<span class="tex-font-style-tt">)(</span>", "<span class="tex-font-style-tt">(</span>" and "<span class="tex-font-style-tt">)</span>" are not. </li></ul><p>There was an RBS. Some brackets have been replaced with question marks. Is it true that there is a <span class="tex-font-style-bf">unique</span> way to replace question marks with brackets, so that the resulting sequence is an RBS?</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 5 \cdot 10^4$)&nbsp;— the number of testcases.</p><p>The only line of each testcase contains an RBS with some brackets replaced with question marks. Each character is either '<span class="tex-font-style-tt">(</span>', '<span class="tex-font-style-tt">)</span>' or '<span class="tex-font-style-tt">?</span>'. At least one RBS can be recovered from the given sequence.</p><p>The total length of the sequences over all testcases doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each testcase, print "<span class="tex-font-style-tt">YES</span>" if the way to replace question marks with brackets, so that the resulting sequence is an RBS, is <span class="tex-font-style-bf">unique</span>. If there is more than one way, then print "<span class="tex-font-style-tt">NO</span>".</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 5 \cdot 10^4$)&nbsp;— the number of testcases.</p><p>The only line of each testcase contains an RBS with some brackets replaced with question marks. Each character is either '<span class="tex-font-style-tt">(</span>', '<span class="tex-font-style-tt">)</span>' or '<span class="tex-font-style-tt">?</span>'. At least one RBS can be recovered from the given sequence.</p><p>The total length of the sequences over all testcases doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each testcase, print "<span class="tex-font-style-tt">YES</span>" if the way to replace question marks with brackets, so that the resulting sequence is an RBS, is <span class="tex-font-style-bf">unique</span>. If there is more than one way, then print "<span class="tex-font-style-tt">NO</span>".</p>





```input1|2,4,6
5
(?))
??????
()
??
?(?)()?)
```




```output1
YES
NO
YES
YES
NO
```



## Note

<p>In the first testcase, the only possible original RBS is "<span class="tex-font-style-tt">(())</span>".</p><p>In the second testcase, there are multiple ways to recover an RBS.</p><p>In the third and the fourth testcases, the only possible original RBS is "<span class="tex-font-style-tt">()</span>".</p><p>In the fifth testcase, the original RBS can be either "<span class="tex-font-style-tt">((()()))</span>" or "<span class="tex-font-style-tt">(())()()</span>".</p>
