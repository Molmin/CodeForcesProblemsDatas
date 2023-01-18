## Description

<div><p>Professor Bajtocy is conducting experiments on alien DNA. He has discovered that it is subject to repetitive mutations — each mutation happens in the same way: some continuous subsequence of the alien DNA becomes active, copies itself, the copy gets mangled and inserts itself right after the original subsequence. The mangled copy of the activated continuous subsequence is formed by first joining all the elements at the even positions in that subsequence, and then joining all the elements at the odd ones at the end. That is, if the activated subsequence consists of 11 elements and represented as <span class="tex-span"><i>s</i><sub class="lower-index">1</sub><i>s</i><sub class="lower-index">2</sub>... <i>s</i><sub class="lower-index">11</sub></span>, its mangled copy is <span class="tex-span"><i>s</i><sub class="lower-index">2</sub><i>s</i><sub class="lower-index">4</sub><i>s</i><sub class="lower-index">6</sub><i>s</i><sub class="lower-index">8</sub><i>s</i><sub class="lower-index">10</sub><i>s</i><sub class="lower-index">1</sub><i>s</i><sub class="lower-index">3</sub><i>s</i><sub class="lower-index">5</sub><i>s</i><sub class="lower-index">7</sub><i>s</i><sub class="lower-index">9</sub><i>s</i><sub class="lower-index">11</sub></span>.</p><p>For example, if the original sequence was "<span class="tex-font-style-tt">ACTGG</span>" and the mutation happened on the segment <span class="tex-span">[2, 4]</span> (that is the activated subsequence is "<span class="tex-font-style-tt">CTG</span>"), the mutated DNA is: "<span class="tex-font-style-tt">ACTG<span class="tex-font-style-bf">TCG</span>G</span>". The mangled copy of the activated subsequence is marked with bold font.</p><p>Professor Bajtocy has written down the original DNA sequence and the mutations that sequentially happened to it, and he now asks you to recover the first <span class="tex-span"><i>k</i></span> elements of the DNA sequence after all the mutations.</p></div><div class="input-specification"><p>The first line of input contains the original DNA sequence, consisting only of letters "<span class="tex-font-style-tt">A</span>", "<span class="tex-font-style-tt">C</span>", "<span class="tex-font-style-tt">T</span>" and "<span class="tex-font-style-tt">G</span>" and not exceeding <span class="tex-span">3·10<sup class="upper-index">6</sup></span> in length. </p><p>The second line contains a single integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 3·10<sup class="upper-index">6</sup></span>).</p><p>The third line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 5000</span>) — the number of mutations. The next <span class="tex-span"><i>n</i></span> lines describe the mutations in chronological order — each mutation is described by two numbers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), meaning that the continuous subsequence <span class="tex-span">[<i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>]</span> has become active and cloned itself, joining itself with the mangled copy. </p><p>It is guaranteed that the input data is correct, that is, no mutation acts on non-existing elements of the DNA sequence, and the resulting DNA sequence has at least <span class="tex-span"><i>k</i></span> elements.</p><p>Assume that the DNA elements are indexed starting from 1 and that the notation <span class="tex-span">[<i>l</i>, <i>r</i>]</span> meaning the continuous subsequence of DNA sequence that consists of <span class="tex-span"><i>r</i> - <i>l</i> + 1</span> elements starting at the <span class="tex-span"><i>l</i></span>-th DNA sequence element and ending at the <span class="tex-span"><i>r</i></span>-th DNA sequence element.</p></div><div class="output-specification"><p>Output a single line, containing the first <span class="tex-span"><i>k</i></span> letters of the mutated DNA sequence.</p></div>

## Input

<p>The first line of input contains the original DNA sequence, consisting only of letters "<span class="tex-font-style-tt">A</span>", "<span class="tex-font-style-tt">C</span>", "<span class="tex-font-style-tt">T</span>" and "<span class="tex-font-style-tt">G</span>" and not exceeding <span class="tex-span">3·10<sup class="upper-index">6</sup></span> in length. </p><p>The second line contains a single integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 3·10<sup class="upper-index">6</sup></span>).</p><p>The third line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 5000</span>) — the number of mutations. The next <span class="tex-span"><i>n</i></span> lines describe the mutations in chronological order — each mutation is described by two numbers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), meaning that the continuous subsequence <span class="tex-span">[<i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>]</span> has become active and cloned itself, joining itself with the mangled copy. </p><p>It is guaranteed that the input data is correct, that is, no mutation acts on non-existing elements of the DNA sequence, and the resulting DNA sequence has at least <span class="tex-span"><i>k</i></span> elements.</p><p>Assume that the DNA elements are indexed starting from 1 and that the notation <span class="tex-span">[<i>l</i>, <i>r</i>]</span> meaning the continuous subsequence of DNA sequence that consists of <span class="tex-span"><i>r</i> - <i>l</i> + 1</span> elements starting at the <span class="tex-span"><i>l</i></span>-th DNA sequence element and ending at the <span class="tex-span"><i>r</i></span>-th DNA sequence element.</p>

## Output

<p>Output a single line, containing the first <span class="tex-span"><i>k</i></span> letters of the mutated DNA sequence.</p>





```input1
GAGA
4
0

```




```input2
ACGTACGT
16
2
1 2
2 8

```




```output1
GAGA

```




```output2
ACCAGTACCGACATCG

```



## Note

<p>In the second example, after the first mutation the sequence is "<span class="tex-font-style-tt">ACCAGTACGT</span>". After the second mutation it's "<span class="tex-font-style-tt">ACCAGTACCGACATCGT</span>".</p>
