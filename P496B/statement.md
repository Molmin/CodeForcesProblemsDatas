## Description

<div><p>You got a box with a combination lock. The lock has a display showing <span class="tex-span"><i>n</i></span> digits. There are two buttons on the box, each button changes digits on the display. You have quickly discovered that the first button adds 1 to all the digits (all digits 9 become digits 0), and the second button shifts all the digits on the display one position to the right (the last digit becomes the first one). For example, if the display is currently showing number <span class="tex-font-style-tt">579</span>, then if we push the first button, the display will show <span class="tex-font-style-tt">680</span>, and if after that we push the second button, the display will show <span class="tex-font-style-tt">068</span>.</p><p>You know that the lock will open if the display is showing the smallest possible number that can be obtained by pushing the buttons in some order. The leading zeros are ignored while comparing numbers. Now your task is to find the desired number.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>)&nbsp;— the number of digits on the display.</p><p>The second line contains <span class="tex-span"><i>n</i></span> digits&nbsp;— the initial state of the display.</p></div><div class="output-specification"><p>Print a single line containing <span class="tex-span"><i>n</i></span> digits&nbsp;— the desired state of the display containing the smallest possible number.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>)&nbsp;— the number of digits on the display.</p><p>The second line contains <span class="tex-span"><i>n</i></span> digits&nbsp;— the initial state of the display.</p>

## Output

<p>Print a single line containing <span class="tex-span"><i>n</i></span> digits&nbsp;— the desired state of the display containing the smallest possible number.</p>





```input1
3
579

```




```input2
4
2014

```




```output1
024

```




```output2
0142

```


