## Description

<div><p>You are given two arrays <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span>, each of size <span class="tex-span"><i>n</i></span>. The error, <span class="tex-span"><i>E</i></span>, between these two arrays is defined <img align="middle" class="tex-formula" src="file://hVlng4Hq.png" style="max-width: 100.0%;max-height: 100.0%;">. You have to perform <span class="tex-font-style-bf">exactly</span> <span class="tex-span"><i>k</i><sub class="lower-index">1</sub></span> operations on array <span class="tex-span"><i>A</i></span> and <span class="tex-font-style-bf">exactly</span> <span class="tex-span"><i>k</i><sub class="lower-index">2</sub></span> operations on array <span class="tex-span"><i>B</i></span>. In one operation, you have to choose one element of the array and increase or decrease it by <span class="tex-span">1</span>.</p><p>Output the minimum possible value of error after <span class="tex-span"><i>k</i><sub class="lower-index">1</sub></span> operations on array <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>k</i><sub class="lower-index">2</sub></span> operations on array <span class="tex-span"><i>B</i></span> have been performed.</p></div><div class="input-specification"><p>The first line contains three space-separated integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">3</sup></span>), <span class="tex-span"><i>k</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>k</i><sub class="lower-index">2</sub></span> (<span class="tex-span">0 ≤ <i>k</i><sub class="lower-index">1</sub> + <i>k</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">3</sup></span>, <span class="tex-span"><i>k</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>k</i><sub class="lower-index">2</sub></span> are non-negative) — size of arrays and number of operations to perform on <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span> respectively.</p><p>Second line contains <span class="tex-span"><i>n</i></span> space separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">6</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — array <span class="tex-span"><i>A</i></span>.</p><p>Third line contains <span class="tex-span"><i>n</i></span> space separated integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">6</sup> ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>)— array <span class="tex-span"><i>B</i></span>.</p></div><div class="output-specification"><p>Output a single integer — the minimum possible value of <img align="middle" class="tex-formula" src="file://YwROIEik.png" style="max-width: 100.0%;max-height: 100.0%;"> after doing exactly <span class="tex-span"><i>k</i><sub class="lower-index">1</sub></span> operations on array <span class="tex-span"><i>A</i></span> and exactly <span class="tex-span"><i>k</i><sub class="lower-index">2</sub></span> operations on array <span class="tex-span"><i>B</i></span>.</p></div>

## Input

<p>The first line contains three space-separated integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">3</sup></span>), <span class="tex-span"><i>k</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>k</i><sub class="lower-index">2</sub></span> (<span class="tex-span">0 ≤ <i>k</i><sub class="lower-index">1</sub> + <i>k</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">3</sup></span>, <span class="tex-span"><i>k</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>k</i><sub class="lower-index">2</sub></span> are non-negative) — size of arrays and number of operations to perform on <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span> respectively.</p><p>Second line contains <span class="tex-span"><i>n</i></span> space separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">6</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — array <span class="tex-span"><i>A</i></span>.</p><p>Third line contains <span class="tex-span"><i>n</i></span> space separated integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">6</sup> ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>)— array <span class="tex-span"><i>B</i></span>.</p>

## Output

<p>Output a single integer — the minimum possible value of <img align="middle" class="tex-formula" src="file://YwROIEik.png" style="max-width: 100.0%;max-height: 100.0%;"> after doing exactly <span class="tex-span"><i>k</i><sub class="lower-index">1</sub></span> operations on array <span class="tex-span"><i>A</i></span> and exactly <span class="tex-span"><i>k</i><sub class="lower-index">2</sub></span> operations on array <span class="tex-span"><i>B</i></span>.</p>





```input1
2 0 0
1 2
2 3

```




```input2
2 1 0
1 2
2 2

```




```input3
2 5 7
3 4
14 4

```




```output1
2
```




```output2
0
```




```output3
1
```



## Note

<p>In the first sample case, we cannot perform any operations on <span class="tex-span"><i>A</i></span> or <span class="tex-span"><i>B</i></span>. Therefore the minimum possible error <span class="tex-span"><i>E</i> = (1 - 2)<sup class="upper-index">2</sup> + (2 - 3)<sup class="upper-index">2</sup> = 2</span>. </p><p>In the second sample case, we are required to perform exactly one operation on <span class="tex-span"><i>A</i></span>. In order to minimize error, we increment the first element of <span class="tex-span"><i>A</i></span> by <span class="tex-span">1</span>. Now, <span class="tex-span"><i>A</i> = [2, 2]</span>. The error is now <span class="tex-span"><i>E</i> = (2 - 2)<sup class="upper-index">2</sup> + (2 - 2)<sup class="upper-index">2</sup> = 0</span>. This is the minimum possible error obtainable.</p><p>In the third sample case, we can increase the first element of <span class="tex-span"><i>A</i></span> to <span class="tex-span">8</span>, using the all of the <span class="tex-span">5</span> moves available to us. Also, the first element of <span class="tex-span"><i>B</i></span> can be reduced to <span class="tex-span">8</span> using the <span class="tex-span">6</span> of the <span class="tex-span">7</span> available moves. Now <span class="tex-span"><i>A</i> = [8, 4]</span> and <span class="tex-span"><i>B</i> = [8, 4]</span>. The error is now <span class="tex-span"><i>E</i> = (8 - 8)<sup class="upper-index">2</sup> + (4 - 4)<sup class="upper-index">2</sup> = 0</span>, but we are still left with <span class="tex-span">1</span> move for array <span class="tex-span"><i>B</i></span>. Increasing the second element of <span class="tex-span"><i>B</i></span> to <span class="tex-span">5</span> using the left move, we get <span class="tex-span"><i>B</i> = [8, 5]</span> and <span class="tex-span"><i>E</i> = (8 - 8)<sup class="upper-index">2</sup> + (4 - 5)<sup class="upper-index">2</sup> = 1</span>.</p>
