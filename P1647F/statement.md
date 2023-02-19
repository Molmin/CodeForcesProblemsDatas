## Description

<div><p>Madoka has become too lazy to write a legend, so let's go straight to the formal description of the problem.</p><p>An array of integers $a_1, a_2, \ldots, a_n$ is called a hill if it is not empty and there is an index $i$ in it, for which the following is true: $a_1 &lt; a_2 &lt; \ldots &lt; a_i &gt; a_{i + 1} &gt; a_{i + 2} &gt; \ldots &gt; a_n$.</p><p>A sequence $x$ is a subsequence of a sequence $y$ if $x$ can be obtained from $y$ by deletion of several (possibly, zero or all) elements keeping the order of the other elements. For example, for an array $[69, 1000, 228, -7]$ the array $[1000, -7]$ is a subsequence, while $[1]$ and $[-7, 1000]$ are not.</p><p>Splitting an array into two subsequences is called good if each element belongs to exactly one subsequence, and also each of these subsequences is a hill.</p><p>You are given an array of <span class="tex-font-style-bf">distinct</span> positive integers $a_1, a_2, \ldots a_n$. It is required to find the number of different pairs of maxima of the first and second subsequences among all good splits. Two pairs that only differ in the order of elements are considered same.</p></div><div class="input-specification"><p>The first line of input contains a single integer $n$ ($2 \le n \le 5 \cdot 10^5$)&nbsp;— array size.</p><p>The second line of input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— the elements of the array. It is guaranteed that all $a_i$ are pairwise distinct.</p></div><div class="output-specification"><p>In a single line, print exactly one number&nbsp;— the number of different pairs of maxima of the first and second subsequences among all good splits.</p></div>

## Input

<p>The first line of input contains a single integer $n$ ($2 \le n \le 5 \cdot 10^5$)&nbsp;— array size.</p><p>The second line of input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— the elements of the array. It is guaranteed that all $a_i$ are pairwise distinct.</p>

## Output

<p>In a single line, print exactly one number&nbsp;— the number of different pairs of maxima of the first and second subsequences among all good splits.</p>





```input1
4
1 2 4 3
```




```input2
8
2 12 13 7 14 6 11 8
```




```input3
7
9 5 3 10 2 6 8
```




```input4
8
8 6 10 9 1 5 2 14
```




```output1
3
```




```output2
4
```




```output3
0
```




```output4
0
```



## Note

<p>In the first test case there are 3 possible pairs: $(3, 4)$, $(2, 4)$, $(1, 4)$. And they are achieved with the following partitions: $[1, 2, 3], [4]$; $[4, 3], [1, 2]$; $[1], [2, 4, 3]$</p>
