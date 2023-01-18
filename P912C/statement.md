## Description

<div><p>A lot of students spend their winter holidays productively. Vlad has advanced very well in doing so! For three days already, fueled by salads and tangerines&nbsp;— the leftovers from New Year celebration&nbsp;— he has been calibrating his rating in his favorite MOBA game, playing as a hero named Perun.</p><p>Perun has an ultimate ability called "Thunderwrath". At the instant of its activation, each enemy on the map (<span class="tex-span"><i>n</i></span> of them in total) loses <img align="middle" class="tex-formula" src="file://1yi1L2a8.png" style="max-width: 100.0%;max-height: 100.0%;"> health points as a single-time effect. It also has a restriction: it can only activated when the moment of time is an <span class="tex-font-style-bf">integer</span>. The initial bounty for killing an enemy is <img align="middle" class="tex-formula" src="file://JkmQgtR2.png" style="max-width: 100.0%;max-height: 100.0%;">. Additionally, it increases by <img align="middle" class="tex-formula" src="file://tMXmJbCi.png" style="max-width: 100.0%;max-height: 100.0%;"> each second. Formally, if at some second <span class="tex-span"><i>t</i></span> the ability is activated and the <span class="tex-span"><i>i</i></span>-th enemy is killed as a result (i.e. his health drops to zero or lower), Vlad earns <img align="middle" class="tex-formula" src="file://ApjJ9PuR.png" style="max-width: 100.0%;max-height: 100.0%;"> units of gold.</p><p>Every enemy can receive damage, as well as be healed. There are multiple ways of doing so, but Vlad is not interested in details. For each of <span class="tex-span"><i>n</i></span> enemies he knows: </p><ul> <li> <img align="middle" class="tex-formula" src="file://yDR4TF5V.png" style="max-width: 100.0%;max-height: 100.0%;">&nbsp;— maximum number of health points for the <span class="tex-span"><i>i</i></span>-th enemy; </li><li> <img align="middle" class="tex-formula" src="file://hliN9Xnz.png" style="max-width: 100.0%;max-height: 100.0%;">&nbsp;— initial health of the enemy (on the <span class="tex-span">0</span>-th second); </li><li> <img align="middle" class="tex-formula" src="file://ueBk4Wk6.png" style="max-width: 100.0%;max-height: 100.0%;">&nbsp;— the amount of health the <span class="tex-span"><i>i</i></span>-th enemy can regenerate per second. </li></ul><p>There also <span class="tex-span"><i>m</i></span> health updates Vlad knows about: </p><ul> <li> <img align="middle" class="tex-formula" src="file://Tr4mNsS0.png" style="max-width: 100.0%;max-height: 100.0%;">&nbsp;— time when the health was updated; </li><li> <img align="middle" class="tex-formula" src="file://IFK37u0g.png" style="max-width: 100.0%;max-height: 100.0%;">&nbsp;— the enemy whose health was updated; </li><li> <img align="middle" class="tex-formula" src="file://lzathQJc.png" style="max-width: 100.0%;max-height: 100.0%;">&nbsp;— updated health points for <span class="tex-span"><i>enemy</i><sub class="lower-index"><i>j</i></sub></span>. </li></ul><p>Obviously, Vlad wants to maximize his profit. If it's necessary, he could even wait for years to activate his ability at the right second. Help him determine the exact second (note that it must be <span class="tex-font-style-bf">an integer</span>) from <span class="tex-span">0</span> (inclusively) to <span class="tex-span"> + ∞</span> so that a single activation of the ability would yield Vlad the maximum possible amount of gold, and print this amount.</p></div><div class="input-specification"><p>In the first line, two integers are given (separated by spaces)&nbsp;— <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>In the second line, there are three integers: <img align="middle" class="tex-formula" src="file://P2Lwuudl.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://ac1nHKj9.png" style="max-width: 100.0%;max-height: 100.0%;"> and <img align="middle" class="tex-formula" src="file://ILySrY7D.png" style="max-width: 100.0%;max-height: 100.0%;"> (<img align="middle" class="tex-formula" src="file://p7EyjV2Y.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://8UmvC32G.png" style="max-width: 100.0%;max-height: 100.0%;">).</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines has three integers&nbsp;— <img align="middle" class="tex-formula" src="file://uRpauaXH.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://hETkLcIu.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://OtYRln12.png" style="max-width: 100.0%;max-height: 100.0%;"> (<img align="middle" class="tex-formula" src="file://6wivq3uG.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://AMhSEaAZ.png" style="max-width: 100.0%;max-height: 100.0%;">).</p><p>The next <span class="tex-span"><i>m</i></span> lines contain three integers each&nbsp;— <img align="middle" class="tex-formula" src="file://fmNH8Sah.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://3RXZ61QE.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://VqzF1lgZ.png" style="max-width: 100.0%;max-height: 100.0%;"> (<img align="middle" class="tex-formula" src="file://1xJFc71V.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://2FrO9nDx.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://o2FKxTEo.png" style="max-width: 100.0%;max-height: 100.0%;">). It is guaranteed that there is no more than one hearth change per second for each enemy: more formally, for each <span class="tex-span"><i>a</i>, <i>b</i></span> so that <span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>m</i>, <i>a</i> ≠ <i>b</i></span> holds that if <img align="middle" class="tex-formula" src="file://69IgLCuH.png" style="max-width: 100.0%;max-height: 100.0%;">, then <img align="middle" class="tex-formula" src="file://9h15FkZ5.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div><div class="output-specification"><p>Output the single integer&nbsp;— the maximum amount of gold Vlad can obtain if he applies "Thunderwrath" exactly once, or <span class="tex-font-style-tt">-1</span> if this amount can be <span class="tex-font-style-bf">infinitely</span> large.</p></div>

## Input

<p>In the first line, two integers are given (separated by spaces)&nbsp;— <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>In the second line, there are three integers: <img align="middle" class="tex-formula" src="file://P2Lwuudl.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://ac1nHKj9.png" style="max-width: 100.0%;max-height: 100.0%;"> and <img align="middle" class="tex-formula" src="file://ILySrY7D.png" style="max-width: 100.0%;max-height: 100.0%;"> (<img align="middle" class="tex-formula" src="file://p7EyjV2Y.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://8UmvC32G.png" style="max-width: 100.0%;max-height: 100.0%;">).</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines has three integers&nbsp;— <img align="middle" class="tex-formula" src="file://uRpauaXH.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://hETkLcIu.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://OtYRln12.png" style="max-width: 100.0%;max-height: 100.0%;"> (<img align="middle" class="tex-formula" src="file://6wivq3uG.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://AMhSEaAZ.png" style="max-width: 100.0%;max-height: 100.0%;">).</p><p>The next <span class="tex-span"><i>m</i></span> lines contain three integers each&nbsp;— <img align="middle" class="tex-formula" src="file://fmNH8Sah.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://3RXZ61QE.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://VqzF1lgZ.png" style="max-width: 100.0%;max-height: 100.0%;"> (<img align="middle" class="tex-formula" src="file://1xJFc71V.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://2FrO9nDx.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://o2FKxTEo.png" style="max-width: 100.0%;max-height: 100.0%;">). It is guaranteed that there is no more than one hearth change per second for each enemy: more formally, for each <span class="tex-span"><i>a</i>, <i>b</i></span> so that <span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>m</i>, <i>a</i> ≠ <i>b</i></span> holds that if <img align="middle" class="tex-formula" src="file://69IgLCuH.png" style="max-width: 100.0%;max-height: 100.0%;">, then <img align="middle" class="tex-formula" src="file://9h15FkZ5.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>

## Output

<p>Output the single integer&nbsp;— the maximum amount of gold Vlad can obtain if he applies "Thunderwrath" exactly once, or <span class="tex-font-style-tt">-1</span> if this amount can be <span class="tex-font-style-bf">infinitely</span> large.</p>





```input1
3 2
1000 10 50
70 5 5
90 70 1
110 20 2
20 2 10
30 3 10

```




```input2
1 1
500 50 1000
750 750 20
10 1 300

```




```output1
3000

```




```output2
-1

```



## Note

<p>On the pictures you can see health points of each enemy versus time in sample cases.</p><p><span class="tex-font-style-it">Periods when Vlad can kill one enemy are marked with yellow color.</span></p><p><span class="tex-font-style-it">Periods when Vlad can kill two enemies are marked with purple color.</span></p><center> <img class="tex-graphics" height="354px" src="file://vIYBIref.png" style="max-width: 100.0%;max-height: 100.0%;" width="567px"> </center><p>In the first sample case, Vlad can activate the ability at the <span class="tex-span">50</span>-th second: the enemies <span class="tex-span">2</span> and <span class="tex-span">3</span> will die since they would have <span class="tex-span">40</span> and <span class="tex-span">50</span> health points correspondingly. Vlad will earn <span class="tex-span">2·(1000 + 50·10) = 3000</span> gold.</p><center> <img class="tex-graphics" height="354px" src="file://rOSNHMbV.png" style="max-width: 100.0%;max-height: 100.0%;" width="567px"> </center><p>In the second sample case, the maximum amount of health for the enemy <span class="tex-span">1</span> is less than the damage dealt by the ability. Hence, the enemy could be killed anytime. As the bounty increases by <span class="tex-span">50</span> over the time, the maximum possible amount of gold is infinite.</p>
