## Description

<div><p>Police headquarter is monitoring signal on different frequency levels. They have got two suspiciously encoded strings <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> from two different frequencies as signals. They are suspecting that these two strings are from two different criminals and they are planning to do some evil task.</p><p>Now they are trying to find a common substring of minimum length between these two strings. The substring must occur only once in the first string, and also it must occur only once in the second string.</p><p>Given two strings <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> consist of lowercase Latin letters, find the smallest (by length) common substring <span class="tex-span"><i>p</i></span> of both <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span>, where <span class="tex-span"><i>p</i></span> is a unique substring in <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> and also in <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span>. See notes for formal definition of substring and uniqueness.</p></div><div class="input-specification"><p>The first line of input contains <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> and the second line contains <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> <span class="tex-span">(1 ≤ |<i>s</i><sub class="lower-index">1</sub>|, |<i>s</i><sub class="lower-index">2</sub>| ≤ 5000)</span>. Both strings consist of lowercase Latin letters.</p></div><div class="output-specification"><p>Print the length of the smallest common unique substring of <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span>. If there are no common unique substrings of <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> print -1.</p></div>

## Input

<p>The first line of input contains <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> and the second line contains <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> <span class="tex-span">(1 ≤ |<i>s</i><sub class="lower-index">1</sub>|, |<i>s</i><sub class="lower-index">2</sub>| ≤ 5000)</span>. Both strings consist of lowercase Latin letters.</p>

## Output

<p>Print the length of the smallest common unique substring of <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span>. If there are no common unique substrings of <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> print -1.</p>





```input1
apple
pepperoni

```




```input2
lover
driver

```




```input3
bidhan
roy

```




```input4
testsetses
teeptes

```




```output1
2

```




```output2
1

```




```output3
-1

```




```output4
3

```



## Note

<p>Imagine we have string <span class="tex-span"><i>a</i> = <i>a</i><sub class="lower-index">1</sub><i>a</i><sub class="lower-index">2</sub><i>a</i><sub class="lower-index">3</sub>...<i>a</i><sub class="lower-index">|<i>a</i>|</sub></span>, where <span class="tex-span">|<i>a</i>|</span> is the length of string <span class="tex-span"><i>a</i></span>, and <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the <span class="tex-span"><i>i</i><sup class="upper-index"><i>th</i></sup></span> letter of the string. </p><p>We will call string <span class="tex-span"><i>a</i><sub class="lower-index"><i>l</i></sub><i>a</i><sub class="lower-index"><i>l</i> + 1</sub><i>a</i><sub class="lower-index"><i>l</i> + 2</sub>...<i>a</i><sub class="lower-index"><i>r</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i> ≤ <i>r</i> ≤ |<i>a</i>|)</span> the substring <span class="tex-span">[<i>l</i>, <i>r</i>]</span> of the string <span class="tex-span"><i>a</i></span>. </p><p>The substring <span class="tex-span">[<i>l</i>, <i>r</i>]</span> is unique in <span class="tex-span"><i>a</i></span> if and only if there is no pair <span class="tex-span"><i>l</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">1</sub></span> such that <span class="tex-span"><i>l</i><sub class="lower-index">1</sub> ≠ <i>l</i></span> and the substring <span class="tex-span">[<i>l</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">1</sub>]</span> is equal to the substring <span class="tex-span">[<i>l</i>, <i>r</i>]</span> in <span class="tex-span"><i>a</i></span>.</p>
