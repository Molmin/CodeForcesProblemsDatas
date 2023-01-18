## Description

<div><p>Petya and Vasya are brothers. Today is a special day for them as their parents left them home alone and commissioned them to do <span class="tex-span"><i>n</i></span> chores. Each chore is characterized by a single parameter — its complexity. The complexity of the <span class="tex-span"><i>i</i></span>-th chore equals <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>As Petya is older, he wants to take the chores with complexity larger than some value <span class="tex-span"><i>x</i></span> (<span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub> &gt; <i>x</i></span>) to leave to Vasya the chores with complexity less than or equal to <span class="tex-span"><i>x</i></span> (<span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub> ≤ <i>x</i></span>). The brothers have already decided that Petya will do exactly <span class="tex-span"><i>a</i></span> chores and Vasya will do exactly <span class="tex-span"><i>b</i></span> chores (<span class="tex-span"><i>a</i> + <i>b</i> = <i>n</i></span>).</p><p>In how many ways can they choose an integer <span class="tex-span"><i>x</i></span> so that Petya got exactly <span class="tex-span"><i>a</i></span> chores and Vasya got exactly <span class="tex-span"><i>b</i></span> chores?</p></div><div class="input-specification"><p>The first input line contains three integers <span class="tex-span"><i>n</i>, <i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2000</span>; <span class="tex-span"><i>a</i>, <i>b</i> ≥ 1</span>; <span class="tex-span"><i>a</i> + <i>b</i> = <i>n</i></span>) — the total number of chores, the number of Petya's chores and the number of Vasya's chores.</p><p>The next line contains a sequence of integers <span class="tex-span"><i>h</i><sub class="lower-index">1</sub>, <i>h</i><sub class="lower-index">2</sub>, ..., <i>h</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> is the complexity of the <span class="tex-span"><i>i</i></span>-th chore. The numbers in the given sequence are not necessarily different.</p><p>All numbers on the lines are separated by single spaces.</p></div><div class="output-specification"><p>Print the required number of ways to choose an integer value of <span class="tex-span"><i>x</i></span>. If there are no such ways, print <span class="tex-font-style-tt">0</span>.</p></div>

## Input

<p>The first input line contains three integers <span class="tex-span"><i>n</i>, <i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2000</span>; <span class="tex-span"><i>a</i>, <i>b</i> ≥ 1</span>; <span class="tex-span"><i>a</i> + <i>b</i> = <i>n</i></span>) — the total number of chores, the number of Petya's chores and the number of Vasya's chores.</p><p>The next line contains a sequence of integers <span class="tex-span"><i>h</i><sub class="lower-index">1</sub>, <i>h</i><sub class="lower-index">2</sub>, ..., <i>h</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> is the complexity of the <span class="tex-span"><i>i</i></span>-th chore. The numbers in the given sequence are not necessarily different.</p><p>All numbers on the lines are separated by single spaces.</p>

## Output

<p>Print the required number of ways to choose an integer value of <span class="tex-span"><i>x</i></span>. If there are no such ways, print <span class="tex-font-style-tt">0</span>.</p>





```input1
5 2 3
6 2 3 100 1

```




```input2
7 3 4
1 1 9 1 1 1 1

```




```output1
3

```




```output2
0

```



## Note

<p>In the first sample the possible values of <span class="tex-span"><i>x</i></span> are 3, 4 or 5.</p><p>In the second sample it is impossible to find such <span class="tex-span"><i>x</i></span>, that Petya got 3 chores and Vasya got 4.</p>
