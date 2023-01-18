## Description

<div><p>Andrewid the Android is a galaxy-famous detective. He is now investigating a case of frauds who make fake copies of the famous Stolp's gears, puzzles that are as famous as the Rubik's cube once was.</p><p>Its most important components are a button and a line of <span class="tex-span"><i>n</i></span> similar gears. Each gear has <span class="tex-span"><i>n</i></span> teeth containing all numbers from <span class="tex-span">0</span> to <span class="tex-span"><i>n</i> - 1</span> in the counter-clockwise order. When you push a button, the first gear rotates <span class="tex-font-style-it">clockwise</span>, then the second gear rotates <span class="tex-font-style-it">counter-clockwise</span>, the the third gear rotates <span class="tex-font-style-it">clockwise</span> an so on.</p><p>Besides, each gear has exactly one active tooth. When a gear turns, a new active tooth is the one following after the current active tooth according to the direction of the rotation. For example, if <span class="tex-span"><i>n</i> = 5</span>, and the active tooth is the one containing number <span class="tex-span">0</span>, then clockwise rotation makes the tooth with number <span class="tex-span">1</span> active, or the counter-clockwise rotating makes the tooth number <span class="tex-span">4</span> active.</p><p>Andrewid remembers that the real puzzle has the following property: you can push the button multiple times in such a way that in the end the numbers on the active teeth of the gears from first to last form sequence <span class="tex-span">0, 1, 2, ..., <i>n</i> - 1</span>. Write a program that determines whether the given puzzle is real or fake.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) — the number of gears.</p><p>The second line contains <span class="tex-span"><i>n</i></span> digits <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> - 1</span>) — the sequence of active teeth: the active tooth of the <span class="tex-span"><i>i</i></span>-th gear contains number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p></div><div class="output-specification"><p>In a single line print <span class="tex-font-style-tt">"Yes"</span> (without the quotes), if the given Stolp's gears puzzle is real, and <span class="tex-font-style-tt">"No"</span> (without the quotes) otherwise.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) — the number of gears.</p><p>The second line contains <span class="tex-span"><i>n</i></span> digits <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> - 1</span>) — the sequence of active teeth: the active tooth of the <span class="tex-span"><i>i</i></span>-th gear contains number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p>

## Output

<p>In a single line print <span class="tex-font-style-tt">"Yes"</span> (without the quotes), if the given Stolp's gears puzzle is real, and <span class="tex-font-style-tt">"No"</span> (without the quotes) otherwise.</p>





```input1
3
1 0 0

```




```input2
5
4 2 1 4 3

```




```input3
4
0 2 3 1

```




```output1
Yes

```




```output2
Yes

```




```output3
No

```



## Note

<p>In the first sample test when you push the button for the first time, the sequence of active teeth will be <span class="tex-font-style-tt">2 2 1</span>, when you push it for the second time, you get <span class="tex-font-style-tt">0 1 2</span>.</p>
