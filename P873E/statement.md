## Description

<div><p>Alexey recently held a programming contest for students from Berland. <span class="tex-span"><i>n</i></span> students participated in a contest, <span class="tex-span"><i>i</i></span>-th of them solved <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> problems. Now he wants to award some contestants. Alexey can award the students with diplomas of three different degrees. Each student either will receive one diploma of some degree, or won't receive any diplomas at all. Let <span class="tex-span"><i>cnt</i><sub class="lower-index"><i>x</i></sub></span> be the number of students that are awarded with diplomas of degree <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ 3</span>). The following conditions must hold:</p><ul> <li> For each <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ 3</span>) <span class="tex-span"><i>cnt</i><sub class="lower-index"><i>x</i></sub> &gt; 0</span>; </li><li> For any two degrees <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> <span class="tex-span"><i>cnt</i><sub class="lower-index"><i>x</i></sub> ≤ 2·<i>cnt</i><sub class="lower-index"><i>y</i></sub></span>. </li></ul><p>Of course, there are a lot of ways to distribute the diplomas. Let <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> be the degree of diploma <span class="tex-span"><i>i</i></span>-th student will receive (or <span class="tex-span"> - 1</span> if <span class="tex-span"><i>i</i></span>-th student won't receive any diplomas). Also for any <span class="tex-span"><i>x</i></span> such that <span class="tex-span">1 ≤ <i>x</i> ≤ 3</span> let <span class="tex-span"><i>c</i><sub class="lower-index"><i>x</i></sub></span> be the maximum number of problems solved by a student that receives a diploma of degree <span class="tex-span"><i>x</i></span>, and <span class="tex-span"><i>d</i><sub class="lower-index"><i>x</i></sub></span> be the minimum number of problems solved by a student that receives a diploma of degree <span class="tex-span"><i>x</i></span>. Alexey wants to distribute the diplomas in such a way that:</p><ol> <li> If student <span class="tex-span"><i>i</i></span> solved more problems than student <span class="tex-span"><i>j</i></span>, then he has to be awarded not worse than student <span class="tex-span"><i>j</i></span> (it's impossible that student <span class="tex-span"><i>j</i></span> receives a diploma and <span class="tex-span"><i>i</i></span> doesn't receive any, and also it's impossible that both of them receive a diploma, but <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub> &lt; <i>b</i><sub class="lower-index"><i>i</i></sub></span>); </li><li> <span class="tex-span"><i>d</i><sub class="lower-index">1</sub> - <i>c</i><sub class="lower-index">2</sub></span> is maximum possible; </li><li> Among all ways that maximize the previous expression, <span class="tex-span"><i>d</i><sub class="lower-index">2</sub> - <i>c</i><sub class="lower-index">3</sub></span> is maximum possible; </li><li> Among all ways that correspond to the two previous conditions, <span class="tex-span"><i>d</i><sub class="lower-index">3</sub> - <i>c</i><sub class="lower-index"> - 1</sub></span> is maximum possible, where <span class="tex-span"><i>c</i><sub class="lower-index"> - 1</sub></span> is the maximum number of problems solved by a student that doesn't receive any diploma (or <span class="tex-span">0</span> if each student is awarded with some diploma). </li></ol><p>Help Alexey to find a way to award the contestants!</p></div><div class="input-specification"><p>The first line contains one integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 3000</span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 5000</span>).</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>n</i></span> numbers. <span class="tex-span"><i>i</i></span>-th number must be equal to the degree of diploma <span class="tex-span"><i>i</i></span>-th contestant will receive (or <span class="tex-span"> - 1</span> if he doesn't receive any diploma).</p><p>If there are multiple optimal solutions, print any of them. It is guaranteed that the answer always exists.</p></div>

## Input

<p>The first line contains one integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 3000</span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 5000</span>).</p>

## Output

<p>Output <span class="tex-span"><i>n</i></span> numbers. <span class="tex-span"><i>i</i></span>-th number must be equal to the degree of diploma <span class="tex-span"><i>i</i></span>-th contestant will receive (or <span class="tex-span"> - 1</span> if he doesn't receive any diploma).</p><p>If there are multiple optimal solutions, print any of them. It is guaranteed that the answer always exists.</p>





```input1
4
1 2 3 4

```




```input2
6
1 4 3 1 1 2

```




```output1
3 3 2 1 

```




```output2
-1 1 2 -1 -1 3 

```


