## Description

<div><p>Farmer John has just given the cows a program to play with! The program contains two integer variables, <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>, and performs the following operations on a sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> of positive integers:</p><ol> <li> Initially, <span class="tex-span"><i>x</i> = 1</span> and <span class="tex-span"><i>y</i> = 0</span>. If, after any step, <span class="tex-span"><i>x</i> ≤ 0</span> or <span class="tex-span"><i>x</i> &gt; <i>n</i></span>, the program immediately terminates. </li><li> The program increases both <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> by a value equal to <span class="tex-span"><i>a</i><sub class="lower-index"><i>x</i></sub></span> simultaneously. </li><li> The program now increases <span class="tex-span"><i>y</i></span> by <span class="tex-span"><i>a</i><sub class="lower-index"><i>x</i></sub></span> while decreasing <span class="tex-span"><i>x</i></span> by <span class="tex-span"><i>a</i><sub class="lower-index"><i>x</i></sub></span>. </li><li> The program executes steps 2 and 3 (first step 2, then step 3) repeatedly until it terminates (it may never terminate). So, the sequence of executed steps may start with: step 2, step 3, step 2, step 3, step 2 and so on. </li></ol><p>The cows are not very good at arithmetic though, and they want to see how the program works. Please help them!</p><p>You are given the sequence <span class="tex-span"><i>a</i><sub class="lower-index">2</sub>, <i>a</i><sub class="lower-index">3</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. Suppose for each <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>n</i> - 1)</span> we run the program on the sequence <span class="tex-span"><i>i</i>, <i>a</i><sub class="lower-index">2</sub>, <i>a</i><sub class="lower-index">3</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. For each such run output the final value of <span class="tex-span"><i>y</i></span> if the program terminates or <span class="tex-font-style-tt">-1</span> if it does not terminate.</p></div><div class="input-specification"><p>The first line contains a single integer, <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>). The next line contains <span class="tex-span"><i>n</i> - 1</span> space separated integers, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub>, <i>a</i><sub class="lower-index">3</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>n</i> - 1</span> lines. On the <span class="tex-span"><i>i</i></span>-th line, print the requested value when the program is run on the sequence <span class="tex-span"><i>i</i>, <i>a</i><sub class="lower-index">2</sub>, <i>a</i><sub class="lower-index">3</sub>, ...<i>a</i><sub class="lower-index"><i>n</i></sub></span>.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains a single integer, <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>). The next line contains <span class="tex-span"><i>n</i> - 1</span> space separated integers, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub>, <i>a</i><sub class="lower-index">3</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Output <span class="tex-span"><i>n</i> - 1</span> lines. On the <span class="tex-span"><i>i</i></span>-th line, print the requested value when the program is run on the sequence <span class="tex-span"><i>i</i>, <i>a</i><sub class="lower-index">2</sub>, <i>a</i><sub class="lower-index">3</sub>, ...<i>a</i><sub class="lower-index"><i>n</i></sub></span>.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
4
2 4 1

```




```input2
3
1 2

```




```output1
3
6
8

```




```output2
-1
-1

```



## Note

<p>In the first sample </p><ol> <li> For <span class="tex-span"><i>i</i> = 1, </span> <span class="tex-span"><i>x</i></span> becomes <img align="middle" class="tex-formula" src="file://UQtJe1aL.png" style="max-width: 100.0%;max-height: 100.0%;"> and <span class="tex-span"><i>y</i></span> becomes <span class="tex-span">1 + 2 = 3</span>. </li><li> For <span class="tex-span"><i>i</i> = 2, </span> <span class="tex-span"><i>x</i></span> becomes <img align="middle" class="tex-formula" src="file://KxQrBKq4.png" style="max-width: 100.0%;max-height: 100.0%;"> and <span class="tex-span"><i>y</i></span> becomes <span class="tex-span">2 + 4 = 6.</span> </li><li> For <span class="tex-span"><i>i</i> = 3, </span> <span class="tex-span"><i>x</i></span> becomes <img align="middle" class="tex-formula" src="file://tkQYHhpk.png" style="max-width: 100.0%;max-height: 100.0%;"> and <span class="tex-span"><i>y</i></span> becomes <span class="tex-span">3 + 1 + 4 = 8.</span> </li></ol>
