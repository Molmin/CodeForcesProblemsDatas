## Description

<div><p>One day the Codeforces round author sat exams. He had <span class="tex-span"><i>n</i></span> exams and he needed to get an integer from <span class="tex-span">2</span> to <span class="tex-span">5</span> for each exam. He will have to re-sit each failed exam, i.e. the exam that gets mark <span class="tex-span">2</span>. </p><p>The author would need to spend too much time and effort to make the sum of his marks strictly more than <span class="tex-span"><i>k</i></span>. That could have spoilt the Codeforces round. On the other hand, if the sum of his marks is strictly less than <span class="tex-span"><i>k</i></span>, the author's mum won't be pleased at all. </p><p>The Codeforces authors are very smart and they always get the mark they choose themselves. Also, the Codeforces authors just hate re-sitting exams. </p><p>Help the author and find the minimum number of exams he will have to re-sit if he passes the exams in the way that makes the sum of marks for all <span class="tex-span"><i>n</i></span> exams equal exactly <span class="tex-span"><i>k</i></span>.</p></div><div class="input-specification"><p>The single input line contains space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 250</span>) — the number of exams and the required sum of marks.</p><p>It is guaranteed that there exists a way to pass <span class="tex-span"><i>n</i></span> exams in the way that makes the sum of marks equal exactly <span class="tex-span"><i>k</i></span>.</p></div><div class="output-specification"><p>Print the single number — the minimum number of exams that the author will get a <span class="tex-span">2</span> for, considering that the sum of marks for all exams must equal <span class="tex-span"><i>k</i></span>.</p></div>

## Input

<p>The single input line contains space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 250</span>) — the number of exams and the required sum of marks.</p><p>It is guaranteed that there exists a way to pass <span class="tex-span"><i>n</i></span> exams in the way that makes the sum of marks equal exactly <span class="tex-span"><i>k</i></span>.</p>

## Output

<p>Print the single number — the minimum number of exams that the author will get a <span class="tex-span">2</span> for, considering that the sum of marks for all exams must equal <span class="tex-span"><i>k</i></span>.</p>





```input1
4 8

```




```input2
4 10

```




```input3
1 3

```




```output1
4

```




```output2
2

```




```output3
0

```



## Note

<p>In the first sample the author has to get a <span class="tex-span">2</span> for all his exams.</p><p>In the second sample he should get a <span class="tex-span">3</span> for two exams and a <span class="tex-span">2</span> for two more.</p><p>In the third sample he should get a <span class="tex-span">3</span> for one exam.</p>
