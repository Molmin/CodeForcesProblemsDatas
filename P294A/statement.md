## Description

<div><p>Shaass has decided to hunt some birds. There are <span class="tex-span"><i>n</i></span> horizontal electricity wires aligned parallel to each other. Wires are numbered <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from top to bottom. On each wire there are some oskols sitting next to each other. Oskol is the name of a delicious kind of birds in Shaass's territory. Supposed there are <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> oskols sitting on the <span class="tex-span"><i>i</i></span>-th wire.</p><center> <img class="tex-graphics" src="file://bqhqF9hJ.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Sometimes Shaass shots one of the birds and the bird dies (suppose that this bird sat at the <span class="tex-span"><i>i</i></span>-th wire). Consequently all the birds on the <span class="tex-span"><i>i</i></span>-th wire to the left of the dead bird get scared and jump up on the wire number <span class="tex-span"><i>i</i> - 1</span>, if there exists no upper wire they fly away. Also all the birds to the right of the dead bird jump down on wire number <span class="tex-span"><i>i</i> + 1</span>, if there exists no such wire they fly away. </p><p>Shaass has shot <span class="tex-span"><i>m</i></span> birds. You're given the initial number of birds on each wire, tell him how many birds are sitting on each wire after the shots.</p></div><div class="input-specification"><p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span>, <span class="tex-span">(1 ≤ <i>n</i> ≤ 100)</span>. The next line contains a list of space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>, <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100)</span>. </p><p>The third line contains an integer <span class="tex-span"><i>m</i></span>, <span class="tex-span">(0 ≤ <i>m</i> ≤ 100)</span>. Each of the next <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>. The integers mean that for the <span class="tex-span"><i>i</i></span>-th time Shaass shoot the <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>-th (from left) bird on the <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>-th wire, <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 1 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub>)</span>. It's guaranteed there will be at least <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> birds on the <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>-th wire at that moment.</p></div><div class="output-specification"><p>On the <span class="tex-span"><i>i</i></span>-th line of the output print the number of birds on the <span class="tex-span"><i>i</i></span>-th wire.</p></div>

## Input

<p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span>, <span class="tex-span">(1 ≤ <i>n</i> ≤ 100)</span>. The next line contains a list of space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>, <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100)</span>. </p><p>The third line contains an integer <span class="tex-span"><i>m</i></span>, <span class="tex-span">(0 ≤ <i>m</i> ≤ 100)</span>. Each of the next <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>. The integers mean that for the <span class="tex-span"><i>i</i></span>-th time Shaass shoot the <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>-th (from left) bird on the <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>-th wire, <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 1 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub>)</span>. It's guaranteed there will be at least <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> birds on the <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>-th wire at that moment.</p>

## Output

<p>On the <span class="tex-span"><i>i</i></span>-th line of the output print the number of birds on the <span class="tex-span"><i>i</i></span>-th wire.</p>





```input1
5
10 10 10 10 10
5
2 5
3 13
2 12
1 13
4 6

```




```input2
3
2 4 1
1
2 2

```




```output1
0
12
5
0
16

```




```output2
3
0
3

```


