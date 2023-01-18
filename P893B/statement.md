## Description

<div><p>Recently Luba learned about a special kind of numbers that she calls <span class="tex-font-style-it">beautiful</span> numbers. The number is called <span class="tex-font-style-it">beautiful</span> iff its binary representation consists of <span class="tex-span"><i>k</i> + 1</span> consecutive ones, and then <span class="tex-span"><i>k</i></span> consecutive zeroes.</p><p>Some examples of beautiful numbers: </p><ul> <li> <span class="tex-span">1<sub class="lower-index">2</sub></span> (<span class="tex-span">1<sub class="lower-index">10</sub></span>); </li><li> <span class="tex-span">110<sub class="lower-index">2</sub></span> (<span class="tex-span">6<sub class="lower-index">10</sub></span>); </li><li> <span class="tex-span">1111000<sub class="lower-index">2</sub></span> (<span class="tex-span">120<sub class="lower-index">10</sub></span>); </li><li> <span class="tex-span">111110000<sub class="lower-index">2</sub></span> (<span class="tex-span">496<sub class="lower-index">10</sub></span>). </li></ul><p>More formally, the number is beautiful iff there exists some positive integer <span class="tex-span"><i>k</i></span> such that the number is equal to <span class="tex-span">(2<sup class="upper-index"><i>k</i></sup> - 1) * (2<sup class="upper-index"><i>k</i> - 1</sup>)</span>.</p><p>Luba has got an integer number <span class="tex-span"><i>n</i></span>, and she wants to find its greatest beautiful divisor. Help her to find it!</p></div><div class="input-specification"><p>The only line of input contains one number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number Luba has got.</p></div><div class="output-specification"><p>Output one number — the greatest beautiful divisor of Luba's number. It is obvious that the answer always exists.</p></div>

## Input

<p>The only line of input contains one number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number Luba has got.</p>

## Output

<p>Output one number — the greatest beautiful divisor of Luba's number. It is obvious that the answer always exists.</p>





```input1
3

```




```input2
992

```




```output1
1

```




```output2
496

```


