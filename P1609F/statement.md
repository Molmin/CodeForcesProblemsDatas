## Description

<div><center> <img class="tex-graphics" height="302px" src="file://Yfid6Cvb.png" style="max-width: 100.0%;max-height: 100.0%;" width="454px"> </center><p>William has an array of non-negative numbers $a_1, a_2, \dots, a_n$. He wants you to find out how many segments $l \le r$ pass the check. The check is performed in the following manner: </p><ol> <li> The minimum and maximum numbers are found on the segment of the array starting at $l$ and ending at $r$. </li><li> The check is considered to be passed if the binary representation of the minimum and maximum numbers have the same number of bits equal to 1. </li></ol></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 10^6$), the size of array $a$.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le 10^{18}$), the contents of array $a$.</p></div><div class="output-specification"><p>Output a single number &nbsp;— the total number of segments that passed the check.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 10^6$), the size of array $a$.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le 10^{18}$), the contents of array $a$.</p>

## Output

<p>Output a single number &nbsp;— the total number of segments that passed the check.</p>





```input1
5
1 2 3 4 5
```




```input2
10
0 5 7 3 9 10 1 6 13 7
```




```output1
9
```




```output2
18
```


