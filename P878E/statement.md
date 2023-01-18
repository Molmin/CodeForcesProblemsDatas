## Description

<div><p>A sequence of <span class="tex-span"><i>n</i></span> integers is written on a blackboard. Soon Sasha will come to the blackboard and start the following actions: let <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> be two adjacent numbers (<span class="tex-span"><i>x</i></span> before <span class="tex-span"><i>y</i></span>), then he can remove them and write <span class="tex-span"><i>x</i> + 2<i>y</i></span> instead of them. He will perform these operations until one number is left. Sasha likes big numbers and will get the biggest possible number.</p><p>Nikita wants to get to the blackboard before Sasha and erase some of the numbers. He has <span class="tex-span"><i>q</i></span> options, in the option <span class="tex-span"><i>i</i></span> he erases all numbers to the left of the <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>-th number and all numbers to the right of <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>-th number, i.&nbsp;e. all numbers between the <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>-th and the <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>-th, inclusive, remain on the blackboard. For each of the options he wants to know how big Sasha's final number is going to be. This number can be very big, so output it modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of integers on the blackboard and the number of Nikita's options.</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the sequence on the blackboard.</p><p>Each of the next <span class="tex-span"><i>q</i></span> lines contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), describing Nikita's options.</p></div><div class="output-specification"><p>For each option output Sasha's result modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of integers on the blackboard and the number of Nikita's options.</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the sequence on the blackboard.</p><p>Each of the next <span class="tex-span"><i>q</i></span> lines contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), describing Nikita's options.</p>

## Output

<p>For each option output Sasha's result modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
3 3
1 2 3
1 3
1 2
2 3

```




```input2
3 1
1 2 -3
1 3

```




```input3
4 2
1 1 1 -1
1 4
3 4

```




```output1
17
5
8

```




```output2
1000000006

```




```output3
5
1000000006

```



## Note

<p>In the second sample Nikita doesn't erase anything. Sasha first erases the numbers <span class="tex-span">1</span> and <span class="tex-span">2</span> and writes <span class="tex-span">5</span>. Then he erases <span class="tex-span">5</span> and <span class="tex-font-style-tt">-3</span> and gets <span class="tex-font-style-tt">-1</span>. <span class="tex-font-style-tt">-1</span> modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span> is <span class="tex-span">10<sup class="upper-index">9</sup> + 6</span>.</p>
