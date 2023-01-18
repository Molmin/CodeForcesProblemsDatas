## Description

<div><p>The Little Elephant has got a problem — somebody has been touching his sorted by non-decreasing array <span class="tex-span"><i>a</i></span> of length <span class="tex-span"><i>n</i></span> and possibly swapped some elements of the array.</p><p>The Little Elephant doesn't want to call the police until he understands if he could have accidentally changed the array himself. He thinks that he could have accidentally changed array <span class="tex-span"><i>a</i></span>, only if array <span class="tex-span"><i>a</i></span> can be sorted in no more than one operation of swapping elements (not necessarily adjacent). That is, the Little Elephant could have accidentally swapped some two elements.</p><p>Help the Little Elephant, determine if he could have accidentally changed the array <span class="tex-span"><i>a</i></span>, sorted by non-decreasing, himself.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the size of array <span class="tex-span"><i>a</i></span>. The next line contains <span class="tex-span"><i>n</i></span> positive integers, separated by single spaces and not exceeding <span class="tex-span">10<sup class="upper-index">9</sup></span>, — array <span class="tex-span"><i>a</i></span>.</p><p>Note that the elements of the array are not necessarily distinct numbers.</p></div><div class="output-specification"><p>In a single line print "<span class="tex-font-style-tt">YES</span>" (without the quotes) if the Little Elephant could have accidentally changed the array himself, and "<span class="tex-font-style-tt">NO</span>" (without the quotes) otherwise.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the size of array <span class="tex-span"><i>a</i></span>. The next line contains <span class="tex-span"><i>n</i></span> positive integers, separated by single spaces and not exceeding <span class="tex-span">10<sup class="upper-index">9</sup></span>, — array <span class="tex-span"><i>a</i></span>.</p><p>Note that the elements of the array are not necessarily distinct numbers.</p>

## Output

<p>In a single line print "<span class="tex-font-style-tt">YES</span>" (without the quotes) if the Little Elephant could have accidentally changed the array himself, and "<span class="tex-font-style-tt">NO</span>" (without the quotes) otherwise.</p>





```input1
2
1 2

```




```input2
3
3 2 1

```




```input3
4
4 3 2 1

```




```output1
YES

```




```output2
YES

```




```output3
NO

```



## Note

<p>In the first sample the array has already been sorted, so to sort it, we need 0 swap operations, that is not more than 1. Thus, the answer is "<span class="tex-font-style-tt">YES</span>".</p><p>In the second sample we can sort the array if we swap elements 1 and 3, so we need 1 swap operation to sort the array. Thus, the answer is "<span class="tex-font-style-tt">YES</span>".</p><p>In the third sample we can't sort the array in more than one swap operation, so the answer is "<span class="tex-font-style-tt">NO</span>".</p>
