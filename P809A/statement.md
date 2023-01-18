## Description

<div><p>Leha decided to move to a quiet town Vičkopolis, because he was tired by living in Bankopolis. Upon arrival he immediately began to expand his network of hacked computers. During the week Leha managed to get access to <span class="tex-span"><i>n</i></span> computers throughout the town. Incidentally all the computers, which were hacked by Leha, lie on the same straight line, due to the reason that there is the only one straight street in Vičkopolis.</p><p>Let's denote the coordinate system on this street. Besides let's number all the hacked computers with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. So the <span class="tex-span"><i>i</i></span>-th hacked computer is located at the point <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>. Moreover the coordinates of all computers are distinct. </p><p>Leha is determined to have a little rest after a hard week. Therefore he is going to invite his friend Noora to a restaurant. However the girl agrees to go on a date with the only one condition: Leha have to solve a simple task.</p><p>Leha should calculate a sum of <span class="tex-span"><i>F</i>(<i>a</i>)</span> for all <span class="tex-span"><i>a</i></span>, where <span class="tex-span"><i>a</i></span> is a non-empty subset of the set, that consists of all hacked computers. Formally, let's denote <span class="tex-span"><i>A</i></span> the set of all integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Noora asks the hacker to find value of the expression <img align="middle" class="tex-formula" src="file://Krdzy8tA.png" style="max-width: 100.0%;max-height: 100.0%;">. Here <span class="tex-span"><i>F</i>(<i>a</i>)</span> is calculated as the maximum among the distances between all pairs of computers from the set <span class="tex-span"><i>a</i></span>. Formally, <img align="middle" class="tex-formula" src="file://ePMPu7n8.png" style="max-width: 100.0%;max-height: 100.0%;">. Since the required sum can be quite large Noora asks to find it modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p><p>Though, Leha is too tired. Consequently he is not able to solve this task. Help the hacker to attend a date.</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup>)</span> denoting the number of hacked computers.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> denoting the coordinates of hacked computers. It is guaranteed that all <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> are distinct.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the required sum modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup>)</span> denoting the number of hacked computers.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> denoting the coordinates of hacked computers. It is guaranteed that all <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> are distinct.</p>

## Output

<p>Print a single integer&nbsp;— the required sum modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
2
4 7

```




```input2
3
4 3 1

```




```output1
3

```




```output2
9

```



## Note

<p>There are three non-empty subsets in the first sample test:<img align="middle" class="tex-formula" src="file://wHlv0Gze.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://h8dnptOB.png" style="max-width: 100.0%;max-height: 100.0%;"> and <img align="middle" class="tex-formula" src="file://qcV1NZX3.png" style="max-width: 100.0%;max-height: 100.0%;">. The first and the second subset increase the sum by <span class="tex-span">0</span> and the third subset increases the sum by <span class="tex-span">7 - 4 = 3</span>. In total the answer is <span class="tex-span">0 + 0 + 3 = 3</span>.</p><p>There are seven non-empty subsets in the second sample test. Among them only the following subsets increase the answer: <img align="middle" class="tex-formula" src="file://ZTvVk16S.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://zLGUemNR.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://51oCp0eX.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://E0UP7jXX.png" style="max-width: 100.0%;max-height: 100.0%;">. In total the sum is <span class="tex-span">(4 - 3) + (4 - 1) + (3 - 1) + (4 - 1) = 9</span>.</p>
