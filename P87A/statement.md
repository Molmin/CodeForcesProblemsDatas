## Description

<div><p>Vasya the programmer lives in the middle of the Programming subway branch. He has two girlfriends: Dasha and Masha, who live at the different ends of the branch, each one is unaware of the other one's existence.</p><p>When Vasya has some free time, he goes to one of his girlfriends. He descends into the subway at some time, waits the first train to come and rides on it to the end of the branch to the corresponding girl. However, the trains run with different frequencies: a train goes to Dasha's direction every <span class="tex-span"><i>a</i></span> minutes, but a train goes to Masha's direction every <span class="tex-span"><i>b</i></span> minutes. If two trains approach at the same time, Vasya goes toward the direction with the lower frequency of going trains, that is, to the girl, to whose directions the trains go less frequently (see the note to the third sample).</p><p>We know that the trains begin to go simultaneously before Vasya appears. That is the train schedule is such that there exists a moment of time when the two trains arrive simultaneously.</p><p>Help Vasya count to which girlfriend he will go more often.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span"><i>a</i> ≠ <i>b</i>, 1 ≤ <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">6</sup></span>).</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">Dasha</span>" if Vasya will go to Dasha more frequently, "<span class="tex-font-style-tt">Masha</span>" if he will go to Masha more frequently, or "<span class="tex-font-style-tt">Equal</span>" if he will go to both girlfriends with the same frequency.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span"><i>a</i> ≠ <i>b</i>, 1 ≤ <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">6</sup></span>).</p>

## Output

<p>Print "<span class="tex-font-style-tt">Dasha</span>" if Vasya will go to Dasha more frequently, "<span class="tex-font-style-tt">Masha</span>" if he will go to Masha more frequently, or "<span class="tex-font-style-tt">Equal</span>" if he will go to both girlfriends with the same frequency.</p>





```input1
3 7

```




```input2
5 3

```




```input3
2 3

```




```output1
Dasha

```




```output2
Masha

```




```output3
Equal

```



## Note

<p>Let's take a look at the third sample. Let the trains start to go at the zero moment of time. It is clear that the moments of the trains' arrival will be periodic with period 6. That's why it is enough to show that if Vasya descends to the subway at a moment of time inside the interval <span class="tex-span">(0, 6]</span>, he will go to both girls equally often. </p><p>If he descends to the subway at a moment of time from 0 to 2, he leaves for Dasha on the train that arrives by the second minute.</p><p>If he descends to the subway at a moment of time from 2 to 3, he leaves for Masha on the train that arrives by the third minute.</p><p>If he descends to the subway at a moment of time from 3 to 4, he leaves for Dasha on the train that arrives by the fourth minute.</p><p>If he descends to the subway at a moment of time from 4 to 6, he waits for both trains to arrive by the sixth minute and goes to Masha as trains go less often in Masha's direction.</p><p>In sum Masha and Dasha get equal time — three minutes for each one, thus, Vasya will go to both girlfriends equally often.</p>
