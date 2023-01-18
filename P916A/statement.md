## Description

<div><p>Jamie loves sleeping. One day, he decides that he needs to wake up at exactly <span class="tex-span"><i>hh</i>: <i>mm</i></span>. However, he hates waking up, so he wants to make waking up less painful by setting the alarm at a <span class="tex-font-style-tt">lucky</span> time. He will then press the snooze button every <span class="tex-span"><i>x</i></span> minutes until <span class="tex-span"><i>hh</i>: <i>mm</i></span> is reached, and only then he will wake up. He wants to know what is the smallest number of times he needs to press the snooze button.</p><p>A time is considered <span class="tex-font-style-tt">lucky</span> if it contains a digit '<span class="tex-span">7</span>'. For example, <span class="tex-span">13: 07</span> and <span class="tex-span">17: 27</span> are <span class="tex-font-style-tt">lucky</span>, while <span class="tex-span">00: 48</span> and <span class="tex-span">21: 34</span> are not <span class="tex-font-style-tt">lucky</span>.</p><p>Note that it is not necessary that the time set for the alarm and the wake-up time are on the same day. It is guaranteed that there is a <span class="tex-font-style-tt">lucky</span> time Jamie can set so that he can wake at <span class="tex-span"><i>hh</i>: <i>mm</i></span>.</p><p>Formally, find the smallest possible non-negative integer <span class="tex-span"><i>y</i></span> such that the time representation of the time <span class="tex-span"><i>x</i>·<i>y</i></span> minutes before <span class="tex-span"><i>hh</i>: <i>mm</i></span> contains the digit '<span class="tex-span">7</span>'.</p><p>Jamie uses 24-hours clock, so after <span class="tex-span">23: 59</span> comes <span class="tex-span">00: 00</span>.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ 60</span>).</p><p>The second line contains two two-digit integers, <span class="tex-span"><i>hh</i></span> and <span class="tex-span"><i>mm</i></span> (<span class="tex-span">00 ≤ <i>hh</i> ≤ 23, 00 ≤ <i>mm</i> ≤ 59</span>).</p></div><div class="output-specification"><p>Print the minimum number of times he needs to press the button.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ 60</span>).</p><p>The second line contains two two-digit integers, <span class="tex-span"><i>hh</i></span> and <span class="tex-span"><i>mm</i></span> (<span class="tex-span">00 ≤ <i>hh</i> ≤ 23, 00 ≤ <i>mm</i> ≤ 59</span>).</p>

## Output

<p>Print the minimum number of times he needs to press the button.</p>





```input1
3
11 23

```




```input2
5
01 07

```




```output1
2

```




```output2
0

```



## Note

<p>In the first sample, Jamie needs to wake up at 11:23. So, he can set his alarm at 11:17. He would press the snooze button when the alarm rings at 11:17 and at 11:20.</p><p>In the second sample, Jamie can set his alarm at exactly at 01:07 which is <span class="tex-font-style-tt">lucky</span>.</p>
