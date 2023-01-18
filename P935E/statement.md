## Description

<div><p>Ancient Egyptians are known to have understood difficult concepts in mathematics. The ancient Egyptian mathematician Ahmes liked to write a kind of arithmetic expressions on papyrus paper which he called as <span class="tex-font-style-it">Ahmes arithmetic expression</span>.</p><p>An <span class="tex-font-style-it">Ahmes arithmetic expression</span> can be defined as: </p><ul> <li> "<span class="tex-span"><i>d</i></span>" is an Ahmes arithmetic expression, where <span class="tex-span"><i>d</i></span> is a one-digit positive integer; </li><li> "<span class="tex-span">(<i>E</i><sub class="lower-index">1</sub> <i>op</i> <i>E</i><sub class="lower-index">2</sub>)</span>" is an Ahmes arithmetic expression, where <span class="tex-span"><i>E</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>E</i><sub class="lower-index">2</sub></span> are valid Ahmes arithmetic expressions (without spaces) and <span class="tex-span"><i>op</i></span> is either plus <span class="tex-span">( + )</span> or minus <span class="tex-span">( - )</span>. </li></ul> For example <span class="tex-font-style-tt">5</span>, <span class="tex-font-style-tt">(1-1)</span> and <span class="tex-font-style-tt">((1+(2-3))-5)</span> are valid Ahmes arithmetic expressions.<p>On his trip to Egypt, Fafa found a piece of papyrus paper having one of these Ahmes arithmetic expressions written on it. Being very ancient, the papyrus piece was very worn out. As a result, all the operators were erased, keeping only the numbers and the brackets. Since Fafa loves mathematics, he decided to challenge himself with the following task:</p><p>Given the number of plus and minus operators in the original expression, find out the maximum possible value for the expression on the papyrus paper after putting the plus and minus operators in the place of the original erased operators.</p></div><div class="input-specification"><p>The first line contains a string <span class="tex-span"><i>E</i></span> <span class="tex-span">(1 ≤ |<i>E</i>| ≤ 10<sup class="upper-index">4</sup>)</span> — a valid Ahmes arithmetic expression. All operators are erased and replaced with '<span class="tex-font-style-tt">?</span>'.</p><p>The second line contains two space-separated integers <span class="tex-span"><i>P</i></span> and <span class="tex-span"><i>M</i></span> (<span class="tex-span">0 ≤ <i>min</i>(<i>P</i>, <i>M</i>) ≤ 100</span>) — the number of plus and minus operators, respectively. </p><p>It is guaranteed that <span class="tex-span"><i>P</i> + <i>M</i> = </span> the number of erased operators.</p></div><div class="output-specification"><p>Print one line containing the answer to the problem.</p></div>

## Input

<p>The first line contains a string <span class="tex-span"><i>E</i></span> <span class="tex-span">(1 ≤ |<i>E</i>| ≤ 10<sup class="upper-index">4</sup>)</span> — a valid Ahmes arithmetic expression. All operators are erased and replaced with '<span class="tex-font-style-tt">?</span>'.</p><p>The second line contains two space-separated integers <span class="tex-span"><i>P</i></span> and <span class="tex-span"><i>M</i></span> (<span class="tex-span">0 ≤ <i>min</i>(<i>P</i>, <i>M</i>) ≤ 100</span>) — the number of plus and minus operators, respectively. </p><p>It is guaranteed that <span class="tex-span"><i>P</i> + <i>M</i> = </span> the number of erased operators.</p>

## Output

<p>Print one line containing the answer to the problem.</p>





```input1
(1?1)
1 0

```




```input2
(2?(1?2))
1 1

```




```input3
((1?(5?7))?((6?2)?7))
3 2

```




```input4
((1?(5?7))?((6?2)?7))
2 3

```




```output1
2

```




```output2
1

```




```output3
18

```




```output4
16

```



## Note

<ul> <li> The first sample will be <span class="tex-span">(1 + 1)  =  2</span>. </li><li> The second sample will be <span class="tex-span">(2 + (1 - 2))  =  1</span>. </li><li> The third sample will be <span class="tex-span">((1 - (5 - 7)) + ((6 + 2) + 7))  =  18</span>. </li><li> The fourth sample will be <span class="tex-span">((1 + (5 + 7)) - ((6 - 2) - 7))  =  16</span>. </li></ul>
