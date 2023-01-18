## Description

<div><p>You are given a broken clock. You know, that it is supposed to show time in 12- or 24-hours <span class="tex-font-style-tt">HH:MM</span> format. In 12-hours format hours change from <span class="tex-span">1</span> to <span class="tex-span">12</span>, while in 24-hours it changes from <span class="tex-span">0</span> to <span class="tex-span">23</span>. In both formats minutes change from <span class="tex-span">0</span> to <span class="tex-span">59</span>.</p><p>You are given a time in format <span class="tex-font-style-tt">HH:MM</span> that is currently displayed on the broken clock. Your goal is to change minimum number of digits in order to make clocks display the correct time in the given format.</p><p>For example, if <span class="tex-font-style-tt">00:99</span> is displayed, it is enough to replace the second <span class="tex-font-style-tt">9</span> with <span class="tex-font-style-tt">3</span> in order to get <span class="tex-font-style-tt">00:39</span> that is a correct time in 24-hours format. However, to make <span class="tex-font-style-tt">00:99</span> correct in 12-hours format, one has to change at least two digits. Additionally to the first change one can replace the second <span class="tex-font-style-tt">0</span> with <span class="tex-font-style-tt">1</span> and obtain <span class="tex-font-style-tt">01:39</span>.</p></div><div class="input-specification"><p>The first line of the input contains one integer <span class="tex-span">12</span> or <span class="tex-span">24</span>, that denote 12-hours or 24-hours format respectively.</p><p>The second line contains the time in format <span class="tex-font-style-tt">HH:MM</span>, that is currently displayed on the clock. First two characters stand for the hours, while next two show the minutes.</p></div><div class="output-specification"><p>The only line of the output should contain the time in format <span class="tex-font-style-tt">HH:MM</span> that is a correct time in the given format. It should differ from the original in as few positions as possible. If there are many optimal solutions you can print any of them.</p></div>

## Input

<p>The first line of the input contains one integer <span class="tex-span">12</span> or <span class="tex-span">24</span>, that denote 12-hours or 24-hours format respectively.</p><p>The second line contains the time in format <span class="tex-font-style-tt">HH:MM</span>, that is currently displayed on the clock. First two characters stand for the hours, while next two show the minutes.</p>

## Output

<p>The only line of the output should contain the time in format <span class="tex-font-style-tt">HH:MM</span> that is a correct time in the given format. It should differ from the original in as few positions as possible. If there are many optimal solutions you can print any of them.</p>





```input1
24
17:30

```




```input2
12
17:30

```




```input3
24
99:99

```




```output1
17:30

```




```output2
07:30

```




```output3
09:09

```


