## Description

<div><p><span class="tex-font-style-underline">Petya loves lucky numbers very much. Everybody knows that lucky numbers are positive integers whose decimal record contains only the lucky digits <span class="tex-font-style-bf">4</span> and <span class="tex-font-style-bf">7</span>. For example, numbers <span class="tex-font-style-bf">47</span>, <span class="tex-font-style-bf">744</span>, <span class="tex-font-style-bf">4</span> are lucky and <span class="tex-font-style-bf">5</span>, <span class="tex-font-style-bf">17</span>, <span class="tex-font-style-bf">467</span> are not.</span></p><p>Petya brought home string <span class="tex-span"><i>s</i></span> with the length of <span class="tex-span"><i>n</i></span>. The string only consists of lucky digits. The digits are numbered from the left to the right starting with <span class="tex-span">1</span>. Now Petya should execute <span class="tex-span"><i>m</i></span> queries of the following form:</p><ul> <li> <span class="tex-font-style-underline">switch <span class="tex-span"><i>l</i></span> <span class="tex-span"><i>r</i></span></span> — "switch" digits (i.e. replace them with their opposites) at all positions with indexes from <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span>, inclusive: each digit <span class="tex-span">4</span> is replaced with <span class="tex-span">7</span> and each digit <span class="tex-span">7</span> is replaced with <span class="tex-span">4</span> <span class="tex-span">(1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i>)</span>; </li><li> <span class="tex-font-style-underline">count</span> — find and print on the screen the length of the longest non-decreasing subsequence of string <span class="tex-span"><i>s</i></span>. </li></ul><p>Subsequence of a string <span class="tex-span"><i>s</i></span> is a string that can be obtained from <span class="tex-span"><i>s</i></span> by removing zero or more of its elements. A string is called non-decreasing if each successive digit is not less than the previous one.</p><p>Help Petya process the requests.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>, 1 ≤ <i>m</i> ≤ 3·10<sup class="upper-index">5</sup></span>) — the length of the string <span class="tex-span"><i>s</i></span> and the number of queries correspondingly. The second line contains <span class="tex-span"><i>n</i></span> lucky digits without spaces — Petya's initial string. Next <span class="tex-span"><i>m</i></span> lines contain queries in the form described in the statement.</p></div><div class="output-specification"><p>For each query <span class="tex-font-style-underline">count</span> print an answer on a single line.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>, 1 ≤ <i>m</i> ≤ 3·10<sup class="upper-index">5</sup></span>) — the length of the string <span class="tex-span"><i>s</i></span> and the number of queries correspondingly. The second line contains <span class="tex-span"><i>n</i></span> lucky digits without spaces — Petya's initial string. Next <span class="tex-span"><i>m</i></span> lines contain queries in the form described in the statement.</p>

## Output

<p>For each query <span class="tex-font-style-underline">count</span> print an answer on a single line.</p>





```input1
2 3
47
count
switch 1 2
count

```




```input2
3 5
747
count
switch 1 1
count
switch 1 3
count

```




```output1
2
1

```




```output2
2
3
2

```



## Note

<p>In the first sample the chronology of string <span class="tex-span"><i>s</i></span> after some operations are fulfilled is as follows (the sought maximum subsequence is marked with <span class="tex-font-style-bf">bold</span>): </p><ol> <li> <span class="tex-font-style-bf">47</span> </li><li> 74 </li><li> <span class="tex-font-style-bf">7</span>4 </li></ol> In the second sample: <ol> <li> 7<span class="tex-font-style-bf">47</span> </li><li> 447 </li><li> <span class="tex-font-style-bf">447</span> </li><li> 774 </li><li> <span class="tex-font-style-bf">77</span>4 </li></ol>
