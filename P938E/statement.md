## Description

<div><p>You are given an array <span class="tex-span"><i>a</i></span> of length <span class="tex-span"><i>n</i></span>. We define <span class="tex-span"><i>f</i><sub class="lower-index"><i>a</i></sub></span> the following way:</p><ul> <li> Initially <span class="tex-span"><i>f</i><sub class="lower-index"><i>a</i></sub> = 0</span>, <span class="tex-span"><i>M</i> = 1</span>; </li><li> for every <span class="tex-span">2 ≤ <i>i</i> ≤ <i>n</i></span> if <span class="tex-span"><i>a</i><sub class="lower-index"><i>M</i></sub> &lt; <i>a</i><sub class="lower-index"><i>i</i></sub></span> then we set <span class="tex-span"><i>f</i><sub class="lower-index"><i>a</i></sub> = <i>f</i><sub class="lower-index"><i>a</i></sub> + <i>a</i><sub class="lower-index"><i>M</i></sub></span> and then set <span class="tex-span"><i>M</i> = <i>i</i></span>. </li></ul><p>Calculate the sum of <span class="tex-span"><i>f</i><sub class="lower-index"><i>a</i></sub></span> over all <span class="tex-span"><i>n</i>!</span> permutations of the array <span class="tex-span"><i>a</i></span> modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p><p>Note: two elements are considered different if their indices differ, so for every array <span class="tex-span"><i>a</i></span> there are exactly <span class="tex-span"><i>n</i>!</span> permutations.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤  1 000 000</span>) — the size of array <span class="tex-span"><i>a</i></span>.</p><p>Second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤  <i>a</i><sub class="lower-index"><i>i</i></sub> ≤  10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Print the only integer, the sum of <span class="tex-span"><i>f</i><sub class="lower-index"><i>a</i></sub></span> over all <span class="tex-span"><i>n</i>!</span> permutations of the array <span class="tex-span"><i>a</i></span> modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤  1 000 000</span>) — the size of array <span class="tex-span"><i>a</i></span>.</p><p>Second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤  <i>a</i><sub class="lower-index"><i>i</i></sub> ≤  10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Print the only integer, the sum of <span class="tex-span"><i>f</i><sub class="lower-index"><i>a</i></sub></span> over all <span class="tex-span"><i>n</i>!</span> permutations of the array <span class="tex-span"><i>a</i></span> modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
2
1 3

```




```input2
3
1 1 2

```




```output1
1
```




```output2
4
```



## Note

<p>For the second example all the permutations are:</p><ul> <li> <span class="tex-span"><i>p</i> = [1, 2, 3]</span> : <span class="tex-span"><i>f</i><sub class="lower-index"><i>a</i></sub></span> is equal to <span class="tex-span">1</span>; </li><li> <span class="tex-span"><i>p</i> = [1, 3, 2]</span> : <span class="tex-span"><i>f</i><sub class="lower-index"><i>a</i></sub></span> is equal to <span class="tex-span">1</span>; </li><li> <span class="tex-span"><i>p</i> = [2, 1, 3]</span> : <span class="tex-span"><i>f</i><sub class="lower-index"><i>a</i></sub></span> is equal to <span class="tex-span">1</span>; </li><li> <span class="tex-span"><i>p</i> = [2, 3, 1]</span> : <span class="tex-span"><i>f</i><sub class="lower-index"><i>a</i></sub></span> is equal to <span class="tex-span">1</span>; </li><li> <span class="tex-span"><i>p</i> = [3, 1, 2]</span> : <span class="tex-span"><i>f</i><sub class="lower-index"><i>a</i></sub></span> is equal to <span class="tex-span">0</span>; </li><li> <span class="tex-span"><i>p</i> = [3, 2, 1]</span> : <span class="tex-span"><i>f</i><sub class="lower-index"><i>a</i></sub></span> is equal to <span class="tex-span">0</span>. </li></ul><p>Where <span class="tex-span"><i>p</i></span> is the array of the indices of initial array <span class="tex-span"><i>a</i></span>. The sum of <span class="tex-span"><i>f</i><sub class="lower-index"><i>a</i></sub></span> is equal to <span class="tex-span">4</span>.</p>
