## Description

<div><p>Stepan has a set of <span class="tex-span"><i>n</i></span> strings. Also, he has a favorite string <span class="tex-span"><i>s</i></span>. </p><p>Stepan wants to do the following. He will take some strings of his set and write them down one after another. It is possible that he will take some strings more than once, and will not take some of them at all.</p><p>Your task is to determine the minimum number of strings in the set which Stepan needs to take and write so that the string <span class="tex-span"><i>s</i></span> appears as a subsequence in the resulting written down string. </p><p>For example, in the string "<span class="tex-font-style-tt">abcd</span>" strings "<span class="tex-font-style-tt">ad</span>", "<span class="tex-font-style-tt">acd</span>", "<span class="tex-font-style-tt">abcd</span>" appear as subsequences, and strings "<span class="tex-font-style-tt">ba</span>", "<span class="tex-font-style-tt">abdc</span>" don't appear as subsequences. </p></div><div class="input-specification"><p>The first line contains the integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>) — the number of strings in Stepan's set.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>n</i></span> non-empty strings consisting of lowercase letters of the English alphabet. The length of each of these strings does not exceed <span class="tex-span">50</span> symbols. It is possible that some strings from Stepan's set are the same.</p><p>The next line contains the non-empty string <span class="tex-span"><i>s</i></span>, consisting of lowercase letters of the English alphabet — Stepan's favorite string. The length of this string doesn't exceed <span class="tex-span">2500</span> symbols.</p></div><div class="output-specification"><p>Print the minimum number of strings which Stepan should take from the set and write them down one after another so that the string <span class="tex-span"><i>s</i></span> appears as a subsequence in the resulting written down string. Each string from the set should be counted as many times as Stepan takes it from the set. </p><p>If the answer doesn't exsist, print <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line contains the integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>) — the number of strings in Stepan's set.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>n</i></span> non-empty strings consisting of lowercase letters of the English alphabet. The length of each of these strings does not exceed <span class="tex-span">50</span> symbols. It is possible that some strings from Stepan's set are the same.</p><p>The next line contains the non-empty string <span class="tex-span"><i>s</i></span>, consisting of lowercase letters of the English alphabet — Stepan's favorite string. The length of this string doesn't exceed <span class="tex-span">2500</span> symbols.</p>

## Output

<p>Print the minimum number of strings which Stepan should take from the set and write them down one after another so that the string <span class="tex-span"><i>s</i></span> appears as a subsequence in the resulting written down string. Each string from the set should be counted as many times as Stepan takes it from the set. </p><p>If the answer doesn't exsist, print <span class="tex-font-style-tt">-1</span>.</p>





```input1
3
a
aa
a
aaa

```




```input2
4
ab
aab
aa
bb
baaab

```




```input3
2
aaa
bbb
aaacbbb

```




```output1
2

```




```output2
3

```




```output3
-1

```



## Note

<p>In the first test, Stepan can take, for example, the third and the second strings from the set, write them down, and get exactly his favorite string.</p><p>In the second example Stepan can take, for example, the second, the third and again the second strings from the set and write them down. Then he will get a string "<span class="tex-font-style-tt">aabaaaab</span>", in which his favorite string "<span class="tex-font-style-tt">baaab</span>" is a subsequence.</p><p>In the third test Stepan can not get his favorite string, because it contains the letter "<span class="tex-font-style-tt">c</span>", which is not presented in any of the strings in the set.</p>
