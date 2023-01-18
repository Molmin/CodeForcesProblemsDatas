## Description

<div><p>Let us call a non-empty sequence of lowercase English letters a <span class="tex-font-style-underline">word</span>. <span class="tex-font-style-underline">Prefix</span> of a word <span class="tex-span"><i>x</i></span> is a word <span class="tex-span"><i>y</i></span> that can be obtained from <span class="tex-span"><i>x</i></span> by removing zero or more last letters of <span class="tex-span"><i>x</i></span>.</p><p>Let us call two words <span class="tex-font-style-underline">similar</span>, if one of them can be obtained from the other by removing its first letter.</p><p>You are given a set <span class="tex-span"><i>S</i></span> of words. Find the maximal possible size of set of non-empty words <span class="tex-span"><i>X</i></span> such that they satisfy the following: </p><ul> <li> each word of <span class="tex-span"><i>X</i></span> is prefix of some word from <span class="tex-span"><i>S</i></span>; </li><li> <span class="tex-span"><i>X</i></span> has no similar words. </li></ul></div><div class="input-specification"><p>Input data contains multiple test cases. The first line of the input data contains an integer <span class="tex-span"><i>t</i></span>&nbsp;— the number of test cases. The descriptions of test cases follow.</p><p>The first line of each description contains an integer <span class="tex-span"><i>n</i></span>&nbsp;— the number of words in the set <span class="tex-span"><i>S</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>). Each of the following <span class="tex-span"><i>n</i></span> lines contains one non-empty word&nbsp;— elements of <span class="tex-span"><i>S</i></span>. All words in <span class="tex-span"><i>S</i></span> are different.</p><p>It is guaranteed that the total length of all words in one input data doesn't exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>.</p></div><div class="output-specification"><p>For each test case print one line that contains one integer <span class="tex-span"><i>m</i></span>&nbsp;— the maximal number of words that <span class="tex-span"><i>X</i></span> can contain.</p></div>

## Input

<p>Input data contains multiple test cases. The first line of the input data contains an integer <span class="tex-span"><i>t</i></span>&nbsp;— the number of test cases. The descriptions of test cases follow.</p><p>The first line of each description contains an integer <span class="tex-span"><i>n</i></span>&nbsp;— the number of words in the set <span class="tex-span"><i>S</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>). Each of the following <span class="tex-span"><i>n</i></span> lines contains one non-empty word&nbsp;— elements of <span class="tex-span"><i>S</i></span>. All words in <span class="tex-span"><i>S</i></span> are different.</p><p>It is guaranteed that the total length of all words in one input data doesn't exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>.</p>

## Output

<p>For each test case print one line that contains one integer <span class="tex-span"><i>m</i></span>&nbsp;— the maximal number of words that <span class="tex-span"><i>X</i></span> can contain.</p>





```input1
2
3
aba
baba
aaab
2
aa
a

```




```output1
6
1

```


