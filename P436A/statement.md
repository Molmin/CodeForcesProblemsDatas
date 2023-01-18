## Description

<div><p>The hero of the Cut the Rope game is a little monster named Om Nom. He loves candies. And what a coincidence! He also is the hero of today's problem.</p><center> <img class="tex-graphics" src="file://SplJDMjR.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>One day, Om Nom visited his friend Evan. Evan has <span class="tex-span"><i>n</i></span> candies of two types (fruit drops and caramel drops), the <span class="tex-span"><i>i</i></span>-th candy hangs at the height of <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> centimeters above the floor of the house, its mass is <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span>. Om Nom wants to eat as many candies as possible. At the beginning Om Nom can make at most <span class="tex-span"><i>x</i></span> centimeter high jumps. When Om Nom eats a candy of mass <span class="tex-span"><i>y</i></span>, he gets stronger and the height of his jump increases by <span class="tex-span"><i>y</i></span> centimeters.</p><p>What maximum number of candies can Om Nom eat if he never eats two candies of the same type in a row (Om Nom finds it too boring)?</p></div><div class="input-specification"><p>The first line contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>x</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>x</i> ≤ 2000)</span> — the number of sweets Evan has and the initial height of Om Nom's jump. </p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains three integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub>, <i>h</i><sub class="lower-index"><i>i</i></sub>, <i>m</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 1;&nbsp;1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub>, <i>m</i><sub class="lower-index"><i>i</i></sub> ≤ 2000)</span> — the type, height and the mass of the <span class="tex-span"><i>i</i></span>-th candy. If number <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> equals 0, then the current candy is a caramel drop, otherwise it is a fruit drop.</p></div><div class="output-specification"><p>Print a single integer — the maximum number of candies Om Nom can eat.</p></div>

## Input

<p>The first line contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>x</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>x</i> ≤ 2000)</span> — the number of sweets Evan has and the initial height of Om Nom's jump. </p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains three integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub>, <i>h</i><sub class="lower-index"><i>i</i></sub>, <i>m</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 1;&nbsp;1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub>, <i>m</i><sub class="lower-index"><i>i</i></sub> ≤ 2000)</span> — the type, height and the mass of the <span class="tex-span"><i>i</i></span>-th candy. If number <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> equals 0, then the current candy is a caramel drop, otherwise it is a fruit drop.</p>

## Output

<p>Print a single integer — the maximum number of candies Om Nom can eat.</p>





```input1
5 3
0 2 4
1 3 1
0 8 3
0 20 10
1 5 5

```




```output1
4

```



## Note

<p>One of the possible ways to eat <span class="tex-span">4</span> candies is to eat them in the order: <span class="tex-span">1</span>, <span class="tex-span">5</span>, <span class="tex-span">3</span>, <span class="tex-span">2</span>. Let's assume the following scenario:</p><ol> <li> Initially, the height of Om Nom's jump equals <span class="tex-span">3</span>. He can reach candies <span class="tex-span">1</span> and <span class="tex-span">2</span>. Let's assume that he eats candy <span class="tex-span">1</span>. As the mass of this candy equals <span class="tex-span">4</span>, the height of his jump will rise to <span class="tex-span">3 + 4 = 7</span>. </li><li> Now Om Nom can reach candies <span class="tex-span">2</span> and <span class="tex-span">5</span>. Let's assume that he eats candy <span class="tex-span">5</span>. Then the height of his jump will be <span class="tex-span">7 + 5 = 12</span>. </li><li> At this moment, Om Nom can reach two candies, <span class="tex-span">2</span> and <span class="tex-span">3</span>. He won't eat candy <span class="tex-span">2</span> as its type matches the type of the previously eaten candy. Om Nom eats candy <span class="tex-span">3</span>, the height of his jump is <span class="tex-span">12 + 3 = 15</span>. </li><li> Om Nom eats candy <span class="tex-span">2</span>, the height of his jump is <span class="tex-span">15 + 1 = 16</span>. He cannot reach candy <span class="tex-span">4</span>. </li></ol>
