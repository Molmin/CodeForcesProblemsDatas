## Description

<div><p>Professor Dumbledore is helping Harry destroy the Horcruxes. He went to Gaunt Shack as he suspected a Horcrux to be present there. He saw Marvolo Gaunt's Ring and identified it as a Horcrux. Although he destroyed it, he is still affected by its curse. Professor Snape is helping Dumbledore remove the curse. For this, he wants to give Dumbledore exactly <span class="tex-span"><i>x</i></span> drops of the potion he made. </p><p>Value of <span class="tex-span"><i>x</i></span> is calculated as maximum of <span class="tex-span"><i>p</i>·<i>a</i><sub class="lower-index"><i>i</i></sub> + <i>q</i>·<i>a</i><sub class="lower-index"><i>j</i></sub> + <i>r</i>·<i>a</i><sub class="lower-index"><i>k</i></sub></span> for given <span class="tex-span"><i>p</i>, <i>q</i>, <i>r</i></span> and array <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... <i>a</i><sub class="lower-index"><i>n</i></sub></span> such that <span class="tex-span">1 ≤ <i>i</i> ≤ <i>j</i> ≤ <i>k</i> ≤ <i>n</i></span>. Help Snape find the value of <span class="tex-span"><i>x</i></span>. Do note that the value of <span class="tex-span"><i>x</i></span> may be negative.</p></div><div class="input-specification"><p>First line of input contains <span class="tex-span">4</span> integers <span class="tex-span"><i>n</i>, <i>p</i>, <i>q</i>, <i>r</i></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>p</i>, <i>q</i>, <i>r</i> ≤ 10<sup class="upper-index">9</sup>, 1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>Next line of input contains <span class="tex-span"><i>n</i></span> space separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Output a single integer the maximum value of <span class="tex-span"><i>p</i>·<i>a</i><sub class="lower-index"><i>i</i></sub> + <i>q</i>·<i>a</i><sub class="lower-index"><i>j</i></sub> + <i>r</i>·<i>a</i><sub class="lower-index"><i>k</i></sub></span> that can be obtained provided <span class="tex-span">1 ≤ <i>i</i> ≤ <i>j</i> ≤ <i>k</i> ≤ <i>n</i></span>.</p></div>

## Input

<p>First line of input contains <span class="tex-span">4</span> integers <span class="tex-span"><i>n</i>, <i>p</i>, <i>q</i>, <i>r</i></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>p</i>, <i>q</i>, <i>r</i> ≤ 10<sup class="upper-index">9</sup>, 1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>Next line of input contains <span class="tex-span"><i>n</i></span> space separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Output a single integer the maximum value of <span class="tex-span"><i>p</i>·<i>a</i><sub class="lower-index"><i>i</i></sub> + <i>q</i>·<i>a</i><sub class="lower-index"><i>j</i></sub> + <i>r</i>·<i>a</i><sub class="lower-index"><i>k</i></sub></span> that can be obtained provided <span class="tex-span">1 ≤ <i>i</i> ≤ <i>j</i> ≤ <i>k</i> ≤ <i>n</i></span>.</p>





```input1
5 1 2 3
1 2 3 4 5

```




```input2
5 1 2 -3
-1 -2 -3 -4 -5

```




```output1
30

```




```output2
12

```



## Note

<p>In the first sample case, we can take <span class="tex-span"><i>i</i> = <i>j</i> = <i>k</i> = 5</span>, thus making the answer as <span class="tex-span">1·5 + 2·5 + 3·5 = 30</span>.</p><p>In second sample case, selecting <span class="tex-span"><i>i</i> = <i>j</i> = 1</span> and <span class="tex-span"><i>k</i> = 5</span> gives the answer <span class="tex-span">12</span>.</p>
