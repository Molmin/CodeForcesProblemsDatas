## Description

<div><p>Finally Fox Ciel arrived in front of her castle!</p><p>She have to type a password to enter her castle. An input device attached to her castle is a bit unusual.</p><p>The input device is a <span class="tex-span">1 × <i>n</i></span> rectangle divided into <span class="tex-span"><i>n</i></span> square panels. They are numbered <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from left to right. Each panel has a state either ON or OFF. Initially all panels are in the OFF state. She can enter her castle if and only if <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>-th, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>-th, <span class="tex-span">...</span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>k</i></sub></span>-th panels are in the ON state and other panels are in the OFF state.</p><p>She is given an array <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>l</i></sub></span>. In each move, she can perform the following operation: choose an index <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>l</i></span>), choose consecutive <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> panels, and flip the states of those panels (i.e. ON<span class="tex-span"> → </span>OFF, OFF<span class="tex-span"> → </span>ON).</p><p>Unfortunately she forgets how to type the password with only above operations. Determine the minimal number of operations required to enter her castle.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>l</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10000, 1 ≤ <i>k</i> ≤ 10, 1 ≤ <i>l</i> ≤ 100</span>), separated by single spaces.</p><p>The second line contains <span class="tex-span"><i>k</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, ..., <span class="tex-span"><i>x</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index">1</sub> &lt; <i>x</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>x</i><sub class="lower-index"><i>k</i></sub> ≤ <i>n</i></span>), separated by single spaces.</p><p>The third line contains <span class="tex-span"><i>l</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>l</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), separated by single spaces. It is possible that some elements of the array <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> are equal value.</p></div><div class="output-specification"><p>Print the minimal number of moves required to type the password. If it's impossible, print <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>l</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10000, 1 ≤ <i>k</i> ≤ 10, 1 ≤ <i>l</i> ≤ 100</span>), separated by single spaces.</p><p>The second line contains <span class="tex-span"><i>k</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, ..., <span class="tex-span"><i>x</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index">1</sub> &lt; <i>x</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>x</i><sub class="lower-index"><i>k</i></sub> ≤ <i>n</i></span>), separated by single spaces.</p><p>The third line contains <span class="tex-span"><i>l</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>l</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), separated by single spaces. It is possible that some elements of the array <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> are equal value.</p>

## Output

<p>Print the minimal number of moves required to type the password. If it's impossible, print <span class="tex-font-style-tt">-1</span>.</p>





```input1
10 8 2
1 2 3 5 6 7 8 9
3 5

```




```input2
3 2 1
1 2
3

```




```output1
2

```




```output2
-1

```



## Note

<p>One possible way to type the password in the first example is following: In the first move, choose 1st, 2nd, 3rd panels and flip those panels. In the second move, choose 5th, 6th, 7th, 8th, 9th panels and flip those panels.</p>
