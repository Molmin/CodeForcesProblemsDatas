## Description

<div><p><span class="tex-font-style-underline">Petya loves lucky numbers. Everybody knows that lucky numbers are positive integers whose decimal representation contains only the lucky digits <span class="tex-font-style-bf">4</span> and <span class="tex-font-style-bf">7</span>. For example, numbers <span class="tex-font-style-bf">47</span>, <span class="tex-font-style-bf">744</span>, <span class="tex-font-style-bf">4</span> are lucky and <span class="tex-font-style-bf">5</span>, <span class="tex-font-style-bf">17</span>, <span class="tex-font-style-bf">467</span> are not.</span></p><p>One day Petya dreamt of a lexicographically <span class="tex-span"><i>k</i></span>-th permutation of integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Determine how many lucky numbers in the permutation are located on the positions whose indexes are also lucky numbers.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>k</i> ≤ 10<sup class="upper-index">9</sup>)</span> — the number of elements in the permutation and the lexicographical number of the permutation.</p></div><div class="output-specification"><p>If the <span class="tex-span"><i>k</i></span>-th permutation of numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> does not exist, print the single number "-1" (without the quotes). Otherwise, print the answer to the problem: the number of such indexes <span class="tex-span"><i>i</i></span>, that <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> are both lucky numbers.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>k</i> ≤ 10<sup class="upper-index">9</sup>)</span> — the number of elements in the permutation and the lexicographical number of the permutation.</p>

## Output

<p>If the <span class="tex-span"><i>k</i></span>-th permutation of numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> does not exist, print the single number "-1" (without the quotes). Otherwise, print the answer to the problem: the number of such indexes <span class="tex-span"><i>i</i></span>, that <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> are both lucky numbers.</p>





```input1
7 4

```




```input2
4 7

```




```output1
1

```




```output2
1

```



## Note

<p>A permutation is an ordered set of <span class="tex-span"><i>n</i></span> elements, where each integer from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> occurs exactly once. The element of permutation in position with index <span class="tex-span"><i>i</i></span> is denoted as <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>). Permutation <span class="tex-span"><i>a</i></span> is lexicographically smaller that permutation <span class="tex-span"><i>b</i></span> if there is such a <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>), that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>i</i></sub></span>, and for any <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>j</i> &lt; <i>i</i></span>) <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub> = <i>b</i><sub class="lower-index"><i>j</i></sub></span>. Let's make a list of all possible permutations of <span class="tex-span"><i>n</i></span> elements and sort it in the order of lexicographical increasing. Then the lexicographically <span class="tex-span"><i>k</i></span>-th permutation is the <span class="tex-span"><i>k</i></span>-th element of this list of permutations.</p><p>In the first sample the permutation looks like that:</p><p><span class="tex-font-style-tt">1 2 3 4 6 7 5</span></p><p>The only suitable position is 4.</p><p>In the second sample the permutation looks like that:</p><p><span class="tex-font-style-tt">2 1 3 4</span></p><p>The only suitable position is 4.</p>
