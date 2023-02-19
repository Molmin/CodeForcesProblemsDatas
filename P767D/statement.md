## Description

<div><p>Olya likes milk very much. She drinks <span class="tex-span"><i>k</i></span> cartons of milk each day if she has at least <span class="tex-span"><i>k</i></span> and drinks all of them if she doesn't. But there's an issue&nbsp;— expiration dates. Each carton has a date after which you can't drink it (you still can drink it exactly at the date written on the carton). Due to this, if Olya's fridge contains a carton past its expiry date, she throws it away.</p><p>Olya hates throwing out cartons, so when she drinks a carton, she chooses the one which expires the fastest. It's easy to understand that this strategy minimizes the amount of cartons thrown out and lets her avoid it if it's even possible.</p><center> <img class="tex-graphics" height="291px" src="file://0AkDj8sy.png" style="max-width: 100.0%;max-height: 100.0%;" width="378px">   <span class="tex-font-size-small">Milk. Best before: 20.02.2017.</span> </center><p>The main issue Olya has is the one of buying new cartons. Currently, there are <span class="tex-span"><i>n</i></span> cartons of milk in Olya's fridge, for each one an expiration date is known (how soon does it expire, measured in days). In the shop that Olya visited there are <span class="tex-span"><i>m</i></span> cartons, and the expiration date is known for each of those cartons as well.</p><p>Find the maximum number of cartons Olya can buy so that she wouldn't have to throw away any cartons. Assume that Olya drank no cartons today. </p></div><div class="input-specification"><p>In the first line there are three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> + <i>m</i></span>)&nbsp;— the amount of cartons in Olya's fridge, the amount of cartons in the shop and the number of cartons Olya drinks each day.</p><p>In the second line there are <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>f</i><sub class="lower-index">1</sub>, <i>f</i><sub class="lower-index">2</sub>, ..., <i>f</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>f</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup></span>)&nbsp;— expiration dates of the cartons in Olya's fridge. The expiration date is expressed by the number of days the drinking of this carton can be delayed. For example, a <span class="tex-span">0</span> expiration date means it must be drunk today, <span class="tex-span">1</span>&nbsp;— no later than tomorrow, etc.</p><p>In the third line there are <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">0 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup></span>)&nbsp;— expiration dates of the cartons in the shop in a similar format.</p></div><div class="output-specification"><p>If there's no way for Olya to drink the cartons she already has in her fridge, print <span class="tex-font-style-tt">-1</span>.</p><p>Otherwise, in the first line print the maximum number <span class="tex-span"><i>x</i></span> of cartons which Olya can buy so that she wouldn't have to throw a carton away. The next line should contain exactly <span class="tex-span"><i>x</i></span> integers&nbsp;— the numbers of the cartons that should be bought (cartons are numbered in an order in which they are written in the input, starting with <span class="tex-span">1</span>). Numbers should not repeat, but can be in arbitrary order. If there are multiple correct answers, print any of them.</p></div>

## Input

<p>In the first line there are three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> + <i>m</i></span>)&nbsp;— the amount of cartons in Olya's fridge, the amount of cartons in the shop and the number of cartons Olya drinks each day.</p><p>In the second line there are <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>f</i><sub class="lower-index">1</sub>, <i>f</i><sub class="lower-index">2</sub>, ..., <i>f</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>f</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup></span>)&nbsp;— expiration dates of the cartons in Olya's fridge. The expiration date is expressed by the number of days the drinking of this carton can be delayed. For example, a <span class="tex-span">0</span> expiration date means it must be drunk today, <span class="tex-span">1</span>&nbsp;— no later than tomorrow, etc.</p><p>In the third line there are <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">0 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup></span>)&nbsp;— expiration dates of the cartons in the shop in a similar format.</p>

## Output

<p>If there's no way for Olya to drink the cartons she already has in her fridge, print <span class="tex-font-style-tt">-1</span>.</p><p>Otherwise, in the first line print the maximum number <span class="tex-span"><i>x</i></span> of cartons which Olya can buy so that she wouldn't have to throw a carton away. The next line should contain exactly <span class="tex-span"><i>x</i></span> integers&nbsp;— the numbers of the cartons that should be bought (cartons are numbered in an order in which they are written in the input, starting with <span class="tex-span">1</span>). Numbers should not repeat, but can be in arbitrary order. If there are multiple correct answers, print any of them.</p>





```input1
3 6 2
1 0 1
2 0 2 0 0 2

```




```input2
3 1 2
0 0 0
1

```




```input3
2 1 2
0 1
0

```




```output1
3
1 2 3
```




```output2
-1
```




```output3
1
1
```



## Note

<p>In the first example <span class="tex-span"><i>k</i> = 2</span> and Olya has three cartons with expiry dates <span class="tex-span">0</span>, <span class="tex-span">1</span> and <span class="tex-span">1</span> (they expire today, tomorrow and tomorrow), and the shop has <span class="tex-span">3</span> cartons with expiry date <span class="tex-span">0</span> and <span class="tex-span">3</span> cartons with expiry date <span class="tex-span">2</span>. Olya can buy three cartons, for example, one with the expiry date <span class="tex-span">0</span> and two with expiry date <span class="tex-span">2</span>.</p><p>In the second example all three cartons Olya owns expire today and it means she would have to throw packets away regardless of whether she buys an extra one or not.</p><p>In the third example Olya would drink <span class="tex-span"><i>k</i> = 2</span> cartons today (one she alreay has in her fridge and one from the shop) and the remaining one tomorrow.</p>
