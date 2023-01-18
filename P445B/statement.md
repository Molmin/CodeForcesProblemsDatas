## Description

<div><p><span class="tex-font-style-it">DZY loves chemistry, and he enjoys mixing chemicals.</span></p><p>DZY has <span class="tex-span"><i>n</i></span> chemicals, and <span class="tex-span"><i>m</i></span> pairs of them will react. He wants to pour these chemicals into a test tube, and he needs to pour them in one by one, in any order. </p><p>Let's consider the danger of a test tube. Danger of an empty test tube is <span class="tex-span">1</span>. And every time when DZY pours a chemical, if there are already one or more chemicals in the test tube that can react with it, the danger of the test tube will be multiplied by <span class="tex-span">2</span>. Otherwise the danger remains as it is.</p><p>Find the maximum possible danger after pouring all the chemicals one by one in optimal order.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <img align="middle" class="tex-formula" src="file://kqrj87kO.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains two space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> &lt; <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>. These integers mean that the chemical <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> will react with the chemical <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>. Each pair of chemicals will appear at most once in the input.</p><p>Consider all the chemicals numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> in some order.</p></div><div class="output-specification"><p>Print a single integer — the maximum possible danger.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <img align="middle" class="tex-formula" src="file://kqrj87kO.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains two space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> &lt; <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>. These integers mean that the chemical <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> will react with the chemical <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>. Each pair of chemicals will appear at most once in the input.</p><p>Consider all the chemicals numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> in some order.</p>

## Output

<p>Print a single integer — the maximum possible danger.</p>





```input1
1 0

```




```input2
2 1
1 2

```




```input3
3 2
1 2
2 3

```




```output1
1

```




```output2
2

```




```output3
4

```



## Note

<p>In the first sample, there's only one way to pour, and the danger won't increase.</p><p>In the second sample, no matter we pour the <span class="tex-span">1</span>st chemical first, or pour the <span class="tex-span">2</span>nd chemical first, the answer is always <span class="tex-span">2</span>.</p><p>In the third sample, there are four ways to achieve the maximum possible danger: 2-1-3, 2-3-1, 1-2-3 and 3-2-1 (that is the numbers of the chemicals in order of pouring).</p>
