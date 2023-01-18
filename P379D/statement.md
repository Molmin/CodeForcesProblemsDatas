## Description

<div><p>Many countries have such a New Year or Christmas tradition as writing a letter to Santa including a wish list for presents. Vasya is an ordinary programmer boy. Like all ordinary boys, he is going to write the letter to Santa on the New Year Eve (we Russians actually expect Santa for the New Year, not for Christmas). </p><p>Vasya has come up with an algorithm he will follow while writing a letter. First he chooses two strings, <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> anf <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span>, consisting of uppercase English letters. Then the boy makes string <span class="tex-span"><i>s</i><sub class="lower-index"><i>k</i></sub></span>, using a recurrent equation <span class="tex-span"><i>s</i><sub class="lower-index"><i>n</i></sub> = <i>s</i><sub class="lower-index"><i>n</i> - 2</sub> + <i>s</i><sub class="lower-index"><i>n</i> - 1</sub></span>, operation '<span class="tex-font-style-tt">+</span>' means a concatenation (that is, the sequential record) of strings in the given order. Then Vasya writes down string <span class="tex-span"><i>s</i><sub class="lower-index"><i>k</i></sub></span> on a piece of paper, puts it in the envelope and sends in to Santa. </p><p>Vasya is absolutely sure that Santa will bring him the best present if the resulting string <span class="tex-span"><i>s</i><sub class="lower-index"><i>k</i></sub></span> has exactly <span class="tex-span"><i>x</i></span> occurrences of substring <span class="tex-font-style-tt">AC</span> (the short-cut reminds him оf accepted problems). Besides, Vasya decided that string <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> should have length <span class="tex-span"><i>n</i></span>, and string <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> should have length <span class="tex-span"><i>m</i></span>. Vasya hasn't decided anything else.</p><p>At the moment Vasya's got urgent New Year business, so he asks you to choose two strings for him, <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> in the required manner. Help Vasya.</p></div><div class="input-specification"><p>The first line contains four integers <span class="tex-span"><i>k</i>, <i>x</i>, <i>n</i>, <i>m</i></span> <span class="tex-span">(3 ≤ <i>k</i> ≤ 50;&nbsp;0 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup>;&nbsp;1 ≤ <i>n</i>, <i>m</i> ≤ 100)</span>.</p></div><div class="output-specification"><p>In the first line print string <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span>, consisting of <span class="tex-span"><i>n</i></span> uppercase English letters. In the second line print string <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span>, consisting of <span class="tex-span"><i>m</i></span> uppercase English letters. If there are multiple valid strings, print any of them.</p><p>If the required pair of strings doesn't exist, print "<span class="tex-font-style-tt">Happy new year!</span>" without the quotes.</p></div>

## Input

<p>The first line contains four integers <span class="tex-span"><i>k</i>, <i>x</i>, <i>n</i>, <i>m</i></span> <span class="tex-span">(3 ≤ <i>k</i> ≤ 50;&nbsp;0 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup>;&nbsp;1 ≤ <i>n</i>, <i>m</i> ≤ 100)</span>.</p>

## Output

<p>In the first line print string <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span>, consisting of <span class="tex-span"><i>n</i></span> uppercase English letters. In the second line print string <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span>, consisting of <span class="tex-span"><i>m</i></span> uppercase English letters. If there are multiple valid strings, print any of them.</p><p>If the required pair of strings doesn't exist, print "<span class="tex-font-style-tt">Happy new year!</span>" without the quotes.</p>





```input1
3 2 2 2

```




```input2
3 3 2 2

```




```input3
3 0 2 2

```




```input4
4 3 2 1

```




```input5
4 2 2 1

```




```output1
AC
AC

```




```output2
Happy new year!

```




```output3
AA
AA

```




```output4
Happy new year!

```




```output5
Happy new year!

```


