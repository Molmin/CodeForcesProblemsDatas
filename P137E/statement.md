## Description

<div><p>Having read half of the book called "Storm and Calm" on the IT lesson, Innocentius was absolutely determined to finish the book on the maths lessons. All was fine until the math teacher Ms. Watkins saw Innocentius reading fiction books instead of solving equations of the fifth degree. As during the last maths class Innocentius suggested the algorithm of solving equations of the fifth degree in the general case, Ms. Watkins had no other choice but to give him a new task.</p><p>The teacher asked to write consecutively (without spaces) all words from the "Storm and Calm" in one long string <span class="tex-span"><i>s</i></span>. She thought that a string is good if the number of vowels in the string is no more than twice more than the number of consonants. That is, the string with <span class="tex-span"><i>v</i></span> vowels and <span class="tex-span"><i>c</i></span> consonants is good if and only if <span class="tex-span"><i>v</i> ≤ 2<i>c</i></span>.</p><p>The task Innocentius had to solve turned out to be rather simple: he should find the number of the longest good substrings of the string <span class="tex-span"><i>s</i></span>.</p></div><div class="input-specification"><p>The only input line contains a non-empty string <span class="tex-span"><i>s</i></span> consisting of no more than <span class="tex-span">2·10<sup class="upper-index">5</sup></span> uppercase and lowercase Latin letters. We shall regard letters "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">e</span>", "<span class="tex-font-style-tt">i</span>", "<span class="tex-font-style-tt">o</span>", "<span class="tex-font-style-tt">u</span>" and their uppercase variants as vowels.</p></div><div class="output-specification"><p>Print on a single line two numbers without a space: the maximum length of a good substring and the number of good substrings with this length. If no good substring exists, print "<span class="tex-font-style-tt">No solution</span>" without the quotes.</p><p>Two substrings are considered different if their positions of occurrence are different. So if some string occurs more than once, then it should be counted more than once.</p></div>

## Input

<p>The only input line contains a non-empty string <span class="tex-span"><i>s</i></span> consisting of no more than <span class="tex-span">2·10<sup class="upper-index">5</sup></span> uppercase and lowercase Latin letters. We shall regard letters "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">e</span>", "<span class="tex-font-style-tt">i</span>", "<span class="tex-font-style-tt">o</span>", "<span class="tex-font-style-tt">u</span>" and their uppercase variants as vowels.</p>

## Output

<p>Print on a single line two numbers without a space: the maximum length of a good substring and the number of good substrings with this length. If no good substring exists, print "<span class="tex-font-style-tt">No solution</span>" without the quotes.</p><p>Two substrings are considered different if their positions of occurrence are different. So if some string occurs more than once, then it should be counted more than once.</p>





```input1
Abo

```




```input2
OEIS

```




```input3
auBAAbeelii

```




```input4
AaaBRAaaCAaaDAaaBRAaa

```




```input5
EA

```




```output1
3 1

```




```output2
3 1

```




```output3
9 3

```




```output4
18 4

```




```output5
No solution

```



## Note

<p>In the first sample there is only one longest good substring: "<span class="tex-font-style-tt">Abo</span>" itself. The other good substrings are "<span class="tex-font-style-tt">b</span>", "<span class="tex-font-style-tt">Ab</span>", "<span class="tex-font-style-tt">bo</span>", but these substrings have shorter length.</p><p>In the second sample there is only one longest good substring: "<span class="tex-font-style-tt">EIS</span>". The other good substrings are: "<span class="tex-font-style-tt">S</span>", "<span class="tex-font-style-tt">IS</span>".</p>
