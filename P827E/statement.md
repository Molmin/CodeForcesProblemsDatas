## Description

<div><p>Grigory loves strings. Recently he found a metal strip on a loft. The strip had length <span class="tex-span"><i>n</i></span> and consisted of letters "<span class="tex-font-style-tt">V</span>" and "<span class="tex-font-style-tt">K</span>". Unfortunately, rust has eaten some of the letters so that it's now impossible to understand which letter was written.</p><p>Grigory couldn't understand for a long time what these letters remind him of, so he became interested in the following question: if we put a letter "<span class="tex-font-style-tt">V</span>" or "<span class="tex-font-style-tt">K</span>" on each unreadable position, which values can the period of the resulting string be equal to?</p><p>A period of a string is such an integer <span class="tex-span"><i>d</i></span> from <span class="tex-span">1</span> to the length of the string that if we put the string shifted by <span class="tex-span"><i>d</i></span> positions to the right on itself, then all overlapping letters coincide. For example, <span class="tex-span">3</span> and <span class="tex-span">5</span> are periods of "<span class="tex-font-style-tt">VKKVK</span>".</p></div><div class="input-specification"><p>There are several (at least one) test cases in the input. The first line contains single integer&nbsp;— the number of test cases.</p><p>There is an empty line before each test case. Each test case is described in two lines: the first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>)&nbsp;— the length of the string, the second line contains the string of length <span class="tex-span"><i>n</i></span>, consisting of letters "<span class="tex-font-style-tt">V</span>", "<span class="tex-font-style-tt">K</span>" and characters "<span class="tex-font-style-tt">?</span>". The latter means the letter on its position is unreadable.</p><p>It is guaranteed that the sum of lengths among all test cases doesn't exceed <span class="tex-span">5·10<sup class="upper-index">5</sup></span>.</p><p><span class="tex-font-style-bf">For hacks</span> you can only use tests with one test case.</p></div><div class="output-specification"><p>For each test case print two lines. In the first line print the number of possible periods after we replace each unreadable letter with "<span class="tex-font-style-tt">V</span>" or "<span class="tex-font-style-tt">K</span>". In the next line print all these values in increasing order.</p></div>

## Input

<p>There are several (at least one) test cases in the input. The first line contains single integer&nbsp;— the number of test cases.</p><p>There is an empty line before each test case. Each test case is described in two lines: the first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>)&nbsp;— the length of the string, the second line contains the string of length <span class="tex-span"><i>n</i></span>, consisting of letters "<span class="tex-font-style-tt">V</span>", "<span class="tex-font-style-tt">K</span>" and characters "<span class="tex-font-style-tt">?</span>". The latter means the letter on its position is unreadable.</p><p>It is guaranteed that the sum of lengths among all test cases doesn't exceed <span class="tex-span">5·10<sup class="upper-index">5</sup></span>.</p><p><span class="tex-font-style-bf">For hacks</span> you can only use tests with one test case.</p>

## Output

<p>For each test case print two lines. In the first line print the number of possible periods after we replace each unreadable letter with "<span class="tex-font-style-tt">V</span>" or "<span class="tex-font-style-tt">K</span>". In the next line print all these values in increasing order.</p>





```input1
3
&nbsp;
5
V??VK
&nbsp;
6
??????
&nbsp;
4
?VK?

```




```output1
2
3 5
6
1 2 3 4 5 6
3
2 3 4

```



## Note

<p>In the first test case from example we can obtain, for example, "<span class="tex-font-style-tt">VKKVK</span>", which has periods <span class="tex-span">3</span> and <span class="tex-span">5</span>.</p><p>In the second test case we can obtain "<span class="tex-font-style-tt">VVVVVV</span>" which has all periods from <span class="tex-span">1</span> to <span class="tex-span">6</span>.</p><p>In the third test case string "<span class="tex-font-style-tt">KVKV</span>" has periods <span class="tex-span">2</span> and <span class="tex-span">4</span>, and string "<span class="tex-font-style-tt">KVKK</span>" has periods <span class="tex-span">3</span> and <span class="tex-span">4</span>.</p>
