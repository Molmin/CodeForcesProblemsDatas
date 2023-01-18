## Description

<div><p>This task is very simple. Given a string <span class="tex-span"><i>S</i></span> of length <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> queries each query is on the format <span class="tex-span"><i>i</i></span> <span class="tex-span"><i>j</i></span> <span class="tex-span"><i>k</i></span> which means sort the substring consisting of the characters from <span class="tex-span"><i>i</i></span> to <span class="tex-span"><i>j</i></span> in non-decreasing order if <span class="tex-span"><i>k</i> = 1</span> or in non-increasing order if <span class="tex-span"><i>k</i> = 0</span>.</p><p>Output the final string after applying the queries.</p></div><div class="input-specification"><p>The first line will contain two integers <span class="tex-span"><i>n</i>, <i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>q</i> ≤ 50 000</span>), the length of the string and the number of queries respectively. </p><p><span class="tex-font-style-bf">Next line contains a string <span class="tex-span"><i>S</i></span> itself. It contains only lowercase English letters.</span></p><p>Next <span class="tex-span"><i>q</i></span> lines will contain three integers each <span class="tex-span"><i>i</i>, <i>j</i>, <i>k</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>j</i> ≤ <i>n</i></span>, <img align="middle" class="tex-formula" src="file://6t2SlwTi.png" style="max-width: 100.0%;max-height: 100.0%;">).</p></div><div class="output-specification"><p>Output one line, the string <span class="tex-span"><i>S</i></span> after applying the queries.</p></div>

## Input

<p>The first line will contain two integers <span class="tex-span"><i>n</i>, <i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>q</i> ≤ 50 000</span>), the length of the string and the number of queries respectively. </p><p><span class="tex-font-style-bf">Next line contains a string <span class="tex-span"><i>S</i></span> itself. It contains only lowercase English letters.</span></p><p>Next <span class="tex-span"><i>q</i></span> lines will contain three integers each <span class="tex-span"><i>i</i>, <i>j</i>, <i>k</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>j</i> ≤ <i>n</i></span>, <img align="middle" class="tex-formula" src="file://6t2SlwTi.png" style="max-width: 100.0%;max-height: 100.0%;">).</p>

## Output

<p>Output one line, the string <span class="tex-span"><i>S</i></span> after applying the queries.</p>





```input1
10 5
abacdabcda
7 10 0
5 8 1
1 4 0
3 6 0
7 10 1

```




```input2
10 1
agjucbvdfk
1 10 1

```




```output1
cbcaaaabdd
```




```output2
abcdfgjkuv
```



## Note

<p>First sample test explanation:</p><p><img align="middle" class="tex-formula" src="file://2D7HiC4S.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p><img align="middle" class="tex-formula" src="file://PGWaAWGx.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p><img align="middle" class="tex-formula" src="file://myw6cWda.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p><img align="middle" class="tex-formula" src="file://9MYhqR7m.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p><img align="middle" class="tex-formula" src="file://PmWOLWis.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
