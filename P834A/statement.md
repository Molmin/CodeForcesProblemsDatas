## Description

<div><center> <img class="tex-graphics" src="file://kjvV5JwV.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Walking through the streets of Marshmallow City, Slastyona have spotted some merchants selling a kind of useless toy which is very popular nowadays&nbsp;– caramel spinner! Wanting to join the craze, she has immediately bought the strange contraption.</p><p>Spinners in Sweetland have the form of V-shaped pieces of caramel. Each spinner can, well, spin around an invisible magic axis. At a specific point in time, a spinner can take 4 positions shown below (each one rotated 90 degrees relative to the previous, with the fourth one followed by the first one):</p><center> <img class="tex-graphics" src="file://X608jO3y.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>After the spinner was spun, it starts its rotation, which is described by a following algorithm: the spinner maintains its position for a second then majestically switches to the next position in clockwise or counter-clockwise order, depending on the direction the spinner was spun in.</p><p>Slastyona managed to have spinner rotating for exactly <span class="tex-span"><i>n</i></span> seconds. Being fascinated by elegance of the process, she completely forgot the direction the spinner was spun in! Lucky for her, she managed to recall the starting position, and wants to deduct the direction given the information she knows. Help her do this.</p></div><div class="input-specification"><p>There are two characters in the first string&nbsp;– the starting and the ending position of a spinner. The position is encoded with one of the following characters: <span class="tex-font-style-tt">v</span> (ASCII code <span class="tex-span">118</span>, lowercase v), <span class="tex-font-style-tt">&lt;</span> (ASCII code <span class="tex-span">60</span>), <span class="tex-font-style-tt">^</span> (ASCII code <span class="tex-span">94</span>) or <span class="tex-font-style-tt">&gt;</span> (ASCII code <span class="tex-span">62</span>) (see the picture above for reference). Characters are separated by a single space.</p><p>In the second strings, a single number <span class="tex-span"><i>n</i></span> is given (<span class="tex-span">0 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;– the duration of the rotation.</p><p>It is guaranteed that the ending position of a spinner is a result of a <span class="tex-span"><i>n</i></span> second spin in any of the directions, assuming the given starting position.</p></div><div class="output-specification"><p>Output <span class="tex-font-style-tt">cw</span>, if the direction is clockwise, <span class="tex-font-style-tt">ccw</span>&nbsp;– if counter-clockwise, and <span class="tex-font-style-tt">undefined</span> otherwise.</p></div>

## Input

<p>There are two characters in the first string&nbsp;– the starting and the ending position of a spinner. The position is encoded with one of the following characters: <span class="tex-font-style-tt">v</span> (ASCII code <span class="tex-span">118</span>, lowercase v), <span class="tex-font-style-tt">&lt;</span> (ASCII code <span class="tex-span">60</span>), <span class="tex-font-style-tt">^</span> (ASCII code <span class="tex-span">94</span>) or <span class="tex-font-style-tt">&gt;</span> (ASCII code <span class="tex-span">62</span>) (see the picture above for reference). Characters are separated by a single space.</p><p>In the second strings, a single number <span class="tex-span"><i>n</i></span> is given (<span class="tex-span">0 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;– the duration of the rotation.</p><p>It is guaranteed that the ending position of a spinner is a result of a <span class="tex-span"><i>n</i></span> second spin in any of the directions, assuming the given starting position.</p>

## Output

<p>Output <span class="tex-font-style-tt">cw</span>, if the direction is clockwise, <span class="tex-font-style-tt">ccw</span>&nbsp;– if counter-clockwise, and <span class="tex-font-style-tt">undefined</span> otherwise.</p>





```input1
^ &gt;
1

```




```input2
&lt; ^
3

```




```input3
^ v
6

```




```output1
cw

```




```output2
ccw

```




```output3
undefined

```


