## Description

<div><p>You are given an <span class="tex-span"><i>n</i> × <i>m</i></span> rectangular table consisting of lower case English letters. In one operation you can completely remove one column from the table. The remaining parts are combined forming a new table. For example, after removing the second column from the table</p><pre class="verbatim"><br>abcd<br>edfg<br>hijk<br></pre><p>&nbsp;</p><p>we obtain the table:</p><pre class="verbatim"><br>acd<br>efg<br>hjk<br></pre><p>&nbsp;</p><p>A table is called <span class="tex-font-style-underline">good</span> if its rows are ordered from top to bottom lexicographically, i.e. each row is lexicographically no larger than the following one. Determine the minimum number of operations of removing a column needed to make a given table good.</p></div><div class="input-specification"><p>The first line contains two integers &nbsp;— <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ </span><span class="tex-font-style-bf">100</span>).</p><p>Next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> small English letters each&nbsp;— the characters of the table.</p></div><div class="output-specification"><p>Print a single number&nbsp;— the minimum number of columns that you need to remove in order to make the table good.</p></div>

## Input

<p>The first line contains two integers &nbsp;— <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ </span><span class="tex-font-style-bf">100</span>).</p><p>Next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> small English letters each&nbsp;— the characters of the table.</p>

## Output

<p>Print a single number&nbsp;— the minimum number of columns that you need to remove in order to make the table good.</p>





```input1
1 10
codeforces

```




```input2
4 4
case
care
test
code

```




```input3
5 4
code
forc
esco
defo
rces

```




```output1
0

```




```output2
2

```




```output3
4

```



## Note

<p>In the first sample the table is already good.</p><p>In the second sample you may remove the first and third column.</p><p>In the third sample you have to remove all the columns (note that the table where all rows are empty is considered good by definition).</p><p>Let strings <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> have equal length. Then, <span class="tex-span"><i>s</i></span> is <span class="tex-font-style-underline">lexicographically larger</span> than <span class="tex-span"><i>t</i></span> if they are not equal and the character following the largest common prefix of <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> (the prefix may be empty) in <span class="tex-span"><i>s</i></span> is alphabetically larger than the corresponding character of <span class="tex-span"><i>t</i></span>.</p>
