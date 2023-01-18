## Description

<div><p>There are <span class="tex-span"><i>b</i></span> blocks of digits. Each one consisting of the same <span class="tex-span"><i>n</i></span> digits, which are given to you in the input. Wet Shark must choose <span class="tex-font-style-bf">exactly one</span> digit from each block and concatenate all of those digits together to form one large integer. For example, if he chooses digit <span class="tex-span">1</span> from the first block and digit <span class="tex-span">2</span> from the second block, he gets the integer <span class="tex-span">12</span>. </p><p>Wet Shark then takes this number modulo <span class="tex-span"><i>x</i></span>. Please, tell him how many ways he can choose one digit from each block so that he gets exactly <span class="tex-span"><i>k</i></span> as the final result. As this number may be too large, print it modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p><p>Note, that the number of ways to choose some digit in the block is equal to the number of it's occurrences. For example, there are <span class="tex-span">3</span> ways to choose digit <span class="tex-span">5</span> from block <span class="tex-font-style-tt">3 5 6 7 8 9 5 1 1 1 1 5</span>.</p></div><div class="input-specification"><p>The first line of the input contains four space-separated integers, <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>x</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 50 000, 1 ≤ <i>b</i> ≤ 10<sup class="upper-index">9</sup>, 0 ≤ <i>k</i> &lt; <i>x</i> ≤ 100, <i>x</i> ≥ 2</span>)&nbsp;— the number of digits in one block, the number of blocks, interesting remainder modulo <span class="tex-span"><i>x</i></span> and modulo <span class="tex-span"><i>x</i></span> itself.</p><p>The next line contains <span class="tex-span"><i>n</i></span> space separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 9</span>), that give the digits contained in each block.</p></div><div class="output-specification"><p>Print the number of ways to pick exactly one digit from each blocks, such that the resulting integer equals <span class="tex-span"><i>k</i></span> modulo <span class="tex-span"><i>x</i></span>.</p></div>

## Input

<p>The first line of the input contains four space-separated integers, <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>x</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 50 000, 1 ≤ <i>b</i> ≤ 10<sup class="upper-index">9</sup>, 0 ≤ <i>k</i> &lt; <i>x</i> ≤ 100, <i>x</i> ≥ 2</span>)&nbsp;— the number of digits in one block, the number of blocks, interesting remainder modulo <span class="tex-span"><i>x</i></span> and modulo <span class="tex-span"><i>x</i></span> itself.</p><p>The next line contains <span class="tex-span"><i>n</i></span> space separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 9</span>), that give the digits contained in each block.</p>

## Output

<p>Print the number of ways to pick exactly one digit from each blocks, such that the resulting integer equals <span class="tex-span"><i>k</i></span> modulo <span class="tex-span"><i>x</i></span>.</p>





```input1
12 1 5 10
3 5 6 7 8 9 5 1 1 1 1 5

```




```input2
3 2 1 2
6 2 2

```




```input3
3 2 1 2
3 1 2

```




```output1
3

```




```output2
0

```




```output3
6

```



## Note

<p>In the second sample possible integers are <span class="tex-span">22</span>, <span class="tex-span">26</span>, <span class="tex-span">62</span> and <span class="tex-span">66</span>. None of them gives the remainder <span class="tex-span">1</span> modulo <span class="tex-span">2</span>.</p><p>In the third sample integers <span class="tex-span">11</span>, <span class="tex-span">13</span>, <span class="tex-span">21</span>, <span class="tex-span">23</span>, <span class="tex-span">31</span> and <span class="tex-span">33</span> have remainder <span class="tex-span">1</span> modulo <span class="tex-span">2</span>. There is exactly one way to obtain each of these integers, so the total answer is <span class="tex-span">6</span>.</p>
