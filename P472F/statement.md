## Description

<div><p>There are some tasks which have the following structure: you are given a model, and you can do some operations, you should use these operations to achive the goal. One way to create a new task is to use the same model and same operations, but change the goal.</p><p>Let's have a try. I have created the following task for Topcoder SRM 557 Div1-Hard: you are given <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span>. You are allowed to perform the assignments (as many as you want) of the following form <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> ^= <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub></span> (in the original task <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> must be different, but in this task we allow <span class="tex-span"><i>i</i></span> to equal <span class="tex-span"><i>j</i></span>). The goal is to maximize the sum of all <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Now we just change the goal. You are also given <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub>, ..., <i>y</i><sub class="lower-index"><i>n</i></sub></span>. You should make <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> exactly equal to <span class="tex-span"><i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub>, ..., <i>y</i><sub class="lower-index"><i>n</i></sub></span>. In other words, for each <span class="tex-span"><i>i</i></span> number <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> should be equal to <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10000)</span>. The second line contains <span class="tex-span"><i>n</i></span> integers: <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span> to <span class="tex-span"><i>x</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>. The third line contains <span class="tex-span"><i>n</i></span> integers: <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span> to <span class="tex-span"><i>y</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p></div><div class="output-specification"><p>If there is no solution, output <span class="tex-font-style-tt">-1</span>.</p><p>If there is a solution, then in the first line output an integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(0 ≤ <i>m</i> ≤ 1000000)</span> – the number of assignments you need to perform. Then print <span class="tex-span"><i>m</i></span> lines, each line should contain two integers <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> <span class="tex-span">(1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i>)</span>, which denote assignment <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> ^= <span class="tex-font-style-bf"><span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub></span></span>.</p><p>If there are multiple solutions you can print any of them. We can prove that under these constraints if there exists a solution then there always exists a solution with no more than <span class="tex-span">10<sup class="upper-index">6</sup></span> operations.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10000)</span>. The second line contains <span class="tex-span"><i>n</i></span> integers: <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span> to <span class="tex-span"><i>x</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>. The third line contains <span class="tex-span"><i>n</i></span> integers: <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span> to <span class="tex-span"><i>y</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p>

## Output

<p>If there is no solution, output <span class="tex-font-style-tt">-1</span>.</p><p>If there is a solution, then in the first line output an integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(0 ≤ <i>m</i> ≤ 1000000)</span> – the number of assignments you need to perform. Then print <span class="tex-span"><i>m</i></span> lines, each line should contain two integers <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> <span class="tex-span">(1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i>)</span>, which denote assignment <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> ^= <span class="tex-font-style-bf"><span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub></span></span>.</p><p>If there are multiple solutions you can print any of them. We can prove that under these constraints if there exists a solution then there always exists a solution with no more than <span class="tex-span">10<sup class="upper-index">6</sup></span> operations.</p>





```input1
2
3 5
6 0

```




```input2
5
0 0 0 0 0
1 2 3 4 5

```




```input3
3
4 5 6
1 2 3

```




```input4
3
1 2 3
4 5 6

```




```output1
2
1 2
2 2

```




```output2
-1

```




```output3
5
3 1
1 2
2 2
2 3
3 1

```




```output4
-1

```



## Note

<p>Assignment <span class="tex-span"><i>a</i></span> ^= <span class="tex-span"><i>b</i></span> denotes assignment <span class="tex-span"><i>a</i></span> = <span class="tex-span"><i>a</i></span> ^ <span class="tex-span"><i>b</i></span>, where operation "<span class="tex-font-style-tt">^</span>" is bitwise XOR of two integers.</p>
