## Description

<div><p>Anfisa the monkey learns to type. She is yet unfamiliar with the "space" key and can only type in lower-case Latin letters. Having typed for a fairly long line, Anfisa understood that it would be great to divide what she has written into <span class="tex-span"><i>k</i></span> lines not shorter than <span class="tex-span"><i>a</i></span> and not longer than <span class="tex-span"><i>b</i></span>, for the text to resemble human speech more. Help Anfisa.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 200</span>, <span class="tex-span">1 ≤ <i>a</i> ≤ <i>b</i> ≤ 200</span>). The second line contains a sequence of lowercase Latin letters — the text typed by Anfisa. It is guaranteed that the given line is not empty and its length does not exceed <span class="tex-span">200</span> symbols.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>k</i></span> lines, each of which contains no less than <span class="tex-span"><i>a</i></span> and no more than <span class="tex-span"><i>b</i></span> symbols — Anfisa's text divided into lines. It is not allowed to perform any changes in the text, such as: deleting or adding symbols, changing their order, etc. If the solution is not unique, print any of them. If there is no solution, print "No solution" (without quotes). </p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 200</span>, <span class="tex-span">1 ≤ <i>a</i> ≤ <i>b</i> ≤ 200</span>). The second line contains a sequence of lowercase Latin letters — the text typed by Anfisa. It is guaranteed that the given line is not empty and its length does not exceed <span class="tex-span">200</span> symbols.</p>

## Output

<p>Print <span class="tex-span"><i>k</i></span> lines, each of which contains no less than <span class="tex-span"><i>a</i></span> and no more than <span class="tex-span"><i>b</i></span> symbols — Anfisa's text divided into lines. It is not allowed to perform any changes in the text, such as: deleting or adding symbols, changing their order, etc. If the solution is not unique, print any of them. If there is no solution, print "No solution" (without quotes). </p>





```input1
3 2 5
abrakadabra

```




```input2
4 1 2
abrakadabra

```




```output1
ab
rakad
abra

```




```output2
No solution

```


