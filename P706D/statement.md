## Description

<div><p>Author has gone out of the stories about Vasiliy, so here is just a formal task description.</p><p>You are given <span class="tex-span"><i>q</i></span> queries and a multiset <span class="tex-span"><i>A</i></span>, initially containing only integer <span class="tex-span">0</span>. There are three types of queries:</p><ol> <li> "<span class="tex-font-style-tt">+ x</span>"&nbsp;— add integer <span class="tex-span"><i>x</i></span> to multiset <span class="tex-span"><i>A</i></span>.</li><li> "<span class="tex-font-style-tt">- x</span>"&nbsp;— erase one occurrence of integer <span class="tex-span"><i>x</i></span> from multiset <span class="tex-span"><i>A</i></span>. It's guaranteed that at least one <span class="tex-span"><i>x</i></span> is present in the multiset <span class="tex-span"><i>A</i></span> before this query.</li><li> "<span class="tex-font-style-tt">? x</span>"&nbsp;— you are given integer <span class="tex-span"><i>x</i></span> and need to compute the value <img align="middle" class="tex-formula" src="file://92HexauY.png" style="max-width: 100.0%;max-height: 100.0%;">, i.e. the maximum value of bitwise exclusive OR (also know as XOR) of integer <span class="tex-span"><i>x</i></span> and some integer <span class="tex-span"><i>y</i></span> from the multiset <span class="tex-span"><i>A</i></span>.</li></ol><p>Multiset is a set, where equal elements are allowed.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 200 000</span>)&nbsp;— the number of queries Vasiliy has to perform.</p><p>Each of the following <span class="tex-span"><i>q</i></span> lines of the input contains one of three characters '<span class="tex-font-style-tt">+</span>', '<span class="tex-font-style-tt">-</span>' or '<span class="tex-font-style-tt">?</span>' and an integer <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). It's guaranteed that there is at least one query of the third type.</p><p>Note, that the integer <span class="tex-span">0</span> will always be present in the set <span class="tex-span"><i>A</i></span>.</p></div><div class="output-specification"><p>For each query of the type '<span class="tex-font-style-tt">?</span>' print one integer&nbsp;— the maximum value of bitwise exclusive OR (XOR) of integer <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and some integer from the multiset <span class="tex-span"><i>A</i></span>.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 200 000</span>)&nbsp;— the number of queries Vasiliy has to perform.</p><p>Each of the following <span class="tex-span"><i>q</i></span> lines of the input contains one of three characters '<span class="tex-font-style-tt">+</span>', '<span class="tex-font-style-tt">-</span>' or '<span class="tex-font-style-tt">?</span>' and an integer <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). It's guaranteed that there is at least one query of the third type.</p><p>Note, that the integer <span class="tex-span">0</span> will always be present in the set <span class="tex-span"><i>A</i></span>.</p>

## Output

<p>For each query of the type '<span class="tex-font-style-tt">?</span>' print one integer&nbsp;— the maximum value of bitwise exclusive OR (XOR) of integer <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and some integer from the multiset <span class="tex-span"><i>A</i></span>.</p>





```input1
10
+ 8
+ 9
+ 11
+ 6
+ 1
? 3
- 8
? 3
? 8
? 11

```




```output1
11
10
14
13

```



## Note

<p>After first five operations multiset <span class="tex-span"><i>A</i></span> contains integers <span class="tex-span">0</span>, <span class="tex-span">8</span>, <span class="tex-span">9</span>, <span class="tex-span">11</span>, <span class="tex-span">6</span> and <span class="tex-span">1</span>.</p><p>The answer for the sixth query is integer <img align="middle" class="tex-formula" src="file://28XfBA23.png" style="max-width: 100.0%;max-height: 100.0%;">&nbsp;— maximum among integers <img align="middle" class="tex-formula" src="file://Y6rK2Uhx.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://GZRVX5r5.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://EfHoNnpN.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://Pa0uFXpG.png" style="max-width: 100.0%;max-height: 100.0%;"> and <img align="middle" class="tex-formula" src="file://pCX5pkGr.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
