## Description

<div><p>Given a string <span class="tex-span"><i>s</i></span>, process <span class="tex-span"><i>q</i></span> queries, each having one of the following forms:</p><ul> <li> <span class="tex-span">1 <i>i</i> <i>c</i></span> — Change the <span class="tex-span"><i>i</i></span>-th character in the string to <span class="tex-span"><i>c</i></span>. </li><li> <span class="tex-span">2 <i>l</i> <i>r</i> <i>y</i></span> — Consider the substring of <span class="tex-span"><i>s</i></span> starting at position <span class="tex-span"><i>l</i></span> and ending at position <span class="tex-span"><i>r</i></span>. Output the number of times <span class="tex-span"><i>y</i></span> occurs as a substring in it. </li></ul></div><div class="input-specification"><p>The first line of the input contains the string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 10<sup class="upper-index">5</sup></span>) of lowercase English letters.</p><p>The second line contains an integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>) &nbsp;— the number of queries to process.</p><p>The next <span class="tex-span"><i>q</i></span> lines describe the queries and may have one of the following forms:</p><ul> <li> <span class="tex-span">1 <i>i</i> <i>c</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ |<i>s</i>|</span>) </li><li> <span class="tex-span">2 <i>l</i> <i>r</i> <i>y</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ |<i>s</i>|</span>) </li></ul><p><span class="tex-span"><i>c</i></span> is a lowercase English letter and <span class="tex-span"><i>y</i></span> is a non-empty string consisting of only lowercase English letters.</p><p>The sum of <span class="tex-span">|<i>y</i>|</span> over all queries of second type is at most <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p><p>It is guaranteed that there is at least one query of second type.</p><p>All strings are <span class="tex-span">1</span>-indexed.</p><p><span class="tex-span">|<i>s</i>|</span> is the length of the string <span class="tex-span"><i>s</i></span>.</p></div><div class="output-specification"><p>For each query of type <span class="tex-span">2</span>, output the required answer in a separate line.</p></div>

## Input

<p>The first line of the input contains the string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 10<sup class="upper-index">5</sup></span>) of lowercase English letters.</p><p>The second line contains an integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>) &nbsp;— the number of queries to process.</p><p>The next <span class="tex-span"><i>q</i></span> lines describe the queries and may have one of the following forms:</p><ul> <li> <span class="tex-span">1 <i>i</i> <i>c</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ |<i>s</i>|</span>) </li><li> <span class="tex-span">2 <i>l</i> <i>r</i> <i>y</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ |<i>s</i>|</span>) </li></ul><p><span class="tex-span"><i>c</i></span> is a lowercase English letter and <span class="tex-span"><i>y</i></span> is a non-empty string consisting of only lowercase English letters.</p><p>The sum of <span class="tex-span">|<i>y</i>|</span> over all queries of second type is at most <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p><p>It is guaranteed that there is at least one query of second type.</p><p>All strings are <span class="tex-span">1</span>-indexed.</p><p><span class="tex-span">|<i>s</i>|</span> is the length of the string <span class="tex-span"><i>s</i></span>.</p>

## Output

<p>For each query of type <span class="tex-span">2</span>, output the required answer in a separate line.</p>





```input1
ababababa
3
2 1 7 aba
1 5 c
2 1 7 aba

```




```input2
abcdcbc
5
2 1 7 bc
1 4 b
2 4 7 bc
1 2 a
2 1 4 aa

```




```output1
3
1

```




```output2
2
2
1

```



## Note

<p>Consider the first sample case. Initially, the string <span class="tex-font-style-tt">aba</span> occurs <span class="tex-span">3</span> times in the range <span class="tex-span">[1, 7]</span>. Note that two occurrences may overlap. </p><p>After the update, the string becomes <span class="tex-font-style-tt">ababcbaba</span> and now <span class="tex-font-style-tt">aba</span> occurs only once in the range <span class="tex-span">[1, 7]</span>.</p>
