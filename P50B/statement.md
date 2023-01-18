## Description

<div><p>There is a given string <span class="tex-span"><i>S</i></span> consisting of <span class="tex-span"><i>N</i></span> symbols. Your task is to find the number of ordered pairs of integers <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> such that</p><p>1. <span class="tex-span">1 ≤ <i>i</i>, <i>j</i> ≤ <i>N</i></span></p><p>2. <span class="tex-span"><i>S</i>[<i>i</i>] = <i>S</i>[<i>j</i>]</span>, that is the <span class="tex-span"><i>i</i></span>-th symbol of string <span class="tex-span"><i>S</i></span> is equal to the <span class="tex-span"><i>j</i></span>-th.</p></div><div class="input-specification"><p>The single input line contains <span class="tex-span"><i>S</i></span>, consisting of lowercase Latin letters and digits. It is guaranteed that string <span class="tex-span"><i>S</i></span> in not empty and its length does not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p></div><div class="output-specification"><p>Print a single number which represents the number of pairs <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> with the needed property. Pairs <span class="tex-span">(<i>x</i>, <i>y</i>)</span> and <span class="tex-span">(<i>y</i>, <i>x</i>)</span> should be considered different, i.e. the ordered pairs count.</p></div>

## Input

<p>The single input line contains <span class="tex-span"><i>S</i></span>, consisting of lowercase Latin letters and digits. It is guaranteed that string <span class="tex-span"><i>S</i></span> in not empty and its length does not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p>

## Output

<p>Print a single number which represents the number of pairs <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> with the needed property. Pairs <span class="tex-span">(<i>x</i>, <i>y</i>)</span> and <span class="tex-span">(<i>y</i>, <i>x</i>)</span> should be considered different, i.e. the ordered pairs count.</p>





```input1
great10

```




```input2
aaaaaaaaaa

```




```output1
7

```




```output2
100

```


