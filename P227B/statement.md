## Description

<div><p>Once at a team training Vasya, Petya and Sasha got a problem on implementing linear search in an array.</p><p>According to the boys, linear search works as follows. The array elements in a pre-selected order are in turn compared with the number that you need to find. Once you find the array element that is equal to the required one, the search ends. The efficiency of the algorithm is the number of performed comparisons. The fewer comparisons the linear search has made, the more effective it is.</p><p>Vasya believes that a linear search would work better if it sequentially iterates through the elements, starting with the <span class="tex-span">1</span>-st one (in this problem we consider the elements of the array indexed from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>) and ending with the <span class="tex-span"><i>n</i></span>-th one. And Petya says that Vasya is wrong: the search will need less comparisons if it sequentially iterates the elements starting from the <span class="tex-span"><i>n</i></span>-th and ending with the <span class="tex-span">1</span>-st one. Sasha argues that the two approaches are equivalent.</p><p>To finally begin the task, the teammates decided to settle the debate and compare the two approaches on an example. For this, they took an array that is a permutation of integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, and generated <span class="tex-span"><i>m</i></span> queries of the form: find element with value <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> in the array. They want to calculate for both approaches how many comparisons in total the linear search will need to respond to all queries. If the first search needs fewer comparisons, then the winner of the dispute is Vasya. If the second one does, then the winner is Petya. If both approaches make the same number of comparisons, then Sasha's got the upper hand.</p><p>But the problem is, linear search is too slow. That's why the boys aren't going to find out who is right before the end of the training, unless you come in here. Help them to determine who will win the dispute.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of elements in the array. The second line contains <span class="tex-span"><i>n</i></span> distinct space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the elements of array. </p><p>The third line contains integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of queries. The last line contains <span class="tex-span"><i>m</i></span> space-separated integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub></span> <span class="tex-span">(1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the search queries. Note that the queries can repeat.</p></div><div class="output-specification"><p>Print two integers, showing how many comparisons Vasya's approach needs and how many comparisons Petya's approach needs. Separate the numbers by spaces.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of elements in the array. The second line contains <span class="tex-span"><i>n</i></span> distinct space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the elements of array. </p><p>The third line contains integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of queries. The last line contains <span class="tex-span"><i>m</i></span> space-separated integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub></span> <span class="tex-span">(1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the search queries. Note that the queries can repeat.</p>

## Output

<p>Print two integers, showing how many comparisons Vasya's approach needs and how many comparisons Petya's approach needs. Separate the numbers by spaces.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
2
1 2
1
1

```




```input2
2
2 1
1
1

```




```input3
3
3 1 2
3
1 2 3

```




```output1
1 2

```




```output2
2 1

```




```output3
6 6

```



## Note

<p>In the first sample Vasya's approach will make one comparison (it starts with the <span class="tex-span">1</span>-st element and immediately finds the required number), and Petya's approach makes two comparisons (first he compares with the <span class="tex-span">2</span>-nd array element, doesn't find the search item and compares with the <span class="tex-span">1</span>-st element).</p><p>In the second sample, on the contrary, Vasya's approach will need two comparisons (first with <span class="tex-span">1</span>-st element, and then with the <span class="tex-span">2</span>-nd), and Petya's approach will find the required value in one comparison (the first comparison with the <span class="tex-span">2</span>-nd element).</p>
