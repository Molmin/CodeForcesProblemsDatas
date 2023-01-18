## Description

<div><p>One day in the IT lesson Anna and Maria learned about the lexicographic order.</p><p>String <span class="tex-span"><i>x</i></span> is lexicographically less than string <span class="tex-span"><i>y</i></span>, if either <span class="tex-span"><i>x</i></span> is a prefix of <span class="tex-span"><i>y</i></span> (and <span class="tex-span"><i>x</i> ≠ <i>y</i></span>), or there exists such <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>min</i>(|<i>x</i>|, |<i>y</i>|)</span>), that <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> &lt; <i>y</i><sub class="lower-index"><i>i</i></sub></span>, and for any <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>j</i> &lt; <i>i</i></span>) <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub> = <i>y</i><sub class="lower-index"><i>j</i></sub></span>. Here <span class="tex-span">|<i>a</i>|</span> denotes the length of the string <span class="tex-span"><i>a</i></span>. The lexicographic comparison of strings is implemented by operator &lt; in modern programming languages​​.</p><p>The teacher gave Anna and Maria homework. She gave them a string of length <span class="tex-span"><i>n</i></span>. They should write out all substrings of the given string, including the whole initial string, and the equal substrings (for example, one should write out the following substrings from the string "<span class="tex-font-style-tt">aab</span>": "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">aa</span>", "<span class="tex-font-style-tt">ab</span>", "<span class="tex-font-style-tt">aab</span>", "<span class="tex-font-style-tt">b</span>"). The resulting strings should be sorted in the lexicographical order. The cunning teacher doesn't want to check all these strings. That's why she said to find only the <span class="tex-span"><i>k</i></span>-th string from the list. Help Anna and Maria do the homework.</p></div><div class="input-specification"><p>The first line contains a non-empty string that only consists of small Latin letters ("<span class="tex-font-style-tt">a</span>"-"<span class="tex-font-style-tt">z</span>"), whose length does not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>. The second line contains the only integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>).</p></div><div class="output-specification"><p>Print the string Anna and Maria need — the <span class="tex-span"><i>k</i></span>-th (in the lexicographical order) substring of the given string. If the total number of substrings is less than <span class="tex-span"><i>k</i></span>, print a string saying "<span class="tex-font-style-tt">No such line.</span>" (without the quotes).</p></div>

## Input

<p>The first line contains a non-empty string that only consists of small Latin letters ("<span class="tex-font-style-tt">a</span>"-"<span class="tex-font-style-tt">z</span>"), whose length does not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>. The second line contains the only integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>).</p>

## Output

<p>Print the string Anna and Maria need — the <span class="tex-span"><i>k</i></span>-th (in the lexicographical order) substring of the given string. If the total number of substrings is less than <span class="tex-span"><i>k</i></span>, print a string saying "<span class="tex-font-style-tt">No such line.</span>" (without the quotes).</p>





```input1
aa
2

```




```input2
abc
5

```




```input3
abab
7

```




```output1
a

```




```output2
bc

```




```output3
b

```



## Note

<p>In the second sample before string "<span class="tex-font-style-tt">bc</span>" follow strings "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">ab</span>", "<span class="tex-font-style-tt">abc</span>", "<span class="tex-font-style-tt">b</span>".</p>
