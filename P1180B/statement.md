## Description

<div><p>Nick had received an awesome array of integers $a=[a_1, a_2, \dots, a_n]$ as a gift for his $5$ birthday from his mother. He was already going to explore its various properties but after unpacking he was disappointed a lot because the product $a_1 \cdot a_2 \cdot \dots a_n$ of its elements seemed to him not large enough.</p><p>He was ready to throw out the array, but his mother reassured him. She told him, that array would not be spoiled after the following operation: choose any index $i$ ($1 \le i \le n$) and do $a_i := -a_i - 1$.</p><p>For example, he can change array $[3, -1, -4, 1]$ to an array $[-4, -1, 3, 1]$ after applying this operation to elements with indices $i=1$ and $i=3$. </p><p>Kolya had immediately understood that sometimes it's possible to increase the product of integers of the array a lot. Now he has decided that he wants to get an array with the maximal possible product of integers using only this operation with its elements (possibly zero, one or more times, as many as he wants), it is not forbidden to do this operation several times for the same index. </p><p>Help Kolya and print the array with the maximal possible product of elements $a_1 \cdot a_2 \cdot \dots a_n$ which can be received using only this operation in some order.</p><p>If there are multiple answers, print any of them.</p></div><div class="input-specification"><p>The first line contains integer $n$ ($1 \leq n \leq 10^{5}$)&nbsp;— number of integers in the array.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($-10^{6} \leq a_i \leq 10^{6}$)&nbsp;— elements of the array</p></div><div class="output-specification"><p>Print $n$ numbers&nbsp;— elements of the array with the maximal possible product of elements which can be received using only this operation in some order from the given array.</p><p>If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line contains integer $n$ ($1 \leq n \leq 10^{5}$)&nbsp;— number of integers in the array.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($-10^{6} \leq a_i \leq 10^{6}$)&nbsp;— elements of the array</p>

## Output

<p>Print $n$ numbers&nbsp;— elements of the array with the maximal possible product of elements which can be received using only this operation in some order from the given array.</p><p>If there are multiple answers, print any of them.</p>





```input1
4
2 2 2 2
```




```input2
1
0
```




```input3
3
-3 -3 2
```




```output1
-3 -3 -3 -3
```




```output2
0
```




```output3
-3 -3 2
```


