## Description

<div><p>Polycarpus analyzes a string called <span class="tex-font-style-it">abracadabra</span>. This string is constructed using the following algorithm: </p><ul> <li> On the first step the string consists of a single character "<span class="tex-font-style-tt">a</span>". </li><li> On the <span class="tex-span"><i>k</i></span>-th step Polycarpus concatenates two copies of the string obtained on the <span class="tex-span">(<i>k</i> - 1)</span>-th step, while inserting the <span class="tex-span"><i>k</i></span>-th character of the alphabet between them. Polycarpus uses the alphabet that consists of lowercase Latin letters and digits (a total of 36 characters). The alphabet characters are numbered like this: the 1-st character is "<span class="tex-font-style-tt">a</span>", the 2-nd — "<span class="tex-font-style-tt">b</span>", ..., the 26-th — "<span class="tex-font-style-tt">z</span>", the 27-th — "<span class="tex-font-style-tt">0</span>", the 28-th — "<span class="tex-font-style-tt">1</span>", ..., the 36-th — "<span class="tex-font-style-tt">9</span>". </li></ul><p>Let's have a closer look at the algorithm. On the second step Polycarpus will concatenate two strings "<span class="tex-font-style-tt">a</span>" and insert the character "<span class="tex-font-style-tt">b</span>" between them, resulting in "<span class="tex-font-style-tt">aba</span>" string. The third step will transform it into "<span class="tex-font-style-tt">abacaba</span>", and the fourth one - into "<span class="tex-font-style-tt">abacabadabacaba</span>". Thus, the string constructed on the <span class="tex-span"><i>k</i></span>-th step will consist of <span class="tex-span">2<sup class="upper-index"><i>k</i></sup> - 1</span> characters. </p><p>Polycarpus wrote down the string he got after 30 steps of the given algorithm and chose two non-empty substrings of it. Your task is to find the length of the longest common substring of the two substrings selected by Polycarpus.</p><p>A substring <span class="tex-span"><i>s</i>[<i>i</i>... <i>j</i>]</span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>j</i> ≤ |<i>s</i>|</span>) of string <span class="tex-span"><i>s</i></span> = <span class="tex-span"><i>s</i><sub class="lower-index">1</sub><i>s</i><sub class="lower-index">2</sub>... <i>s</i><sub class="lower-index">|<i>s</i>|</sub></span> is a string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub><i>s</i><sub class="lower-index"><i>i</i> + 1</sub>... <i>s</i><sub class="lower-index"><i>j</i></sub></span>. For example, substring <span class="tex-span"><i>s</i>[2...4]</span> of string <span class="tex-span"><i>s</i></span> = "<span class="tex-font-style-tt">abacaba</span>" equals "<span class="tex-font-style-tt">bac</span>". The string is its own substring.</p><p>The longest common substring of two strings <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> is the longest string that is a substring of both <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span>. For example, the longest common substring of "<span class="tex-font-style-tt">contest</span>" and "<span class="tex-font-style-tt">systemtesting</span>" is string "<span class="tex-font-style-tt">test</span>". There can be several common substrings of maximum length.</p></div><div class="input-specification"><p>The input consists of a single line containing four integers <span class="tex-span"><i>l</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>l</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span"><i>i</i> = 1, 2</span>). The numbers are separated by single spaces. <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> give the indices of the first and the last characters of the <span class="tex-span"><i>i</i></span>-th chosen substring, correspondingly (<span class="tex-span"><i>i</i> = 1, 2</span>). The characters of string <span class="tex-font-style-it">abracadabra</span> are numbered starting from <span class="tex-span">1</span>.</p></div><div class="output-specification"><p>Print a single number — the length of the longest common substring of the given strings. If there are no common substrings, print 0.</p></div>

## Input

<p>The input consists of a single line containing four integers <span class="tex-span"><i>l</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>l</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span"><i>i</i> = 1, 2</span>). The numbers are separated by single spaces. <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> give the indices of the first and the last characters of the <span class="tex-span"><i>i</i></span>-th chosen substring, correspondingly (<span class="tex-span"><i>i</i> = 1, 2</span>). The characters of string <span class="tex-font-style-it">abracadabra</span> are numbered starting from <span class="tex-span">1</span>.</p>

## Output

<p>Print a single number — the length of the longest common substring of the given strings. If there are no common substrings, print 0.</p>





```input1
3 6 1 4

```




```input2
1 1 4 4

```




```output1
2

```




```output2
0

```



## Note

<p>In the first sample the first substring is "<span class="tex-font-style-tt">acab</span>", the second one is "<span class="tex-font-style-tt">abac</span>". These two substrings have two longest common substrings "<span class="tex-font-style-tt">ac</span>" and "<span class="tex-font-style-tt">ab</span>", but we are only interested in their length — 2.</p><p>In the second sample the first substring is "<span class="tex-font-style-tt">a</span>", the second one is "<span class="tex-font-style-tt">c</span>". These two substrings don't have any common characters, so the length of their longest common substring is 0.</p>
