## Description

<div><p>George has recently entered the BSUCP (Berland State University for Cool Programmers). George has a friend Alex who has also entered the university. Now they are moving into a dormitory. </p><p>George and Alex want to live in the same room. The dormitory has <span class="tex-span"><i>n</i></span> rooms in total. At the moment the <span class="tex-span"><i>i</i></span>-th room has <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> people living in it and the room can accommodate <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span> people in total (<span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>q</i><sub class="lower-index"><i>i</i></sub></span>). Your task is to count how many rooms has free place for both George and Alex.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 100)</span> — the number of rooms.</p><p>The <span class="tex-span"><i>i</i></span>-th of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>q</i><sub class="lower-index"><i>i</i></sub> ≤ 100)</span> — the number of people who already live in the <span class="tex-span"><i>i</i></span>-th room and the room's capacity.</p></div><div class="output-specification"><p>Print a single integer — the number of rooms where George and Alex can move in.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 100)</span> — the number of rooms.</p><p>The <span class="tex-span"><i>i</i></span>-th of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>q</i><sub class="lower-index"><i>i</i></sub> ≤ 100)</span> — the number of people who already live in the <span class="tex-span"><i>i</i></span>-th room and the room's capacity.</p>

## Output

<p>Print a single integer — the number of rooms where George and Alex can move in.</p>





```input1
3
1 1
2 2
3 3

```




```input2
3
1 10
0 10
10 10

```




```output1
0

```




```output2
2

```


