## Description

<div><p>Little Victor adores the sets theory. Let us remind you that a set is a group of numbers where all numbers are pairwise distinct. Today Victor wants to find a set of integers <span class="tex-span"><i>S</i></span> that has the following properties:</p><ul> <li> for all <span class="tex-span"><i>x</i></span> <img align="middle" class="tex-formula" src="file://WJnc8FtN.png" style="max-width: 100.0%;max-height: 100.0%;"> the following inequality holds <span class="tex-span"><i>l</i> ≤ <i>x</i> ≤ <i>r</i></span>; </li><li> <span class="tex-span">1 ≤ |<i>S</i>| ≤ <i>k</i></span>; </li><li> lets denote the <span class="tex-span"><i>i</i></span>-th element of the set <span class="tex-span"><i>S</i></span> as <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>; value <img align="middle" class="tex-formula" src="file://eLO2vYBw.png" style="max-width: 100.0%;max-height: 100.0%;"> must be as small as possible. </li></ul><p>Help Victor find the described set.</p></div><div class="input-specification"><p>The first line contains three space-separated integers <span class="tex-span"><i>l</i>, <i>r</i>, <i>k</i></span> <span class="tex-span">(1 ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">12</sup>;&nbsp;1 ≤ <i>k</i> ≤ <i>min</i>(10<sup class="upper-index">6</sup>, <i>r</i> - <i>l</i> + 1))</span>.</p></div><div class="output-specification"><p>Print the minimum possible value of <span class="tex-span"><i>f</i>(<i>S</i>)</span>. Then print the cardinality of set <span class="tex-span">|<i>S</i>|</span>. Then print the elements of the set in any order.</p><p>If there are multiple optimal sets, you can print any of them.</p></div>

## Input

<p>The first line contains three space-separated integers <span class="tex-span"><i>l</i>, <i>r</i>, <i>k</i></span> <span class="tex-span">(1 ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">12</sup>;&nbsp;1 ≤ <i>k</i> ≤ <i>min</i>(10<sup class="upper-index">6</sup>, <i>r</i> - <i>l</i> + 1))</span>.</p>

## Output

<p>Print the minimum possible value of <span class="tex-span"><i>f</i>(<i>S</i>)</span>. Then print the cardinality of set <span class="tex-span">|<i>S</i>|</span>. Then print the elements of the set in any order.</p><p>If there are multiple optimal sets, you can print any of them.</p>





```input1
8 15 3

```




```input2
8 30 7

```




```output1
1
2
10 11

```




```output2
0
5
14 9 28 11 16

```



## Note

<p>Operation <img align="middle" class="tex-formula" src="file://ot1xX3mR.png" style="max-width: 100.0%;max-height: 100.0%;"> represents the operation of bitwise exclusive OR. In other words, it is the XOR operation.</p>
