## Description

<div><p>Petya loves computer games. Finally a game that he's been waiting for so long came out!</p><p>The main character of this game has <span class="tex-span"><i>n</i></span> different skills, each of which is characterized by an integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> from 0 to 100. The higher the number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is, the higher is the <span class="tex-span"><i>i</i></span>-th skill of the character. The total rating of the character is calculated as the sum of the values ​​of <img align="middle" class="tex-formula" src="file://qLJJ40dW.png" style="max-width: 100.0%;max-height: 100.0%;"> for all <span class="tex-span"><i>i</i></span> from 1 to <span class="tex-span"><i>n</i></span>. The expression <span class="tex-span">⌊ <i>x</i>⌋</span> denotes the result of rounding the number <span class="tex-span"><i>x</i></span> <span class="tex-font-style-it">down</span> to the nearest integer.</p><p>At the beginning of the game Petya got <span class="tex-span"><i>k</i></span> improvement units as a bonus that he can use to increase the skills of his character and his total rating. One improvement unit can increase any skill of Petya's character by exactly one. For example, if <span class="tex-span"><i>a</i><sub class="lower-index">4</sub> = 46</span>, after using one imporvement unit to this skill, it becomes equal to 47. A hero's skill cannot rise higher more than 100. Thus, it is permissible that some of the units will remain unused.</p><p>Your task is to determine the optimal way of using the improvement units so as to maximize the overall rating of the character. It is not necessary to use all the improvement units.</p></div><div class="input-specification"><p>The first line of the input contains two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 10<sup class="upper-index">7</sup></span>) — the number of skills of the character and the number of units of improvements at Petya's disposal.</p><p>The second line of the input contains a sequence of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> characterizes the level of the <span class="tex-span"><i>i</i></span>-th skill of the character.</p></div><div class="output-specification"><p>The first line of the output should contain a single non-negative integer — the maximum total rating of the character that Petya can get using <span class="tex-span"><i>k</i></span> or less improvement units.</p></div>

## Input

<p>The first line of the input contains two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 10<sup class="upper-index">7</sup></span>) — the number of skills of the character and the number of units of improvements at Petya's disposal.</p><p>The second line of the input contains a sequence of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> characterizes the level of the <span class="tex-span"><i>i</i></span>-th skill of the character.</p>

## Output

<p>The first line of the output should contain a single non-negative integer — the maximum total rating of the character that Petya can get using <span class="tex-span"><i>k</i></span> or less improvement units.</p>





```input1
2 4
7 9

```




```input2
3 8
17 15 19

```




```input3
2 2
99 100

```




```output1
2

```




```output2
5

```




```output3
20

```



## Note

<p>In the first test case the optimal strategy is as follows. Petya has to improve the first skill to 10 by spending 3 improvement units, and the second skill to 10, by spending one improvement unit. Thus, Petya spends all his improvement units and the total rating of the character becomes equal to <span class="tex-span"> <i>lfloor</i> <i>frac</i>{100}{10} <i>rfloor</i> +  <i>lfloor</i> <i>frac</i>{100}{10} <i>rfloor</i> = 10 + 10 = </span> 20.</p><p>In the second test the optimal strategy for Petya is to improve the first skill to 20 (by spending 3 improvement units) and to improve the third skill to 20 (in this case by spending 1 improvement units). Thus, Petya is left with 4 improvement units and he will be able to increase the second skill to 19 (which does not change the overall rating, so Petya does not necessarily have to do it). Therefore, the highest possible total rating in this example is <img align="middle" class="tex-formula" src="file://pknggVBC.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>In the third test case the optimal strategy for Petya is to increase the first skill to 100 by spending 1 improvement unit. Thereafter, both skills of the character will be equal to 100, so Petya will not be able to spend the remaining improvement unit. So the answer is equal to <img align="middle" class="tex-formula" src="file://pa6vCWNf.png" style="max-width: 100.0%;max-height: 100.0%;">. </p>
