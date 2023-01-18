## Description

<div><p>The process of mammoth's genome decoding in Berland comes to its end!</p><p>One of the few remaining tasks is to restore unrecognized nucleotides in a found chain <span class="tex-span"><i>s</i></span>. Each nucleotide is coded with a capital letter of English alphabet: '<span class="tex-font-style-tt">A</span>', '<span class="tex-font-style-tt">C</span>', '<span class="tex-font-style-tt">G</span>' or '<span class="tex-font-style-tt">T</span>'. Unrecognized nucleotides are coded by a question mark '<span class="tex-font-style-tt">?</span>'. Thus, <span class="tex-span"><i>s</i></span> is a string consisting of letters '<span class="tex-font-style-tt">A</span>', '<span class="tex-font-style-tt">C</span>', '<span class="tex-font-style-tt">G</span>', '<span class="tex-font-style-tt">T</span>' and characters '<span class="tex-font-style-tt">?</span>'.</p><p>It is known that the number of nucleotides of each of the four types in the decoded genome of mammoth in Berland should be equal.</p><p>Your task is to decode the genome and replace each unrecognized nucleotide with one of the four types so that the number of nucleotides of each of the four types becomes equal.</p></div><div class="input-specification"><p>The first line contains the integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">4 ≤ <i>n</i> ≤ 255</span>)&nbsp;— the length of the genome.</p><p>The second line contains the string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span>&nbsp;— the coded genome. It consists of characters '<span class="tex-font-style-tt">A</span>', '<span class="tex-font-style-tt">C</span>', '<span class="tex-font-style-tt">G</span>', '<span class="tex-font-style-tt">T</span>' and '<span class="tex-font-style-tt">?</span>'.</p></div><div class="output-specification"><p>If it is possible to decode the genome, print it. If there are multiple answer, print any of them. If it is not possible, print three equals signs in a row: "<span class="tex-font-style-tt">===</span>" (without quotes).</p></div>

## Input

<p>The first line contains the integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">4 ≤ <i>n</i> ≤ 255</span>)&nbsp;— the length of the genome.</p><p>The second line contains the string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span>&nbsp;— the coded genome. It consists of characters '<span class="tex-font-style-tt">A</span>', '<span class="tex-font-style-tt">C</span>', '<span class="tex-font-style-tt">G</span>', '<span class="tex-font-style-tt">T</span>' and '<span class="tex-font-style-tt">?</span>'.</p>

## Output

<p>If it is possible to decode the genome, print it. If there are multiple answer, print any of them. If it is not possible, print three equals signs in a row: "<span class="tex-font-style-tt">===</span>" (without quotes).</p>





```input1
8
AG?C??CT

```




```input2
4
AGCT

```




```input3
6
????G?

```




```input4
4
AA??

```




```output1
AGACGTCT

```




```output2
AGCT

```




```output3
===

```




```output4
===

```



## Note

<p>In the first example you can replace the first question mark with the letter '<span class="tex-font-style-tt">A</span>', the second question mark with the letter '<span class="tex-font-style-tt">G</span>', the third question mark with the letter '<span class="tex-font-style-tt">T</span>', then each nucleotide in the genome would be presented twice.</p><p>In the second example the genome is already decoded correctly and each nucleotide is exactly once in it.</p><p>In the third and the fourth examples it is impossible to decode the genom. </p>
