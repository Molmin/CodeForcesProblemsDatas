## Description

<div><p>PolandBall is standing in a row with Many Other Balls. More precisely, there are exactly <span class="tex-span"><i>n</i></span> Balls. Balls are proud of their home land&nbsp;— and they want to prove that it's strong.</p><p>The Balls decided to start with selecting exactly <span class="tex-span"><i>m</i></span> groups of Balls, each consisting either of single Ball or two neighboring Balls. Each Ball can join no more than one group.</p><p>The Balls really want to impress their Enemies. They kindly asked you to calculate number of such divisions for all <span class="tex-span"><i>m</i></span> where <span class="tex-span">1 ≤ <i>m</i> ≤ <i>k</i></span>. Output all these values modulo <span class="tex-span">998244353</span>, the Enemies will be impressed anyway.</p></div><div class="input-specification"><p>There are exactly two numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>k</i> &lt; 2<sup class="upper-index">15</sup></span>), denoting the number of Balls and the maximim number of groups, respectively.</p></div><div class="output-specification"><p>You should output a sequence of <span class="tex-span"><i>k</i></span> values. The <span class="tex-span"><i>i</i></span>-th of them should represent the sought number of divisions into exactly <span class="tex-span"><i>i</i></span> groups, according to PolandBall's rules.</p></div>

## Input

<p>There are exactly two numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>k</i> &lt; 2<sup class="upper-index">15</sup></span>), denoting the number of Balls and the maximim number of groups, respectively.</p>

## Output

<p>You should output a sequence of <span class="tex-span"><i>k</i></span> values. The <span class="tex-span"><i>i</i></span>-th of them should represent the sought number of divisions into exactly <span class="tex-span"><i>i</i></span> groups, according to PolandBall's rules.</p>





```input1
3 3

```




```input2
1 1

```




```input3
5 10

```




```output1
5 5 1
```




```output2
1
```




```output3
9 25 25 9 1 0 0 0 0 0
```



## Note

<p>In the first sample case we can divide Balls into groups as follows: </p><p><span class="tex-span">{1}</span>, <span class="tex-span">{2}</span>, <span class="tex-span">{3}</span>, <span class="tex-span">{12}</span>, <span class="tex-span">{23}</span>.</p><p><span class="tex-span">{12}{3}</span>, <span class="tex-span">{1}{23}</span>, <span class="tex-span">{1}{2}</span>, <span class="tex-span">{1}{3}</span>, <span class="tex-span">{2}{3}</span>.</p><p><span class="tex-span">{1}{2}{3}</span>.</p><p>Therefore, output is: <span class="tex-font-style-tt">5 5 1</span>.</p>
