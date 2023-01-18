## Description

<div><p>There are <span class="tex-span"><i>n</i></span> students living in the campus. Every morning all students wake up at the same time and go to wash. There are <span class="tex-span"><i>m</i></span> rooms with wash basins. The <span class="tex-span"><i>i</i></span>-th of these rooms contains <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> wash basins. Every student independently select one the rooms with equal probability and goes to it. After all students selected their rooms, students in each room divide into queues by the number of wash basins so that the size of the largest queue is the least possible. Calculate the expected value of the size of the largest queue among all rooms.</p></div><div class="input-specification"><p>The first line contains two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 50</span>) — the amount of students and the amount of rooms. The second line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... , <i>a</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 50</span>). <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> means the amount of wash basins in the <span class="tex-span"><i>i</i></span>-th room.</p></div><div class="output-specification"><p>Output single number: the expected value of the size of the largest queue. Your answer must have an absolute or relative error less than <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p></div>

## Input

<p>The first line contains two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 50</span>) — the amount of students and the amount of rooms. The second line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... , <i>a</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 50</span>). <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> means the amount of wash basins in the <span class="tex-span"><i>i</i></span>-th room.</p>

## Output

<p>Output single number: the expected value of the size of the largest queue. Your answer must have an absolute or relative error less than <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p>





```input1
1 1
2

```




```input2
2 2
1 1

```




```input3
2 3
1 1 1

```




```input4
7 5
1 1 2 3 1

```




```output1
1.00000000000000000000

```




```output2
1.50000000000000000000

```




```output3
1.33333333333333350000

```




```output4
2.50216960000000070000

```


