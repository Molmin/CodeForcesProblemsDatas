## Description

<div><p>Bizon the Champion isn't just friendly, he also is a rigorous coder.</p><p>Let's define function <span class="tex-span"><i>f</i>(<i>a</i>)</span>, where <span class="tex-span"><i>a</i></span> is a sequence of integers. Function <span class="tex-span"><i>f</i>(<i>a</i>)</span> returns the following sequence: first all divisors of <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> go in the increasing order, then all divisors of <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span> go in the increasing order, and so on till the last element of sequence <span class="tex-span"><i>a</i></span>. For example, <span class="tex-span"><i>f</i>([2, 9, 1]) = [1, 2, 1, 3, 9, 1]</span>.</p><p>Let's determine the sequence <span class="tex-span"><i>X</i><sub class="lower-index"><i>i</i></sub></span>, for integer <span class="tex-span"><i>i</i></span> <span class="tex-span">(<i>i</i> ≥ 0)</span>: <span class="tex-span"><i>X</i><sub class="lower-index">0</sub> = [<i>X</i>]</span> (<span class="tex-span">[<i>X</i>]</span> is a sequence consisting of a single number <span class="tex-span"><i>X</i></span>), <span class="tex-span"><i>X</i><sub class="lower-index"><i>i</i></sub> = <i>f</i>(<i>X</i><sub class="lower-index"><i>i</i> - 1</sub>)</span> <span class="tex-span">(<i>i</i> &gt; 0)</span>. For example, at <span class="tex-span"><i>X</i> = 6</span> we get <span class="tex-span"><i>X</i><sub class="lower-index">0</sub> = [6]</span>, <span class="tex-span"><i>X</i><sub class="lower-index">1</sub> = [1, 2, 3, 6]</span>, <span class="tex-span"><i>X</i><sub class="lower-index">2</sub> = [1, 1, 2, 1, 3, 1, 2, 3, 6]</span>.</p><p>Given the numbers <span class="tex-span"><i>X</i></span> and <span class="tex-span"><i>k</i></span>, find the sequence <span class="tex-span"><i>X</i><sub class="lower-index"><i>k</i></sub></span>. As the answer can be rather large, find only the first <span class="tex-span">10<sup class="upper-index">5</sup></span> elements of this sequence.</p></div><div class="input-specification"><p>A single line contains two space-separated integers — <span class="tex-span"><i>X</i></span> <span class="tex-span">(1 ≤ <i>X</i> ≤ 10<sup class="upper-index">12</sup>)</span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(0 ≤ <i>k</i> ≤ 10<sup class="upper-index">18</sup>)</span>.</p></div><div class="output-specification"><p>Print the elements of the sequence <span class="tex-span"><i>X</i><sub class="lower-index"><i>k</i></sub></span> in a single line, separated by a space. If the number of elements exceeds <span class="tex-span">10<sup class="upper-index">5</sup></span>, then print only the first <span class="tex-span">10<sup class="upper-index">5</sup></span> elements.</p></div>

## Input

<p>A single line contains two space-separated integers — <span class="tex-span"><i>X</i></span> <span class="tex-span">(1 ≤ <i>X</i> ≤ 10<sup class="upper-index">12</sup>)</span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(0 ≤ <i>k</i> ≤ 10<sup class="upper-index">18</sup>)</span>.</p>

## Output

<p>Print the elements of the sequence <span class="tex-span"><i>X</i><sub class="lower-index"><i>k</i></sub></span> in a single line, separated by a space. If the number of elements exceeds <span class="tex-span">10<sup class="upper-index">5</sup></span>, then print only the first <span class="tex-span">10<sup class="upper-index">5</sup></span> elements.</p>





```input1
6 1

```




```input2
4 2

```




```input3
10 3

```




```output1
1 2 3 6 

```




```output2
1 1 2 1 2 4 

```




```output3
1 1 1 2 1 1 5 1 1 2 1 5 1 2 5 10 

```


