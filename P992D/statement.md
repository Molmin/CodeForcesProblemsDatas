## Description

<div><p>Nastya received one more array on her birthday, this array can be used to play a traditional Byteland game on it. However, to play the game the players should first select such a subsegment of the array that <img align="middle" class="tex-formula" src="file://H8JfHdYY.png" style="max-width: 100.0%;max-height: 100.0%;">, where <span class="tex-span"><i>p</i></span> is the product of all integers on the given array, <span class="tex-span"><i>s</i></span> is their sum, and <span class="tex-span"><i>k</i></span> is a given constant for all subsegments. </p><p>Nastya wonders how many subsegments of the array fit the described conditions. A subsegment of an array is several consecutive integers of the array.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>), where <span class="tex-span"><i>n</i></span> is the length of the array and <span class="tex-span"><i>k</i></span> is the constant described above.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup></span>)&nbsp;— the elements of the array.</p></div><div class="output-specification"><p>In the only line print the number of subsegments such that the ratio between the product and the sum on them is equal to <span class="tex-span"><i>k</i></span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>), where <span class="tex-span"><i>n</i></span> is the length of the array and <span class="tex-span"><i>k</i></span> is the constant described above.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup></span>)&nbsp;— the elements of the array.</p>

## Output

<p>In the only line print the number of subsegments such that the ratio between the product and the sum on them is equal to <span class="tex-span"><i>k</i></span>.</p>





```input1
1 1
1

```




```input2
4 2
6 3 8 1

```




```output1
1

```




```output2
2

```



## Note

<p>In the first example the only subsegment is <span class="tex-span">[1]</span>. The sum equals <span class="tex-span">1</span>, the product equals <span class="tex-span">1</span>, so it suits us because <img align="middle" class="tex-formula" src="file://Bo9xdW7h.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>There are two suitable subsegments in the second example — <span class="tex-span">[6, 3]</span> and <span class="tex-span">[3, 8, 1]</span>. Subsegment <span class="tex-span">[6, 3]</span> has sum <span class="tex-span">9</span> and product <span class="tex-span">18</span>, so it suits us because <img align="middle" class="tex-formula" src="file://wLos0zti.png" style="max-width: 100.0%;max-height: 100.0%;">. Subsegment <span class="tex-span">[3, 8, 1]</span> has sum <span class="tex-span">12</span> and product <span class="tex-span">24</span>, so it suits us because <img align="middle" class="tex-formula" src="file://LSnlu2na.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
