## Description

<div><p>Today, Wet Shark is given <span class="tex-span"><i>n</i></span> integers. Using any of these integers no more than once, Wet Shark wants to get maximum possible even (divisible by <span class="tex-span">2</span>) sum. Please, calculate this value for Wet Shark. </p><p>Note, that if Wet Shark uses no integers from the <span class="tex-span"><i>n</i></span> integers, the sum is an even integer <span class="tex-span">0</span>.</p></div><div class="input-specification"><p>The first line of the input contains one integer, <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>). The next line contains <span class="tex-span"><i>n</i></span> space separated integers given to Wet Shark. Each of these integers is in range from <span class="tex-span">1</span> to <span class="tex-span">10<sup class="upper-index">9</sup></span>, inclusive. </p></div><div class="output-specification"><p>Print the maximum possible even sum that can be obtained if we use some of the given integers. </p></div>

## Input

<p>The first line of the input contains one integer, <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>). The next line contains <span class="tex-span"><i>n</i></span> space separated integers given to Wet Shark. Each of these integers is in range from <span class="tex-span">1</span> to <span class="tex-span">10<sup class="upper-index">9</sup></span>, inclusive. </p>

## Output

<p>Print the maximum possible even sum that can be obtained if we use some of the given integers. </p>





```input1
3
1 2 3

```




```input2
5
999999999 999999999 999999999 999999999 999999999

```




```output1
6
```




```output2
3999999996
```



## Note

<p>In the first sample, we can simply take all three integers for a total sum of <span class="tex-span">6</span>.</p><p>In the second sample Wet Shark should take any four out of five integers <span class="tex-span">999 999 999</span>.</p>
