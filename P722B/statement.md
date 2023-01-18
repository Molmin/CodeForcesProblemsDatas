## Description

<div><p>You are given a text consisting of <span class="tex-span"><i>n</i></span> lines. Each line contains some space-separated words, consisting of lowercase English letters.</p><p>We define a syllable as a string that contains exactly one vowel and any arbitrary number (possibly none) of consonants. In English alphabet following letters are considered to be vowels: '<span class="tex-font-style-tt">a</span>', '<span class="tex-font-style-tt">e</span>', '<span class="tex-font-style-tt">i</span>', '<span class="tex-font-style-tt">o</span>', '<span class="tex-font-style-tt">u</span>' and '<span class="tex-font-style-tt">y</span>'.</p><p>Each word of the text that contains at least one vowel can be divided into syllables. Each character should be a part of exactly one syllable. For example, the word "<span class="tex-font-style-tt">mamma</span>" can be divided into syllables as "<span class="tex-font-style-tt">ma</span>" and "<span class="tex-font-style-tt">mma</span>", "<span class="tex-font-style-tt">mam</span>" and "<span class="tex-font-style-tt">ma</span>", and "<span class="tex-font-style-tt">mamm</span>" and "<span class="tex-font-style-tt">a</span>". Words that consist of only consonants should be ignored.</p><p>The verse patterns for the given text is a sequence of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span>. Text matches the given verse pattern if for each <span class="tex-span"><i>i</i></span> from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> one can divide words of the <span class="tex-span"><i>i</i></span>-th line in syllables in such a way that the total number of syllables is equal to <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>You are given the text and the verse pattern. Check, if the given text matches the given verse pattern.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the number of lines in the text.</p><p>The second line contains integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>)&nbsp;— the verse pattern.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain the text itself. Text consists of lowercase English letters and spaces. It's guaranteed that all lines are non-empty, each line starts and ends with a letter and words are separated by exactly one space. The length of each line doesn't exceed <span class="tex-span">100</span> characters.</p></div><div class="output-specification"><p>If the given text matches the given verse pattern, then print "<span class="tex-font-style-tt">YES</span>" (without quotes) in the only line of the output. Otherwise, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the number of lines in the text.</p><p>The second line contains integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>)&nbsp;— the verse pattern.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain the text itself. Text consists of lowercase English letters and spaces. It's guaranteed that all lines are non-empty, each line starts and ends with a letter and words are separated by exactly one space. The length of each line doesn't exceed <span class="tex-span">100</span> characters.</p>

## Output

<p>If the given text matches the given verse pattern, then print "<span class="tex-font-style-tt">YES</span>" (without quotes) in the only line of the output. Otherwise, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p>





```input1
3
2 2 3
intel
code
ch allenge

```




```input2
4
1 2 3 1
a
bcdefghi
jklmnopqrstu
vwxyz

```




```input3
4
13 11 15 15
to be or not to be that is the question
whether tis nobler in the mind to suffer
the slings and arrows of outrageous fortune
or to take arms against a sea of troubles

```




```output1
YES

```




```output2
NO

```




```output3
YES

```



## Note

<p>In the first sample, one can split words into syllables in the following way: </p><pre class="verbatim">in-tel<br>co-de<br>ch al-len-ge<br></pre><p>Since the word "<span class="tex-font-style-tt">ch</span>" in the third line doesn't contain vowels, we can ignore it. As the result we get <span class="tex-span">2</span> syllabels in first two lines and <span class="tex-span">3</span> syllables in the third one.</p>
