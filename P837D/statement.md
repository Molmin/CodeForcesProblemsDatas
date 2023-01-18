## Description

<div><p>Let's call the <span class="tex-font-style-it">roundness</span> of the number the number of zeros to which it ends.</p><p>You have an array of <span class="tex-span"><i>n</i></span> numbers. You need to choose a subset of exactly <span class="tex-span"><i>k</i></span> numbers so that the <span class="tex-font-style-it">roundness</span> of the product of the selected numbers will be maximum possible.</p></div><div class="input-specification"><p>The first line contains two integer numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200, 1 ≤ <i>k</i> ≤ <i>n</i></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">18</sup></span>).</p></div><div class="output-specification"><p>Print maximal roundness of product of the chosen subset of length <span class="tex-span"><i>k</i></span>.</p></div>

## Input

<p>The first line contains two integer numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200, 1 ≤ <i>k</i> ≤ <i>n</i></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">18</sup></span>).</p>

## Output

<p>Print maximal roundness of product of the chosen subset of length <span class="tex-span"><i>k</i></span>.</p>





```input1
3 2
50 4 20

```




```input2
5 3
15 16 3 25 9

```




```input3
3 3
9 77 13

```




```output1
3

```




```output2
3

```




```output3
0

```



## Note

<p>In the first example there are <span class="tex-font-style-tt">3</span> subsets of <span class="tex-font-style-tt">2</span> numbers. <span class="tex-span">[50, 4]</span> has product <span class="tex-font-style-tt">200</span> with <span class="tex-font-style-it">roundness</span> <span class="tex-font-style-tt">2</span>, <span class="tex-span">[4, 20]</span> — product <span class="tex-font-style-tt">80</span>, <span class="tex-font-style-it">roundness</span> <span class="tex-font-style-tt">1</span>, <span class="tex-span">[50, 20]</span> — product <span class="tex-font-style-tt">1000</span>, <span class="tex-font-style-it">roundness</span> <span class="tex-font-style-tt">3</span>.</p><p>In the second example subset <span class="tex-span">[15, 16, 25]</span> has product <span class="tex-font-style-tt">6000</span>, <span class="tex-font-style-it">roundness</span> <span class="tex-font-style-tt">3</span>.</p><p>In the third example all subsets has product with <span class="tex-font-style-it">roundness</span> <span class="tex-font-style-tt">0</span>.</p>
