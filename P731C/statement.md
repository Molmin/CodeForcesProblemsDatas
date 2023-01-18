## Description

<div><p>Arseniy is already grown-up and independent. His mother decided to leave him alone for <span class="tex-span"><i>m</i></span> days and left on a vacation. She have prepared a lot of food, left some money and washed all Arseniy's clothes. </p><p>Ten minutes before her leave she realized that it would be also useful to prepare instruction of which particular clothes to wear on each of the days she will be absent. Arseniy's family is a bit weird so all the clothes is enumerated. For example, each of Arseniy's <span class="tex-span"><i>n</i></span> socks is assigned a unique integer from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Thus, the only thing his mother had to do was to write down two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> for each of the days&nbsp;— the indices of socks to wear on the day <span class="tex-span"><i>i</i></span> (obviously, <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> stands for the left foot and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> for the right). Each sock is painted in one of <span class="tex-span"><i>k</i></span> colors.</p><p>When mother already left Arseniy noticed that according to instruction he would wear the socks of different colors on some days. Of course, that is a terrible mistake cause by a rush. Arseniy is a smart boy, and, by some magical coincidence, he posses <span class="tex-span"><i>k</i></span> jars with the paint&nbsp;— one for each of <span class="tex-span"><i>k</i></span> colors.</p><p>Arseniy wants to repaint some of the socks in such a way, that for each of <span class="tex-span"><i>m</i></span> days he can follow the mother's instructions and wear the socks of the same color. As he is going to be very busy these days he will have no time to change the colors of any socks so he has to finalize the colors now.</p><p>The new computer game Bota-3 was just realised and Arseniy can't wait to play it. What is the minimum number of socks that need their color to be changed in order to make it possible to follow mother's instructions and wear the socks of the same color during each of <span class="tex-span"><i>m</i></span> days.</p></div><div class="input-specification"><p>The first line of input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200 000</span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 200 000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 200 000</span>)&nbsp;— the number of socks, the number of days and the number of available colors respectively.</p><p>The second line contain <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>c</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>k</i></span>)&nbsp;— current colors of Arseniy's socks.</p><p>Each of the following <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub> ≠ <i>r</i><sub class="lower-index"><i>i</i></sub></span>)&nbsp;— indices of socks which Arseniy should wear during the <span class="tex-span"><i>i</i></span>-th day.</p></div><div class="output-specification"><p>Print one integer&nbsp;— the minimum number of socks that should have their colors changed in order to be able to obey the instructions and not make people laugh from watching the socks of different colors.</p></div>

## Input

<p>The first line of input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200 000</span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 200 000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 200 000</span>)&nbsp;— the number of socks, the number of days and the number of available colors respectively.</p><p>The second line contain <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>c</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>k</i></span>)&nbsp;— current colors of Arseniy's socks.</p><p>Each of the following <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub> ≠ <i>r</i><sub class="lower-index"><i>i</i></sub></span>)&nbsp;— indices of socks which Arseniy should wear during the <span class="tex-span"><i>i</i></span>-th day.</p>

## Output

<p>Print one integer&nbsp;— the minimum number of socks that should have their colors changed in order to be able to obey the instructions and not make people laugh from watching the socks of different colors.</p>





```input1
3 2 3
1 2 3
1 2
2 3

```




```input2
3 2 2
1 1 2
1 2
2 1

```




```output1
2

```




```output2
0

```



## Note

<p>In the first sample, Arseniy can repaint the first and the third socks to the second color.</p><p>In the second sample, there is no need to change any colors.</p>
