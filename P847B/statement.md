## Description

<div><p>Ivan has an array consisting of <span class="tex-span"><i>n</i></span> different integers. He decided to reorder all elements in increasing order. Ivan loves merge sort so he decided to represent his array with one or several increasing sequences which he then plans to merge into one sorted array.</p><p>Ivan represent his array with increasing sequences with help of the following algorithm.</p><p>While there is at least one unused number in array Ivan repeats the following procedure:</p><ul> <li> iterate through array from the left to the right; </li><li> Ivan only looks at unused numbers on current iteration; </li><li> if current number is the first unused number on this iteration or this number is greater than previous unused number on current iteration, then Ivan marks the number as used and writes it down. </li></ul><p>For example, if Ivan's array looks like <span class="tex-font-style-tt">[1, 3, 2, 5, 4]</span> then he will perform two iterations. On first iteration Ivan will use and write numbers <span class="tex-font-style-tt">[1, 3, 5]</span>, and on second one — <span class="tex-font-style-tt">[2, 4]</span>.</p><p>Write a program which helps Ivan and finds representation of the given array with one or several increasing sequences in accordance with algorithm described above.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of elements in Ivan's array.</p><p>The second line contains a sequence consisting of distinct integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — Ivan's array.</p></div><div class="output-specification"><p>Print representation of the given array in the form of one or more increasing sequences in accordance with the algorithm described above. Each sequence must be printed on a new line.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of elements in Ivan's array.</p><p>The second line contains a sequence consisting of distinct integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — Ivan's array.</p>

## Output

<p>Print representation of the given array in the form of one or more increasing sequences in accordance with the algorithm described above. Each sequence must be printed on a new line.</p>





```input1
5
1 3 2 5 4

```




```input2
4
4 3 2 1

```




```input3
4
10 30 50 101

```




```output1
1 3 5 
2 4 

```




```output2
4 
3 
2 
1 

```




```output3
10 30 50 101 

```


