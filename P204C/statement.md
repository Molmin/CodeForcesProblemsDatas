## Description

<div><p>Little Elephant loves Furik and Rubik, who he met in a small city Kremenchug.</p><p>The Little Elephant has two strings of equal length <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>, consisting only of uppercase English letters. The Little Elephant selects a pair of substrings of equal length — the first one from string <span class="tex-span"><i>a</i></span>, the second one from string <span class="tex-span"><i>b</i></span>. The choice is equiprobable among all possible pairs. Let's denote the substring of <span class="tex-span"><i>a</i></span> as <span class="tex-span"><i>x</i></span>, and the substring of <span class="tex-span"><i>b</i></span> — as <span class="tex-span"><i>y</i></span>. The Little Elephant gives string <span class="tex-span"><i>x</i></span> to Furik and string <span class="tex-span"><i>y</i></span> — to Rubik.</p><p>Let's assume that <span class="tex-span"><i>f</i>(<i>x</i>, <i>y</i>)</span> is the number of such positions of <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ |<i>x</i>|</span>), that <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> = <i>y</i><sub class="lower-index"><i>i</i></sub></span> (where <span class="tex-span">|<i>x</i>|</span> is the length of lines <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>, and <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> are the <span class="tex-span"><i>i</i></span>-th characters of strings <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>, correspondingly). Help Furik and Rubik find the expected value of <span class="tex-span"><i>f</i>(<i>x</i>, <i>y</i>)</span>.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the length of strings <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>. The second line contains string <span class="tex-span"><i>a</i></span>, the third line contains string <span class="tex-span"><i>b</i></span>. The strings consist of uppercase English letters only. The length of both strings equals <span class="tex-span"><i>n</i></span>.</p></div><div class="output-specification"><p>On a single line print a real number — the answer to the problem. The answer will be considered correct if its relative or absolute error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the length of strings <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>. The second line contains string <span class="tex-span"><i>a</i></span>, the third line contains string <span class="tex-span"><i>b</i></span>. The strings consist of uppercase English letters only. The length of both strings equals <span class="tex-span"><i>n</i></span>.</p>

## Output

<p>On a single line print a real number — the answer to the problem. The answer will be considered correct if its relative or absolute error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
2
AB
BA

```




```input2
3
AAB
CAA

```




```output1
0.400000000

```




```output2
0.642857143

```



## Note

<p>Let's assume that we are given string <span class="tex-span"><i>a</i> = <i>a</i><sub class="lower-index">1</sub><i>a</i><sub class="lower-index">2</sub>... <i>a</i><sub class="lower-index">|<i>a</i>|</sub></span>, then let's denote the string's length as <span class="tex-span">|<i>a</i>|</span>, and its <span class="tex-span"><i>i</i></span>-th character — as <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>A substring <span class="tex-span"><i>a</i>[<i>l</i>... <i>r</i>]</span> <span class="tex-span">(1 ≤ <i>l</i> ≤ <i>r</i> ≤ |<i>a</i>|)</span> of string <span class="tex-span"><i>a</i></span> is string <span class="tex-span"><i>a</i><sub class="lower-index"><i>l</i></sub><i>a</i><sub class="lower-index"><i>l</i> + 1</sub>... <i>a</i><sub class="lower-index"><i>r</i></sub></span>.</p><p>String <span class="tex-span"><i>a</i></span> is a substring of string <span class="tex-span"><i>b</i></span>, if there exists such pair of integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> <span class="tex-span">(1 ≤ <i>l</i> ≤ <i>r</i> ≤ |<i>b</i>|)</span>, that <span class="tex-span"><i>b</i>[<i>l</i>... <i>r</i>] = <i>a</i></span>.</p><p>Let's consider the first test sample. The first sample has <span class="tex-span">5</span> possible substring pairs: <span class="tex-font-style-tt">("A", "B"), ("A", "A"), ("B", "B"), ("B", "A"), ("AB", "BA")</span>. For the second and third pair value <span class="tex-span"><i>f</i>(<i>x</i>, <i>y</i>)</span> equals <span class="tex-span">1</span>, for the rest it equals <span class="tex-span">0</span>. The probability of choosing each pair equals <img align="middle" class="tex-formula" src="file://vabJtAuu.png" style="max-width: 100.0%;max-height: 100.0%;">, that's why the answer is <img align="middle" class="tex-formula" src="file://zvsijEZ5.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-span">·</span> <span class="tex-span">0</span> <span class="tex-span"> + </span> <img align="middle" class="tex-formula" src="file://b7JbW38t.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-span">·</span> <span class="tex-span">1</span> <span class="tex-span"> + </span> <img align="middle" class="tex-formula" src="file://9j4c5Loz.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-span">·</span> <span class="tex-span">1</span> <span class="tex-span"> + </span> <img align="middle" class="tex-formula" src="file://t4syh2FE.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-span">·</span> <span class="tex-span">0</span> <span class="tex-span"> + </span> <img align="middle" class="tex-formula" src="file://iT4L1Bxe.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-span">·</span> <span class="tex-span">0</span> <span class="tex-span"> = </span> <img align="middle" class="tex-formula" src="file://UZ7shCaE.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-span"> = </span> <span class="tex-span">0.4</span>.</p>
