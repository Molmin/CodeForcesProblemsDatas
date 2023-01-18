## Description

<div><p>Berland scientists face a very important task - given the parts of short DNA fragments, restore the dinosaur DNA! The genome of a berland dinosaur has noting in common with the genome that we've used to: it can have <span class="tex-span">26</span> distinct nucleotide types, a nucleotide of each type can occur <span class="tex-font-style-bf">at most once</span>. If we assign distinct English letters to all nucleotides, then the genome of a Berland dinosaur will represent a non-empty string consisting of small English letters, such that each letter occurs in it at most once.</p><p>Scientists have <span class="tex-span"><i>n</i></span> genome fragments that are represented as <span class="tex-font-style-bf">substrings</span> (non-empty sequences of consecutive nucleotides) of the sought genome.</p><p>You face the following problem: help scientists restore the dinosaur genome. It is guaranteed that the input is not contradictory and at least one suitable line always exists. When the scientists found out that you are a strong programmer, they asked you in addition to choose the one with the minimum length. If there are multiple such strings, choose any string.</p></div><div class="input-specification"><p>The first line of the input contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the number of genome fragments.</p><p>Each of the next lines contains one descriptions of a fragment. Each fragment is a non-empty string consisting of distinct small letters of the English alphabet. It is not guaranteed that the given fragments are distinct. Fragments could arbitrarily overlap and one fragment could be a substring of another one.</p><p>It is guaranteed that there is such string of distinct letters that contains all the given fragments as substrings.</p></div><div class="output-specification"><p>In the single line of the output print the genome of the minimum length that contains all the given parts. All the nucleotides in the genome must be distinct. If there are multiple suitable strings, print the string of the minimum length. If there also are multiple suitable strings, you can print any of them.</p></div>

## Input

<p>The first line of the input contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the number of genome fragments.</p><p>Each of the next lines contains one descriptions of a fragment. Each fragment is a non-empty string consisting of distinct small letters of the English alphabet. It is not guaranteed that the given fragments are distinct. Fragments could arbitrarily overlap and one fragment could be a substring of another one.</p><p>It is guaranteed that there is such string of distinct letters that contains all the given fragments as substrings.</p>

## Output

<p>In the single line of the output print the genome of the minimum length that contains all the given parts. All the nucleotides in the genome must be distinct. If there are multiple suitable strings, print the string of the minimum length. If there also are multiple suitable strings, you can print any of them.</p>





```input1
3
bcd
ab
cdef

```




```input2
4
x
y
z
w

```




```output1
abcdef

```




```output2
xyzw

```


