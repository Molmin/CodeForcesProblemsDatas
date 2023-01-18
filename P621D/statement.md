## Description

<div><p>Wet Shark asked Rat Kwesh to generate three positive real numbers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> and <span class="tex-span"><i>z</i></span>, from <span class="tex-span">0.1</span> to <span class="tex-span">200.0</span>, inclusive. Wet Krash wants to impress Wet Shark, so all generated numbers will have <span class="tex-font-style-bf">exactly one</span> digit after the decimal point.</p><p>Wet Shark knows Rat Kwesh will want a lot of cheese. So he will give the Rat an opportunity to earn a lot of cheese. He will hand the three numbers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> and <span class="tex-span"><i>z</i></span> to Rat Kwesh, and Rat Kwesh will pick one of the these twelve options:</p><ol> <li> <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> = <i>x</i><sup class="upper-index"><i>y</i><sup class="upper-index"><i>z</i></sup></sup></span>; </li><li> <span class="tex-span"><i>a</i><sub class="lower-index">2</sub> = <i>x</i><sup class="upper-index"><i>z</i><sup class="upper-index"><i>y</i></sup></sup></span>; </li><li> <span class="tex-span"><i>a</i><sub class="lower-index">3</sub> = (<i>x</i><sup class="upper-index"><i>y</i></sup>)<sup class="upper-index"><i>z</i></sup></span>; </li><li> <span class="tex-span"><i>a</i><sub class="lower-index">4</sub> = (<i>x</i><sup class="upper-index"><i>z</i></sup>)<sup class="upper-index"><i>y</i></sup></span>; </li><li> <span class="tex-span"><i>a</i><sub class="lower-index">5</sub> = <i>y</i><sup class="upper-index"><i>x</i><sup class="upper-index"><i>z</i></sup></sup></span>; </li><li> <span class="tex-span"><i>a</i><sub class="lower-index">6</sub> = <i>y</i><sup class="upper-index"><i>z</i><sup class="upper-index"><i>x</i></sup></sup></span>; </li><li> <span class="tex-span"><i>a</i><sub class="lower-index">7</sub> = (<i>y</i><sup class="upper-index"><i>x</i></sup>)<sup class="upper-index"><i>z</i></sup></span>; </li><li> <span class="tex-span"><i>a</i><sub class="lower-index">8</sub> = (<i>y</i><sup class="upper-index"><i>z</i></sup>)<sup class="upper-index"><i>x</i></sup></span>; </li><li> <span class="tex-span"><i>a</i><sub class="lower-index">9</sub> = <i>z</i><sup class="upper-index"><i>x</i><sup class="upper-index"><i>y</i></sup></sup></span>; </li><li> <span class="tex-span"><i>a</i><sub class="lower-index">10</sub> = <i>z</i><sup class="upper-index"><i>y</i><sup class="upper-index"><i>x</i></sup></sup></span>; </li><li> <span class="tex-span"><i>a</i><sub class="lower-index">11</sub> = (<i>z</i><sup class="upper-index"><i>x</i></sup>)<sup class="upper-index"><i>y</i></sup></span>; </li><li> <span class="tex-span"><i>a</i><sub class="lower-index">12</sub> = (<i>z</i><sup class="upper-index"><i>y</i></sup>)<sup class="upper-index"><i>x</i></sup></span>. </li></ol><p>Let <span class="tex-span"><i>m</i></span> be the maximum of all the <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, and <span class="tex-span"><i>c</i></span> be the smallest index (from <span class="tex-span">1</span> to <span class="tex-span">12</span>) such that <span class="tex-span"><i>a</i><sub class="lower-index"><i>c</i></sub> = <i>m</i></span>. Rat's goal is to find that <span class="tex-span"><i>c</i></span>, and he asks you to help him. Rat Kwesh wants to see how much cheese he gets, so he you will have to print the expression corresponding to that <span class="tex-span"><i>a</i><sub class="lower-index"><i>c</i></sub></span>.</p><p> </p></div><div class="input-specification"><p>The only line of the input contains three space-separated real numbers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> and <span class="tex-span"><i>z</i></span> (<span class="tex-span">0.1 ≤ <i>x</i>, <i>y</i>, <i>z</i> ≤ 200.0</span>). Each of <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> and <span class="tex-span"><i>z</i></span> is given with exactly one digit after the decimal point.</p></div><div class="output-specification"><p>Find the maximum value of expression among <span class="tex-span"><i>x</i><sup class="upper-index"><i>y</i><sup class="upper-index"><i>z</i></sup></sup></span>, <span class="tex-span"><i>x</i><sup class="upper-index"><i>z</i><sup class="upper-index"><i>y</i></sup></sup></span>, <span class="tex-span">(<i>x</i><sup class="upper-index"><i>y</i></sup>)<sup class="upper-index"><i>z</i></sup></span>, <span class="tex-span">(<i>x</i><sup class="upper-index"><i>z</i></sup>)<sup class="upper-index"><i>y</i></sup></span>, <span class="tex-span"><i>y</i><sup class="upper-index"><i>x</i><sup class="upper-index"><i>z</i></sup></sup></span>, <span class="tex-span"><i>y</i><sup class="upper-index"><i>z</i><sup class="upper-index"><i>x</i></sup></sup></span>, <span class="tex-span">(<i>y</i><sup class="upper-index"><i>x</i></sup>)<sup class="upper-index"><i>z</i></sup></span>, <span class="tex-span">(<i>y</i><sup class="upper-index"><i>z</i></sup>)<sup class="upper-index"><i>x</i></sup></span>, <span class="tex-span"><i>z</i><sup class="upper-index"><i>x</i><sup class="upper-index"><i>y</i></sup></sup></span>, <span class="tex-span"><i>z</i><sup class="upper-index"><i>y</i><sup class="upper-index"><i>x</i></sup></sup></span>, <span class="tex-span">(<i>z</i><sup class="upper-index"><i>x</i></sup>)<sup class="upper-index"><i>y</i></sup></span>, <span class="tex-span">(<i>z</i><sup class="upper-index"><i>y</i></sup>)<sup class="upper-index"><i>x</i></sup></span> and print the corresponding expression. If there are many maximums, print the one that comes first in the list. </p><p><span class="tex-span"><i>x</i><sup class="upper-index"><i>y</i><sup class="upper-index"><i>z</i></sup></sup></span> should be outputted as <span class="tex-font-style-tt">x^y^z</span> (without brackets), and <span class="tex-span">(<i>x</i><sup class="upper-index"><i>y</i></sup>)<sup class="upper-index"><i>z</i></sup></span> should be outputted as <span class="tex-font-style-tt">(x^y)^z</span> (quotes for clarity). </p></div>

## Input

<p>The only line of the input contains three space-separated real numbers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> and <span class="tex-span"><i>z</i></span> (<span class="tex-span">0.1 ≤ <i>x</i>, <i>y</i>, <i>z</i> ≤ 200.0</span>). Each of <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> and <span class="tex-span"><i>z</i></span> is given with exactly one digit after the decimal point.</p>

## Output

<p>Find the maximum value of expression among <span class="tex-span"><i>x</i><sup class="upper-index"><i>y</i><sup class="upper-index"><i>z</i></sup></sup></span>, <span class="tex-span"><i>x</i><sup class="upper-index"><i>z</i><sup class="upper-index"><i>y</i></sup></sup></span>, <span class="tex-span">(<i>x</i><sup class="upper-index"><i>y</i></sup>)<sup class="upper-index"><i>z</i></sup></span>, <span class="tex-span">(<i>x</i><sup class="upper-index"><i>z</i></sup>)<sup class="upper-index"><i>y</i></sup></span>, <span class="tex-span"><i>y</i><sup class="upper-index"><i>x</i><sup class="upper-index"><i>z</i></sup></sup></span>, <span class="tex-span"><i>y</i><sup class="upper-index"><i>z</i><sup class="upper-index"><i>x</i></sup></sup></span>, <span class="tex-span">(<i>y</i><sup class="upper-index"><i>x</i></sup>)<sup class="upper-index"><i>z</i></sup></span>, <span class="tex-span">(<i>y</i><sup class="upper-index"><i>z</i></sup>)<sup class="upper-index"><i>x</i></sup></span>, <span class="tex-span"><i>z</i><sup class="upper-index"><i>x</i><sup class="upper-index"><i>y</i></sup></sup></span>, <span class="tex-span"><i>z</i><sup class="upper-index"><i>y</i><sup class="upper-index"><i>x</i></sup></sup></span>, <span class="tex-span">(<i>z</i><sup class="upper-index"><i>x</i></sup>)<sup class="upper-index"><i>y</i></sup></span>, <span class="tex-span">(<i>z</i><sup class="upper-index"><i>y</i></sup>)<sup class="upper-index"><i>x</i></sup></span> and print the corresponding expression. If there are many maximums, print the one that comes first in the list. </p><p><span class="tex-span"><i>x</i><sup class="upper-index"><i>y</i><sup class="upper-index"><i>z</i></sup></sup></span> should be outputted as <span class="tex-font-style-tt">x^y^z</span> (without brackets), and <span class="tex-span">(<i>x</i><sup class="upper-index"><i>y</i></sup>)<sup class="upper-index"><i>z</i></sup></span> should be outputted as <span class="tex-font-style-tt">(x^y)^z</span> (quotes for clarity). </p>





```input1
1.1 3.4 2.5

```




```input2
2.0 2.0 2.0

```




```input3
1.9 1.8 1.7

```




```output1
z^y^x

```




```output2
x^y^z

```




```output3
(x^y)^z

```


