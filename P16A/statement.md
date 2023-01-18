## Description

<div><p>According to a new ISO standard, a flag of every country should have a chequered field <span class="tex-span"><i>n</i> × <i>m</i></span>, each square should be of one of 10 colours, and the flag should be «striped»: each horizontal row of the flag should contain squares of the same colour, and the colours of adjacent horizontal rows should be different. Berland's government asked you to find out whether their flag meets the new ISO standard.</p></div><div class="input-specification"><p>The first line of the input contains numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>), <span class="tex-span"><i>n</i></span> — the amount of rows, <span class="tex-span"><i>m</i></span> — the amount of columns on the flag of Berland. Then there follows the description of the flag: each of the following <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> characters. Each character is a digit between <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">9</span>, and stands for the colour of the corresponding square.</p></div><div class="output-specification"><p>Output <span class="tex-font-style-tt">YES</span>, if the flag meets the new ISO standard, and <span class="tex-font-style-tt">NO</span> otherwise.</p></div>

## Input

<p>The first line of the input contains numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>), <span class="tex-span"><i>n</i></span> — the amount of rows, <span class="tex-span"><i>m</i></span> — the amount of columns on the flag of Berland. Then there follows the description of the flag: each of the following <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> characters. Each character is a digit between <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">9</span>, and stands for the colour of the corresponding square.</p>

## Output

<p>Output <span class="tex-font-style-tt">YES</span>, if the flag meets the new ISO standard, and <span class="tex-font-style-tt">NO</span> otherwise.</p>





```input1
3 3
000
111
222

```




```input2
3 3
000
000
111

```




```input3
3 3
000
111
002

```




```output1
YES

```




```output2
NO

```




```output3
NO

```


