## Description

<div><p>You are given <span class="tex-span"><i>n</i></span> switches and <span class="tex-span"><i>m</i></span> lamps. The <span class="tex-span"><i>i</i></span>-th switch turns on some subset of the lamps. This information is given as the matrix <span class="tex-span"><i>a</i></span> consisting of <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>m</i></span> columns where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> = 1</span> if the <span class="tex-span"><i>i</i></span>-th switch turns on the <span class="tex-span"><i>j</i></span>-th lamp and <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> = 0</span> if the <span class="tex-span"><i>i</i></span>-th switch is not connected to the <span class="tex-span"><i>j</i></span>-th lamp.</p><p>Initially all <span class="tex-span"><i>m</i></span> lamps are turned off.</p><p>Switches change state only from "off" to "on". It means that if you press two or more switches connected to the same lamp then the lamp will be turned on after any of this switches is pressed and will remain its state even if any switch connected to this lamp is pressed afterwards.</p><p>It is guaranteed that if you push all <span class="tex-span"><i>n</i></span> switches then <span class="tex-font-style-bf">all <span class="tex-span"><i>m</i></span> lamps will be turned on</span>.</p><p>Your think that you have too many switches and you would like to ignore one of them. </p><p>Your task is to say if there exists such a switch that if you will ignore (not use) it but press all the other <span class="tex-span"><i>n</i> - 1</span> switches then all the <span class="tex-span"><i>m</i></span> lamps will be turned on.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 2000</span>) — the number of the switches and the number of the lamps.</p><p>The following <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> characters each. The character <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> is equal to '<span class="tex-font-style-tt">1</span>' if the <span class="tex-span"><i>i</i></span>-th switch turns on the <span class="tex-span"><i>j</i></span>-th lamp and '<span class="tex-font-style-tt">0</span>' otherwise.</p><p>It is guaranteed that if you press all <span class="tex-span"><i>n</i></span> switches <span class="tex-font-style-bf">all <span class="tex-span"><i>m</i></span> lamps will be turned on</span>.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">YES</span>" if there is a switch that if you will ignore it and press all the other <span class="tex-span"><i>n</i> - 1</span> switches then all <span class="tex-span"><i>m</i></span> lamps will be turned on. Print "<span class="tex-font-style-tt">NO</span>" if there is no such switch.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 2000</span>) — the number of the switches and the number of the lamps.</p><p>The following <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> characters each. The character <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> is equal to '<span class="tex-font-style-tt">1</span>' if the <span class="tex-span"><i>i</i></span>-th switch turns on the <span class="tex-span"><i>j</i></span>-th lamp and '<span class="tex-font-style-tt">0</span>' otherwise.</p><p>It is guaranteed that if you press all <span class="tex-span"><i>n</i></span> switches <span class="tex-font-style-bf">all <span class="tex-span"><i>m</i></span> lamps will be turned on</span>.</p>

## Output

<p>Print "<span class="tex-font-style-tt">YES</span>" if there is a switch that if you will ignore it and press all the other <span class="tex-span"><i>n</i> - 1</span> switches then all <span class="tex-span"><i>m</i></span> lamps will be turned on. Print "<span class="tex-font-style-tt">NO</span>" if there is no such switch.</p>





```input1
4 5
10101
01000
00111
10000

```




```input2
4 5
10100
01000
00110
00101

```




```output1
YES

```




```output2
NO

```


