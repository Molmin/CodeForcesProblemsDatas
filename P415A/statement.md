## Description

<div><p>Mashmokh works in a factory. At the end of each day he must turn off all of the lights. </p><p>The lights on the factory are indexed from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. There are <span class="tex-span"><i>n</i></span> buttons in Mashmokh's room indexed from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> as well. If Mashmokh pushes button with index <span class="tex-span"><i>i</i></span>, then each light with index not less than <span class="tex-span"><i>i</i></span> that is still turned on turns off.</p><p>Mashmokh is not very clever. So instead of pushing the first button he pushes some of the buttons randomly each night. He pushed <span class="tex-span"><i>m</i></span> distinct buttons <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub></span> (the buttons were pushed consecutively in the given order) this night. Now he wants to know for each light the index of the button that turned this light off. Please note that the index of button <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> is actually <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, not <span class="tex-span"><i>i</i></span>.</p><p>Please, help Mashmokh, print these indices.</p></div><div class="input-specification"><p>The first line of the input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 100)</span>, the number of the factory lights and the pushed buttons respectively. The next line contains <span class="tex-span"><i>m</i></span> distinct space-separated integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub>&nbsp;(1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>.</p><p>It is guaranteed that all lights will be turned off after pushing all buttons.</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>n</i></span> space-separated integers where the <span class="tex-span"><i>i</i></span>-th number is index of the button that turns the <span class="tex-span"><i>i</i></span>-th light off.</p></div>

## Input

<p>The first line of the input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 100)</span>, the number of the factory lights and the pushed buttons respectively. The next line contains <span class="tex-span"><i>m</i></span> distinct space-separated integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub>&nbsp;(1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>.</p><p>It is guaranteed that all lights will be turned off after pushing all buttons.</p>

## Output

<p>Output <span class="tex-span"><i>n</i></span> space-separated integers where the <span class="tex-span"><i>i</i></span>-th number is index of the button that turns the <span class="tex-span"><i>i</i></span>-th light off.</p>





```input1
5 4
4 3 1 2

```




```input2
5 5
5 4 3 2 1

```




```output1
1 1 3 4 4 

```




```output2
1 2 3 4 5 

```



## Note

<p>In the first sample, after pressing button number 4, lights 4 and 5 are turned off and lights 1, 2 and 3 are still on. Then after pressing button number 3, light number 3 is turned off as well. Pressing button number 1 turns off lights number 1 and 2 as well so pressing button number 2 in the end has no effect. Thus button number 4 turned lights 4 and 5 off, button number 3 turned light 3 off and button number 1 turned light 1 and 2 off.</p>
