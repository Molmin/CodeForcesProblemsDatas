## Description

<div><p>Alice is a beginner composer and now she is ready to create another masterpiece. And not even the single one but two at the same time! </p><p>Alice has a sheet with <span class="tex-span"><i>n</i></span> notes written on it. She wants to take two such non-empty non-intersecting subsequences that both of them form a <span class="tex-font-style-it">melody</span> and sum of their lengths is maximal.</p><p><span class="tex-font-style-it">Subsequence is a sequence that can be derived from another sequence by deleting some elements without changing the order of the remaining elements.</span></p><p>Subsequence forms a melody when each two adjacent notes either differs by <span class="tex-font-style-tt">1</span> or are congruent modulo <span class="tex-font-style-tt">7</span>.</p><p>You should write a program which will calculate maximum sum of lengths of such two non-empty non-intersecting subsequences that both of them form a melody.</p></div><div class="input-specification"><p>The first line contains one integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 5000</span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>) — notes written on a sheet.</p></div><div class="output-specification"><p>Print maximum sum of lengths of such two non-empty non-intersecting subsequences that both of them form a melody.</p></div>

## Input

<p>The first line contains one integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 5000</span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>) — notes written on a sheet.</p>

## Output

<p>Print maximum sum of lengths of such two non-empty non-intersecting subsequences that both of them form a melody.</p>





```input1
4
1 2 4 5

```




```input2
6
62 22 60 61 48 49

```




```output1
4

```




```output2
5

```



## Note

<p>In the first example subsequences <span class="tex-span">[1, 2]</span> and <span class="tex-span">[4, 5]</span> give length <span class="tex-font-style-tt">4</span> in total.</p><p>In the second example subsequences <span class="tex-span">[62, 48, 49]</span> and <span class="tex-span">[60, 61]</span> give length <span class="tex-font-style-tt">5</span> in total. If you choose subsequence <span class="tex-span">[62, 61]</span> in the first place then the second melody will have maximum length <span class="tex-font-style-tt">2</span>, that gives the result of <span class="tex-font-style-tt">4</span>, which is not maximal.</p>
