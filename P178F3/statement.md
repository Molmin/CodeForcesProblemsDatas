## Description

<div><p>The Smart Beaver from ABBYY has a long history of cooperating with the "Institute of Cytology and Genetics". Recently, the Institute staff challenged the Beaver with a new problem. The problem is as follows.</p><p>There is a collection of <span class="tex-span"><i>n</i></span> proteins (not necessarily distinct). Each protein is a string consisting of lowercase Latin letters. The problem that the scientists offered to the Beaver is to select a subcollection of size <span class="tex-span"><i>k</i></span> from the initial collection of proteins so that the representativity of the selected subset of proteins is maximum possible.</p><p>The Smart Beaver from ABBYY did some research and came to the conclusion that the representativity of a collection of proteins can be evaluated by a single number, which is simply calculated. Let's suppose we have a collection <span class="tex-span">{<i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i></sub>}</span> consisting of <span class="tex-span"><i>k</i></span> strings describing proteins. The representativity of this collection is the following value:</p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://CBc0xuHM.png" style="max-width: 100.0%;max-height: 100.0%;"></center> <p>where <span class="tex-span"><i>f</i>(<i>x</i>, <i>y</i>)</span> is the length of the longest common prefix of strings <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>; for example, <span class="tex-span"><i>f</i>(</span>"<span class="tex-font-style-tt">abc</span>", "<span class="tex-font-style-tt">abd</span>"<span class="tex-span">) = 2</span>, and <span class="tex-span"><i>f</i>(</span>"<span class="tex-font-style-tt">ab</span>", "<span class="tex-font-style-tt">bcd</span>"<span class="tex-span">) = 0</span>.</p><p>Thus, the representativity of collection of proteins <span class="tex-span">{</span>"<span class="tex-font-style-tt">abc</span>", "<span class="tex-font-style-tt">abd</span>", "<span class="tex-font-style-tt">abe</span>"<span class="tex-span">}</span> equals <span class="tex-span">6</span>, and the representativity of collection <span class="tex-span">{</span>"<span class="tex-font-style-tt">aaa</span>", "<span class="tex-font-style-tt">ba</span>", "<span class="tex-font-style-tt">ba</span>"<span class="tex-span">}</span> equals <span class="tex-span">2</span>.</p><p>Having discovered that, the Smart Beaver from ABBYY asked the Cup contestants to write a program that selects, from the given collection of proteins, a subcollection of size <span class="tex-span"><i>k</i></span> which has the largest possible value of representativity. Help him to solve this problem!</p></div><div class="input-specification"><p>The first input line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i></span>), separated by a single space. The following <span class="tex-span"><i>n</i></span> lines contain the descriptions of proteins, one per line. Each protein is a non-empty string of no more than <span class="tex-span">500</span> characters consisting of only lowercase Latin letters (<span class="tex-font-style-tt">a</span><span class="tex-span">...</span><span class="tex-font-style-tt">z</span>). Some of the strings may be equal.</p><p>The input limitations for getting 20 points are: </p><ul> <li> <span class="tex-span">1 ≤ <i>n</i> ≤ 20</span> </li></ul><p>The input limitations for getting 50 points are: </p><ul> <li> <span class="tex-span">1 ≤ <i>n</i> ≤ 100</span> </li></ul><p>The input limitations for getting 100 points are: </p><ul> <li> <span class="tex-span">1 ≤ <i>n</i> ≤ 2000</span> </li></ul></div><div class="output-specification"><p>Print a single number denoting the largest possible value of representativity that a subcollection of size <span class="tex-span"><i>k</i></span> of the given collection of proteins can have.</p></div>

## Input

<p>The first input line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i></span>), separated by a single space. The following <span class="tex-span"><i>n</i></span> lines contain the descriptions of proteins, one per line. Each protein is a non-empty string of no more than <span class="tex-span">500</span> characters consisting of only lowercase Latin letters (<span class="tex-font-style-tt">a</span><span class="tex-span">...</span><span class="tex-font-style-tt">z</span>). Some of the strings may be equal.</p><p>The input limitations for getting 20 points are: </p><ul> <li> <span class="tex-span">1 ≤ <i>n</i> ≤ 20</span> </li></ul><p>The input limitations for getting 50 points are: </p><ul> <li> <span class="tex-span">1 ≤ <i>n</i> ≤ 100</span> </li></ul><p>The input limitations for getting 100 points are: </p><ul> <li> <span class="tex-span">1 ≤ <i>n</i> ≤ 2000</span> </li></ul>

## Output

<p>Print a single number denoting the largest possible value of representativity that a subcollection of size <span class="tex-span"><i>k</i></span> of the given collection of proteins can have.</p>





```input1
3 2
aba
bzd
abq

```




```input2
4 3
eee
rrr
ttt
qqq

```




```input3
4 3
aaa
abba
abbc
abbd

```




```output1
2

```




```output2
0

```




```output3
9

```


