## Description

<div><p><span class="tex-font-style-underline">Petya loves lucky numbers very much. Everybody knows that lucky numbers are positive integers whose decimal record contains only the lucky digits <span class="tex-font-style-bf">4</span> and <span class="tex-font-style-bf">7</span>. For example, numbers <span class="tex-font-style-bf">47</span>, <span class="tex-font-style-bf">744</span>, <span class="tex-font-style-bf">4</span> are lucky and <span class="tex-font-style-bf">5</span>, <span class="tex-font-style-bf">17</span>, <span class="tex-font-style-bf">467</span> are not.</span></p><p>Petya loves tickets very much. As we know, each ticket has a number that is a positive integer. Its length equals <span class="tex-span"><i>n</i></span> (<span class="tex-span"><i>n</i></span> is always even). Petya calls a ticket lucky if the ticket's number is a lucky number and the sum of digits in the first half (the sum of the first <span class="tex-span"><i>n</i> / 2</span> digits) equals the sum of digits in the second half (the sum of the last <span class="tex-span"><i>n</i> / 2</span> digits). Check if the given ticket is lucky.</p></div><div class="input-specification"><p>The first line contains an even integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 50)</span> — the length of the ticket number that needs to be checked. The second line contains an integer whose length equals exactly <span class="tex-span"><i>n</i></span> — the ticket number. The number may contain leading zeros.</p></div><div class="output-specification"><p>On the first line print "<span class="tex-font-style-tt">YES</span>" if the given ticket number is lucky. Otherwise, print "<span class="tex-font-style-tt">NO</span>" (without the quotes).</p></div>

## Input

<p>The first line contains an even integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 50)</span> — the length of the ticket number that needs to be checked. The second line contains an integer whose length equals exactly <span class="tex-span"><i>n</i></span> — the ticket number. The number may contain leading zeros.</p>

## Output

<p>On the first line print "<span class="tex-font-style-tt">YES</span>" if the given ticket number is lucky. Otherwise, print "<span class="tex-font-style-tt">NO</span>" (without the quotes).</p>





```input1
2
47

```




```input2
4
4738

```




```input3
4
4774

```




```output1
NO

```




```output2
NO

```




```output3
YES

```



## Note

<p>In the first sample the sum of digits in the first half does not equal the sum of digits in the second half (<span class="tex-span">4 ≠ 7</span>).</p><p>In the second sample the ticket number is not the lucky number.</p>
