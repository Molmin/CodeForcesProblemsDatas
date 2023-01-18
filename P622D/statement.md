## Description

<div><p>You have array <span class="tex-span"><i>a</i></span> that contains all integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> twice. You can arbitrary permute any numbers in <span class="tex-span"><i>a</i></span>.</p><p>Let number <span class="tex-span"><i>i</i></span> be in positions <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> &lt; <i>y</i><sub class="lower-index"><i>i</i></sub></span>) in the permuted array <span class="tex-span"><i>a</i></span>. Let's define the value <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub> = <i>y</i><sub class="lower-index"><i>i</i></sub> - <i>x</i><sub class="lower-index"><i>i</i></sub></span> — the distance between the positions of the number <span class="tex-span"><i>i</i></span>. Permute the numbers in array <span class="tex-span"><i>a</i></span> to minimize the value of the sum <img align="middle" class="tex-formula" src="file://1CT6Ej6w.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div><div class="input-specification"><p>The only line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>).</p></div><div class="output-specification"><p>Print <span class="tex-span">2<i>n</i></span> integers — the permuted array <span class="tex-span"><i>a</i></span> that minimizes the value of the sum <span class="tex-span"><i>s</i></span>.</p></div>

## Input

<p>The only line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>).</p>

## Output

<p>Print <span class="tex-span">2<i>n</i></span> integers — the permuted array <span class="tex-span"><i>a</i></span> that minimizes the value of the sum <span class="tex-span"><i>s</i></span>.</p>





```input1
2

```




```input2
1

```




```output1
1 1 2 2

```




```output2
1 1

```


