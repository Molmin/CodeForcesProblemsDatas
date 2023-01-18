## Description

<div><p>Vasya has found a strange device. On the front panel of a device there are: a red button, a blue button and a display showing some positive integer. After clicking the red button, device multiplies the displayed number by two. After clicking the blue button, device subtracts one from the number on the display. If at some point the number stops being positive, the device breaks down. The display can show arbitrarily large numbers. Initially, the display shows number <span class="tex-span"><i>n</i></span>.</p><p>Bob wants to get number <span class="tex-span"><i>m</i></span> on the display. What minimum number of clicks he has to make in order to achieve this result?</p></div><div class="input-specification"><p>The first and the only line of the input contains two distinct integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">4</sup></span>), separated by a space .</p></div><div class="output-specification"><p>Print a single number — the minimum number of times one needs to push the button required to get the number <span class="tex-span"><i>m</i></span> out of number <span class="tex-span"><i>n</i></span>.</p></div>

## Input

<p>The first and the only line of the input contains two distinct integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">4</sup></span>), separated by a space .</p>

## Output

<p>Print a single number — the minimum number of times one needs to push the button required to get the number <span class="tex-span"><i>m</i></span> out of number <span class="tex-span"><i>n</i></span>.</p>





```input1
4 6

```




```input2
10 1

```




```output1
2

```




```output2
9

```



## Note

<p>In the first example you need to push the blue button once, and then push the red button once.</p><p>In the second example, doubling the number is unnecessary, so we need to push the blue button nine times.</p>
