## Description

<div><p>"Multidimensional spaces are completely out of style these days, unlike genetics problems" — thought physicist Woll and changed his subject of study to bioinformatics. Analysing results of sequencing he faced the following problem concerning DNA sequences. We will further think of a DNA sequence as an arbitrary string of uppercase letters "<span class="tex-font-style-tt">A</span>", "<span class="tex-font-style-tt">C</span>", "<span class="tex-font-style-tt">G</span>" and "<span class="tex-font-style-tt">T</span>" (of course, this is a simplified interpretation).</p><p>Let <span class="tex-span"><i>w</i></span> be a long DNA sequence and <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>m</i></sub></span> — collection of short DNA sequences. Let us say that the collection <span class="tex-font-style-it">filters</span> <span class="tex-span"><i>w</i></span> iff <span class="tex-span"><i>w</i></span> can be covered with the sequences from the collection. Certainly, substrings corresponding to the different positions of the string may intersect or even cover each other. More formally: denote by <span class="tex-span">|<i>w</i>|</span> the length of <span class="tex-span"><i>w</i></span>, let symbols of <span class="tex-span"><i>w</i></span> be numbered from <span class="tex-span">1</span> to <span class="tex-span">|<i>w</i>|</span>. Then for each position <span class="tex-span"><i>i</i></span> in <span class="tex-span"><i>w</i></span> there exist pair of indices <span class="tex-span"><i>l</i>, <i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>i</i> ≤ <i>r</i> ≤ |<i>w</i>|</span>) such that the substring <span class="tex-span"><i>w</i>[<i>l</i>&nbsp;...&nbsp;<i>r</i>]</span> equals one of the elements <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>m</i></sub></span> of the collection.</p><p>Woll wants to calculate the number of DNA sequences of a given length filtered by a given collection, but he doesn't know how to deal with it. Help him! Your task is to find the number of different DNA sequences of length <span class="tex-span"><i>n</i></span> filtered by the collection <span class="tex-span">{<i>s</i><sub class="lower-index"><i>i</i></sub>}</span>.</p><p>Answer may appear very large, so output it modulo <span class="tex-span">1000000009</span>.</p></div><div class="input-specification"><p>First line contains two integer numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000, 1 ≤ <i>m</i> ≤ 10</span>) — the length of the string and the number of sequences in the collection correspondently. </p><p>Next <span class="tex-span"><i>m</i></span> lines contain the collection sequences <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>, one per line. Each <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> is a nonempty string of length not greater than <span class="tex-span">10</span>. All the strings consist of uppercase letters "<span class="tex-font-style-tt">A</span>", "<span class="tex-font-style-tt">C</span>", "<span class="tex-font-style-tt">G</span>", "<span class="tex-font-style-tt">T</span>". The collection may contain identical strings.</p></div><div class="output-specification"><p>Output should contain a single integer — the number of strings filtered by the collection modulo <span class="tex-span">1000000009</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 9</span>).</p></div>

## Input

<p>First line contains two integer numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000, 1 ≤ <i>m</i> ≤ 10</span>) — the length of the string and the number of sequences in the collection correspondently. </p><p>Next <span class="tex-span"><i>m</i></span> lines contain the collection sequences <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>, one per line. Each <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> is a nonempty string of length not greater than <span class="tex-span">10</span>. All the strings consist of uppercase letters "<span class="tex-font-style-tt">A</span>", "<span class="tex-font-style-tt">C</span>", "<span class="tex-font-style-tt">G</span>", "<span class="tex-font-style-tt">T</span>". The collection may contain identical strings.</p>

## Output

<p>Output should contain a single integer — the number of strings filtered by the collection modulo <span class="tex-span">1000000009</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 9</span>).</p>





```input1
2 1
A

```




```input2
6 2
CAT
TACT

```




```output1
1

```




```output2
2

```



## Note

<p>In the first sample, a string has to be filtered by "<span class="tex-font-style-tt">A</span>". Clearly, there is only one such string: "<span class="tex-font-style-tt">AA</span>".</p><p>In the second sample, there exist exactly two different strings satisfying the condition (see the pictures below).</p><center> <img class="tex-graphics" src="file://4hXj3STZ.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><center> <img class="tex-graphics" src="file://O08ZXqaw.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
