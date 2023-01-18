## Description

<div><p>Alexey, a merry Berland entrant, got sick of the gray reality and he zealously wants to go to university. There are a lot of universities nowadays, so Alexey is getting lost in the diversity — he has not yet decided what profession he wants to get. At school, he had bad grades in all subjects, and it's only thanks to wealthy parents that he was able to obtain the graduation certificate.</p><p>The situation is complicated by the fact that each high education institution has the determined amount of voluntary donations, paid by the new students for admission — <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span> berubleys. He cannot pay more than <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span>, because then the difference between the paid amount and <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span> can be regarded as a bribe!</p><p>Each rector is wearing the distinctive uniform of his university. Therefore, the uniform's pockets cannot contain coins of denomination more than <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>. The rector also does not carry coins of denomination less than <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> in his pocket — because if everyone pays him with so small coins, they gather a lot of weight and the pocket tears. Therefore, a donation can be paid only by coins of denomination <span class="tex-span"><i>x</i></span> berubleys, where <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>x</i> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub></span> (Berland uses coins of any positive integer denomination). Alexey can use the coins of different denominations and he can use the coins of the same denomination any number of times. When Alexey was first confronted with such orders, he was puzzled because it turned out that not all universities can accept him! Alexey is very afraid of going into the army (even though he had long wanted to get the green uniform, but his dad says that the army bullies will beat his son and he cannot pay to ensure the boy's safety). So, Alexey wants to know for sure which universities he can enter so that he could quickly choose his alma mater.</p><p>Thanks to the parents, Alexey is not limited in money and we can assume that he has an unlimited number of coins of each type.</p><p>In other words, you are given <span class="tex-span"><i>t</i></span> requests, each of them contains numbers <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub>, <i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span>. For each query you need to answer, whether it is possible to gather the sum of exactly <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span> berubleys using only coins with an integer denomination from <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> berubleys. You can use coins of different denominations. Coins of each denomination can be used any number of times.</p></div><div class="input-specification"><p>The first line contains the number of universities <span class="tex-span"><i>t</i></span>, (<span class="tex-span">1 ≤ <i>t</i> ≤ 1000</span>) Each of the next <span class="tex-span"><i>t</i></span> lines contain three space-separated integers: <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub>, <i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>n</i><sub class="lower-index"><i>i</i></sub>, <i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>;&nbsp;<i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub></span>).</p></div><div class="output-specification"><p>For each query print on a single line: either "<span class="tex-font-style-tt">Yes</span>", if Alexey can enter the university, or "<span class="tex-font-style-tt">No</span>" otherwise.</p></div>

## Input

<p>The first line contains the number of universities <span class="tex-span"><i>t</i></span>, (<span class="tex-span">1 ≤ <i>t</i> ≤ 1000</span>) Each of the next <span class="tex-span"><i>t</i></span> lines contain three space-separated integers: <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub>, <i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>n</i><sub class="lower-index"><i>i</i></sub>, <i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>;&nbsp;<i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub></span>).</p>

## Output

<p>For each query print on a single line: either "<span class="tex-font-style-tt">Yes</span>", if Alexey can enter the university, or "<span class="tex-font-style-tt">No</span>" otherwise.</p>





```input1
2
5 2 3
6 4 5

```




```output1
Yes
No

```



## Note

<p>You can pay the donation to the first university with two coins: one of denomination 2 and one of denomination 3 berubleys. The donation to the second university cannot be paid.</p>
