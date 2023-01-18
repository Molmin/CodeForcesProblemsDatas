## Description

<div><p><span class="tex-font-style-it">You will receive 3 points for solving this problem.</span></p><p>Manao is designing the genetic code for a new type of algae to efficiently produce fuel. Specifically, Manao is focusing on a stretch of DNA that encodes one protein. The stretch of DNA is represented by a string containing only the characters '<span class="tex-font-style-tt">A</span>', '<span class="tex-font-style-tt">T</span>', '<span class="tex-font-style-tt">G</span>' and '<span class="tex-font-style-tt">C</span>'.</p><p>Manao has determined that if the stretch of DNA contains a maximal sequence of consecutive identical nucleotides that is of even length, then the protein will be nonfunctional. For example, consider a protein described by DNA string "<span class="tex-font-style-tt">GTTAAAG</span>". It contains four maximal sequences of consecutive identical nucleotides: "<span class="tex-font-style-tt">G</span>", "<span class="tex-font-style-tt">TT</span>", "<span class="tex-font-style-tt">AAA</span>", and "<span class="tex-font-style-tt">G</span>". The protein is nonfunctional because sequence "<span class="tex-font-style-tt">TT</span>" has even length.</p><p>Manao is trying to obtain a functional protein from the protein he currently has. Manao can insert additional nucleotides into the DNA stretch. Each additional nucleotide is a character from the set {'<span class="tex-font-style-tt">A</span>', '<span class="tex-font-style-tt">T</span>', '<span class="tex-font-style-tt">G</span>', '<span class="tex-font-style-tt">C</span>'}. Manao wants to determine the minimum number of insertions necessary to make the DNA encode a functional protein.</p></div><div class="input-specification"><p>The input consists of a single line, containing a string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 100)</span>. Each character of <span class="tex-span"><i>s</i></span> will be from the set {'<span class="tex-font-style-tt">A</span>', '<span class="tex-font-style-tt">T</span>', '<span class="tex-font-style-tt">G</span>', '<span class="tex-font-style-tt">C</span>'}.</p><p><span class="tex-font-style-it">This problem doesn't have subproblems. You will get 3 points for the correct submission.</span></p></div><div class="output-specification"><p>The program should print on one line a single integer representing the minimum number of '<span class="tex-font-style-tt">A</span>', '<span class="tex-font-style-tt">T</span>', '<span class="tex-font-style-tt">G</span>', '<span class="tex-font-style-tt">C</span>' characters that are required to be inserted into the input string in order to make all runs of identical characters have odd length.</p></div>

## Input

<p>The input consists of a single line, containing a string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 100)</span>. Each character of <span class="tex-span"><i>s</i></span> will be from the set {'<span class="tex-font-style-tt">A</span>', '<span class="tex-font-style-tt">T</span>', '<span class="tex-font-style-tt">G</span>', '<span class="tex-font-style-tt">C</span>'}.</p><p><span class="tex-font-style-it">This problem doesn't have subproblems. You will get 3 points for the correct submission.</span></p>

## Output

<p>The program should print on one line a single integer representing the minimum number of '<span class="tex-font-style-tt">A</span>', '<span class="tex-font-style-tt">T</span>', '<span class="tex-font-style-tt">G</span>', '<span class="tex-font-style-tt">C</span>' characters that are required to be inserted into the input string in order to make all runs of identical characters have odd length.</p>





```input1
GTTAAAG

```




```input2
AACCAACCAAAAC

```




```output1
1

```




```output2
5

```



## Note

<p>In the first example, it is sufficient to insert a single nucleotide of any type between the two '<span class="tex-font-style-tt">T</span>'s in the sequence to restore the functionality of the protein.</p>
