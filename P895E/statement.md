## Description

<div><p>Vasya and Petya were tired of studying so they decided to play a game. Before the game begins Vasya looks at array <span class="tex-span"><i>a</i></span> consisting of <span class="tex-span"><i>n</i></span> integers. As soon as he remembers all elements of <span class="tex-span"><i>a</i></span> the game begins. Vasya closes his eyes and Petya does <span class="tex-span"><i>q</i></span> actions of one of two types:</p><p><span class="tex-span">1)</span> Petya says 4 integers <span class="tex-span"><i>l</i>1, <i>r</i>1, <i>l</i>2, <i>r</i>2</span>&nbsp;— boundaries of two non-intersecting segments. After that he swaps one random element from the <span class="tex-span">[<i>l</i>1, <i>r</i>1]</span> segment with another random element from the <span class="tex-span">[<i>l</i>2, <i>r</i>2]</span> segment.</p><p><span class="tex-span">2)</span> Petya asks Vasya the sum of the elements of <span class="tex-span"><i>a</i></span> in the <span class="tex-span">[<i>l</i>, <i>r</i>]</span> segment.</p><p>Vasya is a mathematician so he answers Petya the mathematical expectation of the sum of the elements in the segment.</p><p>Your task is to write a program which will answer the second type questions as Vasya would do it. In other words your program should print the mathematical expectation of the sum of the elements of <span class="tex-span"><i>a</i></span> in the <span class="tex-span">[<i>l</i>, <i>r</i>]</span> segment for every second type query.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i>, <i>q</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>) &nbsp;— the number of elements in the array and the number of queries you need to handle.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) &nbsp;— elements of the array.</p><p>The next <span class="tex-span"><i>q</i></span> lines contain Petya's actions of type 1 or 2.</p><p>If it is a type <span class="tex-span">1</span> action then the line contains <span class="tex-span">5</span> integers <span class="tex-span">1, <i>l</i>1, <i>r</i>1, <i>l</i>2, <i>r</i>2</span> (<span class="tex-span">1 ≤ <i>l</i>1 ≤ <i>r</i>1 ≤ <i>n</i>, 1 ≤ <i>l</i>2 ≤ <i>r</i>2 ≤ <i>n</i></span>).</p><p>If it is a type <span class="tex-span">2</span> query then the line contains <span class="tex-span">3</span> integers <span class="tex-span">2, <i>l</i>, <i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>).</p><p>It is guaranteed that there is at least one type <span class="tex-span">2</span> query and segments <span class="tex-span">[<i>l</i>1, <i>r</i>1], [<i>l</i>2, <i>r</i>2]</span> don't have common elements. </p></div><div class="output-specification"><p>For each type <span class="tex-span">2</span> query print one real number&nbsp;— the mathematical expectation of the sum of elements in the segment.</p><p>Your answer will be considered correct if its absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span> &nbsp;— formally, the answer is correct if <img align="middle" class="tex-formula" src="file://X5DUfTMT.png" style="max-width: 100.0%;max-height: 100.0%;"> where <span class="tex-span"><i>x</i></span> is jury's answer and <span class="tex-span"><i>y</i></span> is yours.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i>, <i>q</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>) &nbsp;— the number of elements in the array and the number of queries you need to handle.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) &nbsp;— elements of the array.</p><p>The next <span class="tex-span"><i>q</i></span> lines contain Petya's actions of type 1 or 2.</p><p>If it is a type <span class="tex-span">1</span> action then the line contains <span class="tex-span">5</span> integers <span class="tex-span">1, <i>l</i>1, <i>r</i>1, <i>l</i>2, <i>r</i>2</span> (<span class="tex-span">1 ≤ <i>l</i>1 ≤ <i>r</i>1 ≤ <i>n</i>, 1 ≤ <i>l</i>2 ≤ <i>r</i>2 ≤ <i>n</i></span>).</p><p>If it is a type <span class="tex-span">2</span> query then the line contains <span class="tex-span">3</span> integers <span class="tex-span">2, <i>l</i>, <i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>).</p><p>It is guaranteed that there is at least one type <span class="tex-span">2</span> query and segments <span class="tex-span">[<i>l</i>1, <i>r</i>1], [<i>l</i>2, <i>r</i>2]</span> don't have common elements. </p>

## Output

<p>For each type <span class="tex-span">2</span> query print one real number&nbsp;— the mathematical expectation of the sum of elements in the segment.</p><p>Your answer will be considered correct if its absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span> &nbsp;— formally, the answer is correct if <img align="middle" class="tex-formula" src="file://X5DUfTMT.png" style="max-width: 100.0%;max-height: 100.0%;"> where <span class="tex-span"><i>x</i></span> is jury's answer and <span class="tex-span"><i>y</i></span> is yours.</p>





```input1
4 4
1 1 2 2
1 2 2 3 3
2 1 2
1 1 2 3 4
2 1 2

```




```input2
10 5
1 1 1 1 1 2 2 2 2 2
1 1 5 6 10
2 1 5
1 1 5 6 10
1 1 5 6 10
2 6 10

```




```input3
10 10
1 2 3 4 5 6 7 8 9 10
1 1 5 6 10
1 1 5 6 10
2 1 5
1 1 3 6 9
2 1 3
1 5 7 8 10
1 1 1 10 10
2 1 5
2 7 10
2 1 10

```




```output1
3.0000000
3.0000000

```




```output2
6.0000000
8.0400000

```




```output3
23.0000000
14.0000000
28.0133333
21.5733333
55.0000000

```


