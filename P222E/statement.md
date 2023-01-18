## Description

<div><p>Recently a top secret mission to Mars has taken place. As a result, scientists managed to obtain some information about the Martian DNA. Now we know that any Martian DNA contains at most <span class="tex-span"><i>m</i></span> different nucleotides, numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>. Special characteristics of the Martian DNA prevent some nucleotide pairs from following consecutively in this chain. For example, if the nucleotide 1 and nucleotide 2 can not follow consecutively in the Martian DNA, then the chain of nucleotides [1, 2] is not a valid chain of Martian DNA, but the chain of nucleotides [2, 1] can be a valid chain (if there is no corresponding restriction). The number of nucleotide pairs that can't follow in the DNA chain consecutively, is <span class="tex-span"><i>k</i></span>. </p><p>The needs of gene research required information about the quantity of correct <span class="tex-span"><i>n</i></span>-long chains of the Martian DNA. Your task is to write a program that will calculate this value.</p></div><div class="input-specification"><p>The first line contains three space-separated integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">15</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 52</span>, <span class="tex-span">0 ≤ <i>k</i> ≤ <i>m</i><sup class="upper-index">2</sup></span>).</p><p>Next <span class="tex-span"><i>k</i></span> lines contain two characters each, without a space between them, representing a forbidden nucleotide pair. The first character represents the first nucleotide in the forbidden pair, the second character represents the second nucleotide.</p><p>The nucleotides with assigned numbers from 1 to 26 are represented by English alphabet letters from "<span class="tex-font-style-tt">a</span>" to "<span class="tex-font-style-tt">z</span>" (1 is an "<span class="tex-font-style-tt">a</span>", 2 is a "<span class="tex-font-style-tt">b</span>", <span class="tex-span">...</span>, 26 is a "<span class="tex-font-style-tt">z</span>"). Nucleotides with assigned numbers from 27 to 52 are represented by English alphabet letters from "<span class="tex-font-style-tt">A</span>" to "<span class="tex-font-style-tt">Z</span>" (27 is an "<span class="tex-font-style-tt">A</span>", 28 is a "<span class="tex-font-style-tt">B</span>", <span class="tex-span">...</span>, 52 is a "<span class="tex-font-style-tt">Z</span>").</p><p>It is guaranteed that each forbidden pair occurs at most once in the input. It is guaranteed that nucleotide's numbers in all forbidden pairs cannot be more than <span class="tex-span"><i>m</i></span>. Note that order is important in nucleotide pairs.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div><div class="output-specification"><p>Print a single integer — the sought number modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The first line contains three space-separated integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">15</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 52</span>, <span class="tex-span">0 ≤ <i>k</i> ≤ <i>m</i><sup class="upper-index">2</sup></span>).</p><p>Next <span class="tex-span"><i>k</i></span> lines contain two characters each, without a space between them, representing a forbidden nucleotide pair. The first character represents the first nucleotide in the forbidden pair, the second character represents the second nucleotide.</p><p>The nucleotides with assigned numbers from 1 to 26 are represented by English alphabet letters from "<span class="tex-font-style-tt">a</span>" to "<span class="tex-font-style-tt">z</span>" (1 is an "<span class="tex-font-style-tt">a</span>", 2 is a "<span class="tex-font-style-tt">b</span>", <span class="tex-span">...</span>, 26 is a "<span class="tex-font-style-tt">z</span>"). Nucleotides with assigned numbers from 27 to 52 are represented by English alphabet letters from "<span class="tex-font-style-tt">A</span>" to "<span class="tex-font-style-tt">Z</span>" (27 is an "<span class="tex-font-style-tt">A</span>", 28 is a "<span class="tex-font-style-tt">B</span>", <span class="tex-span">...</span>, 52 is a "<span class="tex-font-style-tt">Z</span>").</p><p>It is guaranteed that each forbidden pair occurs at most once in the input. It is guaranteed that nucleotide's numbers in all forbidden pairs cannot be more than <span class="tex-span"><i>m</i></span>. Note that order is important in nucleotide pairs.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>

## Output

<p>Print a single integer — the sought number modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
3 3 2
ab
ba

```




```input2
3 3 0

```




```input3
2 1 1
aa

```




```output1
17

```




```output2
27

```




```output3
0

```



## Note

<p>In the second test case all possible three-nucleotide DNAs are permitted. Each nucleotide can take one of three values, thus in total there are 27 distinct three nucleotide DNAs.</p><p>In the third test sample we cannot make any DNA of two nucleotides — the only possible nucleotide "<span class="tex-font-style-tt">a</span>" cannot occur two times consecutively.</p>
