## Description

<div><p><span class="tex-font-style-it">A prime number is a number which has exactly two distinct divisors: one and itself. For example, numbers <span class="tex-span">2</span>, <span class="tex-span">7</span>, <span class="tex-span">3</span> are prime, and <span class="tex-span">1</span>, <span class="tex-span">6</span>, <span class="tex-span">4</span> are not.</span></p><p><span class="tex-font-style-it">The next prime number after <span class="tex-span"><i>x</i></span> is the <span class="tex-font-style-bf">smallest</span> prime number greater than <span class="tex-span"><i>x</i></span>. For example, the next prime number after <span class="tex-span">2</span> is <span class="tex-span">3</span>, and the next prime number after <span class="tex-span">3</span> is <span class="tex-span">5</span>. Note that there is exactly one next prime number after each number. So <span class="tex-span">5</span> <span class="tex-font-style-bf">is&nbsp;not</span> the next prime number for <span class="tex-span">2</span>.</span></p><p>One cold April morning Panoramix predicted that soon Kakofonix will break free from his straitjacket, and this will be a black day for the residents of the Gallic countryside.</p><p>Panoramix's prophecy tells that if some day Asterix and Obelix beat exactly <span class="tex-span"><i>x</i></span> Roman soldiers, where <span class="tex-span"><i>x</i></span> is a prime number, and next day they beat exactly <span class="tex-span"><i>y</i></span> Roman soldiers, where <span class="tex-span"><i>y</i></span> is <span class="tex-font-style-bf">the next prime number</span> after <span class="tex-span"><i>x</i></span>, then it's time to wait for Armageddon, for nothing can shut Kakofonix up while he sings his infernal song.</p><p>Yesterday the Gauls beat <span class="tex-span"><i>n</i></span> Roman soldiers and it turned out that the number <span class="tex-span"><i>n</i></span> was prime! Today their victims were a troop of <span class="tex-span"><i>m</i></span> Romans (<span class="tex-span"><i>m</i> &gt; <i>n</i></span>). Determine whether the Gauls should wait for the black day after today's victory of Asterix and Obelix?</p></div><div class="input-specification"><p>The first and only input line contains two positive integers — <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> &lt; <i>m</i> ≤ 50</span>). It is guaranteed that <span class="tex-span"><i>n</i></span> is prime.</p><p>Pretests contain all the cases with restrictions <span class="tex-span">2 ≤ <i>n</i> &lt; <i>m</i> ≤ 4</span>.</p></div><div class="output-specification"><p>Print <span class="tex-font-style-tt">YES</span>, if <span class="tex-span"><i>m</i></span> is the next prime number after <span class="tex-span"><i>n</i></span>, or <span class="tex-font-style-tt">NO</span> otherwise.</p></div>

## Input

<p>The first and only input line contains two positive integers — <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> &lt; <i>m</i> ≤ 50</span>). It is guaranteed that <span class="tex-span"><i>n</i></span> is prime.</p><p>Pretests contain all the cases with restrictions <span class="tex-span">2 ≤ <i>n</i> &lt; <i>m</i> ≤ 4</span>.</p>

## Output

<p>Print <span class="tex-font-style-tt">YES</span>, if <span class="tex-span"><i>m</i></span> is the next prime number after <span class="tex-span"><i>n</i></span>, or <span class="tex-font-style-tt">NO</span> otherwise.</p>





```input1
3 5

```




```input2
7 11

```




```input3
7 9

```




```output1
YES
```




```output2
YES
```




```output3
NO
```


