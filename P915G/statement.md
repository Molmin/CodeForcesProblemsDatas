## Description

<div><p>Let's call an array <span class="tex-span"><i>a</i></span> of size <span class="tex-span"><i>n</i></span> <span class="tex-font-style-it">coprime</span> iff <span class="tex-span"><i>gcd</i>(<i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub>) = 1</span>, where <span class="tex-span"><i>gcd</i></span> is the greatest common divisor of the arguments.</p><p>You are given two numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span>. For each <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>k</i></span>) you have to determine the number of <span class="tex-font-style-it">coprime</span> arrays <span class="tex-span"><i>a</i></span> of size <span class="tex-span"><i>n</i></span> such that for every <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>j</i> ≤ <i>n</i></span>) <span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>j</i></sub> ≤ <i>i</i></span>. Since the answers can be very large, you have to calculate them modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 2·10<sup class="upper-index">6</sup></span>) — the size of the desired arrays and the maximum upper bound on elements, respectively.</p></div><div class="output-specification"><p>Since printing <span class="tex-span">2·10<sup class="upper-index">6</sup></span> numbers may take a lot of time, you have to output the answer in such a way:</p><p>Let <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> be the number of <span class="tex-font-style-it">coprime</span> arrays with elements in range <span class="tex-span">[1, <i>i</i>]</span>, taken modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>. You have to print <img align="middle" class="tex-formula" src="file://zmDfcqwk.png" style="max-width: 100.0%;max-height: 100.0%;">, taken modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>. Here <img align="middle" class="tex-formula" src="file://jZZmWI9b.png" style="max-width: 100.0%;max-height: 100.0%;"> denotes bitwise xor operation (<span class="tex-font-style-tt">^</span> in C++ or Java, <span class="tex-font-style-tt">xor</span> in Pascal).</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 2·10<sup class="upper-index">6</sup></span>) — the size of the desired arrays and the maximum upper bound on elements, respectively.</p>

## Output

<p>Since printing <span class="tex-span">2·10<sup class="upper-index">6</sup></span> numbers may take a lot of time, you have to output the answer in such a way:</p><p>Let <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> be the number of <span class="tex-font-style-it">coprime</span> arrays with elements in range <span class="tex-span">[1, <i>i</i>]</span>, taken modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>. You have to print <img align="middle" class="tex-formula" src="file://zmDfcqwk.png" style="max-width: 100.0%;max-height: 100.0%;">, taken modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>. Here <img align="middle" class="tex-formula" src="file://jZZmWI9b.png" style="max-width: 100.0%;max-height: 100.0%;"> denotes bitwise xor operation (<span class="tex-font-style-tt">^</span> in C++ or Java, <span class="tex-font-style-tt">xor</span> in Pascal).</p>





```input1
3 4

```




```input2
2000000 8

```




```output1
82

```




```output2
339310063

```



## Note

<p>Explanation of the example:</p><p>Since the number of <span class="tex-font-style-it">coprime</span> arrays is large, we will list the arrays that are non-coprime, but contain only elements in range <span class="tex-span">[1, <i>i</i>]</span>:</p><p>For <span class="tex-span"><i>i</i> = 1</span>, the only array is coprime. <span class="tex-span"><i>b</i><sub class="lower-index">1</sub> = 1</span>.</p><p>For <span class="tex-span"><i>i</i> = 2</span>, array <span class="tex-span">[2, 2, 2]</span> is not coprime. <span class="tex-span"><i>b</i><sub class="lower-index">2</sub> = 7</span>.</p><p>For <span class="tex-span"><i>i</i> = 3</span>, arrays <span class="tex-span">[2, 2, 2]</span> and <span class="tex-span">[3, 3, 3]</span> are not coprime. <span class="tex-span"><i>b</i><sub class="lower-index">3</sub> = 25</span>.</p><p>For <span class="tex-span"><i>i</i> = 4</span>, arrays <span class="tex-span">[2, 2, 2]</span>, <span class="tex-span">[3, 3, 3]</span>, <span class="tex-span">[2, 2, 4]</span>, <span class="tex-span">[2, 4, 2]</span>, <span class="tex-span">[2, 4, 4]</span>, <span class="tex-span">[4, 2, 2]</span>, <span class="tex-span">[4, 2, 4]</span>, <span class="tex-span">[4, 4, 2]</span> and <span class="tex-span">[4, 4, 4]</span> are not coprime. <span class="tex-span"><i>b</i><sub class="lower-index">4</sub> = 55</span>.</p>
