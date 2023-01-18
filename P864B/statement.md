## Description

<div><p>Polycarp loves lowercase letters and dislikes uppercase ones. Once he got a string <span class="tex-span"><i>s</i></span> consisting only of lowercase and uppercase Latin letters.</p><p>Let <span class="tex-span"><i>A</i></span> be a set of positions in the string. Let's call it <span class="tex-font-style-it">pretty</span> if following conditions are met:</p><ul> <li> letters on positions from <span class="tex-span"><i>A</i></span> in the string are all distinct and lowercase; </li><li> there are no uppercase letters in the string which are situated between positions from <span class="tex-span"><i>A</i></span> (i.e. there is no such <span class="tex-span"><i>j</i></span> that <span class="tex-span"><i>s</i>[<i>j</i>]</span> is an uppercase letter, and <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> &lt; <i>j</i> &lt; <i>a</i><sub class="lower-index">2</sub></span> for some <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span> from <span class="tex-span"><i>A</i></span>). </li></ul><p>Write a program that will determine the maximum number of elements in a <span class="tex-font-style-it">pretty</span> set of positions.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200</span>) — length of string <span class="tex-span"><i>s</i></span>.</p><p>The second line contains a string <span class="tex-span"><i>s</i></span> consisting of lowercase and uppercase Latin letters.</p></div><div class="output-specification"><p>Print maximum number of elements in <span class="tex-font-style-it">pretty</span> set of positions for string <span class="tex-span"><i>s</i></span>.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200</span>) — length of string <span class="tex-span"><i>s</i></span>.</p><p>The second line contains a string <span class="tex-span"><i>s</i></span> consisting of lowercase and uppercase Latin letters.</p>

## Output

<p>Print maximum number of elements in <span class="tex-font-style-it">pretty</span> set of positions for string <span class="tex-span"><i>s</i></span>.</p>





```input1
11
aaaaBaabAbA

```




```input2
12
zACaAbbaazzC

```




```input3
3
ABC

```




```output1
2

```




```output2
3

```




```output3
0

```



## Note

<p>In the first example the desired positions might be <span class="tex-span">6</span> and <span class="tex-span">8</span> or <span class="tex-span">7</span> and <span class="tex-span">8</span>. Positions <span class="tex-span">6</span> and <span class="tex-span">7</span> contain letters '<span class="tex-font-style-tt">a</span>', position <span class="tex-span">8</span> contains letter '<span class="tex-font-style-tt">b</span>'. The pair of positions <span class="tex-span">1</span> and <span class="tex-span">8</span> is not suitable because there is an uppercase letter '<span class="tex-font-style-tt">B</span>' between these position.</p><p>In the second example desired positions can be <span class="tex-span">7</span>, <span class="tex-span">8</span> and <span class="tex-span">11</span>. There are other ways to choose <span class="tex-font-style-it">pretty</span> set consisting of three elements.</p><p>In the third example the given string <span class="tex-span"><i>s</i></span> does not contain any lowercase letters, so the answer is <span class="tex-span">0</span>.</p>
