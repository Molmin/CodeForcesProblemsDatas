## Description

<div><p>BerOilGasDiamondBank has branches in <span class="tex-span"><i>n</i></span> cities, at that <span class="tex-span"><i>n</i></span> is an even number. The bank management wants to publish a calendar with the names of all those cities written in two columns: the calendar should consist of exactly <span class="tex-span"><i>n</i> / 2</span> lines of strictly equal length, each of which contains exactly two names and exactly one separator character between them. The name of every city should be used in the calendar exactly once. For historical reasons the symbol <span class="tex-span"><i>d</i></span> is used as the separator of words in the calendar. </p><p>The BerOilGasDiamondBank management wants to show that all its branches are equally important to it, that's why the order of their appearance in the calendar should be following: if we "glue"(concatinate) all the <span class="tex-span"><i>n</i> / 2</span> calendar lines (from top to bottom) to make a single line, then the lexicographically minimal line is obtained. No separator character will be used to separate calendar lines. For example, if the lines are "bertown!berville", "newberville!bera", then the resulting line is "bertown!bervillenewberville!bera". In some sense one has to find the lexicographically minimal calendar, where the comparison of calendars happens line by line.</p><p>Help BerOilGasDiamondBank and construct the required calendar.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">4</sup></span>, <span class="tex-span"><i>n</i></span> is even) which is the number of branches. Then follow <span class="tex-span"><i>n</i></span> lines which are the names of the cities. All the names consist of lowercase Latin letters; their lengths are no less than 1 and no more than 10 symbols. The next line contains a single symbol <span class="tex-span"><i>d</i></span> (<span class="tex-span"><i>d</i></span> has an ASCII-code from 33 to 126 inclusively, excluding lowercase Latin letters) which is the separator between words in the calendar lines. It is guaranteed that the calendar is possible to be constructed and all the names are different.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i> / 2</span> lines of similar length which are the required calendar. Every line should contain exactly two words and exactly one separator between them. If there are several solutions, print the lexicographically minimal one. The lexicographical comparison of lines is realized by the "<span class="tex-font-style-tt">&lt;</span>" operator in the modern programming languages.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">4</sup></span>, <span class="tex-span"><i>n</i></span> is even) which is the number of branches. Then follow <span class="tex-span"><i>n</i></span> lines which are the names of the cities. All the names consist of lowercase Latin letters; their lengths are no less than 1 and no more than 10 symbols. The next line contains a single symbol <span class="tex-span"><i>d</i></span> (<span class="tex-span"><i>d</i></span> has an ASCII-code from 33 to 126 inclusively, excluding lowercase Latin letters) which is the separator between words in the calendar lines. It is guaranteed that the calendar is possible to be constructed and all the names are different.</p>

## Output

<p>Print <span class="tex-span"><i>n</i> / 2</span> lines of similar length which are the required calendar. Every line should contain exactly two words and exactly one separator between them. If there are several solutions, print the lexicographically minimal one. The lexicographical comparison of lines is realized by the "<span class="tex-font-style-tt">&lt;</span>" operator in the modern programming languages.</p>





```input1
4
b
aa
hg
c
.

```




```input2
2
aa
a
!

```




```input3
2
aa
a
|

```




```output1
aa.b
c.hg

```




```output2
a!aa

```




```output3
aa|a

```


