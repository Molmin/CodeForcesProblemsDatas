## Description

<div><p>Arkady plays Gardenscapes a lot. Arkady wants to build two new fountains. There are <span class="tex-span"><i>n</i></span> available fountains, for each fountain its beauty and cost are known. There are two types of money in the game: coins and diamonds, so each fountain cost can be either in coins or diamonds. No money changes between the types are allowed.</p><p>Help Arkady to find two fountains with maximum total beauty so that he can buy both at the same time.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>c</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">0 ≤ <i>c</i>, <i>d</i> ≤ 100 000</span>)&nbsp;— the number of fountains, the number of coins and diamonds Arkady has.</p><p>The next <span class="tex-span"><i>n</i></span> lines describe fountains. Each of these lines contain two integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 100 000</span>)&nbsp;— the beauty and the cost of the <span class="tex-span"><i>i</i></span>-th fountain, and then a letter "<span class="tex-font-style-tt">C</span>" or "<span class="tex-font-style-tt">D</span>", describing in which type of money is the cost of fountain <span class="tex-span"><i>i</i></span>: in coins or in diamonds, respectively.</p></div><div class="output-specification"><p>Print the maximum total beauty of exactly two fountains Arkady can build. If he can't build two fountains, print <span class="tex-font-style-tt">0</span>.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>c</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">0 ≤ <i>c</i>, <i>d</i> ≤ 100 000</span>)&nbsp;— the number of fountains, the number of coins and diamonds Arkady has.</p><p>The next <span class="tex-span"><i>n</i></span> lines describe fountains. Each of these lines contain two integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 100 000</span>)&nbsp;— the beauty and the cost of the <span class="tex-span"><i>i</i></span>-th fountain, and then a letter "<span class="tex-font-style-tt">C</span>" or "<span class="tex-font-style-tt">D</span>", describing in which type of money is the cost of fountain <span class="tex-span"><i>i</i></span>: in coins or in diamonds, respectively.</p>

## Output

<p>Print the maximum total beauty of exactly two fountains Arkady can build. If he can't build two fountains, print <span class="tex-font-style-tt">0</span>.</p>





```input1
3 7 6
10 8 C
4 3 C
5 6 D

```




```input2
2 4 5
2 5 C
2 1 D

```




```input3
3 10 10
5 5 C
5 5 C
10 11 D

```




```output1
9

```




```output2
0

```




```output3
10

```



## Note

<p>In the first example Arkady should build the second fountain with beauty <span class="tex-span">4</span>, which costs <span class="tex-span">3</span> coins. The first fountain he can't build because he don't have enough coins. Also Arkady should build the third fountain with beauty <span class="tex-span">5</span> which costs <span class="tex-span">6</span> diamonds. Thus the total beauty of built fountains is <span class="tex-span">9</span>.</p><p>In the second example there are two fountains, but Arkady can't build both of them, because he needs <span class="tex-span">5</span> coins for the first fountain, and Arkady has only <span class="tex-span">4</span> coins. </p>
