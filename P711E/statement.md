## Description

<div><p>ZS the Coder has recently found an interesting concept called the Birthday Paradox. It states that given a random set of <span class="tex-span">23</span> people, there is around <span class="tex-span">50%</span> chance that some two of them share the same birthday. ZS the Coder finds this very interesting, and decides to test this with the inhabitants of Udayland.</p><p>In Udayland, there are <span class="tex-span">2<sup class="upper-index"><i>n</i></sup></span> days in a year. ZS the Coder wants to interview <span class="tex-span"><i>k</i></span> people from Udayland, each of them has birthday in one of <span class="tex-span">2<sup class="upper-index"><i>n</i></sup></span> days (each day with equal probability). He is interested in the probability of at least two of them have the birthday at the same day. </p><p>ZS the Coder knows that the answer can be written as an irreducible fraction <img align="middle" class="tex-formula" src="file://xbC195cy.png" style="max-width: 100.0%;max-height: 100.0%;">. He wants to find the values of <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span> (he does not like to deal with floating point numbers). Can you help him?</p></div><div class="input-specification"><p>The first and only line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">18</sup>, 2 ≤ <i>k</i> ≤ 10<sup class="upper-index">18</sup>)</span>, meaning that there are <span class="tex-span">2<sup class="upper-index"><i>n</i></sup></span> days in a year and that ZS the Coder wants to interview exactly <span class="tex-span"><i>k</i></span> people.</p></div><div class="output-specification"><p>If the probability of at least two <span class="tex-span"><i>k</i></span> people having the same birthday in <span class="tex-span">2<sup class="upper-index"><i>n</i></sup></span> days long year equals <img align="middle" class="tex-formula" src="file://jVU4SFwJ.png" style="max-width: 100.0%;max-height: 100.0%;"> (<span class="tex-span"><i>A</i> ≥ 0</span>, <span class="tex-span"><i>B</i> ≥ 1</span>, <img align="middle" class="tex-formula" src="file://NxW8WcU0.png" style="max-width: 100.0%;max-height: 100.0%;">), print the <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span> in a single line.</p><p>Since these numbers may be too large, print them modulo <span class="tex-span">10<sup class="upper-index">6</sup> + 3</span>. Note that <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span> must be coprime <span class="tex-font-style-bf">before</span> their remainders modulo <span class="tex-span">10<sup class="upper-index">6</sup> + 3</span> are taken.</p></div>

## Input

<p>The first and only line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">18</sup>, 2 ≤ <i>k</i> ≤ 10<sup class="upper-index">18</sup>)</span>, meaning that there are <span class="tex-span">2<sup class="upper-index"><i>n</i></sup></span> days in a year and that ZS the Coder wants to interview exactly <span class="tex-span"><i>k</i></span> people.</p>

## Output

<p>If the probability of at least two <span class="tex-span"><i>k</i></span> people having the same birthday in <span class="tex-span">2<sup class="upper-index"><i>n</i></sup></span> days long year equals <img align="middle" class="tex-formula" src="file://jVU4SFwJ.png" style="max-width: 100.0%;max-height: 100.0%;"> (<span class="tex-span"><i>A</i> ≥ 0</span>, <span class="tex-span"><i>B</i> ≥ 1</span>, <img align="middle" class="tex-formula" src="file://NxW8WcU0.png" style="max-width: 100.0%;max-height: 100.0%;">), print the <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span> in a single line.</p><p>Since these numbers may be too large, print them modulo <span class="tex-span">10<sup class="upper-index">6</sup> + 3</span>. Note that <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span> must be coprime <span class="tex-font-style-bf">before</span> their remainders modulo <span class="tex-span">10<sup class="upper-index">6</sup> + 3</span> are taken.</p>





```input1
3 2

```




```input2
1 3

```




```input3
4 3

```




```output1
1 8
```




```output2
1 1
```




```output3
23 128
```



## Note

<p>In the first sample case, there are <span class="tex-span">2<sup class="upper-index">3</sup> = 8</span> days in Udayland. The probability that <span class="tex-span">2</span> people have the same birthday among <span class="tex-span">2</span> people is clearly <img align="middle" class="tex-formula" src="file://4JB8KCbb.png" style="max-width: 100.0%;max-height: 100.0%;">, so <span class="tex-span"><i>A</i> = 1</span>, <span class="tex-span"><i>B</i> = 8</span>.</p><p>In the second sample case, there are only <span class="tex-span">2<sup class="upper-index">1</sup> = 2</span> days in Udayland, but there are <span class="tex-span">3</span> people, so it is guaranteed that two of them have the same birthday. Thus, the probability is <span class="tex-span">1</span> and <span class="tex-span"><i>A</i> = <i>B</i> = 1</span>.</p>
