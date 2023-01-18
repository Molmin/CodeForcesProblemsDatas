## Description

<div><p>There are <span class="tex-span"><i>n</i></span> stones on the table in a row, each of them can be red, green or blue. Count the minimum number of stones to take from the table so that any two neighboring stones had different colors. Stones in a row are considered neighboring if there are no other stones between them.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 50)</span> — the number of stones on the table. </p><p>The next line contains string <span class="tex-span"><i>s</i></span>, which represents the colors of the stones. We'll consider the stones in the row numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from left to right. Then the <span class="tex-span"><i>i</i></span>-th character <span class="tex-span"><i>s</i></span> equals "<span class="tex-font-style-tt">R</span>", if the <span class="tex-span"><i>i</i></span>-th stone is red, "<span class="tex-font-style-tt">G</span>", if it's green and "<span class="tex-font-style-tt">B</span>", if it's blue.</p></div><div class="output-specification"><p>Print a single integer — the answer to the problem.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 50)</span> — the number of stones on the table. </p><p>The next line contains string <span class="tex-span"><i>s</i></span>, which represents the colors of the stones. We'll consider the stones in the row numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from left to right. Then the <span class="tex-span"><i>i</i></span>-th character <span class="tex-span"><i>s</i></span> equals "<span class="tex-font-style-tt">R</span>", if the <span class="tex-span"><i>i</i></span>-th stone is red, "<span class="tex-font-style-tt">G</span>", if it's green and "<span class="tex-font-style-tt">B</span>", if it's blue.</p>

## Output

<p>Print a single integer — the answer to the problem.</p>





```input1
3
RRG

```




```input2
5
RRRRR

```




```input3
4
BRBG

```




```output1
1

```




```output2
4

```




```output3
0

```


