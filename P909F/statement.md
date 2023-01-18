## Description

<div><p>Given an integer <span class="tex-span"><i>N</i></span>, find two permutations:</p><ol> <li> Permutation <span class="tex-span"><i>p</i></span> of numbers from 1 to <span class="tex-span"><i>N</i></span> such that <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> ≠ <i>i</i></span> and <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> &amp; <i>i</i> = 0</span> for all <span class="tex-span"><i>i</i> = 1, 2, ..., <i>N</i></span>. </li><li> Permutation <span class="tex-span"><i>q</i></span> of numbers from 1 to <span class="tex-span"><i>N</i></span> such that <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub> ≠ <i>i</i></span> and <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub> &amp; <i>i</i> ≠ 0</span> for all <span class="tex-span"><i>i</i> = 1, 2, ..., <i>N</i></span>. </li></ol><p><span class="tex-span">&amp;</span> is the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#AND">bitwise AND operation</a>.</p></div><div class="input-specification"><p>The input consists of one line containing a single integer <span class="tex-span"><i>N</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤ 10<sup class="upper-index">5</sup></span>).</p></div><div class="output-specification"><p>For each subtask, if the required permutation doesn't exist, output a single line containing the word "<span class="tex-font-style-tt">NO</span>"; otherwise output the word "<span class="tex-font-style-tt">YES</span>" in the first line and <span class="tex-span"><i>N</i></span> elements of the permutation, separated by spaces, in the second line. If there are several possible permutations in a subtask, output any of them.</p></div>

## Input

<p>The input consists of one line containing a single integer <span class="tex-span"><i>N</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤ 10<sup class="upper-index">5</sup></span>).</p>

## Output

<p>For each subtask, if the required permutation doesn't exist, output a single line containing the word "<span class="tex-font-style-tt">NO</span>"; otherwise output the word "<span class="tex-font-style-tt">YES</span>" in the first line and <span class="tex-span"><i>N</i></span> elements of the permutation, separated by spaces, in the second line. If there are several possible permutations in a subtask, output any of them.</p>





```input1
3

```




```input2
6

```




```output1
NO
NO

```




```output2
YES
6 5 4 3 2 1 
YES
3 6 2 5 1 4

```


