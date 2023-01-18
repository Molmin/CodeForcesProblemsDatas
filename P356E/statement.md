## Description

<div><p>Xenia the coder went to The Olympiad of Informatics and got a string problem. Unfortunately, Xenia isn't fabulous in string algorithms. Help her solve the problem.</p><p><span class="tex-font-style-it">String</span> <span class="tex-span"><i>s</i></span> is a sequence of characters <span class="tex-span"><i>s</i><sub class="lower-index">1</sub><i>s</i><sub class="lower-index">2</sub>... <i>s</i><sub class="lower-index">|<i>s</i>|</sub></span>, where record <span class="tex-span">|<i>s</i>|</span> shows the length of the string. </p><p><span class="tex-font-style-it">Substring</span> <span class="tex-span"><i>s</i>[<i>i</i>... <i>j</i>]</span> of string <span class="tex-span"><i>s</i></span> is string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub><i>s</i><sub class="lower-index"><i>i</i> + 1</sub>... <i>s</i><sub class="lower-index"><i>j</i></sub></span>.</p><p>String <span class="tex-span"><i>s</i></span> is a <span class="tex-font-style-it">Gray</span> string, if it meets the conditions:</p><ul> <li> the length of string <span class="tex-span">|<i>s</i>|</span> is odd; </li><li> character <img align="middle" class="tex-formula" src="file://R6ooAWAI.png" style="max-width: 100.0%;max-height: 100.0%;"> occurs exactly once in the string; </li><li> either <span class="tex-span">|<i>s</i>| = 1</span>, or substrings <img align="middle" class="tex-formula" src="file://a8MMfEQP.png" style="max-width: 100.0%;max-height: 100.0%;"> and <img align="middle" class="tex-formula" src="file://6HmB62JG.png" style="max-width: 100.0%;max-height: 100.0%;"> are the same and are Gray strings. </li></ul><p>For example, strings "<span class="tex-font-style-tt">abacaba</span>", "<span class="tex-font-style-tt">xzx</span>", "<span class="tex-font-style-tt">g</span>" are Gray strings and strings "<span class="tex-font-style-tt">aaa</span>", "<span class="tex-font-style-tt">xz</span>", "<span class="tex-font-style-tt">abaxcbc</span>" are not.</p><p>The <span class="tex-font-style-it">beauty</span> of string <span class="tex-span"><i>p</i></span> is the sum of the squares of the lengths of all substrings of string <span class="tex-span"><i>p</i></span> that are Gray strings. In other words, consider all pairs of values <span class="tex-span"><i>i</i>, <i>j</i></span> <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>j</i> ≤ |<i>p</i>|)</span>. If substring <span class="tex-span"><i>p</i>[<i>i</i>... <i>j</i>]</span> is a Gray string, you should add <span class="tex-span">(<i>j</i> - <i>i</i> + 1)<sup class="upper-index">2</sup></span> to the beauty.</p><p>Xenia has got string <span class="tex-span"><i>t</i></span> consisting of lowercase English letters. She is allowed to replace at most one letter of the string by any other English letter. The task is to get a string of maximum beauty.</p></div><div class="input-specification"><p>The first line contains a non-empty string <span class="tex-span"><i>t</i></span> <span class="tex-span">(1 ≤ |<i>t</i>| ≤ 10<sup class="upper-index">5</sup>)</span>. String <span class="tex-span"><i>t</i></span> only consists of lowercase English letters.</p></div><div class="output-specification"><p>Print the sought maximum beauty value Xenia can get.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains a non-empty string <span class="tex-span"><i>t</i></span> <span class="tex-span">(1 ≤ |<i>t</i>| ≤ 10<sup class="upper-index">5</sup>)</span>. String <span class="tex-span"><i>t</i></span> only consists of lowercase English letters.</p>

## Output

<p>Print the sought maximum beauty value Xenia can get.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
zzz

```




```input2
aba

```




```input3
abacaba

```




```input4
aaaaaa

```




```output1
12

```




```output2
12

```




```output3
83

```




```output4
15

```



## Note

<p>In the first test sample the given string can be transformed into string <span class="tex-span"><i>p</i></span> = "<span class="tex-font-style-tt">zbz</span>". Such string contains Gray strings as substrings <span class="tex-span"><i>p</i>[1... 1]</span>, <span class="tex-span"><i>p</i>[2... 2]</span>, <span class="tex-span"><i>p</i>[3... 3]</span> и <span class="tex-span"><i>p</i>[1... 3]</span>. In total, the beauty of string <span class="tex-span"><i>p</i></span> gets equal to <span class="tex-span">1<sup class="upper-index">2</sup> + 1<sup class="upper-index">2</sup> + 1<sup class="upper-index">2</sup> + 3<sup class="upper-index">2</sup> = 12</span>. You can't obtain a more beautiful string.</p><p>In the second test case it is not necessary to perform any operation. The initial string has the maximum possible beauty.</p>
