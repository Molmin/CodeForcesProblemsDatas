## Description

<div><p>Once upon a time in the Kingdom of Far Far Away lived Sir Lancelot, the chief Royal General. He was very proud of his men and he liked to invite the King to come and watch drill exercises which demonstrated the fighting techniques and tactics of the squad he was in charge of. But time went by and one day Sir Lancelot had a major argument with the Fairy Godmother (there were rumors that the argument occurred after the general spoke badly of the Godmother's flying techniques. That seemed to hurt the Fairy Godmother very deeply). </p><p>As the result of the argument, the Godmother put a rather strange curse upon the general. It sounded all complicated and quite harmless: "<span class="tex-font-style-underline">If the squared distance between some two soldiers equals to <span class="tex-span">5</span>, then those soldiers will conflict with each other!</span>"</p><p>The drill exercises are held on a rectangular <span class="tex-span"><i>n</i> × <i>m</i></span> field, split into <span class="tex-span"><i>nm</i></span> square <span class="tex-span">1 × 1</span> segments for each soldier. Thus, the square of the distance between the soldiers that stand on squares <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span> and <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span> equals exactly <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub> - <i>x</i><sub class="lower-index">2</sub>)<sup class="upper-index">2</sup> + (<i>y</i><sub class="lower-index">1</sub> - <i>y</i><sub class="lower-index">2</sub>)<sup class="upper-index">2</sup></span>. Now not all <span class="tex-span"><i>nm</i></span> squad soldiers can participate in the drill exercises as it was before the Fairy Godmother's curse. Unless, of course, the general wants the soldiers to fight with each other or even worse... For example, if he puts a soldier in the square <span class="tex-span">(2, 2)</span>, then he cannot put soldiers in the squares <span class="tex-span">(1, 4)</span>, <span class="tex-span">(3, 4)</span>, <span class="tex-span">(4, 1)</span> and <span class="tex-span">(4, 3)</span> — each of them will conflict with the soldier in the square <span class="tex-span">(2, 2)</span>.</p><p>Your task is to help the general. You are given the size of the drill exercise field. You are asked to calculate the maximum number of soldiers that can be simultaneously positioned on this field, so that no two soldiers fall under the Fairy Godmother's curse.</p></div><div class="input-specification"><p>The single line contains space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>) that represent the size of the drill exercise field.</p></div><div class="output-specification"><p>Print the desired maximum number of warriors.</p></div>

## Input

<p>The single line contains space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>) that represent the size of the drill exercise field.</p>

## Output

<p>Print the desired maximum number of warriors.</p>





```input1
2 4

```




```input2
3 4

```




```output1
4
```




```output2
6
```



## Note

<p>In the first sample test Sir Lancelot can place his 4 soldiers on the <span class="tex-span">2 × 4</span> court as follows (the soldiers' locations are marked with gray circles on the scheme):</p><center> <img class="tex-graphics" src="file://e86RYuBx.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the second sample test he can place 6 soldiers on the <span class="tex-span">3 × 4</span> site in the following manner:</p><center> <img class="tex-graphics" src="file://C1aX5rcZ.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
