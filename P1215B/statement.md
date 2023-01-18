## Description

<div><p>You are given a sequence $a_1, a_2, \dots, a_n$ consisting of $n$ non-zero integers (i.e. $a_i \ne 0$). </p><p>You have to calculate two following values:</p><ol> <li> the number of pairs of indices $(l, r)$ $(l \le r)$ such that $a_l \cdot a_{l + 1} \dots a_{r - 1} \cdot a_r$ is negative; </li><li> the number of pairs of indices $(l, r)$ $(l \le r)$ such that $a_l \cdot a_{l + 1} \dots a_{r - 1} \cdot a_r$ is positive; </li></ol></div><div class="input-specification"><p>The first line contains one integer $n$ $(1 \le n \le 2 \cdot 10^{5})$ — the number of elements in the sequence.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ $(-10^{9} \le a_i \le 10^{9}; a_i \neq 0)$ — the elements of the sequence.</p></div><div class="output-specification"><p>Print two integers — the number of subsegments with negative product and the number of subsegments with positive product, respectively.</p></div>

## Input

<p>The first line contains one integer $n$ $(1 \le n \le 2 \cdot 10^{5})$ — the number of elements in the sequence.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ $(-10^{9} \le a_i \le 10^{9}; a_i \neq 0)$ — the elements of the sequence.</p>

## Output

<p>Print two integers — the number of subsegments with negative product and the number of subsegments with positive product, respectively.</p>





```input1
5
5 -3 3 -1 1
```




```input2
10
4 2 -4 3 1 2 -4 3 2 3
```




```input3
5
-1 -2 -3 -4 -5
```




```output1
8 7
```




```output2
28 27
```




```output3
9 6
```


