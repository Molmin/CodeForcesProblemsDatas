## Description

<div><p>A smile house is created to raise the mood. It has <span class="tex-span"><i>n</i></span> rooms. Some of the rooms are connected by doors. For each two rooms (number <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span>), which are connected by a door, Petya knows their value <span class="tex-span"><i>c</i><sub class="lower-index"><i>ij</i></sub></span> — the value which is being added to his mood when he moves from room <span class="tex-span"><i>i</i></span> to room <span class="tex-span"><i>j</i></span>.</p><p>Petya wondered whether he can raise his mood infinitely, moving along some cycle? And if he can, then what minimum number of rooms he will need to visit during one period of a cycle?</p></div><div class="input-specification"><p>The first line contains two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<img align="middle" class="tex-formula" src="file://7KXJWoZC.png" style="max-width: 100.0%;max-height: 100.0%;">), where <span class="tex-span"><i>n</i></span> is the number of rooms, and <span class="tex-span"><i>m</i></span> is the number of doors in the Smile House. Then follows the description of the doors: <span class="tex-span"><i>m</i></span> lines each containing four integers <span class="tex-span"><i>i</i></span>, <span class="tex-span"><i>j</i></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>ij</i></sub></span> и <span class="tex-span"><i>c</i><sub class="lower-index"><i>ji</i></sub></span> (<span class="tex-span">1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i>, <i>i</i> ≠ <i>j</i>,  - 10<sup class="upper-index">4</sup> ≤ <i>c</i><sub class="lower-index"><i>ij</i></sub>, <i>c</i><sub class="lower-index"><i>ji</i></sub> ≤ 10<sup class="upper-index">4</sup></span>). It is guaranteed that no more than one door connects any two rooms. No door connects the room with itself.</p></div><div class="output-specification"><p>Print the minimum number of rooms that one needs to visit during one traverse of the cycle that can raise mood infinitely. If such cycle does not exist, print number <span class="tex-span">0</span>.</p></div>

## Input

<p>The first line contains two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<img align="middle" class="tex-formula" src="file://7KXJWoZC.png" style="max-width: 100.0%;max-height: 100.0%;">), where <span class="tex-span"><i>n</i></span> is the number of rooms, and <span class="tex-span"><i>m</i></span> is the number of doors in the Smile House. Then follows the description of the doors: <span class="tex-span"><i>m</i></span> lines each containing four integers <span class="tex-span"><i>i</i></span>, <span class="tex-span"><i>j</i></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>ij</i></sub></span> и <span class="tex-span"><i>c</i><sub class="lower-index"><i>ji</i></sub></span> (<span class="tex-span">1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i>, <i>i</i> ≠ <i>j</i>,  - 10<sup class="upper-index">4</sup> ≤ <i>c</i><sub class="lower-index"><i>ij</i></sub>, <i>c</i><sub class="lower-index"><i>ji</i></sub> ≤ 10<sup class="upper-index">4</sup></span>). It is guaranteed that no more than one door connects any two rooms. No door connects the room with itself.</p>

## Output

<p>Print the minimum number of rooms that one needs to visit during one traverse of the cycle that can raise mood infinitely. If such cycle does not exist, print number <span class="tex-span">0</span>.</p>





```input1
4 4
1 2 -10 3
1 3 1 -10
2 4 -10 -1
3 4 0 -3

```




```output1
4

```



## Note

<p>Cycle is such a sequence of rooms <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>k</i></sub></span>, that <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> is connected with <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span> is connected with <span class="tex-span"><i>a</i><sub class="lower-index">3</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>k</i> - 1</sub></span> is connected with <span class="tex-span"><i>a</i><sub class="lower-index"><i>k</i></sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>k</i></sub></span> is connected with <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>. Some elements of the sequence can coincide, that is, the cycle should not necessarily be simple. The number of rooms in the cycle is considered as <span class="tex-span"><i>k</i></span>, the sequence's length. Note that the minimum possible length equals two.</p>
