## Description

<div><p>By the age of three Smart Beaver mastered all arithmetic operations and got this summer homework from the amazed teacher:</p><p>You are given a sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. Your task is to perform on it <span class="tex-span"><i>m</i></span> consecutive operations of the following type:</p><ol> <li> For given numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> assign value <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> to element <span class="tex-span"><i>a</i><sub class="lower-index"><i>x</i><sub class="lower-index"><i>i</i></sub></sub></span>. </li><li> For given numbers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> you've got to calculate sum <img align="middle" class="tex-formula" src="file://64uViaXi.png" style="max-width: 100.0%;max-height: 100.0%;">, where <span class="tex-span"><i>f</i><sub class="lower-index">0</sub> = <i>f</i><sub class="lower-index">1</sub> = 1</span> and at <span class="tex-span"><i>i</i> ≥ 2</span>: <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub> = <i>f</i><sub class="lower-index"><i>i</i> - 1</sub> + <i>f</i><sub class="lower-index"><i>i</i> - 2</sub></span>. </li><li> For a group of three numbers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> you should increase value <span class="tex-span"><i>a</i><sub class="lower-index"><i>x</i></sub></span> by <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> for all <span class="tex-span"><i>x</i></span> <span class="tex-span">(<i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>x</i> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub>)</span>. </li></ol><p>Smart Beaver planned a tour around great Canadian lakes, so he asked you to help him solve the given problem.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of integers in the sequence and the number of operations, correspondingly. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>). Then follow <span class="tex-span"><i>m</i></span> lines, each describes an operation. Each line starts with an integer <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 3</span>) — the operation type: </p><ul> <li> if <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 1</span>, then next follow two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 0 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>); </li><li> if <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 2</span>, then next follow two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>); </li><li> if <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 3</span>, then next follow three integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 0 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>). </li></ul><p>The input limits for scoring <span class="tex-span">30</span> points are (subproblem E1): </p><ul> <li> It is guaranteed that <span class="tex-span"><i>n</i></span> does not exceed <span class="tex-span">100</span>, <span class="tex-span"><i>m</i></span> does not exceed <span class="tex-span">10000</span> and there will be no queries of the <span class="tex-span">3</span>-rd type. </li></ul><p>The input limits for scoring <span class="tex-span">70</span> points are (subproblems E1+E2): </p><ul> <li> It is guaranteed that there will be queries of the <span class="tex-span">1</span>-st and <span class="tex-span">2</span>-nd type only. </li></ul><p>The input limits for scoring <span class="tex-span">100</span> points are (subproblems E1+E2+E3): </p><ul> <li> No extra limitations. </li></ul></div><div class="output-specification"><p>For each query print the calculated sum modulo <span class="tex-span">1000000000</span> <span class="tex-span">(10<sup class="upper-index">9</sup>)</span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of integers in the sequence and the number of operations, correspondingly. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>). Then follow <span class="tex-span"><i>m</i></span> lines, each describes an operation. Each line starts with an integer <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 3</span>) — the operation type: </p><ul> <li> if <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 1</span>, then next follow two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 0 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>); </li><li> if <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 2</span>, then next follow two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>); </li><li> if <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 3</span>, then next follow three integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 0 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>). </li></ul><p>The input limits for scoring <span class="tex-span">30</span> points are (subproblem E1): </p><ul> <li> It is guaranteed that <span class="tex-span"><i>n</i></span> does not exceed <span class="tex-span">100</span>, <span class="tex-span"><i>m</i></span> does not exceed <span class="tex-span">10000</span> and there will be no queries of the <span class="tex-span">3</span>-rd type. </li></ul><p>The input limits for scoring <span class="tex-span">70</span> points are (subproblems E1+E2): </p><ul> <li> It is guaranteed that there will be queries of the <span class="tex-span">1</span>-st and <span class="tex-span">2</span>-nd type only. </li></ul><p>The input limits for scoring <span class="tex-span">100</span> points are (subproblems E1+E2+E3): </p><ul> <li> No extra limitations. </li></ul>

## Output

<p>For each query print the calculated sum modulo <span class="tex-span">1000000000</span> <span class="tex-span">(10<sup class="upper-index">9</sup>)</span>.</p>





```input1
5 5
1 3 1 2 4
2 1 4
2 1 5
2 2 4
1 3 10
2 1 5

```




```input2
5 4
1 3 1 2 4
3 1 4 1
2 2 4
1 2 10
2 1 5

```




```output1
12
32
8
50

```




```output2
12
45

```


