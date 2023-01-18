## Description

<div><p>Mahmoud and Ehab play a game called the even-odd game. Ehab chooses his favorite integer <span class="tex-span"><i>n</i></span> and then they take turns, starting from Mahmoud. In each player's turn, he has to choose an integer <span class="tex-span"><i>a</i></span> and subtract it from <span class="tex-span"><i>n</i></span> such that:</p><ul> <li> <span class="tex-span">1 ≤ <i>a</i> ≤ <i>n</i></span>. </li><li> If it's Mahmoud's turn, <span class="tex-span"><i>a</i></span> has to be even, but if it's Ehab's turn, <span class="tex-span"><i>a</i></span> has to be odd. </li></ul><p>If the current player can't choose any number satisfying the conditions, he loses. Can you determine the winner if they both play optimally?</p></div><div class="input-specification"><p>The only line contains an integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup>)</span>, the number at the beginning of the game.</p></div><div class="output-specification"><p>Output "<span class="tex-font-style-tt">Mahmoud</span>" (without quotes) if Mahmoud wins and "<span class="tex-font-style-tt">Ehab</span>" (without quotes) otherwise.</p></div>

## Input

<p>The only line contains an integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup>)</span>, the number at the beginning of the game.</p>

## Output

<p>Output "<span class="tex-font-style-tt">Mahmoud</span>" (without quotes) if Mahmoud wins and "<span class="tex-font-style-tt">Ehab</span>" (without quotes) otherwise.</p>





```input1
1

```




```input2
2

```




```output1
Ehab
```




```output2
Mahmoud
```



## Note

<p>In the first sample, Mahmoud can't choose any integer <span class="tex-span"><i>a</i></span> initially because there is no positive even integer less than or equal to <span class="tex-span">1</span> so Ehab wins.</p><p>In the second sample, Mahmoud has to choose <span class="tex-span"><i>a</i> = 2</span> and subtract it from <span class="tex-span"><i>n</i></span>. It's Ehab's turn and <span class="tex-span"><i>n</i> = 0</span>. There is no positive odd integer less than or equal to <span class="tex-span">0</span> so Mahmoud wins.</p>
