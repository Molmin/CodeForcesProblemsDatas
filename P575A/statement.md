## Description

<div><p>Fibonotci sequence is an integer recursive sequence defined by the recurrence relation </p><center> <span class="tex-span"><i>F</i><sub class="lower-index"><i>n</i></sub> = <i>s</i><sub class="lower-index"><i>n</i> - 1</sub>·<i>F</i><sub class="lower-index"><i>n</i> - 1</sub> + <i>s</i><sub class="lower-index"><i>n</i> - 2</sub>·<i>F</i><sub class="lower-index"><i>n</i> - 2</sub></span> </center> with <center> <span class="tex-span"><i>F</i><sub class="lower-index">0</sub> = 0, <i>F</i><sub class="lower-index">1</sub> = 1</span> </center><p>Sequence <span class="tex-span"><i>s</i></span> is an infinite and almost cyclic sequence with a cycle of length <span class="tex-span"><i>N</i></span>. A sequence <span class="tex-span"><i>s</i></span> is called almost cyclic with a cycle of length <span class="tex-span"><i>N</i></span> if <img align="middle" class="tex-formula" src="file://l35ayLYa.png" style="max-width: 100.0%;max-height: 100.0%;">, for <span class="tex-span"><i>i</i> ≥ <i>N</i></span>, except for a finite number of values <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>, for which <img align="middle" class="tex-formula" src="file://4qToOiGn.png" style="max-width: 100.0%;max-height: 100.0%;"> (<span class="tex-span"><i>i</i> ≥ <i>N</i></span>).</p><p>Following is an example of an almost cyclic sequence with a cycle of length 4: </p><center> s = (5,3,8,11,5,3,7,11,5,3,8,11,…) </center><p>Notice that the only value of <span class="tex-span"><i>s</i></span> for which the equality <img align="middle" class="tex-formula" src="file://nAB5ymmQ.png" style="max-width: 100.0%;max-height: 100.0%;"> does not hold is <span class="tex-span"><i>s</i><sub class="lower-index">6</sub></span> (<span class="tex-span"><i>s</i><sub class="lower-index">6</sub> = 7</span> and <span class="tex-span"><i>s</i><sub class="lower-index">2</sub> = 8</span>). You are given <span class="tex-span"><i>s</i><sub class="lower-index">0</sub>, <i>s</i><sub class="lower-index">1</sub>, ...<i>s</i><sub class="lower-index"><i>N</i> - 1</sub></span> and all the values of sequence <span class="tex-span"><i>s</i></span> for which <img align="middle" class="tex-formula" src="file://4V6hXVzB.png" style="max-width: 100.0%;max-height: 100.0%;"> (<span class="tex-span"><i>i</i> ≥ <i>N</i></span>).</p><p>Find <img align="middle" class="tex-formula" src="file://fctvMpYR.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div><div class="input-specification"><p>The first line contains two numbers <span class="tex-span"><i>K</i></span> and <span class="tex-span"><i>P</i></span>. The second line contains a single number <span class="tex-span"><i>N</i></span>. The third line contains <span class="tex-span"><i>N</i></span> numbers separated by spaces, that represent the first <span class="tex-span"><i>N</i></span> numbers of the sequence <span class="tex-span"><i>s</i></span>. The fourth line contains a single number <span class="tex-span"><i>M</i></span>, the number of values of sequence <span class="tex-span"><i>s</i></span> for which <img align="middle" class="tex-formula" src="file://yGXELVHT.png" style="max-width: 100.0%;max-height: 100.0%;">. Each of the following <span class="tex-span"><i>M</i></span> lines contains two numbers <span class="tex-span"><i>j</i></span> and <span class="tex-span"><i>v</i></span>, indicating that <img align="middle" class="tex-formula" src="file://iYzp5nAo.png" style="max-width: 100.0%;max-height: 100.0%;"> and <span class="tex-span"><i>s</i><sub class="lower-index"><i>j</i></sub> = <i>v</i></span>. All j-s are distinct.</p><ul> <li> <span class="tex-span">1 ≤ <i>N</i>, <i>M</i> ≤ 50000</span> </li><li> <span class="tex-span">0 ≤ <i>K</i> ≤ 10<sup class="upper-index">18</sup></span> </li><li> <span class="tex-span">1 ≤ <i>P</i> ≤ 10<sup class="upper-index">9</sup></span> </li><li> <span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, for all <span class="tex-span"><i>i</i> = 0, 1, ...<i>N</i> - 1</span> </li><li> <span class="tex-span"><i>N</i> ≤ <i>j</i> ≤ 10<sup class="upper-index">18</sup></span> </li><li> <span class="tex-span">1 ≤ <i>v</i> ≤ 10<sup class="upper-index">9</sup></span> </li><li> All values are integers </li></ul></div><div class="output-specification"><p>Output should contain a single integer equal to <img align="middle" class="tex-formula" src="file://8agYjtrA.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line contains two numbers <span class="tex-span"><i>K</i></span> and <span class="tex-span"><i>P</i></span>. The second line contains a single number <span class="tex-span"><i>N</i></span>. The third line contains <span class="tex-span"><i>N</i></span> numbers separated by spaces, that represent the first <span class="tex-span"><i>N</i></span> numbers of the sequence <span class="tex-span"><i>s</i></span>. The fourth line contains a single number <span class="tex-span"><i>M</i></span>, the number of values of sequence <span class="tex-span"><i>s</i></span> for which <img align="middle" class="tex-formula" src="file://yGXELVHT.png" style="max-width: 100.0%;max-height: 100.0%;">. Each of the following <span class="tex-span"><i>M</i></span> lines contains two numbers <span class="tex-span"><i>j</i></span> and <span class="tex-span"><i>v</i></span>, indicating that <img align="middle" class="tex-formula" src="file://iYzp5nAo.png" style="max-width: 100.0%;max-height: 100.0%;"> and <span class="tex-span"><i>s</i><sub class="lower-index"><i>j</i></sub> = <i>v</i></span>. All j-s are distinct.</p><ul> <li> <span class="tex-span">1 ≤ <i>N</i>, <i>M</i> ≤ 50000</span> </li><li> <span class="tex-span">0 ≤ <i>K</i> ≤ 10<sup class="upper-index">18</sup></span> </li><li> <span class="tex-span">1 ≤ <i>P</i> ≤ 10<sup class="upper-index">9</sup></span> </li><li> <span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, for all <span class="tex-span"><i>i</i> = 0, 1, ...<i>N</i> - 1</span> </li><li> <span class="tex-span"><i>N</i> ≤ <i>j</i> ≤ 10<sup class="upper-index">18</sup></span> </li><li> <span class="tex-span">1 ≤ <i>v</i> ≤ 10<sup class="upper-index">9</sup></span> </li><li> All values are integers </li></ul>

## Output

<p>Output should contain a single integer equal to <img align="middle" class="tex-formula" src="file://8agYjtrA.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
10 8
3
1 2 1
2
7 3
5 4

```




```output1
4

```


