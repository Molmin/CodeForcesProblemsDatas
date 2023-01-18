## Description

<div><p>Fibonacci strings are defined as follows: </p><ul> <li> <span class="tex-span"><i>f</i><sub class="lower-index">1</sub></span> = «<span class="tex-font-style-tt">a</span>» </li><li> <span class="tex-span"><i>f</i><sub class="lower-index">2</sub></span> = «<span class="tex-font-style-tt">b</span>» </li><li> <span class="tex-span"><i>f</i><sub class="lower-index"><i>n</i></sub></span> = <span class="tex-span"><i>f</i><sub class="lower-index"><i>n</i> - 1</sub>&nbsp;<i>f</i><sub class="lower-index"><i>n</i> - 2</sub></span>, <span class="tex-span"><i>n</i> &gt; 2</span> </li></ul><p>Thus, the first five Fibonacci strings are: "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">b</span>", "<span class="tex-font-style-tt">ba</span>", "<span class="tex-font-style-tt">bab</span>", "<span class="tex-font-style-tt">babba</span>".</p><p>You are given a Fibonacci string and <span class="tex-span"><i>m</i></span> strings <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>. For each string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>, find the number of times it occurs in the given Fibonacci string as a substring.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>m</i></span> — the number of a Fibonacci string and the number of queries, correspondingly.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain strings <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> that correspond to the queries. It is guaranteed that strings <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> aren't empty and consist only of characters "<span class="tex-font-style-tt">a</span>" and "<span class="tex-font-style-tt">b</span>".</p><p>The input limitations for getting 30 points are: </p><ul> <li> <span class="tex-span">1 ≤ <i>k</i> ≤ 3000</span> </li><li> <span class="tex-span">1 ≤ <i>m</i> ≤ 3000</span> </li><li> The total length of strings <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> doesn't exceed <span class="tex-span">3000</span> </li></ul> <p>The input limitations for getting 100 points are: </p><ul> <li> <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">18</sup></span> </li><li> <span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">4</sup></span> </li><li> The total length of strings <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span> </li></ul> <p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div><div class="output-specification"><p>For each string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> print the number of times it occurs in the given Fibonacci string as a substring. Since the numbers can be large enough, print them modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>. Print the answers for the strings in the order in which they are given in the input.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>m</i></span> — the number of a Fibonacci string and the number of queries, correspondingly.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain strings <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> that correspond to the queries. It is guaranteed that strings <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> aren't empty and consist only of characters "<span class="tex-font-style-tt">a</span>" and "<span class="tex-font-style-tt">b</span>".</p><p>The input limitations for getting 30 points are: </p><ul> <li> <span class="tex-span">1 ≤ <i>k</i> ≤ 3000</span> </li><li> <span class="tex-span">1 ≤ <i>m</i> ≤ 3000</span> </li><li> The total length of strings <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> doesn't exceed <span class="tex-span">3000</span> </li></ul> <p>The input limitations for getting 100 points are: </p><ul> <li> <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">18</sup></span> </li><li> <span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">4</sup></span> </li><li> The total length of strings <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span> </li></ul> <p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>

## Output

<p>For each string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> print the number of times it occurs in the given Fibonacci string as a substring. Since the numbers can be large enough, print them modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>. Print the answers for the strings in the order in which they are given in the input.</p>





```input1
6 5
a
b
ab
ba
aba

```




```output1
3
5
3
3
1

```


