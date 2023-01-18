## Description

<div><p>You are given <span class="tex-span"><i>n</i></span> sequences. Each sequence consists of positive integers, not exceeding <span class="tex-span"><i>m</i></span>. All integers in one sequence are distinct, but the same integer may appear in multiple sequences. The length of the <span class="tex-span"><i>i</i></span>-th sequence is <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Each second integers in each of the sequences are shifted by one to the left, i.e. integers at positions <span class="tex-span"><i>i</i> &gt; 1</span> go to positions <span class="tex-span"><i>i</i> - 1</span>, while the first integers becomes the last.</p><p>Each second we take the first integer of each sequence and write it down to a new array. Then, for each value <span class="tex-span"><i>x</i></span> from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> we compute the longest <span class="tex-font-style-bf">segment</span> of the array consisting of element <span class="tex-span"><i>x</i></span> only.</p><p>The above operation is performed for <span class="tex-span">10<sup class="upper-index">100</sup></span> seconds. For each integer from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> find out the longest segment found at this time.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100 000</span>)&nbsp;— the number of sequences and the maximum integer that can appear in the sequences. </p><p>Then follow <span class="tex-span"><i>n</i></span> lines providing the sequences. Each of them starts with an integer <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 40</span>)&nbsp;— the number of integers in the sequence, proceeded by <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> positive integers&nbsp;— elements of the sequence. It's guaranteed that all integers in each sequence are pairwise distinct and do not exceed <span class="tex-span"><i>m</i></span>.</p><p><span class="tex-font-style-bf">The total length</span> of all sequences doesn't exceed <span class="tex-span">200 000</span>.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> integers, the <span class="tex-span"><i>i</i></span>-th of them should be equal to the length of the longest segment of the array with all its values equal to <span class="tex-span"><i>i</i></span> during the first <span class="tex-span">10<sup class="upper-index">100</sup></span> seconds.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100 000</span>)&nbsp;— the number of sequences and the maximum integer that can appear in the sequences. </p><p>Then follow <span class="tex-span"><i>n</i></span> lines providing the sequences. Each of them starts with an integer <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 40</span>)&nbsp;— the number of integers in the sequence, proceeded by <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> positive integers&nbsp;— elements of the sequence. It's guaranteed that all integers in each sequence are pairwise distinct and do not exceed <span class="tex-span"><i>m</i></span>.</p><p><span class="tex-font-style-bf">The total length</span> of all sequences doesn't exceed <span class="tex-span">200 000</span>.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> integers, the <span class="tex-span"><i>i</i></span>-th of them should be equal to the length of the longest segment of the array with all its values equal to <span class="tex-span"><i>i</i></span> during the first <span class="tex-span">10<sup class="upper-index">100</sup></span> seconds.</p>





```input1
3 4
3 3 4 1
4 1 3 4 2
3 3 1 4

```




```input2
5 5
2 3 1
4 5 1 3 2
4 2 1 3 5
1 3
2 5 3

```




```input3
4 6
3 4 5 3
2 6 3
2 3 6
3 3 6 5

```




```output1
2
1
3
2

```




```output2
3
1
4
0
1

```




```output3
0
0
2
1
1
2

```


