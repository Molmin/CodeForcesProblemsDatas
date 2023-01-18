## Description

<div><p>Tomorrow Ann takes the hardest exam of programming where she should get an excellent mark. </p><p>On the last theoretical class the teacher introduced the notion of a <span class="tex-font-style-it">half-palindrome</span>. </p><p>String <span class="tex-span"><i>t</i></span> is a <span class="tex-font-style-it">half-palindrome</span>, if for all the odd positions <span class="tex-span"><i>i</i></span> (<img align="middle" class="tex-formula" src="file://jA2WIW2g.png" style="max-width: 100.0%;max-height: 100.0%;">) the following condition is held: <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = <i>t</i><sub class="lower-index">|<i>t</i>| - <i>i</i> + 1</sub></span>, where <span class="tex-span">|<i>t</i>|</span> is the length of string <span class="tex-span"><i>t</i></span> if positions are indexed from <span class="tex-span">1</span>. For example, strings "<span class="tex-font-style-tt">abaa</span>", "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">bb</span>", "<span class="tex-font-style-tt">abbbaa</span>" are half-palindromes and strings "<span class="tex-font-style-tt">ab</span>", "<span class="tex-font-style-tt">bba</span>" and "<span class="tex-font-style-tt">aaabaa</span>" are not.</p><p>Ann knows that on the exam she will get string <span class="tex-span"><i>s</i></span>, consisting only of letters <span class="tex-font-style-tt">a</span> and <span class="tex-font-style-tt">b</span>, and number <span class="tex-span"><i>k</i></span>. To get an excellent mark she has to find the <span class="tex-span"><i>k</i></span>-th in the lexicographical order string among all substrings of <span class="tex-span"><i>s</i></span> that are half-palyndromes. Note that each substring in this order is considered as many times as many times it occurs in <span class="tex-span"><i>s</i></span>.</p><p>The teachers guarantees that the given number <span class="tex-span"><i>k</i></span> doesn't exceed the number of substrings of the given string that are half-palindromes.</p><p>Can you cope with this problem?</p></div><div class="input-specification"><p>The first line of the input contains string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 5000</span>), consisting only of characters '<span class="tex-font-style-tt">a</span>' and '<span class="tex-font-style-tt">b</span>', where <span class="tex-span">|<i>s</i>|</span> is the length of string <span class="tex-span"><i>s</i></span>.</p><p>The second line contains a positive integer <span class="tex-span"><i>k</i></span>&nbsp;—&nbsp; the lexicographical number of the requested string among all the half-palindrome substrings of the given string <span class="tex-span"><i>s</i></span>. The strings are numbered starting from one. </p><p>It is guaranteed that number <span class="tex-span"><i>k</i></span> doesn't exceed the number of substrings of the given string that are half-palindromes.</p></div><div class="output-specification"><p>Print a substring of the given string that is the <span class="tex-span"><i>k</i></span>-th in the lexicographical order of all substrings of the given string that are half-palindromes.</p></div>

## Input

<p>The first line of the input contains string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 5000</span>), consisting only of characters '<span class="tex-font-style-tt">a</span>' and '<span class="tex-font-style-tt">b</span>', where <span class="tex-span">|<i>s</i>|</span> is the length of string <span class="tex-span"><i>s</i></span>.</p><p>The second line contains a positive integer <span class="tex-span"><i>k</i></span>&nbsp;—&nbsp; the lexicographical number of the requested string among all the half-palindrome substrings of the given string <span class="tex-span"><i>s</i></span>. The strings are numbered starting from one. </p><p>It is guaranteed that number <span class="tex-span"><i>k</i></span> doesn't exceed the number of substrings of the given string that are half-palindromes.</p>

## Output

<p>Print a substring of the given string that is the <span class="tex-span"><i>k</i></span>-th in the lexicographical order of all substrings of the given string that are half-palindromes.</p>





```input1
abbabaab
7

```




```input2
aaaaa
10

```




```input3
bbaabb
13

```




```output1
abaa

```




```output2
aaa

```




```output3
bbaabb

```



## Note

<p>By definition, string <span class="tex-span"><i>a</i> = <i>a</i><sub class="lower-index">1</sub><i>a</i><sub class="lower-index">2</sub>... <i>a</i><sub class="lower-index"><i>n</i></sub></span> is lexicographically less than string <span class="tex-span"><i>b</i> = <i>b</i><sub class="lower-index">1</sub><i>b</i><sub class="lower-index">2</sub>... <i>b</i><sub class="lower-index"><i>m</i></sub></span>, if either <span class="tex-span"><i>a</i></span> is a prefix of <span class="tex-span"><i>b</i></span> and doesn't coincide with <span class="tex-span"><i>b</i></span>, or there exists such <span class="tex-span"><i>i</i></span>, that <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> = <i>b</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub> = <i>b</i><sub class="lower-index">2</sub>, ... <i>a</i><sub class="lower-index"><i>i</i> - 1</sub> = <i>b</i><sub class="lower-index"><i>i</i> - 1</sub>, <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>In the first sample half-palindrome substrings are the following strings&nbsp;—&nbsp;<span class="tex-font-style-tt">a</span>, <span class="tex-font-style-tt">a</span>, <span class="tex-font-style-tt">a</span>, <span class="tex-font-style-tt">a</span>, <span class="tex-font-style-tt">aa</span>, <span class="tex-font-style-tt">aba</span>, <span class="tex-font-style-tt">abaa</span>, <span class="tex-font-style-tt">abba</span>, <span class="tex-font-style-tt">abbabaa</span>, <span class="tex-font-style-tt">b</span>, <span class="tex-font-style-tt">b</span>, <span class="tex-font-style-tt">b</span>, <span class="tex-font-style-tt">b</span>, <span class="tex-font-style-tt">baab</span>, <span class="tex-font-style-tt">bab</span>, <span class="tex-font-style-tt">bb</span>, <span class="tex-font-style-tt">bbab</span>, <span class="tex-font-style-tt">bbabaab</span> (the list is given in the lexicographical order). </p>
