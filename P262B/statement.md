## Description

<div><p>Roma works in a company that sells TVs. Now he has to prepare a report for the last year.</p><p>Roma has got a list of the company's incomes. The list is a sequence that consists of <span class="tex-span"><i>n</i></span> integers. The total income of the company is the sum of all integers in sequence. Roma decided to perform exactly <span class="tex-span"><i>k</i></span> changes of signs of several numbers in the sequence. He can also change the sign of a number one, two or more times.</p><p>The operation of changing a number's sign is the operation of multiplying this number by -<span class="tex-span">1</span>.</p><p>Help Roma perform the changes so as to make the total income of the company (the sum of numbers in the resulting sequence) maximum. Note that Roma should perform <span class="tex-font-style-bf">exactly</span> <span class="tex-span"><i>k</i></span> changes.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>k</i> ≤ 10<sup class="upper-index">5</sup>)</span>, showing, how many numbers are in the sequence and how many swaps are to be made.</p><p>The second line contains a <span class="tex-font-style-bf">non-decreasing</span> sequence, consisting of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(|<i>a</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">4</sup>)</span>.</p><p>The numbers in the lines are separated by single spaces. Please note that the given sequence is sorted in non-decreasing order.</p></div><div class="output-specification"><p>In the single line print the answer to the problem — the maximum total income that we can obtain after exactly <span class="tex-span"><i>k</i></span> changes.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>k</i> ≤ 10<sup class="upper-index">5</sup>)</span>, showing, how many numbers are in the sequence and how many swaps are to be made.</p><p>The second line contains a <span class="tex-font-style-bf">non-decreasing</span> sequence, consisting of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(|<i>a</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">4</sup>)</span>.</p><p>The numbers in the lines are separated by single spaces. Please note that the given sequence is sorted in non-decreasing order.</p>

## Output

<p>In the single line print the answer to the problem — the maximum total income that we can obtain after exactly <span class="tex-span"><i>k</i></span> changes.</p>





```input1
3 2
-1 -1 1

```




```input2
3 1
-1 -1 1

```




```output1
3

```




```output2
1

```



## Note

<p>In the first sample we can get sequence <span class="tex-font-style-tt">[1, 1, 1]</span>, thus the total income equals <span class="tex-span">3</span>.</p><p>In the second test, the optimal strategy is to get sequence <span class="tex-font-style-tt">[-1, 1, 1]</span>, thus the total income equals <span class="tex-span">1</span>.</p>
