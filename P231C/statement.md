## Description

<div><p>A piece of paper contains an array of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. Your task is to find a number that occurs the maximum number of times in this array.</p><p>However, before looking for such number, you are allowed to perform not more than <span class="tex-span"><i>k</i></span> following operations — choose an arbitrary element from the array and add <span class="tex-span">1</span> to it. In other words, you are allowed to increase some array element by <span class="tex-span">1</span> no more than <span class="tex-span"><i>k</i></span> times (you are allowed to increase the same element of the array multiple times).</p><p>Your task is to find the maximum number of occurrences of some number in the array after performing no more than <span class="tex-span"><i>k</i></span> allowed operations. If there are several such numbers, your task is to find the minimum one.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>; <span class="tex-span">0 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>) — the number of elements in the array and the number of operations you are allowed to perform, correspondingly.</p><p>The third line contains a sequence of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(|<i>a</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup>)</span> — the initial array. The numbers in the lines are separated by single spaces.</p></div><div class="output-specification"><p>In a single line print two numbers — the maximum number of occurrences of some number in the array after at most <span class="tex-span"><i>k</i></span> allowed operations are performed, and the minimum number that reaches the given maximum. Separate the printed numbers by whitespaces.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>; <span class="tex-span">0 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>) — the number of elements in the array and the number of operations you are allowed to perform, correspondingly.</p><p>The third line contains a sequence of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(|<i>a</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup>)</span> — the initial array. The numbers in the lines are separated by single spaces.</p>

## Output

<p>In a single line print two numbers — the maximum number of occurrences of some number in the array after at most <span class="tex-span"><i>k</i></span> allowed operations are performed, and the minimum number that reaches the given maximum. Separate the printed numbers by whitespaces.</p>





```input1
5 3
6 3 4 0 2

```




```input2
3 4
5 5 5

```




```input3
5 3
3 1 2 2 1

```




```output1
3 4

```




```output2
3 5

```




```output3
4 2

```



## Note

<p>In the first sample your task is to increase the second element of the array once and increase the fifth element of the array twice. Thus, we get sequence <span class="tex-span">6, 4, 4, 0, 4</span>, where number <span class="tex-span">4</span> occurs <span class="tex-span">3</span> times.</p><p>In the second sample you don't need to perform a single operation or increase each element by one. If we do nothing, we get array <span class="tex-span">5, 5, 5</span>, if we increase each by one, we get <span class="tex-span">6, 6, 6</span>. In both cases the maximum number of occurrences equals <span class="tex-span">3</span>. So we should do nothing, as number <span class="tex-span">5</span> is less than number <span class="tex-span">6</span>.</p><p>In the third sample we should increase the second array element once and the fifth element once. Thus, we get sequence <span class="tex-span">3, 2, 2, 2, 2</span>, where number <span class="tex-span">2</span> occurs <span class="tex-span">4</span> times.</p>
