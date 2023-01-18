## Description

<div><p>Berland National Library has recently been built in the capital of Berland. In addition, in the library you can take any of the collected works of Berland leaders, the library has a <span class="tex-font-style-it">reading room</span>.</p><p>Today was the pilot launch of an automated reading room visitors' accounting system! The scanner of the system is installed at the entrance to the reading room. It records the events of the form "reader entered room", "reader left room". Every reader is assigned a <span class="tex-font-style-it">registration number</span> during the registration procedure at the library — it's a unique integer from <span class="tex-span">1</span> to <span class="tex-span">10<sup class="upper-index">6</sup></span>. Thus, the system logs events of two forms:</p><ul> <li> "<span class="tex-font-style-tt">+</span> <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>" — the reader with registration number <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> entered the room; </li><li> "<span class="tex-font-style-tt">-</span> <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>" — the reader with registration number <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> left the room. </li></ul><p>The first launch of the system was a success, it functioned for some period of time, and, at the time of its launch and at the time of its shutdown, the reading room may already have visitors.</p><p>Significant funds of the budget of Berland have been spent on the design and installation of the system. Therefore, some of the citizens of the capital now demand to explain the need for this system and the benefits that its implementation will bring. Now, the developers of the system need to urgently come up with reasons for its existence.</p><p>Help the system developers to find the minimum possible capacity of the reading room (in visitors) using the log of the system available to you.</p></div><div class="input-specification"><p>The first line contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of records in the system log. Next follow <span class="tex-span"><i>n</i></span> events from the system journal in the order in which the were made. Each event was written on a single line and looks as "<span class="tex-font-style-tt">+</span> <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>" or "<span class="tex-font-style-tt">-</span> <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>", where <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> is an integer from <span class="tex-span">1</span> to <span class="tex-span">10<sup class="upper-index">6</sup></span>, the registration number of the visitor (that is, distinct visitors always have distinct registration numbers).</p><p>It is guaranteed that the log is not contradictory, that is, for every visitor the types of any of his two consecutive events are distinct. Before starting the system, and after stopping the room may possibly contain visitors.</p></div><div class="output-specification"><p>Print a single integer — the minimum possible capacity of the reading room.</p></div>

## Input

<p>The first line contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of records in the system log. Next follow <span class="tex-span"><i>n</i></span> events from the system journal in the order in which the were made. Each event was written on a single line and looks as "<span class="tex-font-style-tt">+</span> <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>" or "<span class="tex-font-style-tt">-</span> <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>", where <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> is an integer from <span class="tex-span">1</span> to <span class="tex-span">10<sup class="upper-index">6</sup></span>, the registration number of the visitor (that is, distinct visitors always have distinct registration numbers).</p><p>It is guaranteed that the log is not contradictory, that is, for every visitor the types of any of his two consecutive events are distinct. Before starting the system, and after stopping the room may possibly contain visitors.</p>

## Output

<p>Print a single integer — the minimum possible capacity of the reading room.</p>





```input1
6
+ 12001
- 12001
- 1
- 1200
+ 1
+ 7

```




```input2
2
- 1
- 2

```




```input3
2
+ 1
- 1

```




```output1
3
```




```output2
2
```




```output3
1
```



## Note

<p>In the first sample test, the system log will ensure that at some point in the reading room were visitors with registration numbers <span class="tex-span">1</span>, <span class="tex-span">1200</span> and <span class="tex-span">12001</span>. More people were not in the room at the same time based on the log. Therefore, the answer to the test is 3.</p>
