## Description

<div><p>You've got an array <span class="tex-span"><i>a</i></span>, consisting of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. You are allowed to perform two operations on this array:</p><ol> <li> Calculate the sum of current array elements on the segment <span class="tex-span">[<i>l</i>, <i>r</i>]</span>, that is, count value <span class="tex-span"><i>a</i><sub class="lower-index"><i>l</i></sub> + <i>a</i><sub class="lower-index"><i>l</i> + 1</sub> + ... + <i>a</i><sub class="lower-index"><i>r</i></sub></span>. </li><li> Apply the xor operation with a given number <span class="tex-span"><i>x</i></span> to each array element on the segment <span class="tex-span">[<i>l</i>, <i>r</i>]</span>, that is, execute <img align="middle" class="tex-formula" src="file://8YUqness.png" style="max-width: 100.0%;max-height: 100.0%;">. This operation changes exactly <span class="tex-span"><i>r</i> - <i>l</i> + 1</span> array elements. </li></ol><p>Expression <img align="middle" class="tex-formula" src="file://YTKcswQR.png" style="max-width: 100.0%;max-height: 100.0%;"> means applying bitwise xor operation to numbers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>. The given operation exists in all modern programming languages, for example in language <span class="tex-font-style-it">C++</span> and <span class="tex-font-style-it">Java</span> it is marked as "<span class="tex-font-style-tt">^</span>", in <span class="tex-font-style-it">Pascal</span> — as "<span class="tex-font-style-tt">xor</span>".</p><p>You've got a list of <span class="tex-span"><i>m</i></span> operations of the indicated type. Your task is to perform all given operations, for each sum query you should print the result you get.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the size of the array. The second line contains space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — the original array.</p><p>The third line contains integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 5·10<sup class="upper-index">4</sup></span>) — the number of operations with the array. The <span class="tex-span"><i>i</i></span>-th of the following <span class="tex-span"><i>m</i></span> lines first contains an integer <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>) — the type of the <span class="tex-span"><i>i</i></span>-th query. If <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 1</span>, then this is the query of the sum, if <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 2</span>, then this is the query to change array elements. If the <span class="tex-span"><i>i</i></span>-th operation is of type <span class="tex-span">1</span>, then next follow two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>). If the <span class="tex-span"><i>i</i></span>-th operation is of type <span class="tex-span">2</span>, then next follow three integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>, <i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>). The numbers on the lines are separated by single spaces.</p></div><div class="output-specification"><p>For each query of type <span class="tex-span">1</span> print in a single line the sum of numbers on the given segment. Print the answers to the queries in the order in which the queries go in the input.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams, or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the size of the array. The second line contains space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — the original array.</p><p>The third line contains integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 5·10<sup class="upper-index">4</sup></span>) — the number of operations with the array. The <span class="tex-span"><i>i</i></span>-th of the following <span class="tex-span"><i>m</i></span> lines first contains an integer <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>) — the type of the <span class="tex-span"><i>i</i></span>-th query. If <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 1</span>, then this is the query of the sum, if <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 2</span>, then this is the query to change array elements. If the <span class="tex-span"><i>i</i></span>-th operation is of type <span class="tex-span">1</span>, then next follow two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>). If the <span class="tex-span"><i>i</i></span>-th operation is of type <span class="tex-span">2</span>, then next follow three integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>, <i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>). The numbers on the lines are separated by single spaces.</p>

## Output

<p>For each query of type <span class="tex-span">1</span> print in a single line the sum of numbers on the given segment. Print the answers to the queries in the order in which the queries go in the input.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams, or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
5
4 10 3 13 7
8
1 2 4
2 1 3 3
1 2 4
1 3 3
2 2 5 5
1 1 5
2 1 2 10
1 2 3

```




```input2
6
4 7 4 0 7 3
5
2 2 3 8
1 1 5
2 3 5 1
2 4 5 6
1 2 3

```




```output1
26
22
0
34
11

```




```output2
38
28

```


