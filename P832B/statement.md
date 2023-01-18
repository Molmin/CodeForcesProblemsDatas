## Description

<div><p>It's hard times now. Today Petya needs to score 100 points on Informatics exam. The tasks seem easy to Petya, but he thinks he lacks time to finish them all, so he asks you to help with one..</p><p>There is a glob pattern in the statements (a string consisting of lowercase English letters, characters "<span class="tex-font-style-tt">?</span>" and "<span class="tex-font-style-tt">*</span>"). It is known that character "<span class="tex-font-style-tt">*</span>" occurs <span class="tex-font-style-bf">no more than once</span> in the pattern.</p><p>Also, <span class="tex-span"><i>n</i></span> query strings are given, it is required to determine for each of them if the pattern matches it or not.</p><p>Everything seemed easy to Petya, but then he discovered that <span class="tex-font-style-bf">the special pattern characters differ from their usual meaning</span>.</p><p>A pattern matches a string if it is possible to replace each character "<span class="tex-font-style-tt">?</span>" with one <span class="tex-font-style-it">good</span> lowercase English letter, and the character "<span class="tex-font-style-tt">*</span>" (if there is one) with any, including empty, string of <span class="tex-font-style-it">bad</span> lowercase English letters, so that the resulting string is the same as the given string.</p><p>The good letters are given to Petya. All the others are bad.</p></div><div class="input-specification"><p>The first line contains a string with length from <span class="tex-span">1</span> to <span class="tex-span">26</span> consisting of distinct lowercase English letters. These letters are good letters, all the others are bad.</p><p>The second line contains the pattern&nbsp;— a string <span class="tex-span"><i>s</i></span> of lowercase English letters, characters "<span class="tex-font-style-tt">?</span>" and "<span class="tex-font-style-tt">*</span>" (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 10<sup class="upper-index">5</sup></span>). It is guaranteed that character "<span class="tex-font-style-tt">*</span>" occurs in <span class="tex-span"><i>s</i></span> no more than once.</p><p>The third line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of query strings.</p><p><span class="tex-span"><i>n</i></span> lines follow, each of them contains single non-empty string consisting of lowercase English letters&nbsp;— a query string.</p><p>It is guaranteed that the total length of all query strings is not greater than <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> lines: in the <span class="tex-span"><i>i</i></span>-th of them print "<span class="tex-font-style-tt">YES</span>" if the pattern matches the <span class="tex-span"><i>i</i></span>-th query string, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You can choose the case (lower or upper) for each letter arbitrary.</p></div>

## Input

<p>The first line contains a string with length from <span class="tex-span">1</span> to <span class="tex-span">26</span> consisting of distinct lowercase English letters. These letters are good letters, all the others are bad.</p><p>The second line contains the pattern&nbsp;— a string <span class="tex-span"><i>s</i></span> of lowercase English letters, characters "<span class="tex-font-style-tt">?</span>" and "<span class="tex-font-style-tt">*</span>" (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 10<sup class="upper-index">5</sup></span>). It is guaranteed that character "<span class="tex-font-style-tt">*</span>" occurs in <span class="tex-span"><i>s</i></span> no more than once.</p><p>The third line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of query strings.</p><p><span class="tex-span"><i>n</i></span> lines follow, each of them contains single non-empty string consisting of lowercase English letters&nbsp;— a query string.</p><p>It is guaranteed that the total length of all query strings is not greater than <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> lines: in the <span class="tex-span"><i>i</i></span>-th of them print "<span class="tex-font-style-tt">YES</span>" if the pattern matches the <span class="tex-span"><i>i</i></span>-th query string, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You can choose the case (lower or upper) for each letter arbitrary.</p>





```input1
ab
a?a
2
aaa
aab

```




```input2
abc
a?a?a*
4
abacaba
abaca
apapa
aaaaax

```




```output1
YES
NO

```




```output2
NO
YES
NO
YES

```



## Note

<p>In the first example we can replace "<span class="tex-font-style-tt">?</span>" with good letters "<span class="tex-font-style-tt">a</span>" and "<span class="tex-font-style-tt">b</span>", so we can see that the answer for the first query is "<span class="tex-font-style-tt">YES</span>", and the answer for the second query is "<span class="tex-font-style-tt">NO</span>", because we can't match the third letter.</p><p>Explanation of the second example. </p><ul> <li> The first query: "<span class="tex-font-style-tt">NO</span>", because character "<span class="tex-font-style-tt">*</span>" can be replaced with a string of bad letters only, but the only way to match the query string is to replace it with the string "<span class="tex-font-style-tt">ba</span>", in which both letters are good. </li><li> The second query: "<span class="tex-font-style-tt">YES</span>", because characters "<span class="tex-font-style-tt">?</span>" can be replaced with corresponding good letters, and character "<span class="tex-font-style-tt">*</span>" can be replaced with empty string, and the strings will coincide. </li><li> The third query: "<span class="tex-font-style-tt">NO</span>", because characters "<span class="tex-font-style-tt">?</span>" can't be replaced with bad letters. </li><li> The fourth query: "<span class="tex-font-style-tt">YES</span>", because characters "<span class="tex-font-style-tt">?</span>" can be replaced with good letters "<span class="tex-font-style-tt">a</span>", and character "<span class="tex-font-style-tt">*</span>" can be replaced with a string of bad letters "<span class="tex-font-style-tt">x</span>". </li></ul>
