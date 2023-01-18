## Description

<div><p>Little Artem found a grasshopper. He brought it to his house and constructed a jumping area for him.</p><p>The area looks like a strip of cells <span class="tex-span">1 × <i>n</i></span>. Each cell contains the direction for the next jump and the length of that jump. Grasshopper starts in the first cell and follows the instructions written on the cells. Grasshopper stops immediately if it jumps out of the strip. Now Artem wants to find out if this will ever happen.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— length of the strip. </p><p>Next line contains a string of length <span class="tex-span"><i>n</i></span> which consists of characters "<span class="tex-font-style-tt">&lt;</span>" and "<span class="tex-font-style-tt">&gt;</span>" only, that provide the direction of the jump from the corresponding cell. Next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the length of the jump from the <span class="tex-span"><i>i</i></span>-th cell.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">INFINITE</span>" (without quotes) if grasshopper will continue his jumps forever. Otherwise print "<span class="tex-font-style-tt">FINITE</span>" (without quotes).</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— length of the strip. </p><p>Next line contains a string of length <span class="tex-span"><i>n</i></span> which consists of characters "<span class="tex-font-style-tt">&lt;</span>" and "<span class="tex-font-style-tt">&gt;</span>" only, that provide the direction of the jump from the corresponding cell. Next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the length of the jump from the <span class="tex-span"><i>i</i></span>-th cell.</p>

## Output

<p>Print "<span class="tex-font-style-tt">INFINITE</span>" (without quotes) if grasshopper will continue his jumps forever. Otherwise print "<span class="tex-font-style-tt">FINITE</span>" (without quotes).</p>





```input1
2
&gt;&lt;
1 2

```




```input2
3
&gt;&gt;&lt;
2 1 1

```




```output1
FINITE

```




```output2
INFINITE
```



## Note

<p>In the first sample grasshopper starts from the first cell and jumps to the right on the next cell. When he is in the second cell he needs to jump two cells left so he will jump out of the strip.</p><p>Second sample grasshopper path is <span class="tex-span">1</span> - <span class="tex-span">3</span> - <span class="tex-span">2</span> - <span class="tex-span">3</span> - <span class="tex-span">2</span> - <span class="tex-span">3</span> and so on. The path is infinite.</p>
