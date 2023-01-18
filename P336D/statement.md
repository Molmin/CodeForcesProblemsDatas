## Description

<div><p>Vasily the Bear loves <span class="tex-font-style-it">beautiful</span> strings. String <span class="tex-span"><i>s</i></span> is <span class="tex-font-style-it">beautiful</span> if it meets the following criteria: </p><ol> <li> String <span class="tex-span"><i>s</i></span> only consists of characters <span class="tex-span">0</span> and <span class="tex-span">1</span>, at that character <span class="tex-span">0</span> must occur in string <span class="tex-span"><i>s</i></span> exactly <span class="tex-span"><i>n</i></span> times, and character <span class="tex-span">1</span> must occur exactly <span class="tex-span"><i>m</i></span> times. </li><li> We can obtain character <span class="tex-span"><i>g</i></span> from string <span class="tex-span"><i>s</i></span> with some (possibly, zero) number of modifications. The character <span class="tex-span"><i>g</i></span> equals either zero or one. </li></ol><p>A <span class="tex-font-style-it">modification</span> of string with length at least two is the following operation: we replace two last characters from the string by exactly one other character. This character equals one if it replaces two zeros, otherwise it equals zero. For example, one modification transforms string "01010" into string "0100", two modifications transform it to "011". It is forbidden to modify a string with length less than two.</p><p>Help the Bear, count the number of <span class="tex-font-style-it">beautiful</span> strings. As the number of beautiful strings can be rather large, print the remainder after dividing the number by <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>. </p></div><div class="input-specification"><p>The first line of the input contains three space-separated integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>g</i></span> <span class="tex-span">(0 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>, <i>n</i> + <i>m</i> ≥ 1, 0 ≤ <i>g</i> ≤ 1)</span>.</p></div><div class="output-specification"><p>Print a single integer — the answer to the problem modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The first line of the input contains three space-separated integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>g</i></span> <span class="tex-span">(0 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>, <i>n</i> + <i>m</i> ≥ 1, 0 ≤ <i>g</i> ≤ 1)</span>.</p>

## Output

<p>Print a single integer — the answer to the problem modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
1 1 0

```




```input2
2 2 0

```




```input3
1 1 1

```




```output1
2

```




```output2
4

```




```output3
0

```



## Note

<p>In the first sample the beautiful strings are: "01", "10".</p><p>In the second sample the beautiful strings are: "0011", "1001", "1010", "1100".</p><p>In the third sample there are no beautiful strings.</p>
