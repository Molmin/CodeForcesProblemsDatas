## Description

<div><p>Consider an array <span class="tex-span"><i>A</i></span> with <span class="tex-span"><i>N</i></span> elements, all being the same integer <span class="tex-span"><i>a</i></span>.</p><p>Define the product transformation as a simultaneous update <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i></sub> = <i>A</i><sub class="lower-index"><i>i</i></sub>·<i>A</i><sub class="lower-index"><i>i</i> + 1</sub></span>, that is multiplying each element to the element right to it for <img align="middle" class="tex-formula" src="file://CrI5Qtq6.png" style="max-width: 100.0%;max-height: 100.0%;">, with the last number <span class="tex-span"><i>A</i><sub class="lower-index"><i>N</i></sub></span> remaining the same. For example, if we start with an array <span class="tex-span"><i>A</i></span> with <span class="tex-span"><i>a</i> = 2</span> and <span class="tex-span"><i>N</i> = 4</span>, then after one product transformation <span class="tex-span"><i>A</i> = [4,  4,  4,  2]</span>, and after two product transformations <span class="tex-span"><i>A</i> = [16,  16,  8,  2]</span>.</p><p>Your simple task is to calculate the array <span class="tex-span"><i>A</i></span> after <span class="tex-span"><i>M</i></span> product transformations. Since the numbers can get quite big you should output them modulo <span class="tex-span"><i>Q</i></span>.</p></div><div class="input-specification"><p>The first and only line of input contains four integers <span class="tex-span"><i>N</i></span>, <span class="tex-span"><i>M</i></span>, <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>Q</i></span> (<span class="tex-span">7 ≤ <i>Q</i> ≤ 10<sup class="upper-index">9</sup> + 123</span>, <span class="tex-span">2 ≤ <i>a</i> ≤ 10<sup class="upper-index">6</sup> + 123</span>, <img align="middle" class="tex-formula" src="file://m4ANK0Ny.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://VubA43kf.png" style="max-width: 100.0%;max-height: 100.0%;"> is prime), where <img align="middle" class="tex-formula" src="file://qy2HVYIX.png" style="max-width: 100.0%;max-height: 100.0%;"> is the multiplicative order of the integer <span class="tex-span"><i>a</i></span> modulo <span class="tex-span"><i>Q</i></span>, see notes for definition.</p></div><div class="output-specification"><p>You should output the array <span class="tex-span"><i>A</i></span> from left to right.</p></div>

## Input

<p>The first and only line of input contains four integers <span class="tex-span"><i>N</i></span>, <span class="tex-span"><i>M</i></span>, <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>Q</i></span> (<span class="tex-span">7 ≤ <i>Q</i> ≤ 10<sup class="upper-index">9</sup> + 123</span>, <span class="tex-span">2 ≤ <i>a</i> ≤ 10<sup class="upper-index">6</sup> + 123</span>, <img align="middle" class="tex-formula" src="file://m4ANK0Ny.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://VubA43kf.png" style="max-width: 100.0%;max-height: 100.0%;"> is prime), where <img align="middle" class="tex-formula" src="file://qy2HVYIX.png" style="max-width: 100.0%;max-height: 100.0%;"> is the multiplicative order of the integer <span class="tex-span"><i>a</i></span> modulo <span class="tex-span"><i>Q</i></span>, see notes for definition.</p>

## Output

<p>You should output the array <span class="tex-span"><i>A</i></span> from left to right.</p>





```input1
2 2 2 7

```




```output1
1 2
```



## Note

<p>The multiplicative order of a number <span class="tex-span"><i>a</i></span> modulo <span class="tex-span"><i>Q</i></span> <img align="middle" class="tex-formula" src="file://VXXEjclu.png" style="max-width: 100.0%;max-height: 100.0%;">, is the smallest natural number <span class="tex-span"><i>x</i></span> such that <span class="tex-span"><i>a</i><sup class="upper-index"><i>x</i></sup> <i>mod</i> <i>Q</i> = 1</span>. For example, <img align="middle" class="tex-formula" src="file://sxE8UZ0H.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
