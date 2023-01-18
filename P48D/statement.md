## Description

<div><p>A permutation is a sequence of integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> of length <span class="tex-span"><i>n</i></span> containing each number exactly once. For example, <span class="tex-span">(1)</span>, <span class="tex-span">(4, 3, 5, 1, 2)</span>, <span class="tex-span">(3, 2, 1)</span> are permutations, and <span class="tex-span">(1, 1)</span>, <span class="tex-span">(4, 3, 1)</span>, <span class="tex-span">(2, 3, 4)</span> are not. </p><p>There are many tasks on permutations. Today you are going to solve one of them. Let’s imagine that somebody took several permutations (perhaps, with a different number of elements), wrote them down consecutively as one array and then shuffled the resulting array. The task is to restore the initial permutations if it is possible.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). The next line contains the mixed array of <span class="tex-span"><i>n</i></span> integers, divided with a single space. The numbers in the array are from <span class="tex-span">1</span> to <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p></div><div class="output-specification"><p>If this array can be split into several permutations so that every element of the array belongs to exactly one permutation, print in the first line the number of permutations. The second line should contain <span class="tex-span"><i>n</i></span> numbers, corresponding to the elements of the given array. If the <span class="tex-span"><i>i</i></span>-th element belongs to the first permutation, the <span class="tex-span"><i>i</i></span>-th number should be <span class="tex-span">1</span>, if it belongs to the second one, then its number should be <span class="tex-span">2</span> and so on. The order of the permutations’ numbering is free.</p><p>If several solutions are possible, print any one of them. If there’s no solution, print in the first line <span class="tex-span"> - 1</span>.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). The next line contains the mixed array of <span class="tex-span"><i>n</i></span> integers, divided with a single space. The numbers in the array are from <span class="tex-span">1</span> to <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p>

## Output

<p>If this array can be split into several permutations so that every element of the array belongs to exactly one permutation, print in the first line the number of permutations. The second line should contain <span class="tex-span"><i>n</i></span> numbers, corresponding to the elements of the given array. If the <span class="tex-span"><i>i</i></span>-th element belongs to the first permutation, the <span class="tex-span"><i>i</i></span>-th number should be <span class="tex-span">1</span>, if it belongs to the second one, then its number should be <span class="tex-span">2</span> and so on. The order of the permutations’ numbering is free.</p><p>If several solutions are possible, print any one of them. If there’s no solution, print in the first line <span class="tex-span"> - 1</span>.</p>





```input1
9
1 2 3 1 2 1 4 2 5

```




```input2
4
4 3 2 1

```




```input3
4
1 2 2 3

```




```output1
3
3 1 2 1 2 2 2 3 2

```




```output2
1
1 1 1 1
```




```output3
-1

```



## Note

<p>In the first sample test the array is split into three permutations: <span class="tex-span">(2, 1)</span>, <span class="tex-span">(3, 2, 1, 4, 5)</span>, <span class="tex-span">(1, 2)</span>. The first permutation is formed by the second and the fourth elements of the array, the second one — by the third, the fifth, the sixth, the seventh and the ninth elements, the third one — by the first and the eigth elements. Clearly, there are other splitting variants possible. </p>
