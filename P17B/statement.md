## Description

<div><p>Nick's company employed <span class="tex-span"><i>n</i></span> people. Now Nick needs to build a tree hierarchy of «supervisor-surbodinate» relations in the company (this is to say that each employee, except one, has exactly one supervisor). There are <span class="tex-span"><i>m</i></span> applications written in the following form: <span class="tex-font-style-underline">«employee <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is ready to become a supervisor of employee <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> at extra cost <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>»</span>. The qualification <span class="tex-span"><i>q</i><sub class="lower-index"><i>j</i></sub></span> of each employee is known, and for each application the following is true: <span class="tex-span"><i>q</i><sub class="lower-index"><i>a</i><sub class="lower-index"><i>i</i></sub></sub> &gt; <i>q</i><sub class="lower-index"><i>b</i><sub class="lower-index"><i>i</i></sub></sub></span>. </p><p>Would you help Nick calculate the minimum cost of such a hierarchy, or find out that it is impossible to build it.</p></div><div class="input-specification"><p>The first input line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) — amount of employees in the company. The following line contains <span class="tex-span"><i>n</i></span> space-separated numbers <span class="tex-span"><i>q</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">0 ≤ <i>q</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">6</sup></span>)— the employees' qualifications. The following line contains number <span class="tex-span"><i>m</i></span> (<span class="tex-span">0 ≤ <i>m</i> ≤ 10000</span>) — amount of received applications. The following <span class="tex-span"><i>m</i></span> lines contain the applications themselves, each of them in the form of three space-separated numbers: <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>). Different applications can be similar, i.e. they can come from one and the same employee who offered to become a supervisor of the same person but at a different cost. For each application <span class="tex-span"><i>q</i><sub class="lower-index"><i>a</i><sub class="lower-index"><i>i</i></sub></sub> &gt; <i>q</i><sub class="lower-index"><i>b</i><sub class="lower-index"><i>i</i></sub></sub></span>.</p></div><div class="output-specification"><p>Output the only line — the minimum cost of building such a hierarchy, or <span class="tex-font-style-tt">-1</span> if it is impossible to build it.</p></div>

## Input

<p>The first input line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) — amount of employees in the company. The following line contains <span class="tex-span"><i>n</i></span> space-separated numbers <span class="tex-span"><i>q</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">0 ≤ <i>q</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">6</sup></span>)— the employees' qualifications. The following line contains number <span class="tex-span"><i>m</i></span> (<span class="tex-span">0 ≤ <i>m</i> ≤ 10000</span>) — amount of received applications. The following <span class="tex-span"><i>m</i></span> lines contain the applications themselves, each of them in the form of three space-separated numbers: <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>). Different applications can be similar, i.e. they can come from one and the same employee who offered to become a supervisor of the same person but at a different cost. For each application <span class="tex-span"><i>q</i><sub class="lower-index"><i>a</i><sub class="lower-index"><i>i</i></sub></sub> &gt; <i>q</i><sub class="lower-index"><i>b</i><sub class="lower-index"><i>i</i></sub></sub></span>.</p>

## Output

<p>Output the only line — the minimum cost of building such a hierarchy, or <span class="tex-font-style-tt">-1</span> if it is impossible to build it.</p>





```input1
4
7 2 3 1
4
1 2 5
2 4 1
3 4 1
1 3 5

```




```input2
3
1 2 3
2
3 1 2
3 1 3

```




```output1
11

```




```output2
-1

```



## Note

<p>In the first sample one of the possible ways for building a hierarchy is to take applications with indexes 1, 2 and 4, which give 11 as the minimum total cost. In the second sample it is impossible to build the required hierarchy, so the answer is <span class="tex-font-style-tt">-1</span>.</p>
