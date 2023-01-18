## Description

<div><p><span class="tex-font-style-underline">Petya loves lucky numbers very much. Everybody knows that lucky numbers are positive integers whose decimal record contains only the lucky digits <span class="tex-font-style-bf">4</span> and <span class="tex-font-style-bf">7</span>. For example, numbers <span class="tex-font-style-bf">47</span>, <span class="tex-font-style-bf">744</span>, <span class="tex-font-style-bf">4</span> are lucky and <span class="tex-font-style-bf">5</span>, <span class="tex-font-style-bf">17</span>, <span class="tex-font-style-bf">467</span> are not.</span></p><p>Petya has an array <span class="tex-span"><i>a</i></span> of <span class="tex-span"><i>n</i></span> integers. The numbers in the array are numbered starting from <span class="tex-span">1</span>. Unfortunately, Petya has been misbehaving and so, his parents don't allow him play with arrays that have many lucky numbers. It is guaranteed that no more than <span class="tex-span">1000</span> elements in the array <span class="tex-span"><i>a</i></span> are lucky numbers. </p><p>Petya needs to find the number of pairs of non-intersecting segments <span class="tex-span">[<i>l</i><sub class="lower-index">1</sub>;<i>r</i><sub class="lower-index">1</sub>]</span> and <span class="tex-span">[<i>l</i><sub class="lower-index">2</sub>;<i>r</i><sub class="lower-index">2</sub>]</span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index">1</sub> ≤ <i>r</i><sub class="lower-index">1</sub> &lt; <i>l</i><sub class="lower-index">2</sub> ≤ <i>r</i><sub class="lower-index">2</sub> ≤ <i>n</i></span>, all four numbers are integers) such that there's no such lucky number that occurs simultaneously in the subarray <span class="tex-span"><i>a</i>[<i>l</i><sub class="lower-index">1</sub>..<i>r</i><sub class="lower-index">1</sub>]</span> and in the subarray <span class="tex-span"><i>a</i>[<i>l</i><sub class="lower-index">2</sub>..<i>r</i><sub class="lower-index">2</sub>]</span>. Help Petya count the number of such pairs.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the size of the array <span class="tex-span"><i>a</i></span>. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — array <span class="tex-span"><i>a</i></span>. It is guaranteed that no more than <span class="tex-span">1000</span> elements in the array <span class="tex-span"><i>a</i></span> are lucky numbers. </p></div><div class="output-specification"><p>On the single line print the only number — the answer to the problem.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specificator.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the size of the array <span class="tex-span"><i>a</i></span>. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — array <span class="tex-span"><i>a</i></span>. It is guaranteed that no more than <span class="tex-span">1000</span> elements in the array <span class="tex-span"><i>a</i></span> are lucky numbers. </p>

## Output

<p>On the single line print the only number — the answer to the problem.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specificator.</p>





```input1
4
1 4 2 4

```




```input2
2
4 7

```




```input3
4
4 4 7 7

```




```output1
9

```




```output2
1

```




```output3
9

```



## Note

<p>The subarray <span class="tex-span"><i>a</i>[<i>l</i>..<i>r</i>]</span> is an array that consists of elements <span class="tex-span"><i>a</i><sub class="lower-index"><i>l</i></sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>l</i> + 1</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>r</i></sub></span>.</p><p>In the first sample there are <span class="tex-span">9</span> possible pairs that satisfy the condition: <span class="tex-span">[1, 1]</span> and <span class="tex-span">[2, 2]</span>, <span class="tex-span">[1, 1]</span> and <span class="tex-span">[2, 3]</span>, <span class="tex-span">[1, 1]</span> and <span class="tex-span">[2, 4]</span>, <span class="tex-span">[1, 1]</span> and <span class="tex-span">[3, 3]</span>, <span class="tex-span">[1, 1]</span> and <span class="tex-span">[3, 4]</span>, <span class="tex-span">[1, 1]</span> and <span class="tex-span">[4, 4]</span>, <span class="tex-span">[1, 2]</span> and <span class="tex-span">[3, 3]</span>, <span class="tex-span">[2, 2]</span> and <span class="tex-span">[3, 3]</span>, <span class="tex-span">[3, 3]</span> and <span class="tex-span">[4, 4]</span>.</p><p>In the second sample there is only one pair of segments — <span class="tex-span">[1;1]</span> and <span class="tex-span">[2;2]</span> and it satisfies the condition.</p>
