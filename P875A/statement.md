## Description

<div><p>Eighth-grader Vova is on duty today in the class. After classes, he went into the office to wash the board, and found on it the number <span class="tex-span"><i>n</i></span>. He asked what is this number and the teacher of mathematics Inna Petrovna answered Vova that <span class="tex-span"><i>n</i></span> is the answer to the arithmetic task for first-graders. In the textbook, a certain <span class="tex-font-style-bf">positive integer</span> <span class="tex-span"><i>x</i></span> was given. The task was to add <span class="tex-span"><i>x</i></span> to the sum of the digits of the number <span class="tex-span"><i>x</i></span> written in decimal numeral system.</p><p>Since the number <span class="tex-span"><i>n</i></span> on the board was small, Vova quickly guessed which <span class="tex-span"><i>x</i></span> could be in the textbook. Now he wants to get a program which will search for arbitrary values of the number <span class="tex-span"><i>n</i></span> for all suitable values of <span class="tex-span"><i>x</i></span> or determine that such <span class="tex-span"><i>x</i></span> does not exist. Write such a program for Vova.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>In the first line print one integer <span class="tex-span"><i>k</i></span>&nbsp;— number of different values of <span class="tex-span"><i>x</i></span> satisfying the condition. </p><p>In next <span class="tex-span"><i>k</i></span> lines print these values in ascending order.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>In the first line print one integer <span class="tex-span"><i>k</i></span>&nbsp;— number of different values of <span class="tex-span"><i>x</i></span> satisfying the condition. </p><p>In next <span class="tex-span"><i>k</i></span> lines print these values in ascending order.</p>





```input1
21

```




```input2
20

```




```output1
1
15

```




```output2
0

```



## Note

<p>In the first test case <span class="tex-span"><i>x</i> = 15</span> there is only one variant: <span class="tex-span">15 + 1 + 5 = 21</span>.</p><p>In the second test case there are no such <span class="tex-span"><i>x</i></span>.</p>
