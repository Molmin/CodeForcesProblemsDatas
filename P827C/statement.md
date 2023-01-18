## Description

<div><p>Everyone knows that DNA strands consist of nucleotides. There are four types of nucleotides: "<span class="tex-font-style-tt">A</span>", "<span class="tex-font-style-tt">T</span>", "<span class="tex-font-style-tt">G</span>", "<span class="tex-font-style-tt">C</span>". A DNA strand is a sequence of nucleotides. Scientists decided to track evolution of a rare species, which DNA strand was string <span class="tex-span"><i>s</i></span> initially. </p><p>Evolution of the species is described as a sequence of changes in the DNA. Every change is a change of some nucleotide, for example, the following change can happen in DNA strand "<span class="tex-font-style-tt">AAGC</span>": the second nucleotide can change to "<span class="tex-font-style-tt">T</span>" so that the resulting DNA strand is "<span class="tex-font-style-tt">ATGC</span>".</p><p>Scientists know that some segments of the DNA strand can be affected by some unknown infections. They can represent an infection as a sequence of nucleotides. Scientists are interested if there are any changes caused by some infections. Thus they sometimes want to know the value of impact of some infection to some segment of the DNA. This value is computed as follows:</p><ul> <li> Let the infection be represented as a string <span class="tex-span"><i>e</i></span>, and let scientists be interested in DNA strand segment starting from position <span class="tex-span"><i>l</i></span> to position <span class="tex-span"><i>r</i></span>, inclusive. </li><li> Prefix of the string <span class="tex-span"><i>eee</i>...</span> (i.e. the string that consists of infinitely many repeats of string <span class="tex-span"><i>e</i></span>) is written under the string <span class="tex-span"><i>s</i></span> from position <span class="tex-span"><i>l</i></span> to position <span class="tex-span"><i>r</i></span>, inclusive. </li><li> The value of impact is the number of positions where letter of string <span class="tex-span"><i>s</i></span> coincided with the letter written under it. </li></ul><p>Being a developer, Innokenty is interested in bioinformatics also, so the scientists asked him for help. Innokenty is busy preparing VK Cup, so he decided to delegate the problem to the competitors. Help the scientists!</p></div><div class="input-specification"><p>The first line contains the string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 10<sup class="upper-index">5</sup></span>) that describes the initial DNA strand. It consists only of capital English letters "<span class="tex-font-style-tt">A</span>", "<span class="tex-font-style-tt">T</span>", "<span class="tex-font-style-tt">G</span>" and "<span class="tex-font-style-tt">C</span>".</p><p>The next line contains single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of events.</p><p>After that, <span class="tex-span"><i>q</i></span> lines follow, each describes one event. Each of the lines has one of two formats: </p><ul> <li> <span class="tex-font-style-tt">1&nbsp;x&nbsp;c</span>, where <span class="tex-span"><i>x</i></span> is an integer (<span class="tex-span">1 ≤ <i>x</i> ≤ |<i>s</i>|</span>), and <span class="tex-span"><i>c</i></span> is a letter "<span class="tex-font-style-tt">A</span>", "<span class="tex-font-style-tt">T</span>", "<span class="tex-font-style-tt">G</span>" or "<span class="tex-font-style-tt">C</span>", which means that there is a change in the DNA: the nucleotide at position <span class="tex-span"><i>x</i></span> is now <span class="tex-span"><i>c</i></span>. </li><li> <span class="tex-font-style-tt">2&nbsp;l&nbsp;r&nbsp;e</span>, where <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span> are integers (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ |<i>s</i>|</span>), and <span class="tex-span"><i>e</i></span> is a string of letters "<span class="tex-font-style-tt">A</span>", "<span class="tex-font-style-tt">T</span>", "<span class="tex-font-style-tt">G</span>" and "<span class="tex-font-style-tt">C</span>" (<span class="tex-span">1 ≤ |<i>e</i>| ≤ 10</span>), which means that scientists are interested in the value of impact of infection <span class="tex-span"><i>e</i></span> to the segment of DNA strand from position <span class="tex-span"><i>l</i></span> to position <span class="tex-span"><i>r</i></span>, inclusive. </li></ul></div><div class="output-specification"><p>For each scientists' query (second type query) print a single integer in a new line&nbsp;— the value of impact of the infection on the DNA.</p></div>

## Input

<p>The first line contains the string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 10<sup class="upper-index">5</sup></span>) that describes the initial DNA strand. It consists only of capital English letters "<span class="tex-font-style-tt">A</span>", "<span class="tex-font-style-tt">T</span>", "<span class="tex-font-style-tt">G</span>" and "<span class="tex-font-style-tt">C</span>".</p><p>The next line contains single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of events.</p><p>After that, <span class="tex-span"><i>q</i></span> lines follow, each describes one event. Each of the lines has one of two formats: </p><ul> <li> <span class="tex-font-style-tt">1&nbsp;x&nbsp;c</span>, where <span class="tex-span"><i>x</i></span> is an integer (<span class="tex-span">1 ≤ <i>x</i> ≤ |<i>s</i>|</span>), and <span class="tex-span"><i>c</i></span> is a letter "<span class="tex-font-style-tt">A</span>", "<span class="tex-font-style-tt">T</span>", "<span class="tex-font-style-tt">G</span>" or "<span class="tex-font-style-tt">C</span>", which means that there is a change in the DNA: the nucleotide at position <span class="tex-span"><i>x</i></span> is now <span class="tex-span"><i>c</i></span>. </li><li> <span class="tex-font-style-tt">2&nbsp;l&nbsp;r&nbsp;e</span>, where <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span> are integers (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ |<i>s</i>|</span>), and <span class="tex-span"><i>e</i></span> is a string of letters "<span class="tex-font-style-tt">A</span>", "<span class="tex-font-style-tt">T</span>", "<span class="tex-font-style-tt">G</span>" and "<span class="tex-font-style-tt">C</span>" (<span class="tex-span">1 ≤ |<i>e</i>| ≤ 10</span>), which means that scientists are interested in the value of impact of infection <span class="tex-span"><i>e</i></span> to the segment of DNA strand from position <span class="tex-span"><i>l</i></span> to position <span class="tex-span"><i>r</i></span>, inclusive. </li></ul>

## Output

<p>For each scientists' query (second type query) print a single integer in a new line&nbsp;— the value of impact of the infection on the DNA.</p>





```input1
ATGCATGC
4
2 1 8 ATGC
2 2 6 TTT
1 4 T
2 2 6 TA

```




```input2
GAGTTGTTAA
6
2 3 4 TATGGTG
1 1 T
1 6 G
2 5 9 AGTAATA
1 10 G
2 2 6 TTGT

```




```output1
8
2
4

```




```output2
0
3
1

```



## Note

<p>Consider the first example. In the first query of second type all characters coincide, so the answer is <span class="tex-span">8</span>. In the second query we compare string "<span class="tex-font-style-tt">TTTTT...</span>" and the substring "<span class="tex-font-style-tt">TGCAT</span>". There are two matches. In the third query, after the DNA change, we compare string "<span class="tex-font-style-tt">TATAT...</span>"' with substring "<span class="tex-font-style-tt">TGTAT</span>". There are <span class="tex-span">4</span> matches.</p>
