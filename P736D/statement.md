## Description

<div><p>Ostap Bender is worried that people started to forget that he is the Great Combinator. Now he wants to show them his skills in combinatorics. Now he studies the permutations of length <span class="tex-span"><i>n</i></span>. He has a list of <span class="tex-span"><i>m</i></span> valid pairs, pair <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> means that he is allowed to place integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> at position <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>He knows that the number of permutations that use only valid pairs is <span class="tex-font-style-bf">odd</span>. Now, for each pair he wants to find out, will the number of valid permutations be <span class="tex-font-style-bf">odd</span> if he <span class="tex-font-style-bf">removes</span> this pair (and only it) from the list.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2000</span>, <span class="tex-span"><i>n</i> ≤ <i>m</i> ≤ <i>min</i>(<i>n</i><sup class="upper-index">2</sup>, 500 000)</span>)&nbsp;— the number of elements in the permutation. Then follow <span class="tex-span"><i>m</i></span> lines, each containing some valid pair <span class="tex-span">(<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>)</span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>). It's guaranteed that no pair occurs in the input twice and that the total number of valid permutations (i.e. using only allowed pairs position-elements) is odd.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> lines, one line for each valid pair. The <span class="tex-span"><i>i</i></span>-th line should contain "<span class="tex-font-style-tt">YES</span>" if after Ostap removes the <span class="tex-span"><i>i</i></span>-th pair (and only it) the remaining number of valid permutations is odd. Otherwise, print «<span class="tex-font-style-tt">NO</span>».</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2000</span>, <span class="tex-span"><i>n</i> ≤ <i>m</i> ≤ <i>min</i>(<i>n</i><sup class="upper-index">2</sup>, 500 000)</span>)&nbsp;— the number of elements in the permutation. Then follow <span class="tex-span"><i>m</i></span> lines, each containing some valid pair <span class="tex-span">(<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>)</span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>). It's guaranteed that no pair occurs in the input twice and that the total number of valid permutations (i.e. using only allowed pairs position-elements) is odd.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> lines, one line for each valid pair. The <span class="tex-span"><i>i</i></span>-th line should contain "<span class="tex-font-style-tt">YES</span>" if after Ostap removes the <span class="tex-span"><i>i</i></span>-th pair (and only it) the remaining number of valid permutations is odd. Otherwise, print «<span class="tex-font-style-tt">NO</span>».</p>





```input1
2 3
1 1
1 2
2 2

```




```input2
3 3
1 1
2 2
3 3

```




```input3
3 7
3 3
3 1
1 3
1 1
2 2
1 2
2 1

```




```output1
NO
YES
NO

```




```output2
NO
NO
NO

```




```output3
YES
NO
NO
NO
YES
NO
NO

```


