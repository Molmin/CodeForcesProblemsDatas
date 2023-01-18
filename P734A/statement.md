## Description

<div><p>Anton likes to play chess, and so does his friend Danik.</p><p>Once they have played <span class="tex-span"><i>n</i></span> games in a row. For each game it's known who was the winner&nbsp;— Anton or Danik. None of the games ended with a tie.</p><p>Now Anton wonders, who won more games, he or Danik? Help him determine this.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of games played.</p><p>The second line contains a string <span class="tex-span"><i>s</i></span>, consisting of <span class="tex-span"><i>n</i></span> uppercase English letters '<span class="tex-font-style-tt">A</span>' and '<span class="tex-font-style-tt">D</span>'&nbsp;— the outcome of each of the games. The <span class="tex-span"><i>i</i></span>-th character of the string is equal to '<span class="tex-font-style-tt">A</span>' if the Anton won the <span class="tex-span"><i>i</i></span>-th game and '<span class="tex-font-style-tt">D</span>' if Danik won the <span class="tex-span"><i>i</i></span>-th game.</p></div><div class="output-specification"><p>If Anton won more games than Danik, print "<span class="tex-font-style-tt">Anton</span>" (without quotes) in the only line of the output.</p><p>If Danik won more games than Anton, print "<span class="tex-font-style-tt">Danik</span>" (without quotes) in the only line of the output.</p><p>If Anton and Danik won the same number of games, print "<span class="tex-font-style-tt">Friendship</span>" (without quotes).</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of games played.</p><p>The second line contains a string <span class="tex-span"><i>s</i></span>, consisting of <span class="tex-span"><i>n</i></span> uppercase English letters '<span class="tex-font-style-tt">A</span>' and '<span class="tex-font-style-tt">D</span>'&nbsp;— the outcome of each of the games. The <span class="tex-span"><i>i</i></span>-th character of the string is equal to '<span class="tex-font-style-tt">A</span>' if the Anton won the <span class="tex-span"><i>i</i></span>-th game and '<span class="tex-font-style-tt">D</span>' if Danik won the <span class="tex-span"><i>i</i></span>-th game.</p>

## Output

<p>If Anton won more games than Danik, print "<span class="tex-font-style-tt">Anton</span>" (without quotes) in the only line of the output.</p><p>If Danik won more games than Anton, print "<span class="tex-font-style-tt">Danik</span>" (without quotes) in the only line of the output.</p><p>If Anton and Danik won the same number of games, print "<span class="tex-font-style-tt">Friendship</span>" (without quotes).</p>





```input1
6
ADAAAA

```




```input2
7
DDDAADA

```




```input3
6
DADADA

```




```output1
Anton

```




```output2
Danik

```




```output3
Friendship

```



## Note

<p>In the first sample, Anton won <span class="tex-span">6</span> games, while Danik&nbsp;— only <span class="tex-span">1</span>. Hence, the answer is "<span class="tex-font-style-tt">Anton</span>".</p><p>In the second sample, Anton won <span class="tex-span">3</span> games and Danik won <span class="tex-span">4</span> games, so the answer is "<span class="tex-font-style-tt">Danik</span>".</p><p>In the third sample, both Anton and Danik won <span class="tex-span">3</span> games and the answer is "<span class="tex-font-style-tt">Friendship</span>".</p>
