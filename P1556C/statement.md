## Description

<div><center> <img class="tex-graphics" height="302px" src="file://m9ofDaIT.png" style="max-width: 100.0%;max-height: 100.0%;" width="454px"> </center><p>William has a favorite bracket sequence. Since his favorite sequence is quite big he provided it to you as a sequence of positive integers $c_1, c_2, \dots, c_n$ where $c_i$ is the number of consecutive brackets "<span class="tex-font-style-tt">(</span>" if $i$ is an odd number or the number of consecutive brackets "<span class="tex-font-style-tt">)</span>" if $i$ is an even number.</p><p>For example for a bracket sequence "<span class="tex-font-style-tt">((())()))</span>" a corresponding sequence of numbers is $[3, 2, 1, 3]$.</p><p>You need to find the total number of continuous subsequences (subsegments) $[l, r]$ ($l \le r$) of the original bracket sequence, which are regular bracket sequences.</p><p>A bracket sequence is called regular if it is possible to obtain correct arithmetic expression by inserting characters "<span class="tex-font-style-tt">+</span>" and "<span class="tex-font-style-tt">1</span>" into this sequence. For example, sequences "<span class="tex-font-style-tt">(())()</span>", "<span class="tex-font-style-tt">()</span>" and "<span class="tex-font-style-tt">(()(()))</span>" are regular, while "<span class="tex-font-style-tt">)(</span>", "<span class="tex-font-style-tt">(()</span>" and "<span class="tex-font-style-tt">(()))(</span>" are not.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ $(1 \le n \le 1000)$, the size of the compressed sequence.</p><p>The second line contains a sequence of integers $c_1, c_2, \dots, c_n$ $(1 \le c_i \le 10^9)$, the compressed sequence.</p></div><div class="output-specification"><p>Output a single integer&nbsp;— the total number of subsegments of the original bracket sequence, which are regular bracket sequences.</p><p>It can be proved that the answer fits in the signed 64-bit integer data type.</p></div>

## Input

<p>The first line contains a single integer $n$ $(1 \le n \le 1000)$, the size of the compressed sequence.</p><p>The second line contains a sequence of integers $c_1, c_2, \dots, c_n$ $(1 \le c_i \le 10^9)$, the compressed sequence.</p>

## Output

<p>Output a single integer&nbsp;— the total number of subsegments of the original bracket sequence, which are regular bracket sequences.</p><p>It can be proved that the answer fits in the signed 64-bit integer data type.</p>





```input1
5
4 1 2 3 1
```




```input2
6
1 3 2 1 2 4
```




```input3
6
1 1 1 1 2 2
```




```output1
5
```




```output2
6
```




```output3
7
```



## Note

<p>In the first example a sequence <span class="tex-font-style-tt">(((()(()))(</span> is described. This bracket sequence contains $5$ subsegments which form regular bracket sequences:</p><ol> <li> Subsequence from the $3$rd to $10$th character: <span class="tex-font-style-tt">(()(()))</span> </li><li> Subsequence from the $4$th to $5$th character: <span class="tex-font-style-tt">()</span> </li><li> Subsequence from the $4$th to $9$th character: <span class="tex-font-style-tt">()(())</span> </li><li> Subsequence from the $6$th to $9$th character: <span class="tex-font-style-tt">(())</span> </li><li> Subsequence from the $7$th to $8$th character: <span class="tex-font-style-tt">()</span> </li></ol><p>In the second example a sequence <span class="tex-font-style-tt">()))(()(())))</span> is described.</p><p>In the third example a sequence <span class="tex-font-style-tt">()()(())</span> is described.</p>
