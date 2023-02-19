## Description

<div><p>You are given two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span>. Find <span class="tex-span"><i>k</i></span>-th smallest divisor of <span class="tex-span"><i>n</i></span>, or report that it doesn't exist.</p><p>Divisor of <span class="tex-span"><i>n</i></span> is any such natural number, that <span class="tex-span"><i>n</i></span> can be divided by it without remainder.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">15</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>If <span class="tex-span"><i>n</i></span> has less than <span class="tex-span"><i>k</i></span> divisors, output <span class="tex-font-style-tt">-1</span>.</p><p>Otherwise, output the <span class="tex-span"><i>k</i></span>-th smallest divisor of <span class="tex-span"><i>n</i></span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">15</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>If <span class="tex-span"><i>n</i></span> has less than <span class="tex-span"><i>k</i></span> divisors, output <span class="tex-font-style-tt">-1</span>.</p><p>Otherwise, output the <span class="tex-span"><i>k</i></span>-th smallest divisor of <span class="tex-span"><i>n</i></span>.</p>





```input1
4 2

```




```input2
5 3

```




```input3
12 5

```




```output1
2

```




```output2
-1

```




```output3
6

```



## Note

<p>In the first example, number <span class="tex-span">4</span> has three divisors: <span class="tex-span">1</span>, <span class="tex-span">2</span> and <span class="tex-span">4</span>. The second one is <span class="tex-span">2</span>.</p><p>In the second example, number <span class="tex-span">5</span> has only two divisors: <span class="tex-span">1</span> and <span class="tex-span">5</span>. The third divisor doesn't exist, so the answer is <span class="tex-font-style-tt">-1</span>.</p>
