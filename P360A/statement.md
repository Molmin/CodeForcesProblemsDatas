## Description

<div><p>Levko loves array <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... , <i>a</i><sub class="lower-index"><i>n</i></sub></span>, consisting of integers, very much. That is why Levko is playing with array <span class="tex-span"><i>a</i></span>, performing all sorts of operations with it. Each operation Levko performs is of one of two types:</p><ol> <li> Increase all elements from <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> by <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>. In other words, perform assignments <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub> = <i>a</i><sub class="lower-index"><i>j</i></sub> + <i>d</i><sub class="lower-index"><i>i</i></sub></span> for all <span class="tex-span"><i>j</i></span> that meet the inequation <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>j</i> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub></span>. </li><li> Find the maximum of elements from <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>. That is, calculate the value <img align="middle" class="tex-formula" src="file://psC5vwKP.png" style="max-width: 100.0%;max-height: 100.0%;">. </li></ol><p>Sadly, Levko has recently lost his array. Fortunately, Levko has records of all operations he has performed on array <span class="tex-span"><i>a</i></span>. Help Levko, given the operation records, find at least one suitable array. The results of all operations for the given array must coincide with the record results. Levko clearly remembers that all numbers in his array didn't exceed <span class="tex-span">10<sup class="upper-index">9</sup></span> in their absolute value, so he asks you to find such an array.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 5000</span>) — the size of the array and the number of operations in Levko's records, correspondingly.</p><p>Next <span class="tex-span"><i>m</i></span> lines describe the operations, the <span class="tex-span"><i>i</i></span>-th line describes the <span class="tex-span"><i>i</i></span>-th operation. The first integer in the <span class="tex-span"><i>i</i></span>-th line is integer <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>) that describes the operation type. If <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 1</span>, then it is followed by three integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"> - 10<sup class="upper-index">4</sup> ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>) — the description of the operation of the first type. If <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 2</span>, then it is followed by three integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"> - 5·10<sup class="upper-index">7</sup> ≤ <i>m</i><sub class="lower-index"><i>i</i></sub> ≤ 5·10<sup class="upper-index">7</sup></span>) — the description of the operation of the second type.</p><p>The operations are given in the order Levko performed them on his array.</p></div><div class="output-specification"><p>In the first line print "<span class="tex-font-style-tt">YES</span>" (without the quotes), if the solution exists and "<span class="tex-font-style-tt">NO</span>" (without the quotes) otherwise.</p><p>If the solution exists, then on the second line print <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... , <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(|<i>a</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup>)</span> — the recovered array.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 5000</span>) — the size of the array and the number of operations in Levko's records, correspondingly.</p><p>Next <span class="tex-span"><i>m</i></span> lines describe the operations, the <span class="tex-span"><i>i</i></span>-th line describes the <span class="tex-span"><i>i</i></span>-th operation. The first integer in the <span class="tex-span"><i>i</i></span>-th line is integer <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>) that describes the operation type. If <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 1</span>, then it is followed by three integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"> - 10<sup class="upper-index">4</sup> ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>) — the description of the operation of the first type. If <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 2</span>, then it is followed by three integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"> - 5·10<sup class="upper-index">7</sup> ≤ <i>m</i><sub class="lower-index"><i>i</i></sub> ≤ 5·10<sup class="upper-index">7</sup></span>) — the description of the operation of the second type.</p><p>The operations are given in the order Levko performed them on his array.</p>

## Output

<p>In the first line print "<span class="tex-font-style-tt">YES</span>" (without the quotes), if the solution exists and "<span class="tex-font-style-tt">NO</span>" (without the quotes) otherwise.</p><p>If the solution exists, then on the second line print <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... , <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(|<i>a</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup>)</span> — the recovered array.</p>





```input1
4 5
1 2 3 1
2 1 2 8
2 3 4 7
1 1 3 3
2 3 4 8

```




```input2
4 5
1 2 3 1
2 1 2 8
2 3 4 7
1 1 3 3
2 3 4 13

```




```output1
YES
4 7 4 7
```




```output2
NO

```


