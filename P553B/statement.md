## Description

<div><p>Let's define the permutation of length <span class="tex-span"><i>n</i></span> as an array <span class="tex-span"><i>p</i> = [<i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub>]</span> consisting of <span class="tex-span"><i>n</i></span> distinct integers from range from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. We say that this permutation maps value <span class="tex-span">1</span> into the value <span class="tex-span"><i>p</i><sub class="lower-index">1</sub></span>, value <span class="tex-span">2</span> into the value <span class="tex-span"><i>p</i><sub class="lower-index">2</sub></span> and so on.</p><p>Kyota Ootori has just learned about <span class="tex-font-style-it">cyclic representation</span> of a permutation. A <span class="tex-font-style-it">cycle</span> is a sequence of numbers such that each element of this sequence is being mapped into the next element of this sequence (and the last element of the cycle is being mapped into the first element of the cycle). The <span class="tex-font-style-it">cyclic representation</span> is a representation of <span class="tex-span"><i>p</i></span> as a collection of cycles forming <span class="tex-span"><i>p</i></span>. For example, permutation <span class="tex-span"><i>p</i> = [4, 1, 6, 2, 5, 3]</span> has a <span class="tex-font-style-it">cyclic representation</span> that looks like <span class="tex-span">(142)(36)(5)</span> because 1 is replaced by 4, 4 is replaced by 2, 2 is replaced by 1, 3 and 6 are swapped, and 5 remains in place. </p><p>Permutation may have several cyclic representations, so Kyoya defines the <span class="tex-font-style-it">standard cyclic representation</span> of a permutation as follows. First, reorder the elements within each cycle so the largest element is first. Then, reorder all of the cycles so they are sorted by their first element. For our example above, the <span class="tex-font-style-it">standard cyclic representation</span> of <span class="tex-span">[4, 1, 6, 2, 5, 3]</span> is <span class="tex-span">(421)(5)(63)</span>.</p><p>Now, Kyoya notices that if we drop the parenthesis in the standard cyclic representation, we get another permutation! For instance, <span class="tex-span">[4, 1, 6, 2, 5, 3]</span> will become <span class="tex-span">[4, 2, 1, 5, 6, 3]</span>.</p><p>Kyoya notices that some permutations don't change after applying operation described above at all. He wrote all permutations of length <span class="tex-span"><i>n</i></span> that do not change in a list in lexicographic order. Unfortunately, his friend Tamaki Suoh lost this list. Kyoya wishes to reproduce the list and he needs your help. Given the integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span>, print the permutation that was <span class="tex-span"><i>k</i></span>-th on Kyoya's list.</p></div><div class="input-specification"><p>The first line will contain two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>min</i>{10<sup class="upper-index">18</sup>, <i>l</i>}</span> where <span class="tex-span"><i>l</i></span> is the length of the Kyoya's list).</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> space-separated integers, representing the permutation that is the answer for the question. </p></div>

## Input

<p>The first line will contain two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>min</i>{10<sup class="upper-index">18</sup>, <i>l</i>}</span> where <span class="tex-span"><i>l</i></span> is the length of the Kyoya's list).</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> space-separated integers, representing the permutation that is the answer for the question. </p>





```input1
4 3

```




```input2
10 1

```




```output1
1 3 2 4

```




```output2
1 2 3 4 5 6 7 8 9 10

```



## Note

<p>The standard cycle representation is <span class="tex-span">(1)(32)(4)</span>, which after removing parenthesis gives us the original permutation. The first permutation on the list would be <span class="tex-span">[1, 2, 3, 4]</span>, while the second permutation would be <span class="tex-span">[1, 2, 4, 3]</span>.</p>
