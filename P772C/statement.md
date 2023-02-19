## Description

<div><p>You are given an integer <span class="tex-span"><i>m</i></span>, and a list of <span class="tex-span"><i>n</i></span> distinct integers between <span class="tex-span">0</span> and <span class="tex-span"><i>m</i> - 1</span>.</p><p>You would like to construct a sequence satisfying the properties:</p><ul> <li> Each element is an integer between <span class="tex-span">0</span> and <span class="tex-span"><i>m</i> - 1</span>, inclusive. </li><li> All prefix products of the sequence modulo <span class="tex-span"><i>m</i></span> are distinct. </li><li> No prefix product modulo <span class="tex-span"><i>m</i></span> appears as an element of the input list. </li><li> The length of the sequence is maximized. </li></ul><p>Construct any sequence satisfying the properties above.</p></div><div class="input-specification"><p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">0 ≤ <i>n</i> &lt; <i>m</i> ≤ 200 000</span>)&nbsp;— the number of forbidden prefix products and the modulus.</p><p>If <span class="tex-span"><i>n</i></span> is non-zero, the next line of input contains <span class="tex-span"><i>n</i></span> distinct integers between <span class="tex-span">0</span> and <span class="tex-span"><i>m</i> - 1</span>, the forbidden prefix products. If <span class="tex-span"><i>n</i></span> is zero, this line doesn't exist.</p></div><div class="output-specification"><p>On the first line, print the number <span class="tex-span"><i>k</i></span>, denoting the length of your sequence.</p><p>On the second line, print <span class="tex-span"><i>k</i></span> space separated integers, denoting your sequence.</p></div>

## Input

<p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">0 ≤ <i>n</i> &lt; <i>m</i> ≤ 200 000</span>)&nbsp;— the number of forbidden prefix products and the modulus.</p><p>If <span class="tex-span"><i>n</i></span> is non-zero, the next line of input contains <span class="tex-span"><i>n</i></span> distinct integers between <span class="tex-span">0</span> and <span class="tex-span"><i>m</i> - 1</span>, the forbidden prefix products. If <span class="tex-span"><i>n</i></span> is zero, this line doesn't exist.</p>

## Output

<p>On the first line, print the number <span class="tex-span"><i>k</i></span>, denoting the length of your sequence.</p><p>On the second line, print <span class="tex-span"><i>k</i></span> space separated integers, denoting your sequence.</p>





```input1
0 5

```




```input2
3 10
2 9 1

```




```output1
5
1 2 4 3 0

```




```output2
6
3 9 2 9 8 0

```



## Note

<p>For the first case, the prefix products of this sequence modulo <span class="tex-span"><i>m</i></span> are <span class="tex-span">[1, 2, 3, 4, 0]</span>.</p><p>For the second case, the prefix products of this sequence modulo <span class="tex-span"><i>m</i></span> are <span class="tex-span">[3, 7, 4, 6, 8, 0]</span>.</p>
