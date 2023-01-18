## Description

<div><p>Sonya was unable to think of a story for this problem, so here comes the formal description.</p><p>You are given the array containing <span class="tex-span"><i>n</i></span> positive integers. At one turn you can pick any element and increase or decrease it by <span class="tex-span">1</span>. The goal is the make the array strictly increasing by making the minimum possible number of operations. You are allowed to change elements in any way, they can become negative or equal to <span class="tex-span">0</span>.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3000</span>)&nbsp;— the length of the array.</p><p>Next line contains <span class="tex-span"><i>n</i></span> integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Print the minimum number of operation required to make the array strictly increasing.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3000</span>)&nbsp;— the length of the array.</p><p>Next line contains <span class="tex-span"><i>n</i></span> integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Print the minimum number of operation required to make the array strictly increasing.</p>





```input1
7
2 1 5 11 5 9 11

```




```input2
5
5 4 3 2 1

```




```output1
9

```




```output2
12

```



## Note

<p>In the first sample, the array is going to look as follows:</p><p><span class="tex-span">2</span> <span class="tex-span">3</span> <span class="tex-span">5</span> <span class="tex-span">6</span> <span class="tex-span">7</span> <span class="tex-span">9</span> <span class="tex-span">11</span></p><p><span class="tex-span">|2 - 2| + |1 - 3| + |5 - 5| + |11 - 6| + |5 - 7| + |9 - 9| + |11 - 11| = 9</span></p><p>And for the second sample:</p><p><span class="tex-span">1</span> <span class="tex-span">2</span> <span class="tex-span">3</span> <span class="tex-span">4</span> <span class="tex-span">5</span></p><p><span class="tex-span">|5 - 1| + |4 - 2| + |3 - 3| + |2 - 4| + |1 - 5| = 12</span></p>
