## Description

<div><p>When new students come to the Specialized Educational and Scientific Centre (SESC) they need to start many things from the beginning. Sometimes the teachers say (not always unfairly) that we cannot even count. So our teachers decided to teach us arithmetics from the start. And what is the best way to teach students add and subtract? — That's right, using counting sticks! An here's our new task: </p><p>An expression of counting sticks is an expression of type:</p><center>[ <span class="tex-span"><i>A</i></span> sticks][sign <span class="tex-font-style-tt">+</span>][<span class="tex-span"><i>B</i></span> sticks][sign <span class="tex-font-style-tt">=</span>][<span class="tex-span"><i>C</i></span> sticks] <span class="tex-span">(1 ≤ <i>A</i>, <i>B</i>, <i>C</i>)</span>.  </center><p>Sign <span class="tex-font-style-tt">+</span> consists of two crossed sticks: one vertical and one horizontal. Sign <span class="tex-font-style-tt">=</span> consists of two horizontal sticks. The expression is arithmetically correct if <span class="tex-span"><i>A</i> + <i>B</i> = <i>C</i></span>.</p><p>We've got an expression that looks like <span class="tex-span"><i>A</i> + <i>B</i> = <i>C</i></span> given by counting sticks. Our task is to shift at most one stick (or we can shift nothing) so that the expression became arithmetically correct. Note that we cannot remove the sticks from the expression, also we cannot shift the sticks from the signs <span class="tex-font-style-tt">+</span> and <span class="tex-font-style-tt">=</span>.</p><p>We really aren't fabulous at arithmetics. Can you help us?</p></div><div class="input-specification"><p>The single line contains the initial expression. It is guaranteed that the expression looks like <span class="tex-span"><i>A</i> + <i>B</i> = <i>C</i></span>, where <span class="tex-span">1 ≤ <i>A</i>, <i>B</i>, <i>C</i> ≤ 100</span>.</p></div><div class="output-specification"><p>If there isn't a way to shift the stick so the expression becomes correct, print on a single line "<span class="tex-font-style-tt">Impossible</span>" (without the quotes). If there is a way, print the resulting expression. Follow the format of the output from the test samples. Don't print extra space characters.</p><p>If there are multiple correct answers, print any of them. For clarifications, you are recommended to see the test samples.</p></div>

## Input

<p>The single line contains the initial expression. It is guaranteed that the expression looks like <span class="tex-span"><i>A</i> + <i>B</i> = <i>C</i></span>, where <span class="tex-span">1 ≤ <i>A</i>, <i>B</i>, <i>C</i> ≤ 100</span>.</p>

## Output

<p>If there isn't a way to shift the stick so the expression becomes correct, print on a single line "<span class="tex-font-style-tt">Impossible</span>" (without the quotes). If there is a way, print the resulting expression. Follow the format of the output from the test samples. Don't print extra space characters.</p><p>If there are multiple correct answers, print any of them. For clarifications, you are recommended to see the test samples.</p>





```input1
||+|=|||||

```




```input2
|||||+||=||

```




```input3
|+|=||||||

```




```input4
||||+||=||||||

```




```output1
|||+|=||||

```




```output2
Impossible

```




```output3
Impossible

```




```output4
||||+||=||||||

```



## Note

<p>In the first sample we can shift stick from the third group of sticks to the first one.</p><p>In the second sample we cannot shift vertical stick from <span class="tex-font-style-tt">+</span> sign to the second group of sticks. So we cannot make a <span class="tex-font-style-tt">-</span> sign.</p><p>There is no answer in the third sample because we cannot remove sticks from the expression.</p><p>In the forth sample the initial expression is already arithmetically correct and that is why we don't have to shift sticks.</p>
