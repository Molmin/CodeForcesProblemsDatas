## Description

<div><p>Bessie and the cows are playing with sequences and need your help. They start with a sequence, initially containing just the number 0, and perform <span class="tex-span"><i>n</i></span> operations. Each operation is one of the following:</p><ol> <li> Add the integer <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> to the first <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> elements of the sequence. </li><li> Append an integer <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> to the end of the sequence. (And hence the size of the sequence increases by 1) </li><li> Remove the last element of the sequence. So, the size of the sequence decreases by one. Note, that this operation can only be done if there are at least two elements in the sequence. </li></ol><p>After each operation, the cows would like to know the average of all the numbers in the sequence. Help them!</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i>&nbsp;(1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup>)</span> — the number of operations. The next <span class="tex-span"><i>n</i></span> lines describe the operations. Each line will start with an integer <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 3)</span>, denoting the type of the operation (see above). If <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 1</span>, it will be followed by two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>x</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(|<i>x</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">3</sup>;&nbsp;1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>)</span>. If <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 2</span>, it will be followed by a single integer <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(|<i>k</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">3</sup>)</span>. If <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 3</span>, it will not be followed by anything.</p><p>It is guaranteed that all operations are correct (don't touch nonexistent elements) and that there will always be at least one element in the sequence.</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>n</i></span> lines each containing the average of the numbers in the sequence after the corresponding operation.</p><p>The answer will be considered correct if its absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i>&nbsp;(1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup>)</span> — the number of operations. The next <span class="tex-span"><i>n</i></span> lines describe the operations. Each line will start with an integer <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 3)</span>, denoting the type of the operation (see above). If <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 1</span>, it will be followed by two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>x</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(|<i>x</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">3</sup>;&nbsp;1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>)</span>. If <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 2</span>, it will be followed by a single integer <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(|<i>k</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">3</sup>)</span>. If <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 3</span>, it will not be followed by anything.</p><p>It is guaranteed that all operations are correct (don't touch nonexistent elements) and that there will always be at least one element in the sequence.</p>

## Output

<p>Output <span class="tex-span"><i>n</i></span> lines each containing the average of the numbers in the sequence after the corresponding operation.</p><p>The answer will be considered correct if its absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
5
2 1
3
2 3
2 1
3

```




```input2
6
2 1
1 2 20
2 2
1 2 -3
3
3

```




```output1
0.500000
0.000000
1.500000
1.333333
1.500000

```




```output2
0.500000
20.500000
14.333333
12.333333
17.500000
17.000000

```



## Note

<p>In the second sample, the sequence becomes <img align="middle" class="tex-formula" src="file://5zg9VfEb.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
