## Description

<div><p>You've got a positive integer sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. All numbers in the sequence are distinct. Let's fix the set of variables <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub></span>. Initially each variable <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>m</i>)</span> contains the value of zero. Consider the following sequence, consisting of <span class="tex-span"><i>n</i></span> operations.</p><p>The first operation is assigning the value of <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> to some variable <span class="tex-span"><i>b</i><sub class="lower-index"><i>x</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i> ≤ <i>m</i>)</span>. Each of the following <span class="tex-span"><i>n</i> - 1</span> operations is assigning to some variable <span class="tex-span"><i>b</i><sub class="lower-index"><i>y</i></sub></span> the value that is equal to the sum of values that are stored in the variables <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span> <span class="tex-span">(1 ≤ <i>i</i>, <i>j</i>, <i>y</i> ≤ <i>m</i>)</span>. At that, the value that is assigned on the <span class="tex-span"><i>t</i></span>-th operation, must equal <span class="tex-span"><i>a</i><sub class="lower-index"><i>t</i></sub></span>. For each operation numbers <span class="tex-span"><i>y</i>, <i>i</i>, <i>j</i></span> are chosen anew.</p><p>Your task is to find the minimum number of variables <span class="tex-span"><i>m</i></span>, such that those variables can help you perform the described sequence of operations.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 23)</span>. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>k</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p><p>It is guaranteed that all numbers in the sequence are distinct.</p></div><div class="output-specification"><p>In a single line print a single number — the minimum number of variables <span class="tex-span"><i>m</i></span>, such that those variables can help you perform the described sequence of operations.</p><p>If you cannot perform the sequence of operations at any <span class="tex-span"><i>m</i></span>, print <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 23)</span>. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>k</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p><p>It is guaranteed that all numbers in the sequence are distinct.</p>

## Output

<p>In a single line print a single number — the minimum number of variables <span class="tex-span"><i>m</i></span>, such that those variables can help you perform the described sequence of operations.</p><p>If you cannot perform the sequence of operations at any <span class="tex-span"><i>m</i></span>, print <span class="tex-font-style-tt">-1</span>.</p>





```input1
5
1 2 3 6 8

```




```input2
3
3 6 5

```




```input3
6
2 4 8 6 10 18

```




```output1
2

```




```output2
-1

```




```output3
3

```



## Note

<p>In the first sample, you can use two variables <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index">2</sub></span> to perform the following sequence of operations.</p><ol> <li> <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span> <span class="tex-font-style-tt">:=</span> <span class="tex-span">1</span>; </li><li> <span class="tex-span"><i>b</i><sub class="lower-index">2</sub></span> <span class="tex-font-style-tt">:=</span> <span class="tex-span"><i>b</i><sub class="lower-index">1</sub> + <i>b</i><sub class="lower-index">1</sub></span>; </li><li> <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span> <span class="tex-font-style-tt">:=</span> <span class="tex-span"><i>b</i><sub class="lower-index">1</sub> + <i>b</i><sub class="lower-index">2</sub></span>; </li><li> <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span> <span class="tex-font-style-tt">:=</span> <span class="tex-span"><i>b</i><sub class="lower-index">1</sub> + <i>b</i><sub class="lower-index">1</sub></span>; </li><li> <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span> <span class="tex-font-style-tt">:=</span> <span class="tex-span"><i>b</i><sub class="lower-index">1</sub> + <i>b</i><sub class="lower-index">2</sub></span>. </li></ol>
