## Description

<div><p>The ancient Berlanders believed that the longer the name, the more important its bearer is. Thus, Berland kings were famous for their long names. But long names are somewhat inconvenient, so the Berlanders started to abbreviate the names of their kings. They called every king by the first letters of its name. Thus, the king, whose name was Victorious Vasily Pupkin, was always called by the berlanders VVP.</p><p>In Berland over its long history many dynasties of kings replaced each other, but they were all united by common traditions. Thus, according to one Berland traditions, to maintain stability in the country, the first name of the heir should be the same as the last name his predecessor (hence, the first letter of the abbreviated name of the heir coincides with the last letter of the abbreviated name of the predecessor). Berlanders appreciate stability, so this tradition has never been broken. Also Berlanders like perfection, so another tradition requires that the first name of the first king in the dynasty coincides with the last name of the last king in this dynasty (hence, the first letter of the abbreviated name of the first king coincides with the last letter of the abbreviated name of the last king). This tradition, of course, has also been always observed.</p><p>The name of a dynasty is formed by very simple rules: we take all the short names of the kings in the order in which they ruled, and write them in one line. Thus, a dynasty of kings "ab" and "ba" is called "abba", and the dynasty, which had only the king "abca", is called "abca".</p><p>Vasya, a historian, has recently found a list of abbreviated names of all Berland kings and their relatives. Help Vasya to find the maximally long name of the dynasty that could have existed in Berland.</p><p>Note that in his list all the names are ordered by the time, that is, if name <span class="tex-span"><i>A</i></span> is earlier in the list than <span class="tex-span"><i>B</i></span>, then if <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span> were kings, then king <span class="tex-span"><i>A</i></span> ruled before king <span class="tex-span"><i>B</i></span>.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>) — the number of names in Vasya's list. Next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>n</i></span> abbreviated names, one per line. An abbreviated name is a non-empty sequence of lowercase Latin letters. Its length does not exceed <span class="tex-span">10</span> characters.</p></div><div class="output-specification"><p>Print a single number — length of the sought dynasty's name in letters.</p><p>If Vasya's list is wrong and no dynasty can be found there, print a single number <span class="tex-span">0</span>.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>) — the number of names in Vasya's list. Next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>n</i></span> abbreviated names, one per line. An abbreviated name is a non-empty sequence of lowercase Latin letters. Its length does not exceed <span class="tex-span">10</span> characters.</p>

## Output

<p>Print a single number — length of the sought dynasty's name in letters.</p><p>If Vasya's list is wrong and no dynasty can be found there, print a single number <span class="tex-span">0</span>.</p>





```input1
3
abc
ca
cba

```




```input2
4
vvp
vvp
dam
vvp

```




```input3
3
ab
c
def

```




```output1
6

```




```output2
0

```




```output3
1

```



## Note

<p>In the first sample two dynasties can exist: the one called "abcca" (with the first and second kings) and the one called "abccba" (with the first and third kings). </p><p>In the second sample there aren't acceptable dynasties.</p><p>The only dynasty in the third sample consists of one king, his name is "c".</p>
