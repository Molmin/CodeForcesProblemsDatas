## Description

<div><p>It's the year 4527 and the tanks game that we all know and love still exists. There also exists Great Gena's code, written in 2016. The problem this code solves is: given the number of tanks that go into the battle from each country, find their product. If it is turns to be too large, then the servers might have not enough time to assign tanks into teams and the whole game will collapse!</p><p>There are exactly <span class="tex-span"><i>n</i></span> distinct countries in the world and the <span class="tex-span"><i>i</i></span>-th country added <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> tanks to the game. As the developers of the game are perfectionists, the number of tanks from each country is beautiful. A <span class="tex-font-style-it">beautiful</span> number, according to the developers, is such number that its decimal representation consists only of digits '<span class="tex-font-style-tt">1</span>' and '<span class="tex-font-style-tt">0</span>', moreover it contains <span class="tex-font-style-bf">at most one</span> digit '<span class="tex-font-style-tt">1</span>'. However, due to complaints from players, some number of tanks of <span class="tex-font-style-bf">one</span> country was removed from the game, hence the number of tanks of this country may not remain beautiful.</p><p>Your task is to write the program that solves exactly the same problem in order to verify Gena's code correctness. Just in case.</p></div><div class="input-specification"><p>The first line of the input contains the number of countries <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>). The second line contains <span class="tex-span"><i>n</i></span> non-negative integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> without leading zeroes&nbsp;— the number of tanks of the <span class="tex-span"><i>i</i></span>-th country.</p><p>It is guaranteed that the second line contains at least <span class="tex-span"><i>n</i> - 1</span> beautiful numbers and the total length of all these number's representations doesn't exceed <span class="tex-span">100 000</span>.</p></div><div class="output-specification"><p>Print a single number without leading zeroes&nbsp;— the product of the number of tanks presented by each country.</p></div>

## Input

<p>The first line of the input contains the number of countries <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>). The second line contains <span class="tex-span"><i>n</i></span> non-negative integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> without leading zeroes&nbsp;— the number of tanks of the <span class="tex-span"><i>i</i></span>-th country.</p><p>It is guaranteed that the second line contains at least <span class="tex-span"><i>n</i> - 1</span> beautiful numbers and the total length of all these number's representations doesn't exceed <span class="tex-span">100 000</span>.</p>

## Output

<p>Print a single number without leading zeroes&nbsp;— the product of the number of tanks presented by each country.</p>





```input1
3
5 10 1

```




```input2
4
1 1 10 11

```




```input3
5
0 3 1 100 1

```




```output1
50
```




```output2
110
```




```output3
0
```



## Note

<p>In sample 1 numbers 10 and 1 are <span class="tex-font-style-it">beautiful</span>, number 5 is not not.</p><p>In sample 2 number 11 is not <span class="tex-font-style-it">beautiful</span> (contains two '<span class="tex-font-style-tt">1</span>'s), all others are <span class="tex-font-style-it">beautiful</span>.</p><p>In sample 3 number 3 is not <span class="tex-font-style-it">beautiful</span>, all others are <span class="tex-font-style-it">beautiful</span>.</p>
