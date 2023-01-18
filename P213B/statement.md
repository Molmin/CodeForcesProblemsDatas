## Description

<div><p>Furik loves writing all sorts of problems, especially such that he can't solve himself. You've got one of his problems, the one Furik gave to Rubik. And Rubik asks you to solve it.</p><p>There is integer <span class="tex-span"><i>n</i></span> and array <span class="tex-span"><i>a</i></span>, consisting of ten integers, indexed by numbers from 0 to 9. Your task is to count the number of positive integers with the following properties:</p><ul> <li> the number's length does not exceed <span class="tex-span"><i>n</i></span>; </li><li> the number doesn't have leading zeroes; </li><li> digit <span class="tex-span"><i>i</i></span> <span class="tex-span">(0 ≤ <i>i</i> ≤ 9)</span> occurs in the number at least <span class="tex-span"><i>a</i>[<i>i</i>]</span> times. </li></ul></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 100)</span>. The next line contains 10 integers <span class="tex-span"><i>a</i>[0]</span>, <span class="tex-span"><i>a</i>[1]</span>, <span class="tex-span">...</span>, <span class="tex-span"><i>a</i>[9]</span> <span class="tex-span">(0 ≤ <i>a</i>[<i>i</i>] ≤ 100)</span> — elements of array <span class="tex-span"><i>a</i></span>. The numbers are separated by spaces.</p></div><div class="output-specification"><p>On a single line print the remainder of dividing the answer to the problem by <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 100)</span>. The next line contains 10 integers <span class="tex-span"><i>a</i>[0]</span>, <span class="tex-span"><i>a</i>[1]</span>, <span class="tex-span">...</span>, <span class="tex-span"><i>a</i>[9]</span> <span class="tex-span">(0 ≤ <i>a</i>[<i>i</i>] ≤ 100)</span> — elements of array <span class="tex-span"><i>a</i></span>. The numbers are separated by spaces.</p>

## Output

<p>On a single line print the remainder of dividing the answer to the problem by <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
1
0 0 0 0 0 0 0 0 0 1

```




```input2
2
1 1 0 0 0 0 0 0 0 0

```




```input3
3
1 1 0 0 0 0 0 0 0 0

```




```output1
1

```




```output2
1

```




```output3
36

```



## Note

<p>In the first sample number 9 meets the requirements.</p><p>In the second sample number 10 meets the requirements.</p><p>In the third sample numbers <span class="tex-font-style-bf">10, 110, 210, 120, 103</span> meet the requirements. There are other suitable numbers, 36 in total.</p>
