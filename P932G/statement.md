## Description

<div><p>Given a string <span class="tex-span"><i>s</i></span>, find the number of ways to split <span class="tex-span"><i>s</i></span> to substrings such that if there are <span class="tex-span"><i>k</i></span> substrings <span class="tex-span">(<i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, <i>p</i><sub class="lower-index">3</sub>, ..., <i>p</i><sub class="lower-index"><i>k</i></sub>)</span> in partition, then <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> = <i>p</i><sub class="lower-index"><i>k</i> - <i>i</i> + 1</sub></span> for all <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>k</i>)</span> and <span class="tex-span"><i>k</i></span> is even.</p><p>Since the number of ways can be large, print it modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The only line of input contains a string <span class="tex-span"><i>s</i></span> <span class="tex-span">(2 ≤ |<i>s</i>| ≤ 10<sup class="upper-index">6</sup>)</span> of even length consisting of lowercase Latin letters. </p></div><div class="output-specification"><p>Print one integer, the number of ways of partitioning the string modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The only line of input contains a string <span class="tex-span"><i>s</i></span> <span class="tex-span">(2 ≤ |<i>s</i>| ≤ 10<sup class="upper-index">6</sup>)</span> of even length consisting of lowercase Latin letters. </p>

## Output

<p>Print one integer, the number of ways of partitioning the string modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
abcdcdab

```




```input2
abbababababbab

```




```output1
1
```




```output2
3
```



## Note

<p>In the first case, the only way to partition the string is <span class="tex-span"><i>ab</i>|<i>cd</i>|<i>cd</i>|<i>ab</i></span>.</p><p>In the second case, the string can be partitioned as <span class="tex-span"><i>ab</i>|<i>b</i>|<i>ab</i>|<i>ab</i>|<i>ab</i>|<i>ab</i>|<i>b</i>|<i>ab</i></span> or <span class="tex-span"><i>ab</i>|<i>b</i>|<i>abab</i>|<i>abab</i>|<i>b</i>|<i>ab</i></span> or <span class="tex-span"><i>abbab</i>|<i>ab</i>|<i>ab</i>|<i>abbab</i></span>.</p>
