## Description

<div><p>Friends are going to play console. They have two joysticks and only one charger for them. Initially first joystick is charged at <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> percent and second one is charged at <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span> percent. You can connect charger to a joystick only at the beginning of each minute. In one minute joystick either discharges by 2 percent (if not connected to a charger) or charges by 1 percent (if connected to a charger).</p><p>Game continues while both joysticks have a positive charge. Hence, if at the beginning of minute some joystick is charged by 1 percent, it has to be connected to a charger, otherwise the game stops. If some joystick completely discharges (its charge turns to 0), the game also stops.</p><p>Determine the maximum number of minutes that game can last. It is prohibited to pause the game, i. e. at each moment both joysticks should be enabled. It is allowed for joystick to be charged by <span class="tex-font-style-bf">more than <span class="tex-span">100</span> percent</span>.</p></div><div class="input-specification"><p>The first line of the input contains two positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub> ≤ 100</span>), the initial charge level of first and second joystick respectively.</p></div><div class="output-specification"><p>Output the only integer, the maximum number of minutes that the game can last. Game continues until some joystick is discharged.</p></div>

## Input

<p>The first line of the input contains two positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub> ≤ 100</span>), the initial charge level of first and second joystick respectively.</p>

## Output

<p>Output the only integer, the maximum number of minutes that the game can last. Game continues until some joystick is discharged.</p>





```input1
3 5

```




```input2
4 4

```




```output1
6

```




```output2
5

```



## Note

<p>In the first sample game lasts for 6 minute by using the following algorithm:</p><ul> <li> at the beginning of the first minute connect first joystick to the charger, by the end of this minute first joystick is at 4%, second is at 3%; </li><li> continue the game without changing charger, by the end of the second minute the first joystick is at 5%, second is at 1%; </li><li> at the beginning of the third minute connect second joystick to the charger, after this minute the first joystick is at 3%, the second one is at 2%; </li><li> continue the game without changing charger, by the end of the fourth minute first joystick is at 1%, second one is at 3%; </li><li> at the beginning of the fifth minute connect first joystick to the charger, after this minute the first joystick is at 2%, the second one is at 1%; </li><li> at the beginning of the sixth minute connect second joystick to the charger, after this minute the first joystick is at 0%, the second one is at 2%. </li></ul><p>After that the first joystick is completely discharged and the game is stopped.</p>
