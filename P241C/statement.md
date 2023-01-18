## Description

<div><p>Mirror Box is a name of a popular game in the Iranian National Amusement Park (INAP). There is a wooden box, <span class="tex-span">10<sup class="upper-index">5</sup></span> cm long and <span class="tex-span">100</span> cm high in this game. Some parts of the box's ceiling and floor are covered by mirrors. There are two negligibly small holes in the opposite sides of the box at heights <span class="tex-span"><i>h</i><sub class="lower-index"><i>l</i></sub></span> and <span class="tex-span"><i>h</i><sub class="lower-index"><i>r</i></sub></span> centimeters above the floor. The picture below shows what the box looks like.</p><center> <img class="tex-graphics" src="file://aJWKy4jA.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the game, you will be given a laser gun to shoot once. The laser beam must enter from one hole and exit from the other one. Each mirror has a preset number <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, which shows the number of points players gain if their laser beam hits that mirror. Also — to make things even funnier — the beam must <span class="tex-font-style-bf">not</span> hit any mirror more than once.</p><p>Given the information about the box, your task is to find the maximum score a player may gain. Please note that the reflection obeys the law "the angle of incidence equals the angle of reflection".</p></div><div class="input-specification"><p>The first line of the input contains three space-separated integers <span class="tex-span"><i>h</i><sub class="lower-index"><i>l</i></sub>, <i>h</i><sub class="lower-index"><i>r</i></sub>, <i>n</i></span> (<span class="tex-span">0 &lt; <i>h</i><sub class="lower-index"><i>l</i></sub>, <i>h</i><sub class="lower-index"><i>r</i></sub> &lt; 100</span>, <span class="tex-span">0 ≤ <i>n</i> ≤ 100</span>) — the heights of the holes and the number of the mirrors.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain the descriptions of the mirrors. The <span class="tex-span"><i>i</i></span>-th line contains space-separated <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span>; the integer <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) is the score for the <span class="tex-span"><i>i</i></span>-th mirror; the character <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> denotes <span class="tex-span"><i>i</i></span>-th mirror's position — the mirror is on the ceiling if <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> equals "<span class="tex-font-style-tt">T</span>" and on the floor if <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> equals "<span class="tex-font-style-tt">F</span>"; integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>) represent the <span class="tex-span"><i>x</i></span>-coordinates of the beginning and the end of the mirror.</p><p>No two mirrors will share a common point. Consider that the <span class="tex-span"><i>x</i></span> coordinate increases in the direction from left to right, so the border with the hole at height <span class="tex-span"><i>h</i><sub class="lower-index"><i>l</i></sub></span> has the <span class="tex-span"><i>x</i></span> coordinate equal to 0 and the border with the hole at height <span class="tex-span"><i>h</i><sub class="lower-index"><i>r</i></sub></span> has the <span class="tex-span"><i>x</i></span> coordinate equal to <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p></div><div class="output-specification"><p>The only line of output should contain a single integer — the maximum possible score a player could gain.</p></div>

## Input

<p>The first line of the input contains three space-separated integers <span class="tex-span"><i>h</i><sub class="lower-index"><i>l</i></sub>, <i>h</i><sub class="lower-index"><i>r</i></sub>, <i>n</i></span> (<span class="tex-span">0 &lt; <i>h</i><sub class="lower-index"><i>l</i></sub>, <i>h</i><sub class="lower-index"><i>r</i></sub> &lt; 100</span>, <span class="tex-span">0 ≤ <i>n</i> ≤ 100</span>) — the heights of the holes and the number of the mirrors.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain the descriptions of the mirrors. The <span class="tex-span"><i>i</i></span>-th line contains space-separated <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span>; the integer <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) is the score for the <span class="tex-span"><i>i</i></span>-th mirror; the character <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> denotes <span class="tex-span"><i>i</i></span>-th mirror's position — the mirror is on the ceiling if <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> equals "<span class="tex-font-style-tt">T</span>" and on the floor if <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> equals "<span class="tex-font-style-tt">F</span>"; integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>) represent the <span class="tex-span"><i>x</i></span>-coordinates of the beginning and the end of the mirror.</p><p>No two mirrors will share a common point. Consider that the <span class="tex-span"><i>x</i></span> coordinate increases in the direction from left to right, so the border with the hole at height <span class="tex-span"><i>h</i><sub class="lower-index"><i>l</i></sub></span> has the <span class="tex-span"><i>x</i></span> coordinate equal to 0 and the border with the hole at height <span class="tex-span"><i>h</i><sub class="lower-index"><i>r</i></sub></span> has the <span class="tex-span"><i>x</i></span> coordinate equal to <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p>

## Output

<p>The only line of output should contain a single integer — the maximum possible score a player could gain.</p>





```input1
50 50 7
10 F 1 80000
20 T 1 80000
30 T 81000 82000
40 T 83000 84000
50 T 85000 86000
60 T 87000 88000
70 F 81000 89000

```




```input2
80 72 9
15 T 8210 15679
10 F 11940 22399
50 T 30600 44789
50 F 32090 36579
5 F 45520 48519
120 F 49250 55229
8 F 59700 80609
35 T 61940 64939
2 T 92540 97769

```




```output1
100

```




```output2
120

```



## Note

<p>The second sample is depicted above. The red beam gets <span class="tex-span">10 + 50 + 5 + 35 + 8 + 2 = 110</span> points and the blue one gets <span class="tex-span">120</span>.</p><p><span class="tex-font-style-bf">The red beam on the picture given in the statement shows how the laser beam can go approximately, this is just illustration how the laser beam can gain score. So for the second sample there is no such beam that gain score 110.</span></p>
