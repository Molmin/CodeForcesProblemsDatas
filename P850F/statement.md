## Description

<div><p>You have a bag of balls of <span class="tex-span"><i>n</i></span> different colors. You have <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> balls of the <span class="tex-span"><i>i</i></span>-th color.</p><p>While there are at least two different colored balls in the bag, perform the following steps: </p><ul> <li> Take out two random balls without replacement one by one. These balls might be the same color. </li><li> Color the second ball to the color of the first ball. You are not allowed to switch the order of the balls in this step. </li><li> Place both balls back in the bag. </li><li> All these actions take exactly one second. </li></ul><p>Let <span class="tex-span"><i>M</i> = 10<sup class="upper-index">9</sup> + 7</span>. It can be proven that the expected amount of time needed before you stop can be represented as a rational number <img align="middle" class="tex-formula" src="file://j6kzFfgK.png" style="max-width: 100.0%;max-height: 100.0%;">, where <span class="tex-span"><i>P</i></span> and <span class="tex-span"><i>Q</i></span> are coprime integers and where <span class="tex-span"><i>Q</i></span> is not divisible by <span class="tex-span"><i>M</i></span>. Return the value <img align="middle" class="tex-formula" src="file://u3F8Ezcf.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div><div class="input-specification"><p>The first line of input will contain a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2 500</span>)&nbsp;— the number of colors.</p><p>The next line of input will contain <span class="tex-span"><i>n</i></span> space separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of balls of each color.</p></div><div class="output-specification"><p>Print a single integer, the answer to the problem.</p></div>

## Input

<p>The first line of input will contain a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2 500</span>)&nbsp;— the number of colors.</p><p>The next line of input will contain <span class="tex-span"><i>n</i></span> space separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of balls of each color.</p>

## Output

<p>Print a single integer, the answer to the problem.</p>





```input1
2
1 1

```




```input2
3
1 2 3

```




```output1
1

```




```output2
750000026

```



## Note

<p>In the first sample, no matter what happens, the balls will become the same color after one step.</p><p>For the second sample, we have 6 balls. Let’s label the balls from 1 to 6, and without loss of generality, let’s say balls 1,2,3 are initially color 1, balls 4,5 are color 2, and ball 6 are color 3.</p><p>Here is an example of how these steps can go: </p><ul> <li> We choose ball 5 and ball 6. Ball 6 then becomes color 2. </li><li> We choose ball 4 and ball 5. Ball 5 remains the same color (color 2). </li><li> We choose ball 1 and ball 5. Ball 5 becomes color 1. </li><li> We choose ball 6 and ball 5. Ball 5 becomes color 2. </li><li> We choose ball 3 and ball 4. Ball 4 becomes color 1. </li><li> We choose ball 4 and ball 6. Ball 6 becomes color 1. </li><li> We choose ball 2 and ball 5. Ball 5 becomes color 1. </li></ul> At this point, the game ends since all the balls are the same color. This particular sequence took 7 seconds.<p>It can be shown that the answer to this case is <img align="middle" class="tex-formula" src="file://yT1HwW1T.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
