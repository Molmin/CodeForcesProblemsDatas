## Description

<div><p>Ayrat has number <span class="tex-span"><i>n</i></span>, represented as it's prime factorization <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> of size <span class="tex-span"><i>m</i></span>, i.e. <span class="tex-span"><i>n</i> = <i>p</i><sub class="lower-index">1</sub>·<i>p</i><sub class="lower-index">2</sub>·...·<i>p</i><sub class="lower-index"><i>m</i></sub></span>. Ayrat got secret information that that the product of all divisors of <span class="tex-span"><i>n</i></span> taken modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span> is the password to the secret data base. Now he wants to calculate this value.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 200 000</span>)&nbsp;— the number of primes in factorization of <span class="tex-span"><i>n</i></span>. </p><p>The second line contains <span class="tex-span"><i>m</i></span> primes numbers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">2 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 200 000</span>).</p></div><div class="output-specification"><p>Print one integer&nbsp;— the product of all divisors of <span class="tex-span"><i>n</i></span> modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 200 000</span>)&nbsp;— the number of primes in factorization of <span class="tex-span"><i>n</i></span>. </p><p>The second line contains <span class="tex-span"><i>m</i></span> primes numbers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">2 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 200 000</span>).</p>

## Output

<p>Print one integer&nbsp;— the product of all divisors of <span class="tex-span"><i>n</i></span> modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
2
2 3

```




```input2
3
2 3 2

```




```output1
36

```




```output2
1728

```



## Note

<p>In the first sample <span class="tex-span"><i>n</i> = 2·3 = 6</span>. The divisors of <span class="tex-span">6</span> are <span class="tex-span">1</span>, <span class="tex-span">2</span>, <span class="tex-span">3</span> and <span class="tex-span">6</span>, their product is equal to <span class="tex-span">1·2·3·6 = 36</span>.</p><p>In the second sample <span class="tex-span">2·3·2 = 12</span>. The divisors of <span class="tex-span">12</span> are <span class="tex-span">1</span>, <span class="tex-span">2</span>, <span class="tex-span">3</span>, <span class="tex-span">4</span>, <span class="tex-span">6</span> and <span class="tex-span">12</span>. <span class="tex-span">1·2·3·4·6·12 = 1728</span>.</p>
