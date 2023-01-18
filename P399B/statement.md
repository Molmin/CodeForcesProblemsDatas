## Description

<div><p>User ainta has a stack of <span class="tex-span"><i>n</i></span> red and blue balls. He can apply a certain operation which changes the colors of the balls inside the stack.</p><ul> <li> While the top ball inside the stack is red, pop the ball from the top of the stack. </li><li> Then replace the blue ball on the top with a red ball. </li><li> And finally push some blue balls to the stack until the stack has total of <span class="tex-span"><i>n</i></span> balls inside. </li></ul> &nbsp;<p>If there are no blue balls inside the stack, ainta can't apply this operation. Given the initial state of the stack, ainta wants to know the maximum number of operations he can repeatedly apply.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>) — the number of balls inside the stack.</p><p>The second line contains a string <span class="tex-span"><i>s</i></span> (<span class="tex-span">|<i>s</i>| = <i>n</i></span>) describing the initial state of the stack. The <span class="tex-span"><i>i</i></span>-th character of the string <span class="tex-span"><i>s</i></span> denotes the color of the <span class="tex-span"><i>i</i></span>-th ball (we'll number the balls from top to bottom of the stack). If the character is "<span class="tex-font-style-tt">R</span>", the color is red. If the character is "<span class="tex-font-style-tt">B</span>", the color is blue.</p></div><div class="output-specification"><p>Print the maximum number of operations ainta can repeatedly apply.</p><p>Please, do not write the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>) — the number of balls inside the stack.</p><p>The second line contains a string <span class="tex-span"><i>s</i></span> (<span class="tex-span">|<i>s</i>| = <i>n</i></span>) describing the initial state of the stack. The <span class="tex-span"><i>i</i></span>-th character of the string <span class="tex-span"><i>s</i></span> denotes the color of the <span class="tex-span"><i>i</i></span>-th ball (we'll number the balls from top to bottom of the stack). If the character is "<span class="tex-font-style-tt">R</span>", the color is red. If the character is "<span class="tex-font-style-tt">B</span>", the color is blue.</p>

## Output

<p>Print the maximum number of operations ainta can repeatedly apply.</p><p>Please, do not write the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
3
RBR

```




```input2
4
RBBR

```




```input3
5
RBBRR

```




```output1
2

```




```output2
6

```




```output3
6

```



## Note

<p>The first example is depicted below.</p><p>The explanation how user ainta applies the first operation. He pops out one red ball, changes the color of the ball in the middle from blue to red, and pushes one blue ball.</p><center> <img class="tex-graphics" src="file://rd8CBhw4.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The explanation how user ainta applies the second operation. He will not pop out red balls, he simply changes the color of the ball on the top from blue to red.</p><center> <img class="tex-graphics" src="file://m4SiaFtG.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>From now on, ainta can't apply any operation because there are no blue balls inside the stack. ainta applied two operations, so the answer is 2.</p><p>The second example is depicted below. The blue arrow denotes a single operation.</p><center> <img class="tex-graphics" src="file://iQs76xVr.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
