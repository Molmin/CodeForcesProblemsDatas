## Description

<div><p>Vasya has <span class="tex-span"><i>n</i></span> items lying in a line. The items are consecutively numbered by numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> in such a way that the leftmost item has number <span class="tex-span">1</span>, the rightmost item has number <span class="tex-span"><i>n</i></span>. Each item has a weight, the <span class="tex-span"><i>i</i></span>-th item weights <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> kilograms.</p><p>Vasya needs to collect all these items, however he won't do it by himself. He uses his brand new robot. The robot has two different arms — the left one and the right one. The robot can consecutively perform the following actions: </p><ol> <li> Take the leftmost item with the left hand and spend <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub> · <i>l</i></span> energy units (<span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> is a weight of the leftmost item, <span class="tex-span"><i>l</i></span> is some parameter). If the previous action was the same (left-hand), then the robot spends extra <span class="tex-span"><i>Q</i><sub class="lower-index"><i>l</i></sub></span> energy units; </li><li> Take the rightmost item with the right hand and spend <span class="tex-span"><i>w</i><sub class="lower-index"><i>j</i></sub> · <i>r</i></span> energy units (<span class="tex-span"><i>w</i><sub class="lower-index"><i>j</i></sub></span> is a weight of the rightmost item, <span class="tex-span"><i>r</i></span> is some parameter). If the previous action was the same (right-hand), then the robot spends extra <span class="tex-span"><i>Q</i><sub class="lower-index"><i>r</i></sub></span> energy units; </li></ol><p>Naturally, Vasya wants to program the robot in a way that the robot spends as little energy as possible. He asked you to solve this problem. Your task is to find the minimum number of energy units robot spends to collect all items.</p></div><div class="input-specification"><p>The first line contains five integers <span class="tex-span"><i>n</i>, <i>l</i>, <i>r</i>, <i>Q</i><sub class="lower-index"><i>l</i></sub>, <i>Q</i><sub class="lower-index"><i>r</i></sub></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>; 1 ≤ <i>l</i>, <i>r</i> ≤ 100; 1 ≤ <i>Q</i><sub class="lower-index"><i>l</i></sub>, <i>Q</i><sub class="lower-index"><i>r</i></sub> ≤ 10<sup class="upper-index">4</sup>)</span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>w</i><sub class="lower-index">1</sub>, <i>w</i><sub class="lower-index">2</sub>, ..., <i>w</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 100)</span>.</p></div><div class="output-specification"><p>In the single line print a single number — the answer to the problem.</p></div>

## Input

<p>The first line contains five integers <span class="tex-span"><i>n</i>, <i>l</i>, <i>r</i>, <i>Q</i><sub class="lower-index"><i>l</i></sub>, <i>Q</i><sub class="lower-index"><i>r</i></sub></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>; 1 ≤ <i>l</i>, <i>r</i> ≤ 100; 1 ≤ <i>Q</i><sub class="lower-index"><i>l</i></sub>, <i>Q</i><sub class="lower-index"><i>r</i></sub> ≤ 10<sup class="upper-index">4</sup>)</span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>w</i><sub class="lower-index">1</sub>, <i>w</i><sub class="lower-index">2</sub>, ..., <i>w</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 100)</span>.</p>

## Output

<p>In the single line print a single number — the answer to the problem.</p>





```input1
3 4 4 19 1
42 3 99

```




```input2
4 7 2 3 9
1 2 3 4

```




```output1
576

```




```output2
34

```



## Note

<p>Consider the first sample. As <span class="tex-span"><i>l</i> = <i>r</i></span>, we can take an item in turns: first from the left side, then from the right one and last item from the left. In total the robot spends <span class="tex-span">4·42 + 4·99 + 4·3 = 576</span> energy units.</p><p>The second sample. The optimal solution is to take one item from the right, then one item from the left and two items from the right. In total the robot spends <span class="tex-span">(2·4) + (7·1) + (2·3) + (2·2 + 9) = 34</span> energy units.</p>
