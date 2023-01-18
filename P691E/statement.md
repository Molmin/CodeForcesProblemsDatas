## Description

<div><p>You are given <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>,  <i>a</i><sub class="lower-index">2</sub>,  ...,  <i>a</i><sub class="lower-index"><i>n</i></sub></span>.</p><p>A sequence of integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>,  <i>x</i><sub class="lower-index">2</sub>,  ...,  <i>x</i><sub class="lower-index"><i>k</i></sub></span> is called a "<span class="tex-font-style-tt">xor-sequence</span>" if for every <span class="tex-span">1  ≤  <i>i</i>  ≤  <i>k</i> - 1</span> the number of ones in the binary representation of the number <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> <img align="middle" class="tex-formula" src="file://9nYQ9C5J.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i>  +  1</sub></span>'s is a multiple of <span class="tex-span">3</span> and <img align="middle" class="tex-formula" src="file://aupGKCEl.png" style="max-width: 100.0%;max-height: 100.0%;"> for all <span class="tex-span">1 ≤ <i>i</i> ≤ <i>k</i></span>. The symbol <img align="middle" class="tex-formula" src="file://sHzvCaYY.png" style="max-width: 100.0%;max-height: 100.0%;"> is used for the binary exclusive or operation.</p><p>How many "<span class="tex-font-style-tt">xor-sequences</span>" of length <span class="tex-span"><i>k</i></span> exist? Output the answer modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p><p><span class="tex-font-style-bf">Note if <span class="tex-span"><i>a</i> = [1, 1]</span> and <span class="tex-span"><i>k</i> = 1</span> then the answer is <span class="tex-span">2</span>, because you should consider the ones from <span class="tex-span"><i>a</i></span> as different.</span></p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">18</sup></span>) — the number of given integers and the length of the "<span class="tex-font-style-tt">xor-sequences</span>".</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">18</sup></span>).</p></div><div class="output-specification"><p>Print the only integer <span class="tex-span"><i>c</i></span> — the number of "<span class="tex-font-style-tt">xor-sequences</span>" of length <span class="tex-span"><i>k</i></span> modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">18</sup></span>) — the number of given integers and the length of the "<span class="tex-font-style-tt">xor-sequences</span>".</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">18</sup></span>).</p>

## Output

<p>Print the only integer <span class="tex-span"><i>c</i></span> — the number of "<span class="tex-font-style-tt">xor-sequences</span>" of length <span class="tex-span"><i>k</i></span> modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
5 2
15 1 2 4 8

```




```input2
5 1
15 1 2 4 8

```




```output1
13

```




```output2
5

```


