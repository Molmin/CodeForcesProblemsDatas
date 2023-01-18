## Description

<div><p><span class="tex-font-style-underline">Petya loves lucky numbers. We all know that lucky numbers are the positive integers whose decimal representations contain only the lucky digits <span class="tex-font-style-bf">4</span> and <span class="tex-font-style-bf">7</span>. For example, numbers <span class="tex-font-style-bf">47</span>, <span class="tex-font-style-bf">744</span>, <span class="tex-font-style-bf">4</span> are lucky and <span class="tex-font-style-bf">5</span>, <span class="tex-font-style-bf">17</span>, <span class="tex-font-style-bf">467</span> are not.</span></p><p>Petya got an array consisting of <span class="tex-span"><i>n</i></span> numbers, it is the gift for his birthday. Now he wants to sort it in the non-decreasing order. However, a usual sorting is boring to perform, that's why Petya invented the following limitation: one can swap any two numbers but only if at least one of them is lucky. Your task is to sort the array according to the specified limitation. Find any possible sequence of the swaps (the number of operations in the sequence should not exceed <span class="tex-span">2<i>n</i></span>).</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of elements in the array. The second line contains <span class="tex-span"><i>n</i></span> positive integers, not exceeding <span class="tex-span">10<sup class="upper-index">9</sup></span> — the array that needs to be sorted in the non-decreasing order.</p></div><div class="output-specification"><p>On the first line print number <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 2<i>n</i></span>) — the number of the swaps in the sorting. On the following <span class="tex-span"><i>k</i></span> lines print one pair of <span class="tex-font-style-bf">distinct</span> numbers (a pair per line) — the indexes of elements to swap. The numbers in the array are numbered starting from 1. If it is impossible to sort the given sequence, print the single number -1.</p><p>If there are several solutions, output any. Note that you don't have to minimize <span class="tex-span"><i>k</i></span>. Any sorting with no more than <span class="tex-span">2<i>n</i></span> swaps is accepted.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of elements in the array. The second line contains <span class="tex-span"><i>n</i></span> positive integers, not exceeding <span class="tex-span">10<sup class="upper-index">9</sup></span> — the array that needs to be sorted in the non-decreasing order.</p>

## Output

<p>On the first line print number <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 2<i>n</i></span>) — the number of the swaps in the sorting. On the following <span class="tex-span"><i>k</i></span> lines print one pair of <span class="tex-font-style-bf">distinct</span> numbers (a pair per line) — the indexes of elements to swap. The numbers in the array are numbered starting from 1. If it is impossible to sort the given sequence, print the single number -1.</p><p>If there are several solutions, output any. Note that you don't have to minimize <span class="tex-span"><i>k</i></span>. Any sorting with no more than <span class="tex-span">2<i>n</i></span> swaps is accepted.</p>





```input1
2
4 7

```




```input2
3
4 2 1

```




```input3
7
77 66 55 44 33 22 11

```




```output1
0

```




```output2
1
1 3

```




```output3
7
1 7
7 2
2 6
6 7
3 4
5 3
4 5

```


