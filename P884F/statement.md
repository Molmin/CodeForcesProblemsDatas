## Description

<div><p>A string <span class="tex-span"><i>a</i></span> of length <span class="tex-span"><i>m</i></span> is called <span class="tex-font-style-it">antipalindromic</span> iff <span class="tex-span"><i>m</i></span> is even, and for each <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>m</i></span>) <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>a</i><sub class="lower-index"><i>m</i> - <i>i</i> + 1</sub></span>.</p><p>Ivan has a string <span class="tex-span"><i>s</i></span> consisting of <span class="tex-span"><i>n</i></span> lowercase Latin letters; <span class="tex-span"><i>n</i></span> is even. He wants to form some string <span class="tex-span"><i>t</i></span> that will be an <span class="tex-font-style-it">antipalindromic</span> permutation of <span class="tex-span"><i>s</i></span>. Also Ivan has denoted the <span class="tex-font-style-it">beauty</span> of index <span class="tex-span"><i>i</i></span> as <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, and the <span class="tex-font-style-it">beauty</span> of <span class="tex-span"><i>t</i></span> as the sum of <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> among all indices <span class="tex-span"><i>i</i></span> such that <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub> = <i>t</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Help Ivan to determine maximum possible <span class="tex-font-style-it">beauty</span> of <span class="tex-span"><i>t</i></span> he can get.</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span"><i>n</i></span> is even) — the number of characters in <span class="tex-span"><i>s</i></span>.</p><p>The second line contains the string <span class="tex-span"><i>s</i></span> itself. It consists of only lowercase Latin letters, and it is guaranteed that its letters can be reordered to form an <span class="tex-font-style-it">antipalindromic</span> string.</p><p>The third line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>), where <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> is the <span class="tex-font-style-it">beauty</span> of index <span class="tex-span"><i>i</i></span>.</p></div><div class="output-specification"><p>Print one number — the maximum possible <span class="tex-font-style-it">beauty</span> of <span class="tex-span"><i>t</i></span>.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span"><i>n</i></span> is even) — the number of characters in <span class="tex-span"><i>s</i></span>.</p><p>The second line contains the string <span class="tex-span"><i>s</i></span> itself. It consists of only lowercase Latin letters, and it is guaranteed that its letters can be reordered to form an <span class="tex-font-style-it">antipalindromic</span> string.</p><p>The third line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>), where <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> is the <span class="tex-font-style-it">beauty</span> of index <span class="tex-span"><i>i</i></span>.</p>

## Output

<p>Print one number — the maximum possible <span class="tex-font-style-it">beauty</span> of <span class="tex-span"><i>t</i></span>.</p>





```input1
8
abacabac
1 1 1 1 1 1 1 1

```




```input2
8
abaccaba
1 2 3 4 5 6 7 8

```




```input3
8
abacabca
1 2 3 4 4 3 2 1

```




```output1
8

```




```output2
26

```




```output3
17

```


