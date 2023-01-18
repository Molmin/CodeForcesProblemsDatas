## Description

<div><p>Happy PMP is freshman and he is learning about algorithmic problems. He enjoys playing algorithmic games a lot.</p><p>One of the seniors gave Happy PMP a nice game. He is given two permutations of numbers <span class="tex-span">1</span> through <span class="tex-span"><i>n</i></span> and is asked to convert the first one to the second. In one move he can remove the last number from the permutation of numbers and inserts it back in an arbitrary position. He can either insert last number between any two consecutive numbers, or he can place it at the beginning of the permutation.</p><p>Happy PMP has an algorithm that solves the problem. But it is not fast enough. He wants to know the minimum number of moves to convert the first permutation to the second. </p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the quantity of the numbers in the both given permutations. </p><p>Next line contains <span class="tex-span"><i>n</i></span> space-separated integers — the first permutation. Each number between <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> will appear in the permutation exactly once. </p><p>Next line describe the second permutation in the same format.</p></div><div class="output-specification"><p>Print a single integer denoting the minimum number of moves required to convert the first permutation to the second.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the quantity of the numbers in the both given permutations. </p><p>Next line contains <span class="tex-span"><i>n</i></span> space-separated integers — the first permutation. Each number between <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> will appear in the permutation exactly once. </p><p>Next line describe the second permutation in the same format.</p>

## Output

<p>Print a single integer denoting the minimum number of moves required to convert the first permutation to the second.</p>





```input1
3
3 2 1
1 2 3

```




```input2
5
1 2 3 4 5
1 5 2 3 4

```




```input3
5
1 5 2 3 4
1 2 3 4 5

```




```output1
2

```




```output2
1

```




```output3
3

```



## Note

<p>In the first sample, he removes number 1 from end of the list and places it at the beginning. After that he takes number 2 and places it between 1 and 3.</p><p>In the second sample, he removes number 5 and inserts it after 1.</p><p>In the third sample, the sequence of changes are like this: </p><ul> <li>1 5 2 3 4 </li><li>1 4 5 2 3 </li><li>1 3 4 5 2 </li><li>1 2 3 4 5 </li></ul> So he needs three moves.
