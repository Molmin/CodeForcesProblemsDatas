## Description

<div><p>Some days ago, WJMZBMR learned how to answer the query "how many times does a string <span class="tex-span"><i>x</i></span> occur in a string <span class="tex-span"><i>s</i></span>" quickly by preprocessing the string <span class="tex-span"><i>s</i></span>. But now he wants to make it harder.</p><p>So he wants to ask "how many consecutive substrings of <span class="tex-span"><i>s</i></span> are cyclical isomorphic to a given string <span class="tex-span"><i>x</i></span>". You are given string <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>n</i></span> strings <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, for each string <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> find, how many consecutive substrings of <span class="tex-span"><i>s</i></span> are cyclical isomorphic to <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Two strings are called <span class="tex-font-style-it">cyclical isomorphic</span> if one can rotate one string to get the other one. 'Rotate' here means 'to take some consecutive chars (maybe none) from the beginning of a string and put them back at the end of the string in the same order'. For example, string "<span class="tex-font-style-tt">abcde</span>" can be rotated to string "<span class="tex-font-style-tt">deabc</span>". We can take characters "<span class="tex-font-style-tt">abc</span>" from the beginning and put them at the end of "<span class="tex-font-style-tt">de</span>".</p></div><div class="input-specification"><p>The first line contains a non-empty string <span class="tex-span"><i>s</i></span>. The length of string <span class="tex-span"><i>s</i></span> is not greater than <span class="tex-span">10<sup class="upper-index">6</sup></span> characters.</p><p>The second line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of queries. Then <span class="tex-span"><i>n</i></span> lines follow: the <span class="tex-span"><i>i</i></span>-th line contains the string <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> — the string for the <span class="tex-span"><i>i</i></span>-th query. The total length of <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> is less than or equal to <span class="tex-span">10<sup class="upper-index">6</sup></span> characters.</p><p>In this problem, strings only consist of lowercase English letters.</p></div><div class="output-specification"><p>For each query <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> print a single integer that shows how many consecutive substrings of <span class="tex-span"><i>s</i></span> are cyclical isomorphic to <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>. Print the answers to the queries in the order they are given in the input.</p></div>

## Input

<p>The first line contains a non-empty string <span class="tex-span"><i>s</i></span>. The length of string <span class="tex-span"><i>s</i></span> is not greater than <span class="tex-span">10<sup class="upper-index">6</sup></span> characters.</p><p>The second line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of queries. Then <span class="tex-span"><i>n</i></span> lines follow: the <span class="tex-span"><i>i</i></span>-th line contains the string <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> — the string for the <span class="tex-span"><i>i</i></span>-th query. The total length of <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> is less than or equal to <span class="tex-span">10<sup class="upper-index">6</sup></span> characters.</p><p>In this problem, strings only consist of lowercase English letters.</p>

## Output

<p>For each query <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> print a single integer that shows how many consecutive substrings of <span class="tex-span"><i>s</i></span> are cyclical isomorphic to <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>. Print the answers to the queries in the order they are given in the input.</p>





```input1
baabaabaaa
5
a
ba
baa
aabaa
aaba

```




```input2
aabbaa
3
aa
aabb
abba

```




```output1
7
5
7
3
5

```




```output2
2
3
3

```


