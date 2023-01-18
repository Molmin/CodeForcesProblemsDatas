## Description

<div><p>Vasya plays Robot Bicorn Attack.</p><p>The game consists of three rounds. For each one a non-negative integer amount of points is given. The result of the game is the sum of obtained points. Vasya has already played three rounds and wrote obtained points one by one (without leading zeros) into the string <span class="tex-span"><i>s</i></span>. Vasya decided to brag about his achievement to the friends. However, he has forgotten how many points he got for each round. The only thing he remembers is the string <span class="tex-span"><i>s</i></span>.</p><p>Help Vasya to find out what is the maximum amount of points he could get. Take into account that Vasya played Robot Bicorn Attack for the first time, so he could not get more than 1000000 (<span class="tex-span">10<sup class="upper-index">6</sup></span>) points for one round.</p></div><div class="input-specification"><p>The only line of input contains non-empty string <span class="tex-span"><i>s</i></span> obtained by Vasya. The string consists of digits only. The string length does not exceed 30 characters.</p></div><div class="output-specification"><p>Print the only number — the maximum amount of points Vasya could get. If Vasya is wrong and the string could not be obtained according to the rules then output number -1.</p></div>

## Input

<p>The only line of input contains non-empty string <span class="tex-span"><i>s</i></span> obtained by Vasya. The string consists of digits only. The string length does not exceed 30 characters.</p>

## Output

<p>Print the only number — the maximum amount of points Vasya could get. If Vasya is wrong and the string could not be obtained according to the rules then output number -1.</p>





```input1
1234

```




```input2
9000

```




```input3
0009

```




```output1
37

```




```output2
90

```




```output3
-1

```



## Note

<p>In the first example the string must be split into numbers 1, 2 and 34.</p><p>In the second example the string must be split into numbers 90, 0 and 0. </p><p>In the third example the string is incorrect, because after splitting the string into 3 numbers number 00 or 09 will be obtained, but numbers cannot have leading zeroes.</p>
