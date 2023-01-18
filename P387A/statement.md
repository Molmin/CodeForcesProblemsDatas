## Description

<div><p>George woke up and saw the current time <span class="tex-span"><i>s</i></span> on the digital clock. Besides, George knows that he has slept for time <span class="tex-span"><i>t</i></span>. </p><p>Help George! Write a program that will, given time <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span>, determine the time <span class="tex-span"><i>p</i></span> when George went to bed. Note that George could have gone to bed yesterday relatively to the current time (see the second test sample). </p></div><div class="input-specification"><p>The first line contains current time <span class="tex-span"><i>s</i></span> as a string in the format "<span class="tex-font-style-tt">hh:mm</span>". The second line contains time <span class="tex-span"><i>t</i></span> in the format "<span class="tex-font-style-tt">hh:mm</span>" — the duration of George's sleep. It is guaranteed that the input contains the correct time in the 24-hour format, that is, <span class="tex-span">00 ≤ <i>hh</i> ≤ 23</span>, <span class="tex-span">00 ≤ <i>mm</i> ≤ 59</span>.</p></div><div class="output-specification"><p>In the single line print time <span class="tex-span"><i>p</i></span> — the time George went to bed in the format similar to the format of the time in the input.</p></div>

## Input

<p>The first line contains current time <span class="tex-span"><i>s</i></span> as a string in the format "<span class="tex-font-style-tt">hh:mm</span>". The second line contains time <span class="tex-span"><i>t</i></span> in the format "<span class="tex-font-style-tt">hh:mm</span>" — the duration of George's sleep. It is guaranteed that the input contains the correct time in the 24-hour format, that is, <span class="tex-span">00 ≤ <i>hh</i> ≤ 23</span>, <span class="tex-span">00 ≤ <i>mm</i> ≤ 59</span>.</p>

## Output

<p>In the single line print time <span class="tex-span"><i>p</i></span> — the time George went to bed in the format similar to the format of the time in the input.</p>





```input1
05:50
05:44

```




```input2
00:00
01:00

```




```input3
00:01
00:00

```




```output1
00:06

```




```output2
23:00

```




```output3
00:01

```



## Note

<p>In the first sample George went to bed at "<span class="tex-font-style-tt">00:06</span>". Note that you should print the time only in the format "<span class="tex-font-style-tt">00:06</span>". That's why answers "<span class="tex-font-style-tt">0:06</span>", "<span class="tex-font-style-tt">00:6</span>" and others will be considered incorrect. </p><p>In the second sample, George went to bed yesterday.</p><p>In the third sample, George didn't do to bed at all.</p>
