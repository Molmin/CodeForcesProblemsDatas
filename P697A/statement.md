## Description

<div><p>Ted has a pineapple. This pineapple is able to bark like a bulldog! At time <span class="tex-span"><i>t</i></span> (in seconds) it barks for the first time. Then every <span class="tex-span"><i>s</i></span> seconds after it, it barks twice with <span class="tex-span">1</span> second interval. Thus it barks at times <span class="tex-span"><i>t</i></span>, <span class="tex-span"><i>t</i> + <i>s</i></span>, <span class="tex-span"><i>t</i> + <i>s</i> + 1</span>, <span class="tex-span"><i>t</i> + 2<i>s</i></span>, <span class="tex-span"><i>t</i> + 2<i>s</i> + 1</span>, etc.</p><center> <img class="tex-graphics" src="file://FZ5TKrdi.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Barney woke up in the morning and wants to eat the pineapple, but he can't eat it when it's barking. Barney plans to eat it at time <span class="tex-span"><i>x</i></span> (in seconds), so he asked you to tell him if it's gonna bark at that time.</p></div><div class="input-specification"><p>The first and only line of input contains three integers <span class="tex-span"><i>t</i></span>, <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>x</i></span> (<span class="tex-span">0 ≤ <i>t</i>, <i>x</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">2 ≤ <i>s</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the time the pineapple barks for the first time, the pineapple barking interval, and the time Barney wants to eat the pineapple respectively.</p></div><div class="output-specification"><p>Print a single "YES" (without quotes) if the pineapple will bark at time <span class="tex-span"><i>x</i></span> or a single "NO" (without quotes) otherwise in the only line of output.</p></div>

## Input

<p>The first and only line of input contains three integers <span class="tex-span"><i>t</i></span>, <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>x</i></span> (<span class="tex-span">0 ≤ <i>t</i>, <i>x</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">2 ≤ <i>s</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the time the pineapple barks for the first time, the pineapple barking interval, and the time Barney wants to eat the pineapple respectively.</p>

## Output

<p>Print a single "YES" (without quotes) if the pineapple will bark at time <span class="tex-span"><i>x</i></span> or a single "NO" (without quotes) otherwise in the only line of output.</p>





```input1
3 10 4

```




```input2
3 10 3

```




```input3
3 8 51

```




```input4
3 8 52

```




```output1
NO

```




```output2
YES

```




```output3
YES

```




```output4
YES

```



## Note

<p>In the first and the second sample cases pineapple will bark at moments <span class="tex-span">3</span>, <span class="tex-span">13</span>, <span class="tex-span">14</span>, ..., so it won't bark at the moment <span class="tex-span">4</span> and will bark at the moment <span class="tex-span">3</span>.</p><p>In the third and fourth sample cases pineapple will bark at moments <span class="tex-span">3</span>, <span class="tex-span">11</span>, <span class="tex-span">12</span>, <span class="tex-span">19</span>, <span class="tex-span">20</span>, <span class="tex-span">27</span>, <span class="tex-span">28</span>, <span class="tex-span">35</span>, <span class="tex-span">36</span>, <span class="tex-span">43</span>, <span class="tex-span">44</span>, <span class="tex-span">51</span>, <span class="tex-span">52</span>, <span class="tex-span">59</span>, ..., so it will bark at both moments <span class="tex-span">51</span> and <span class="tex-span">52</span>.</p>
