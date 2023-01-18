## Description

<div><p>Sereja has got an array, consisting of <span class="tex-span"><i>n</i></span> integers, <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. Sereja is an active boy, so he is now going to complete <span class="tex-span"><i>m</i></span> operations. Each operation will have one of the three forms:</p><ol> <li> Make <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>-th array element equal to <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>. In other words, perform the assignment <span class="tex-span"><i>a</i><sub class="lower-index"><i>v</i><sub class="lower-index"><i>i</i></sub></sub> = <i>x</i><sub class="lower-index"><i>i</i></sub></span>. </li><li> Increase each array element by <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>. In other words, perform <span class="tex-span"><i>n</i></span> assignments <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = <i>a</i><sub class="lower-index"><i>i</i></sub> + <i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>n</i>)</span>. </li><li> Take a piece of paper and write out the <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span>-th array element. That is, the element <span class="tex-span"><i>a</i><sub class="lower-index"><i>q</i><sub class="lower-index"><i>i</i></sub></sub></span>. </li></ol><p>Help Sereja, complete all his operations.</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> — the original array.</p><p>Next <span class="tex-span"><i>m</i></span> lines describe operations, the <span class="tex-span"><i>i</i></span>-th line describes the <span class="tex-span"><i>i</i></span>-th operation. The first number in the <span class="tex-span"><i>i</i></span>-th line is integer <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 3)</span> that represents the operation type. If <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 1</span>, then it is followed by two integers <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span">(1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>. If <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 2</span>, then it is followed by integer <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup>)</span>. And if <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 3</span>, then it is followed by integer <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>q</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>.</p></div><div class="output-specification"><p>For each third type operation print value <span class="tex-span"><i>a</i><sub class="lower-index"><i>q</i><sub class="lower-index"><i>i</i></sub></sub></span>. Print the values in the order, in which the corresponding queries follow in the input.</p></div>

## Input

<p>The first line contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> — the original array.</p><p>Next <span class="tex-span"><i>m</i></span> lines describe operations, the <span class="tex-span"><i>i</i></span>-th line describes the <span class="tex-span"><i>i</i></span>-th operation. The first number in the <span class="tex-span"><i>i</i></span>-th line is integer <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 3)</span> that represents the operation type. If <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 1</span>, then it is followed by two integers <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span">(1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>. If <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 2</span>, then it is followed by integer <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup>)</span>. And if <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 3</span>, then it is followed by integer <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>q</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>.</p>

## Output

<p>For each third type operation print value <span class="tex-span"><i>a</i><sub class="lower-index"><i>q</i><sub class="lower-index"><i>i</i></sub></sub></span>. Print the values in the order, in which the corresponding queries follow in the input.</p>





```input1
10 11
1 2 3 4 5 6 7 8 9 10
3 2
3 9
2 10
3 1
3 10
1 1 10
2 10
2 10
3 1
3 10
3 9

```




```output1
2
9
11
20
30
40
39

```


