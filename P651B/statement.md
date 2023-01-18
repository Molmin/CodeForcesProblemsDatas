## Description

<div><p>There are <span class="tex-span"><i>n</i></span> pictures delivered for the new exhibition. The <span class="tex-span"><i>i</i></span>-th painting has beauty <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. We know that a visitor becomes happy every time he passes from a painting to a more beautiful one.</p><p>We are allowed to arranged pictures in any order. What is the maximum possible number of times the visitor may become happy while passing all pictures from first to last? In other words, we are allowed to rearrange elements of <span class="tex-span"><i>a</i></span> in any order. What is the maximum possible number of indices <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i> - 1</span>), such that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i> + 1</sub> &gt; <i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p></div><div class="input-specification"><p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>)&nbsp;— the number of painting.</p><p>The second line contains the sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> means the beauty of the <span class="tex-span"><i>i</i></span>-th painting.</p></div><div class="output-specification"><p>Print one integer&nbsp;— the maximum possible number of neighbouring pairs, such that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i> + 1</sub> &gt; <i>a</i><sub class="lower-index"><i>i</i></sub></span>, after the optimal rearrangement.</p></div>

## Input

<p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>)&nbsp;— the number of painting.</p><p>The second line contains the sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> means the beauty of the <span class="tex-span"><i>i</i></span>-th painting.</p>

## Output

<p>Print one integer&nbsp;— the maximum possible number of neighbouring pairs, such that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i> + 1</sub> &gt; <i>a</i><sub class="lower-index"><i>i</i></sub></span>, after the optimal rearrangement.</p>





```input1
5
20 30 10 50 40

```




```input2
4
200 100 100 200

```




```output1
4

```




```output2
2

```



## Note

<p>In the first sample, the optimal order is: <span class="tex-span">10, 20, 30, 40, 50</span>.</p><p>In the second sample, the optimal order is: <span class="tex-span">100, 200, 100, 200</span>.</p>
