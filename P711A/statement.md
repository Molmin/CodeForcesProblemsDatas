## Description

<div><p>ZS the Coder and Chris the Baboon are travelling to Udayland! To get there, they have to get on the special IOI bus. The IOI bus has <span class="tex-span"><i>n</i></span> rows of seats. There are <span class="tex-span">4</span> seats in each row, and the seats are separated into pairs by a walkway. When ZS and Chris came, some places in the bus was already occupied.</p><p>ZS and Chris are good friends. They insist to get <span class="tex-font-style-bf">a pair of neighbouring empty seats</span>. Two seats are considered neighbouring if they are in the same row and in the same pair. Given the configuration of the bus, can you help ZS and Chris determine where they should sit?</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 1000)</span>&nbsp;— the number of rows of seats in the bus.</p><p>Then, <span class="tex-span"><i>n</i></span> lines follow. Each line contains exactly <span class="tex-span">5</span> characters, the first two of them denote the first pair of seats in the row, the third character denotes the walkway (it always equals '|') and the last two of them denote the second pair of seats in the row. </p><p>Each character, except the walkway, equals to 'O' or to 'X'. 'O' denotes an empty seat, 'X' denotes an occupied seat. See the sample cases for more details. </p></div><div class="output-specification"><p>If it is possible for Chris and ZS to sit at neighbouring empty seats, print "YES" (without quotes) in the first line. In the next <span class="tex-span"><i>n</i></span> lines print the bus configuration, where the characters in the pair of seats for Chris and ZS is changed with characters '+'. Thus the configuration should differ from the input one by exactly two charaters (they should be equal to 'O' in the input and to '+' in the output).</p><p>If there is no pair of seats for Chris and ZS, print "NO" (without quotes) in a single line.</p><p>If there are multiple solutions, you may print any of them.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 1000)</span>&nbsp;— the number of rows of seats in the bus.</p><p>Then, <span class="tex-span"><i>n</i></span> lines follow. Each line contains exactly <span class="tex-span">5</span> characters, the first two of them denote the first pair of seats in the row, the third character denotes the walkway (it always equals '|') and the last two of them denote the second pair of seats in the row. </p><p>Each character, except the walkway, equals to 'O' or to 'X'. 'O' denotes an empty seat, 'X' denotes an occupied seat. See the sample cases for more details. </p>

## Output

<p>If it is possible for Chris and ZS to sit at neighbouring empty seats, print "YES" (without quotes) in the first line. In the next <span class="tex-span"><i>n</i></span> lines print the bus configuration, where the characters in the pair of seats for Chris and ZS is changed with characters '+'. Thus the configuration should differ from the input one by exactly two charaters (they should be equal to 'O' in the input and to '+' in the output).</p><p>If there is no pair of seats for Chris and ZS, print "NO" (without quotes) in a single line.</p><p>If there are multiple solutions, you may print any of them.</p>





```input1
6
OO|OX
XO|XX
OX|OO
XX|OX
OO|OO
OO|XX

```




```input2
4
XO|OX
XO|XX
OX|OX
XX|OX

```




```input3
5
XX|XX
XX|XX
XO|OX
XO|OO
OX|XO

```




```output1
YES
++|OX
XO|XX
OX|OO
XX|OX
OO|OO
OO|XX

```




```output2
NO

```




```output3
YES
XX|XX
XX|XX
XO|OX
XO|++
OX|XO

```



## Note

<p>Note that the following is an incorrect configuration for the first sample case because the seats must be in the same pair.</p><p><span class="tex-font-style-tt">O+|+X</span></p><p><span class="tex-font-style-tt">XO|XX</span></p><p><span class="tex-font-style-tt">OX|OO</span></p><p><span class="tex-font-style-tt">XX|OX</span></p><p><span class="tex-font-style-tt">OO|OO</span></p><p><span class="tex-font-style-tt">OO|XX</span></p>
