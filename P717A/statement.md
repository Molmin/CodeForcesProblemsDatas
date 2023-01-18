## Description

<div><p>The Prodiggers are quite a cool band and for this reason, they have been the surprise guest at the ENTER festival for the past 80 years. At the beginning of their careers, they weren’t so successful, so they had to spend time digging channels to earn money; hence the name. Anyway, they like to tour a lot and have surprising amounts of energy to do extremely long tours. However, they hate spending two consecutive days without having a concert, so they would like to avoid it.</p><p>A <span class="tex-font-style-it">tour</span> is defined by a sequence of concerts and days-off. You need to count in how many ways The Prodiggers can select <span class="tex-span"><i>k</i></span> different tours of the same length between <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span>.</p><p>For example if <span class="tex-span"><i>k</i> = 2</span>, <span class="tex-span"><i>l</i> = 1</span> and <span class="tex-span"><i>r</i> = 2</span>, if we define concert day as {1} and day-off as {0}, here are all possible tours: {0}, {1}, {00}, {01}, {10}, {11}. But tour 00 can not be selected because it has <span class="tex-span">2</span> days-off in a row. Now, we need to count in how many ways we can select <span class="tex-span"><i>k</i> = 2</span> tours <span class="tex-font-style-bf">of the same length</span> in range <span class="tex-span">[1;2]</span>. Here they are: {0,1}; {01,10}; {01,11}; {10,11}.</p><p>Since their schedule is quite busy, they want you to tell them in how many ways can do that, modulo <span class="tex-span">1 000 000 007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p></div><div class="input-specification"><p>The first line of the input contains three integers <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 200</span>, <span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">18</sup></span>).</p></div><div class="output-specification"><p>Output a single number: the number of ways to select <span class="tex-span"><i>k</i></span> different tours of the same length, modulo <span class="tex-span">1 000 000 007</span>.</p></div>

## Input

<p>The first line of the input contains three integers <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 200</span>, <span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">18</sup></span>).</p>

## Output

<p>Output a single number: the number of ways to select <span class="tex-span"><i>k</i></span> different tours of the same length, modulo <span class="tex-span">1 000 000 007</span>.</p>





```input1
1 1 2

```




```output1
5

```


