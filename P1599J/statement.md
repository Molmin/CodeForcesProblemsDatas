## Description

<div><p>Bob really likes playing with arrays of numbers. That's why for his birthday, his friends bought him a really interesting machine – an array beautifier. </p><p>The array beautifier takes an array $A$ consisting of $N$ integers, and it outputs a new array $B$ of length N that it constructed based on the array given to it. The array beautifier constructs the new array in the following way: it takes two numbers <span class="tex-font-style-bf">at different indices</span> from the original array and writes their sum to the end of the new array. It does this step $N$ times - resulting in an output array of length $N$. During this process, the machine can take the same index multiple times in different steps. </p><p>Bob was very excited about the gift that his friends gave him, so he put his favorite array in the machine. However, when the machine finished, Bob was not happy with the resulting array. He misses his favorite array very much, and hopes to get it back. </p><p>Given the array that the machine outputted, help Bob find an array that could be the original array that he put in the machine. Sometimes the machine makes mistakes, so it is possible that no appropriate input array exists for the array it has outputted. In such case, let Bob know that his array is forever lost.</p></div><div class="input-specification"><p>The first line contains one positive integer $N$ ($2 \leq N \leq 10^3$) – the length of Bob's array.</p><p>The second line contains $N$ integers $B_1$, $B_2$, ..., $B_N$ ($1 \leq B_i \leq 10^6$) – the elements of the array the machine outputted.</p></div><div class="output-specification"><p>If an appropriate input array exists, print "YES", followed by the input array $A_1$, $A_2$, ..., $A_N$ ($-10^9 \leq A_i \leq 10^9$) in the next line. Otherwise, print "NO".</p></div>

## Input

<p>The first line contains one positive integer $N$ ($2 \leq N \leq 10^3$) – the length of Bob's array.</p><p>The second line contains $N$ integers $B_1$, $B_2$, ..., $B_N$ ($1 \leq B_i \leq 10^6$) – the elements of the array the machine outputted.</p>

## Output

<p>If an appropriate input array exists, print "YES", followed by the input array $A_1$, $A_2$, ..., $A_N$ ($-10^9 \leq A_i \leq 10^9$) in the next line. Otherwise, print "NO".</p>





```input1
2
5 5
```




```input2
3
1 2 3
```




```input3
3
2 4 5
```




```input4
4
1 3 5 7
```




```output1
YES
2 3
```




```output2
YES
0 1 2
```




```output3
NO
```




```output4
YES
6 -3 4 1
```


