## Description

<div><p>Just in case somebody missed it: this winter is totally cold in Nvodsk! It is so cold that one gets funny thoughts. For example, let's say there are strings with the length exactly <span class="tex-span"><i>n</i></span>, based on the alphabet of size <span class="tex-span"><i>m</i></span>. Any its substring with length equal to <span class="tex-span"><i>k</i></span> is a palindrome. How many such strings exist? Your task is to find their quantity modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>). Be careful and don't miss a string or two!</p><p>Let us remind you that a string is a palindrome if it can be read the same way in either direction, from the left to the right and from the right to the left.</p></div><div class="input-specification"><p>The first and only line contains three integers: <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i>, <i>k</i> ≤ 2000</span>).</p></div><div class="output-specification"><p>Print a single integer — the number of strings of the described type modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p></div>

## Input

<p>The first and only line contains three integers: <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i>, <i>k</i> ≤ 2000</span>).</p>

## Output

<p>Print a single integer — the number of strings of the described type modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p>





```input1
1 1 1

```




```input2
5 2 4

```




```output1
1

```




```output2
2

```



## Note

<p>In the first sample only one string is valid: "<span class="tex-font-style-tt">a</span>" (let's denote the only letter of our alphabet as "<span class="tex-font-style-tt">a</span>").</p><p>In the second sample (if we denote the alphabet letters as "<span class="tex-font-style-tt">a</span>" and "<span class="tex-font-style-tt">b</span>") the following strings are valid: "<span class="tex-font-style-tt">aaaaa</span>" and "<span class="tex-font-style-tt">bbbbb</span>".</p>
