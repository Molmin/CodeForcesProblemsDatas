## Description

<div><p>The life goes up and down, just like nice sequences. Sequence <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> is called <span class="tex-font-style-it">nice</span> if the following two conditions are satisfied: </p><ul> <li> <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> &lt; <i>t</i><sub class="lower-index"><i>i</i> + 1</sub></span> for each odd <span class="tex-span"><i>i</i> &lt; <i>n</i></span>; </li><li> <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> &gt; <i>t</i><sub class="lower-index"><i>i</i> + 1</sub></span> for each even <span class="tex-span"><i>i</i> &lt; <i>n</i></span>. </li></ul><p>For example, sequences <span class="tex-span">(2, 8)</span>, <span class="tex-span">(1, 5, 1)</span> and <span class="tex-span">(2, 5, 1, 100, 99, 120)</span> are nice, while <span class="tex-span">(1, 1)</span>, <span class="tex-span">(1, 2, 3)</span> and <span class="tex-span">(2, 5, 3, 2)</span> are not.</p><p>Bear Limak has a sequence of positive integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span>. This sequence <span class="tex-font-style-bf">is not nice</span> now and Limak wants to fix it by a single swap. He is going to choose two indices <span class="tex-span"><i>i</i> &lt; <i>j</i></span> and swap elements <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>j</i></sub></span> in order to get a nice sequence. Count the number of ways to do so. Two ways are considered different if indices of elements chosen for a swap are different.</p></div><div class="input-specification"><p>The first line of the input contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 150 000</span>)&nbsp;— the length of the sequence.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 150 000</span>) — the initial sequence. It's guaranteed that the given sequence is not nice.</p></div><div class="output-specification"><p>Print the number of ways to swap two elements exactly once in order to get a nice sequence.</p></div>

## Input

<p>The first line of the input contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 150 000</span>)&nbsp;— the length of the sequence.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 150 000</span>) — the initial sequence. It's guaranteed that the given sequence is not nice.</p>

## Output

<p>Print the number of ways to swap two elements exactly once in order to get a nice sequence.</p>





```input1
5
2 8 4 7 7

```




```input2
4
200 150 100 50

```




```input3
10
3 2 1 4 1 4 1 4 1 4

```




```input4
9
1 2 3 4 5 6 7 8 9

```




```output1
2

```




```output2
1

```




```output3
8

```




```output4
0

```



## Note

<p>In the first sample, there are two ways to get a nice sequence with one swap: </p><ol> <li> Swap <span class="tex-span"><i>t</i><sub class="lower-index">2</sub> = 8</span> with <span class="tex-span"><i>t</i><sub class="lower-index">4</sub> = 7</span>. </li><li> Swap <span class="tex-span"><i>t</i><sub class="lower-index">1</sub> = 2</span> with <span class="tex-span"><i>t</i><sub class="lower-index">5</sub> = 7</span>. </li></ol><p>In the second sample, there is only one way&nbsp;— Limak should swap <span class="tex-span"><i>t</i><sub class="lower-index">1</sub> = 200</span> with <span class="tex-span"><i>t</i><sub class="lower-index">4</sub> = 50</span>.</p>
