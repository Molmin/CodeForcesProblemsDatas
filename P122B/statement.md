## Description

<div><p><span class="tex-font-style-underline">Petya loves lucky numbers. Everybody knows that lucky numbers are positive integers whose decimal representation contains only the lucky digits <span class="tex-font-style-bf">4</span> and <span class="tex-font-style-bf">7</span>. For example, numbers <span class="tex-font-style-bf">47</span>, <span class="tex-font-style-bf">744</span>, <span class="tex-font-style-bf">4</span> are lucky and <span class="tex-font-style-bf">5</span>, <span class="tex-font-style-bf">17</span>, <span class="tex-font-style-bf">467</span> are not.</span></p><p>One day Petya was delivered a string <span class="tex-span"><i>s</i></span>, containing only digits. He needs to find a string that</p><ul><li> represents a lucky number without leading zeroes,</li><li> is not empty,</li><li> is contained in <span class="tex-span"><i>s</i></span> as a substring the maximum number of times.</li></ul><p>Among all the strings for which the three conditions given above are fulfilled, Petya only needs the lexicographically minimum one. Find this string for Petya.</p></div><div class="input-specification"><p>The single line contains a non-empty string <span class="tex-span"><i>s</i></span> whose length can range from <span class="tex-span">1</span> to <span class="tex-span">50</span>, inclusive. The string only contains digits. The string can contain leading zeroes.</p></div><div class="output-specification"><p>In the only line print the answer to Petya's problem. If the sought string does not exist, print "-1" (without quotes).</p></div>

## Input

<p>The single line contains a non-empty string <span class="tex-span"><i>s</i></span> whose length can range from <span class="tex-span">1</span> to <span class="tex-span">50</span>, inclusive. The string only contains digits. The string can contain leading zeroes.</p>

## Output

<p>In the only line print the answer to Petya's problem. If the sought string does not exist, print "-1" (without quotes).</p>





```input1
047

```




```input2
16

```




```input3
472747

```




```output1
4

```




```output2
-1

```




```output3
7

```



## Note

<p>The lexicographical comparison of strings is performed by the &lt; operator in the modern programming languages. String <span class="tex-span"><i>x</i></span> is lexicographically less than string <span class="tex-span"><i>y</i></span> either if <span class="tex-span"><i>x</i></span> is a prefix of <span class="tex-span"><i>y</i></span>, or exists such <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>min</i>(|<i>x</i>|, |<i>y</i>|)</span>), that <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> &lt; <i>y</i><sub class="lower-index"><i>i</i></sub></span> and for any <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>j</i> &lt; <i>i</i></span>) <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub> = <i>y</i><sub class="lower-index"><i>j</i></sub></span>. Here <span class="tex-span">|<i>a</i>|</span> denotes the length of string <span class="tex-span"><i>a</i></span>.</p><p>In the first sample three conditions are fulfilled for strings "<span class="tex-font-style-tt">4</span>", "<span class="tex-font-style-tt">7</span>" and "<span class="tex-font-style-tt">47</span>". The lexicographically minimum one is "<span class="tex-font-style-tt">4</span>".</p><p>In the second sample <span class="tex-span"><i>s</i></span> has no substrings which are lucky numbers.</p><p>In the third sample the three conditions are only fulfilled for string "<span class="tex-font-style-tt">7</span>".</p>
