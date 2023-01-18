## Description

<div><p>Alice has a string consisting of characters '<span class="tex-font-style-tt">A</span>', '<span class="tex-font-style-tt">B</span>' and '<span class="tex-font-style-tt">C</span>'. Bob can use the following transitions on any substring of our string in any order any number of times: </p><ul> <li> <span class="tex-font-style-tt">A</span> <img align="middle" class="tex-formula" src="file://PNvTJD7E.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-style-tt">BC</span> </li><li> <span class="tex-font-style-tt">B</span> <img align="middle" class="tex-formula" src="file://JFkkA6t8.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-style-tt">AC</span> </li><li> <span class="tex-font-style-tt">C</span> <img align="middle" class="tex-formula" src="file://z103TbfY.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-style-tt">AB</span> </li><li> <span class="tex-font-style-tt">AAA</span> <img align="middle" class="tex-formula" src="file://rvu9ESKN.png" style="max-width: 100.0%;max-height: 100.0%;"> empty string </li></ul><p>Note that a substring is one or more consecutive characters. For given queries, determine whether it is possible to obtain the target string from source.</p></div><div class="input-specification"><p>The first line contains a string <span class="tex-span"><i>S</i></span> (<span class="tex-span">1 ≤ |<i>S</i>| ≤ 10<sup class="upper-index">5</sup></span>). The second line contains a string <span class="tex-span"><i>T</i></span> (<span class="tex-span">1 ≤ |<i>T</i>| ≤ 10<sup class="upper-index">5</sup></span>), each of these strings consists only of uppercase English letters '<span class="tex-font-style-tt">A</span>', '<span class="tex-font-style-tt">B</span>' and '<span class="tex-font-style-tt">C</span>'.</p><p>The third line contains the number of queries <span class="tex-span"><i>Q</i></span> (<span class="tex-span">1 ≤ <i>Q</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The following <span class="tex-span"><i>Q</i></span> lines describe queries. The <span class="tex-span"><i>i</i></span>-th of these lines contains four space separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>. These represent the <span class="tex-span"><i>i</i></span>-th query: is it possible to create <span class="tex-span"><i>T</i>[<i>c</i><sub class="lower-index"><i>i</i></sub>..<i>d</i><sub class="lower-index"><i>i</i></sub>]</span> from <span class="tex-span"><i>S</i>[<i>a</i><sub class="lower-index"><i>i</i></sub>..<i>b</i><sub class="lower-index"><i>i</i></sub>]</span> by applying the above transitions finite amount of times?</p><p>Here, <span class="tex-span"><i>U</i>[<i>x</i>..<i>y</i>]</span> is a substring of <span class="tex-span"><i>U</i></span> that begins at index <span class="tex-span"><i>x</i></span> (indexed from 1) and ends at index <span class="tex-span"><i>y</i></span>. In particular, <span class="tex-span"><i>U</i>[1..|<i>U</i>|]</span> is the whole string <span class="tex-span"><i>U</i></span>.</p><p>It is guaranteed that <span class="tex-span">1 ≤ <i>a</i> ≤ <i>b</i> ≤ |<i>S</i>|</span> and <span class="tex-span">1 ≤ <i>c</i> ≤ <i>d</i> ≤ |<i>T</i>|</span>.</p></div><div class="output-specification"><p>Print a string of <span class="tex-span"><i>Q</i></span> characters, where the <span class="tex-span"><i>i</i></span>-th character is '<span class="tex-font-style-tt">1</span>' if the answer to the <span class="tex-span"><i>i</i></span>-th query is positive, and '<span class="tex-font-style-tt">0</span>' otherwise.</p></div>

## Input

<p>The first line contains a string <span class="tex-span"><i>S</i></span> (<span class="tex-span">1 ≤ |<i>S</i>| ≤ 10<sup class="upper-index">5</sup></span>). The second line contains a string <span class="tex-span"><i>T</i></span> (<span class="tex-span">1 ≤ |<i>T</i>| ≤ 10<sup class="upper-index">5</sup></span>), each of these strings consists only of uppercase English letters '<span class="tex-font-style-tt">A</span>', '<span class="tex-font-style-tt">B</span>' and '<span class="tex-font-style-tt">C</span>'.</p><p>The third line contains the number of queries <span class="tex-span"><i>Q</i></span> (<span class="tex-span">1 ≤ <i>Q</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The following <span class="tex-span"><i>Q</i></span> lines describe queries. The <span class="tex-span"><i>i</i></span>-th of these lines contains four space separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>. These represent the <span class="tex-span"><i>i</i></span>-th query: is it possible to create <span class="tex-span"><i>T</i>[<i>c</i><sub class="lower-index"><i>i</i></sub>..<i>d</i><sub class="lower-index"><i>i</i></sub>]</span> from <span class="tex-span"><i>S</i>[<i>a</i><sub class="lower-index"><i>i</i></sub>..<i>b</i><sub class="lower-index"><i>i</i></sub>]</span> by applying the above transitions finite amount of times?</p><p>Here, <span class="tex-span"><i>U</i>[<i>x</i>..<i>y</i>]</span> is a substring of <span class="tex-span"><i>U</i></span> that begins at index <span class="tex-span"><i>x</i></span> (indexed from 1) and ends at index <span class="tex-span"><i>y</i></span>. In particular, <span class="tex-span"><i>U</i>[1..|<i>U</i>|]</span> is the whole string <span class="tex-span"><i>U</i></span>.</p><p>It is guaranteed that <span class="tex-span">1 ≤ <i>a</i> ≤ <i>b</i> ≤ |<i>S</i>|</span> and <span class="tex-span">1 ≤ <i>c</i> ≤ <i>d</i> ≤ |<i>T</i>|</span>.</p>

## Output

<p>Print a string of <span class="tex-span"><i>Q</i></span> characters, where the <span class="tex-span"><i>i</i></span>-th character is '<span class="tex-font-style-tt">1</span>' if the answer to the <span class="tex-span"><i>i</i></span>-th query is positive, and '<span class="tex-font-style-tt">0</span>' otherwise.</p>





```input1
AABCCBAAB
ABCB
5
1 3 1 2
2 2 2 4
7 9 1 1
3 4 2 3
4 5 1 3

```




```output1
10011

```



## Note

<p>In the first query we can achieve the result, for instance, by using transitions <img align="middle" class="tex-formula" src="file://hxqznENi.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>The third query asks for changing <span class="tex-font-style-tt">AAB</span> to <span class="tex-font-style-tt">A</span>&nbsp;— but in this case we are not able to get rid of the character '<span class="tex-font-style-tt">B</span>'.</p>
