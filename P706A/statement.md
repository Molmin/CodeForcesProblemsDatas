## Description

<div><p>Vasiliy lives at point <span class="tex-span">(<i>a</i>, <i>b</i>)</span> of the coordinate plane. He is hurrying up to work so he wants to get out of his house as soon as possible. New app suggested <span class="tex-span"><i>n</i></span> available Beru-taxi nearby. The <span class="tex-span"><i>i</i></span>-th taxi is located at point <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> and moves with a speed <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. </p><p>Consider that each of <span class="tex-span"><i>n</i></span> drivers will move directly to Vasiliy and with a maximum possible speed. Compute the minimum time when Vasiliy will get in any of Beru-taxi cars.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span"> - 100 ≤ <i>a</i>, <i>b</i> ≤ 100</span>)&nbsp;— coordinates of Vasiliy's home.</p><p>The second line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>)&nbsp;— the number of available Beru-taxi cars nearby. </p><p>The <span class="tex-span"><i>i</i></span>-th of the following <span class="tex-span"><i>n</i></span> lines contains three integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 100 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>, <span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>)&nbsp;— the coordinates of the <span class="tex-span"><i>i</i></span>-th car and its speed.</p><p>It's allowed that several cars are located at the same point. Also, cars may be located at exactly the same point where Vasiliy lives.</p></div><div class="output-specification"><p>Print a single real value&nbsp;— the minimum time Vasiliy needs to get in any of the Beru-taxi cars. You answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. </p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct, if <img align="middle" class="tex-formula" src="file://d4OZWiFv.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span"> - 100 ≤ <i>a</i>, <i>b</i> ≤ 100</span>)&nbsp;— coordinates of Vasiliy's home.</p><p>The second line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>)&nbsp;— the number of available Beru-taxi cars nearby. </p><p>The <span class="tex-span"><i>i</i></span>-th of the following <span class="tex-span"><i>n</i></span> lines contains three integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 100 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>, <span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>)&nbsp;— the coordinates of the <span class="tex-span"><i>i</i></span>-th car and its speed.</p><p>It's allowed that several cars are located at the same point. Also, cars may be located at exactly the same point where Vasiliy lives.</p>

## Output

<p>Print a single real value&nbsp;— the minimum time Vasiliy needs to get in any of the Beru-taxi cars. You answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. </p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct, if <img align="middle" class="tex-formula" src="file://d4OZWiFv.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
0 0
2
2 0 1
0 2 2

```




```input2
1 3
3
3 3 2
-2 3 6
-2 7 10

```




```output1
1.00000000000000000000
```




```output2
0.50000000000000000000
```



## Note

<p>In the first sample, first taxi will get to Vasiliy in time <span class="tex-span">2</span>, and second will do this in time <span class="tex-span">1</span>, therefore <span class="tex-span">1</span> is the answer.</p><p>In the second sample, cars <span class="tex-span">2</span> and <span class="tex-span">3</span> will arrive simultaneously.</p>
