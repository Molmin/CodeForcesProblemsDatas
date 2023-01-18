## Description

<div><p>You have a string <span class="tex-span"><i>s</i> = <i>s</i><sub class="lower-index">1</sub><i>s</i><sub class="lower-index">2</sub>...<i>s</i><sub class="lower-index">|<i>s</i>|</sub></span>, where <span class="tex-span">|<i>s</i>|</span> is the length of string <span class="tex-span"><i>s</i></span>, and <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> its <span class="tex-span"><i>i</i></span>-th character. </p><p>Let's introduce several definitions:</p><ul> <li> A substring <span class="tex-span"><i>s</i>[<i>i</i>..<i>j</i>]</span> <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>j</i> ≤ |<i>s</i>|)</span> of string <span class="tex-span"><i>s</i></span> is string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub><i>s</i><sub class="lower-index"><i>i</i> + 1</sub>...<i>s</i><sub class="lower-index"><i>j</i></sub></span>. </li><li> The prefix of string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>l</i></span> <span class="tex-span">(1 ≤ <i>l</i> ≤ |<i>s</i>|)</span> is string <span class="tex-span"><i>s</i>[1..<i>l</i>]</span>. </li><li> The suffix of string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>l</i></span> <span class="tex-span">(1 ≤ <i>l</i> ≤ |<i>s</i>|)</span> is string <span class="tex-span"><i>s</i>[|<i>s</i>| - <i>l</i> + 1..|<i>s</i>|]</span>. </li></ul><p>Your task is, for any prefix of string <span class="tex-span"><i>s</i></span> which matches a suffix of string <span class="tex-span"><i>s</i></span>, print the number of times it occurs in string <span class="tex-span"><i>s</i></span> as a substring.</p></div><div class="input-specification"><p>The single line contains a sequence of characters <span class="tex-span"><i>s</i><sub class="lower-index">1</sub><i>s</i><sub class="lower-index">2</sub>...<i>s</i><sub class="lower-index">|<i>s</i>|</sub></span> <span class="tex-span">(1 ≤ |<i>s</i>| ≤ 10<sup class="upper-index">5</sup>)</span> — string <span class="tex-span"><i>s</i></span>. The string only consists of uppercase English letters.</p></div><div class="output-specification"><p>In the first line, print integer <span class="tex-span"><i>k</i></span> <span class="tex-span">(0 ≤ <i>k</i> ≤ |<i>s</i>|)</span> — the number of prefixes that match a suffix of string <span class="tex-span"><i>s</i></span>. Next print <span class="tex-span"><i>k</i></span> lines, in each line print two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>. Numbers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> mean that the prefix of the length <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> matches the suffix of length <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and occurs in string <span class="tex-span"><i>s</i></span> as a substring <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> times. Print pairs <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-font-style-bf">in the order of increasing</span> <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>.</p></div>

## Input

<p>The single line contains a sequence of characters <span class="tex-span"><i>s</i><sub class="lower-index">1</sub><i>s</i><sub class="lower-index">2</sub>...<i>s</i><sub class="lower-index">|<i>s</i>|</sub></span> <span class="tex-span">(1 ≤ |<i>s</i>| ≤ 10<sup class="upper-index">5</sup>)</span> — string <span class="tex-span"><i>s</i></span>. The string only consists of uppercase English letters.</p>

## Output

<p>In the first line, print integer <span class="tex-span"><i>k</i></span> <span class="tex-span">(0 ≤ <i>k</i> ≤ |<i>s</i>|)</span> — the number of prefixes that match a suffix of string <span class="tex-span"><i>s</i></span>. Next print <span class="tex-span"><i>k</i></span> lines, in each line print two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>. Numbers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> mean that the prefix of the length <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> matches the suffix of length <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and occurs in string <span class="tex-span"><i>s</i></span> as a substring <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> times. Print pairs <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-font-style-bf">in the order of increasing</span> <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>.</p>





```input1
ABACABA

```




```input2
AAA

```




```output1
3
1 4
3 2
7 1

```




```output2
3
1 3
2 2
3 1

```


