## Description

<div><p>Valerian was captured by Shapur. The victory was such a great one that Shapur decided to carve a scene of Valerian's defeat on a mountain. So he had to find the best place to make his victory eternal!</p><p>He decided to visit all <span class="tex-span"><i>n</i></span> cities of Persia to find the best available mountain, but after the recent war he was too tired and didn't want to traverse a lot. So he wanted to visit each of these <span class="tex-span"><i>n</i></span> cities at least once with smallest possible traverse. Persian cities are connected with bidirectional roads. You can go from any city to any other one using these roads and there is a unique path between each two cities.</p><p>All cities are numbered <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Shapur is currently in the city <span class="tex-span">1</span> and he wants to visit all other cities with minimum possible traverse. He can finish his travels in any city.</p><p>Help Shapur find how much He should travel.</p></div><div class="input-specification"><p>First line contains a single natural number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the amount of cities.</p><p>Next <span class="tex-span"><i>n</i> - 1</span> lines contain <span class="tex-span">3</span> integer numbers each <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 0 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 2 × 10<sup class="upper-index">4</sup></span>). <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> are two ends of a road and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> is the length of that road.</p></div><div class="output-specification"><p>A single integer number, the minimal length of Shapur's travel.</p><p>Please, do not use <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preffered to use <span class="tex-font-style-tt">cout</span> (also you may use <span class="tex-font-style-tt">%I64d</span>).</p></div>

## Input

<p>First line contains a single natural number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the amount of cities.</p><p>Next <span class="tex-span"><i>n</i> - 1</span> lines contain <span class="tex-span">3</span> integer numbers each <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 0 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 2 × 10<sup class="upper-index">4</sup></span>). <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> are two ends of a road and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> is the length of that road.</p>

## Output

<p>A single integer number, the minimal length of Shapur's travel.</p><p>Please, do not use <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preffered to use <span class="tex-font-style-tt">cout</span> (also you may use <span class="tex-font-style-tt">%I64d</span>).</p>





```input1
3
1 2 3
2 3 4

```




```input2
3
1 2 3
1 3 3

```




```output1
7

```




```output2
9

```


