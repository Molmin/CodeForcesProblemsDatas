## Description

<div><p>Valera has array <span class="tex-span"><i>a</i></span>, consisting of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">0</sub>, <i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i> - 1</sub></span>, and function <span class="tex-span"><i>f</i>(<i>x</i>)</span>, taking an integer from <span class="tex-span">0</span> to <span class="tex-span">2<sup class="upper-index"><i>n</i></sup> - 1</span> as its single argument. Value <span class="tex-span"><i>f</i>(<i>x</i>)</span> is calculated by formula <img align="middle" class="tex-formula" src="file://mtHv0xBH.png" style="max-width: 100.0%;max-height: 100.0%;">, where value <span class="tex-span"><i>bit</i>(<i>i</i>)</span> equals one if the binary representation of number <span class="tex-span"><i>x</i></span> contains a <span class="tex-span">1</span> on the <span class="tex-span"><i>i</i></span>-th position, and zero otherwise.</p><p>For example, if <span class="tex-span"><i>n</i> = 4</span> and <span class="tex-span"><i>x</i> = 11</span> <span class="tex-span">(11 = 2<sup class="upper-index">0</sup> + 2<sup class="upper-index">1</sup> + 2<sup class="upper-index">3</sup>)</span>, then <span class="tex-span"><i>f</i>(<i>x</i>) = <i>a</i><sub class="lower-index">0</sub> + <i>a</i><sub class="lower-index">1</sub> + <i>a</i><sub class="lower-index">3</sub></span>.</p><p>Help Valera find the maximum of function <span class="tex-span"><i>f</i>(<i>x</i>)</span> among all <span class="tex-span"><i>x</i></span>, for which an inequality holds: <span class="tex-span">0 ≤ <i>x</i> ≤ <i>m</i></span>.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of array elements. The next line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">0</sub>, <i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i> - 1</sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup>)</span> — elements of array <span class="tex-span"><i>a</i></span>.</p><p>The third line contains a sequence of digits zero and one without spaces <span class="tex-span"><i>s</i><sub class="lower-index">0</sub><i>s</i><sub class="lower-index">1</sub>... <i>s</i><sub class="lower-index"><i>n</i> - 1</sub></span> — the binary representation of number <span class="tex-span"><i>m</i></span>. Number <span class="tex-span"><i>m</i></span> equals <img align="middle" class="tex-formula" src="file://l4EHBocs.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div><div class="output-specification"><p>Print a single integer — the maximum value of function <span class="tex-span"><i>f</i>(<i>x</i>)</span> for all <img align="middle" class="tex-formula" src="file://tZqGumKX.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of array elements. The next line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">0</sub>, <i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i> - 1</sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup>)</span> — elements of array <span class="tex-span"><i>a</i></span>.</p><p>The third line contains a sequence of digits zero and one without spaces <span class="tex-span"><i>s</i><sub class="lower-index">0</sub><i>s</i><sub class="lower-index">1</sub>... <i>s</i><sub class="lower-index"><i>n</i> - 1</sub></span> — the binary representation of number <span class="tex-span"><i>m</i></span>. Number <span class="tex-span"><i>m</i></span> equals <img align="middle" class="tex-formula" src="file://l4EHBocs.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>

## Output

<p>Print a single integer — the maximum value of function <span class="tex-span"><i>f</i>(<i>x</i>)</span> for all <img align="middle" class="tex-formula" src="file://tZqGumKX.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
2
3 8
10

```




```input2
5
17 0 10 2 1
11010

```




```output1
3

```




```output2
27

```



## Note

<p>In the first test case <span class="tex-span"><i>m</i> = 2<sup class="upper-index">0</sup> = 1, <i>f</i>(0) = 0, <i>f</i>(1) = <i>a</i><sub class="lower-index">0</sub> = 3</span>.</p><p>In the second sample <span class="tex-span"><i>m</i> = 2<sup class="upper-index">0</sup> + 2<sup class="upper-index">1</sup> + 2<sup class="upper-index">3</sup> = 11</span>, the maximum value of function equals <span class="tex-span"><i>f</i>(5) = <i>a</i><sub class="lower-index">0</sub> + <i>a</i><sub class="lower-index">2</sub> = 17 + 10 = 27</span>.</p>
