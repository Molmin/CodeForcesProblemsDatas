## Description

<div><p>The Smart Beaver from ABBYY has once again surprised us! He has developed a new calculating device, which he called the "Beaver's Calculator <span class="tex-span">1.0</span>". It is very peculiar and it is planned to be used in a variety of scientific problems.</p><p>To test it, the Smart Beaver invited <span class="tex-span"><i>n</i></span> scientists, numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. The <span class="tex-span"><i>i</i></span>-th scientist brought <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> calculating problems for the device developed by the Smart Beaver from ABBYY. The problems of the <span class="tex-span"><i>i</i></span>-th scientist are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span>, and they must be calculated sequentially in the described order, since calculating each problem heavily depends on the results of calculating of the previous ones.</p><p>Each problem of each of the <span class="tex-span"><i>n</i></span> scientists is described by one integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span>, where <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) is the number of the scientist, <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>j</i> ≤ <i>k</i><sub class="lower-index"><i>i</i></sub></span>) is the number of the problem, and <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> is the number of resource units the calculating device needs to solve this problem.</p><p>The calculating device that is developed by the Smart Beaver is pretty unusual. It solves problems sequentially, one after another. After some problem is solved and before the next one is considered, the calculating device allocates or frees resources.</p><p>The most expensive operation for the calculating device is freeing resources, which works much slower than allocating them. It is therefore desirable that each next problem for the calculating device requires no less resources than the previous one.</p><p>You are given the information about the problems the scientists offered for the testing. You need to arrange these problems in such an order that the number of adjacent "bad" pairs of problems in this list is minimum possible. We will call two consecutive problems in this list a "bad pair" if the problem that is performed first requires more resources than the one that goes after it. Do not forget that the problems of the same scientist must be solved in a fixed order.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> — the number of scientists. To lessen the size of the input, each of the next <span class="tex-span"><i>n</i></span> lines contains five integers <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, 1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i>, 1</sub> &lt; <i>m</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the number of problems of the <span class="tex-span"><i>i</i></span>-th scientist, the resources the first problem requires and three parameters that generate the subsequent values of <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span>. For all <span class="tex-span"><i>j</i></span> from <span class="tex-span">2</span> to <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span>, inclusive, you should calculate value <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> by formula <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> = (<i>a</i><sub class="lower-index"><i>i</i>, <i>j</i> - 1</sub> * <i>x</i><sub class="lower-index"><i>i</i></sub> + <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> <span class="tex-span"><i>mod</i></span> <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span>, where <span class="tex-span"><i>a</i></span> <span class="tex-span"><i>mod</i></span> <span class="tex-span"><i>b</i></span> is the operation of taking the remainder of division of number <span class="tex-span"><i>a</i></span> by number <span class="tex-span"><i>b</i></span>.</p><p>To get the full points for the first group of tests it is sufficient to solve the problem with <span class="tex-span"><i>n</i> = 2</span>, <span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 2000</span>.</p><p>To get the full points for the second group of tests it is sufficient to solve the problem with <span class="tex-span"><i>n</i> = 2</span>, <span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 200000</span>.</p><p>To get the full points for the third group of tests it is sufficient to solve the problem with <span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>, <span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 5000</span>.</p></div><div class="output-specification"><p>On the first line print a single number — the number of "bad" pairs in the optimal order.</p><p>If the total number of problems does not exceed <span class="tex-span">200000</span>, also print <img align="middle" class="tex-formula" src="file://UEF184YC.png" style="max-width: 100.0%;max-height: 100.0%;"> lines — the optimal order of the problems. On each of these lines print two integers separated by a single space — the required number of resources for the problem and the number of the scientist who offered this problem, respectively. The scientists are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> in the order of input.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> — the number of scientists. To lessen the size of the input, each of the next <span class="tex-span"><i>n</i></span> lines contains five integers <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, 1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i>, 1</sub> &lt; <i>m</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the number of problems of the <span class="tex-span"><i>i</i></span>-th scientist, the resources the first problem requires and three parameters that generate the subsequent values of <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span>. For all <span class="tex-span"><i>j</i></span> from <span class="tex-span">2</span> to <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span>, inclusive, you should calculate value <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> by formula <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> = (<i>a</i><sub class="lower-index"><i>i</i>, <i>j</i> - 1</sub> * <i>x</i><sub class="lower-index"><i>i</i></sub> + <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> <span class="tex-span"><i>mod</i></span> <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span>, where <span class="tex-span"><i>a</i></span> <span class="tex-span"><i>mod</i></span> <span class="tex-span"><i>b</i></span> is the operation of taking the remainder of division of number <span class="tex-span"><i>a</i></span> by number <span class="tex-span"><i>b</i></span>.</p><p>To get the full points for the first group of tests it is sufficient to solve the problem with <span class="tex-span"><i>n</i> = 2</span>, <span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 2000</span>.</p><p>To get the full points for the second group of tests it is sufficient to solve the problem with <span class="tex-span"><i>n</i> = 2</span>, <span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 200000</span>.</p><p>To get the full points for the third group of tests it is sufficient to solve the problem with <span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>, <span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 5000</span>.</p>

## Output

<p>On the first line print a single number — the number of "bad" pairs in the optimal order.</p><p>If the total number of problems does not exceed <span class="tex-span">200000</span>, also print <img align="middle" class="tex-formula" src="file://UEF184YC.png" style="max-width: 100.0%;max-height: 100.0%;"> lines — the optimal order of the problems. On each of these lines print two integers separated by a single space — the required number of resources for the problem and the number of the scientist who offered this problem, respectively. The scientists are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> in the order of input.</p>





```input1
2
2 1 1 1 10
2 3 1 1 10

```




```input2
2
3 10 2 3 1000
3 100 1 999 1000

```




```output1
0
1 1
2 1
3 2
4 2

```




```output2
2
10 1
23 1
49 1
100 2
99 2
98 2

```



## Note

<p>In the first sample <span class="tex-span"><i>n</i> = 2</span>, <span class="tex-span"><i>k</i><sub class="lower-index">1</sub> = 2</span>, <span class="tex-span"><i>a</i><sub class="lower-index">1, 1</sub> = 1</span>, <span class="tex-span"><i>a</i><sub class="lower-index">1, 2</sub> = 2</span>, <span class="tex-span"><i>k</i><sub class="lower-index">2</sub> = 2</span>, <span class="tex-span"><i>a</i><sub class="lower-index">2, 1</sub> = 3</span>, <span class="tex-span"><i>a</i><sub class="lower-index">2, 2</sub> = 4</span>. We've got two scientists, each of them has two calculating problems. The problems of the first scientist require <span class="tex-span">1</span> and <span class="tex-span">2</span> resource units, the problems of the second one require <span class="tex-span">3</span> and <span class="tex-span">4</span> resource units. Let's list all possible variants of the calculating order (each problem is characterized only by the number of resource units it requires): <span class="tex-span">(1, 2, 3, 4)</span>, <span class="tex-span">(1, 3, 2, 4)</span>, <span class="tex-span">(3, 1, 2, 4)</span>, <span class="tex-span">(1, 3, 4, 2)</span>, <span class="tex-span">(3, 4, 1, 2)</span>, <span class="tex-span">(3, 1, 4, 2)</span>.</p><p>Sequence of problems <span class="tex-span">(1, 3, 2, 4)</span> has one "bad" pair (<span class="tex-span">3</span> and <span class="tex-span">2</span>), <span class="tex-span">(3, 1, 4, 2)</span> has two "bad" pairs (<span class="tex-span">3</span> and <span class="tex-span">1</span>, <span class="tex-span">4</span> and <span class="tex-span">2</span>), and <span class="tex-span">(1, 2, 3, 4)</span> has no "bad" pairs.</p>
