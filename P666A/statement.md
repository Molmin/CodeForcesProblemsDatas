## Description

<div><p>First-rate specialists graduate from Berland State Institute of Peace and Friendship. You are one of the most talented students in this university. The education is not easy because you need to have fundamental knowledge in different areas, which sometimes are not related to each other. </p><p>For example, you should know linguistics very well. You learn a structure of Reberland language as foreign language. In this language words are constructed according to the following rules. First you need to choose the "root" of the word — some string which has more than <span class="tex-span">4</span> letters. Then several strings with the length <span class="tex-span">2</span> or <span class="tex-span">3</span> symbols are appended to this word. The only restriction — <span class="tex-font-style-it"> it is not allowed to append the same string twice in a row</span>. All these strings are considered to be suffixes of the word (this time we use word "suffix" to describe a morpheme but not the few last characters of the string as you may used to). </p><p>Here is one exercise that you have found in your task list. You are given the word <span class="tex-span"><i>s</i></span>. Find all distinct strings with the length <span class="tex-span">2</span> or <span class="tex-span">3</span>, which can be suffixes of this word according to the word constructing rules in Reberland language. </p><p>Two strings are considered distinct if they have different length or there is a position in which corresponding characters do not match. </p><p>Let's look at the example: the word <span class="tex-span"><i>abacabaca</i></span> is given. This word can be obtained in the following ways: <img align="middle" class="tex-formula" src="file://j7p9iWe3.png" style="max-width: 100.0%;max-height: 100.0%;">, where the root of the word is overlined, and suffixes are marked by "corners". Thus, the set of possible suffixes for this word is <span class="tex-span">{<i>aca</i>, <i>ba</i>, <i>ca</i>}</span>. </p></div><div class="input-specification"><p>The only line contains a string <span class="tex-span"><i>s</i></span> (<span class="tex-span">5 ≤ |<i>s</i>| ≤ 10<sup class="upper-index">4</sup></span>) consisting of lowercase English letters.</p></div><div class="output-specification"><p>On the first line print integer <span class="tex-span"><i>k</i></span> — a number of distinct possible suffixes. On the next <span class="tex-span"><i>k</i></span> lines print suffixes. </p><p>Print suffixes in lexicographical (alphabetical) order. </p></div>

## Input

<p>The only line contains a string <span class="tex-span"><i>s</i></span> (<span class="tex-span">5 ≤ |<i>s</i>| ≤ 10<sup class="upper-index">4</sup></span>) consisting of lowercase English letters.</p>

## Output

<p>On the first line print integer <span class="tex-span"><i>k</i></span> — a number of distinct possible suffixes. On the next <span class="tex-span"><i>k</i></span> lines print suffixes. </p><p>Print suffixes in lexicographical (alphabetical) order. </p>





```input1
abacabaca

```




```input2
abaca

```




```output1
3
aca
ba
ca

```




```output2
0

```



## Note

<p>The first test was analysed in the problem statement. </p><p>In the second example the length of the string equals <span class="tex-span">5</span>. The length of the root equals 5, so no string can be used as a suffix.</p>
