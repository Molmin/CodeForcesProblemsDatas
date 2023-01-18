## Description

<div><p>Malek lives in an apartment block with <span class="tex-span">100</span> floors numbered from <span class="tex-span">0</span> to <span class="tex-span">99</span>. The apartment has an elevator with a digital counter showing the floor that the elevator is currently on. The elevator shows each digit of a number with <span class="tex-span">7</span> light sticks by turning them on or off. The picture below shows how the elevator shows each digit.</p><center><img class="tex-graphics" src="file://4Ey4ZcL2.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>One day when Malek wanted to go from floor <span class="tex-span">88</span> to floor <span class="tex-span">0</span> using the elevator he noticed that the counter shows number <span class="tex-span">89</span> instead of <span class="tex-span">88</span>. Then when the elevator started moving the number on the counter changed to <span class="tex-span">87</span>. After a little thinking Malek came to the conclusion that there is only one explanation for this: One of the sticks of the counter was broken. Later that day Malek was thinking about the broken stick and suddenly he came up with the following problem.</p><p>Suppose the digital counter is showing number <span class="tex-span"><i>n</i></span>. Malek calls an integer <span class="tex-span"><i>x</i></span> (<span class="tex-span">0 ≤ <i>x</i> ≤ 99</span>) <span class="tex-font-style-underline">good</span> if it's possible that the digital counter was supposed to show <span class="tex-span"><i>x</i></span> but because of some(possibly none) broken sticks it's showing <span class="tex-span"><i>n</i></span> instead. Malek wants to know number of good integers for a specific <span class="tex-span"><i>n</i></span>. So you must write a program that calculates this number. Please note that the counter <span class="tex-font-style-bf">always</span> shows two digits.</p></div><div class="input-specification"><p>The only line of input contains exactly two digits representing number <span class="tex-span"><i>n</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 99</span>). Note that <span class="tex-span"><i>n</i></span> may have a leading zero.</p></div><div class="output-specification"><p>In the only line of the output print the number of good integers.</p></div>

## Input

<p>The only line of input contains exactly two digits representing number <span class="tex-span"><i>n</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 99</span>). Note that <span class="tex-span"><i>n</i></span> may have a leading zero.</p>

## Output

<p>In the only line of the output print the number of good integers.</p>





```input1
89

```




```input2
00

```




```input3
73

```




```output1
2

```




```output2
4

```




```output3
15

```



## Note

<p>In the first sample the counter may be supposed to show <span class="tex-span">88</span> or <span class="tex-span">89</span>.</p><p>In the second sample the good integers are <span class="tex-span">00</span>, <span class="tex-span">08</span>, <span class="tex-span">80</span> and <span class="tex-span">88</span>.</p><p><span class="tex-font-style-bf">In the third sample the good integers are <span class="tex-span">03, 08, 09, 33, 38, 39, 73, 78, 79, 83, 88, 89, 93, 98, 99</span></span>.</p>
