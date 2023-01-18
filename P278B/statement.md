## Description

<div><p>Coming up with a new problem isn't as easy as many people think. Sometimes it is hard enough to name it. We'll consider a title <span class="tex-font-style-underline">original</span> if it doesn't occur as a substring in any titles of recent Codeforces problems. </p><p>You've got the titles of <span class="tex-span"><i>n</i></span> last problems — the strings, consisting of lowercase English letters. Your task is to find the shortest original title for the new problem. If there are multiple such titles, choose the lexicographically minimum one. Note, that title of the problem can't be an empty string.</p><p>A <span class="tex-font-style-it">substring</span> <span class="tex-span"><i>s</i>[<i>l</i>... <i>r</i>]</span> <span class="tex-span">(1 ≤ <i>l</i> ≤ <i>r</i> ≤ |<i>s</i>|)</span> of string <span class="tex-span"><i>s</i> = <i>s</i><sub class="lower-index">1</sub><i>s</i><sub class="lower-index">2</sub>... <i>s</i><sub class="lower-index">|<i>s</i>|</sub></span> (where <span class="tex-span">|<i>s</i>|</span> is the length of string <span class="tex-span"><i>s</i></span>) is string <span class="tex-span"><i>s</i><sub class="lower-index"><i>l</i></sub><i>s</i><sub class="lower-index"><i>l</i> + 1</sub>... <i>s</i><sub class="lower-index"><i>r</i></sub></span>.</p><p>String <span class="tex-span"><i>x</i> = <i>x</i><sub class="lower-index">1</sub><i>x</i><sub class="lower-index">2</sub>... <i>x</i><sub class="lower-index"><i>p</i></sub></span> is <span class="tex-font-style-it">lexicographically smaller</span> than string <span class="tex-span"><i>y</i> = <i>y</i><sub class="lower-index">1</sub><i>y</i><sub class="lower-index">2</sub>... <i>y</i><sub class="lower-index"><i>q</i></sub></span>, if either <span class="tex-span"><i>p</i> &lt; <i>q</i></span> and <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> = <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub> = <i>y</i><sub class="lower-index">2</sub>, ... , <i>x</i><sub class="lower-index"><i>p</i></sub> = <i>y</i><sub class="lower-index"><i>p</i></sub></span>, or there exists such number <span class="tex-span"><i>r</i></span> <span class="tex-span">(<i>r</i> &lt; <i>p</i>, <i>r</i> &lt; <i>q</i>)</span>, that <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> = <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub> = <i>y</i><sub class="lower-index">2</sub>, ... , <i>x</i><sub class="lower-index"><i>r</i></sub> = <i>y</i><sub class="lower-index"><i>r</i></sub></span> and <span class="tex-span"><i>x</i><sub class="lower-index"><i>r</i> + 1</sub> &lt; <i>y</i><sub class="lower-index"><i>r</i> + 1</sub></span>. The string characters are compared by their ASCII codes.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 30</span>) — the number of titles you've got to consider. Then follow <span class="tex-span"><i>n</i></span> problem titles, one per line. Each title only consists of lowercase English letters (specifically, it doesn't contain any spaces) and has the length from 1 to 20, inclusive.</p></div><div class="output-specification"><p>Print a string, consisting of lowercase English letters — the lexicographically minimum shortest original title.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 30</span>) — the number of titles you've got to consider. Then follow <span class="tex-span"><i>n</i></span> problem titles, one per line. Each title only consists of lowercase English letters (specifically, it doesn't contain any spaces) and has the length from 1 to 20, inclusive.</p>

## Output

<p>Print a string, consisting of lowercase English letters — the lexicographically minimum shortest original title.</p>





```input1
5
threehorses
goodsubstrings
secret
primematrix
beautifulyear

```




```input2
4
aa
bdefghijklmn
opqrstuvwxyz
c

```




```output1
j

```




```output2
ab

```



## Note

<p>In the first sample the first 9 letters of the English alphabet (<span class="tex-font-style-tt">a, b, c, d, e, f, g, h, i</span>) occur in the problem titles, so the answer is letter <span class="tex-font-style-tt">j</span>.</p><p>In the second sample the titles contain 26 English letters, so the shortest original title cannot have length 1. Title <span class="tex-font-style-tt">aa</span> occurs as a substring in the first title.</p>
