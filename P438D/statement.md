## Description

<div><p>At the children's day, the child came to Picks's house, and messed his house up. Picks was angry at him. A lot of important things were lost, in particular the favorite sequence of Picks.</p><p>Fortunately, Picks remembers how to repair the sequence. Initially he should create an integer array <span class="tex-span"><i>a</i>[1], <i>a</i>[2], ..., <i>a</i>[<i>n</i>]</span>. Then he should perform a sequence of <span class="tex-span"><i>m</i></span> operations. An operation can be one of the following:</p><ol> <li> Print operation <span class="tex-span"><i>l</i>, <i>r</i></span>. Picks should write down the value of <img align="middle" class="tex-formula" src="file://ejsUnvWx.png" style="max-width: 100.0%;max-height: 100.0%;">. </li><li> Modulo operation <span class="tex-span"><i>l</i>, <i>r</i>, <i>x</i></span>. Picks should perform assignment <span class="tex-span"><i>a</i>[<i>i</i>] = <i>a</i>[<i>i</i>]&nbsp;<i>mod</i>&nbsp;<i>x</i></span> for each <span class="tex-span"><i>i</i></span> <span class="tex-span">(<i>l</i> ≤ <i>i</i> ≤ <i>r</i>)</span>. </li><li> Set operation <span class="tex-span"><i>k</i>, <i>x</i></span>. Picks should set the value of <span class="tex-span"><i>a</i>[<i>k</i>]</span> to <span class="tex-span"><i>x</i></span> (in other words perform an assignment <span class="tex-span"><i>a</i>[<i>k</i>] = <i>x</i></span>). </li></ol><p>Can you help Picks to perform the whole sequence of operations?</p></div><div class="input-specification"><p>The first line of input contains two integer: <span class="tex-span"><i>n</i>, <i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> integers, separated by space: <span class="tex-span"><i>a</i>[1], <i>a</i>[2], ..., <i>a</i>[<i>n</i>]&nbsp;(1 ≤ <i>a</i>[<i>i</i>] ≤ 10<sup class="upper-index">9</sup>)</span> — initial value of array elements.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines begins with a number <span class="tex-span"><i>type</i></span> <img align="middle" class="tex-formula" src="file://JRKflBWY.png" style="max-width: 100.0%;max-height: 100.0%;">. </p><ul> <li> If <span class="tex-span"><i>type</i> = 1</span>, there will be two integers more in the line: <span class="tex-span"><i>l</i>, <i>r</i>&nbsp;(1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i>)</span>, which correspond the operation 1. </li><li> If <span class="tex-span"><i>type</i> = 2</span>, there will be three integers more in the line: <span class="tex-span"><i>l</i>, <i>r</i>, <i>x</i>&nbsp;(1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i>;&nbsp;1 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup>)</span>, which correspond the operation 2. </li><li> If <span class="tex-span"><i>type</i> = 3</span>, there will be two integers more in the line: <span class="tex-span"><i>k</i>, <i>x</i>&nbsp;(1 ≤ <i>k</i> ≤ <i>n</i>;&nbsp;1 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup>)</span>, which correspond the operation 3. </li></ul></div><div class="output-specification"><p>For each operation 1, please print a line containing the answer. Notice that the answer may exceed the 32-bit integer.</p></div>

## Input

<p>The first line of input contains two integer: <span class="tex-span"><i>n</i>, <i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> integers, separated by space: <span class="tex-span"><i>a</i>[1], <i>a</i>[2], ..., <i>a</i>[<i>n</i>]&nbsp;(1 ≤ <i>a</i>[<i>i</i>] ≤ 10<sup class="upper-index">9</sup>)</span> — initial value of array elements.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines begins with a number <span class="tex-span"><i>type</i></span> <img align="middle" class="tex-formula" src="file://JRKflBWY.png" style="max-width: 100.0%;max-height: 100.0%;">. </p><ul> <li> If <span class="tex-span"><i>type</i> = 1</span>, there will be two integers more in the line: <span class="tex-span"><i>l</i>, <i>r</i>&nbsp;(1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i>)</span>, which correspond the operation 1. </li><li> If <span class="tex-span"><i>type</i> = 2</span>, there will be three integers more in the line: <span class="tex-span"><i>l</i>, <i>r</i>, <i>x</i>&nbsp;(1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i>;&nbsp;1 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup>)</span>, which correspond the operation 2. </li><li> If <span class="tex-span"><i>type</i> = 3</span>, there will be two integers more in the line: <span class="tex-span"><i>k</i>, <i>x</i>&nbsp;(1 ≤ <i>k</i> ≤ <i>n</i>;&nbsp;1 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup>)</span>, which correspond the operation 3. </li></ul>

## Output

<p>For each operation 1, please print a line containing the answer. Notice that the answer may exceed the 32-bit integer.</p>





```input1
5 5
1 2 3 4 5
2 3 5 4
3 3 5
1 2 5
2 1 3 3
1 1 3

```




```input2
10 10
6 9 6 7 6 1 10 10 9 5
1 3 9
2 7 10 9
2 5 10 8
1 4 7
3 3 7
2 7 9 9
1 2 4
1 6 6
1 5 9
3 1 10

```




```output1
8
5

```




```output2
49
15
23
1
9

```



## Note

<p>Consider the first testcase:</p><ul> <li> At first, <span class="tex-span"><i>a</i> = {1, 2, 3, 4, 5}</span>. </li><li> After operation <span class="tex-span">1</span>, <span class="tex-span"><i>a</i> = {1, 2, 3, 0, 1}</span>. </li><li> After operation <span class="tex-span">2</span>, <span class="tex-span"><i>a</i> = {1, 2, 5, 0, 1}</span>. </li><li> At operation <span class="tex-span">3</span>, <span class="tex-span">2 + 5 + 0 + 1 = 8</span>. </li><li> After operation <span class="tex-span">4</span>, <span class="tex-span"><i>a</i> = {1, 2, 2, 0, 1}</span>. </li><li> At operation <span class="tex-span">5</span>, <span class="tex-span">1 + 2 + 2 = 5</span>. <ul></ul></li></ul>
