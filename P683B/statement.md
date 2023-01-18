## Description

<div><p><span class="tex-span"><i>n</i></span> pupils came to Physical Education lesson. We know the name and the height of each pupil. </p><p>Your task is to help the teacher of Physical Education to line up all pupils in non-decreasing order of their heights.</p></div><div class="input-specification"><p>The first line contains the positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>) — the number of pupils.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain the pupils' description. In the <span class="tex-span"><i>i</i></span>-th line there is pupil's name <span class="tex-span"><i>name</i><sub class="lower-index"><i>i</i></sub></span> (a non-empty string which consists of uppercase and lowercase Latin letters, the length does not exceed five) and pupil's height <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">130 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 215</span>). Some pupils can have the same name. Uppercase and lowercase letters of the alphabet should be considered different. </p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> lines — pupils' names in the non-decreasing order of their heights. Each line must contain exactly one name. </p><p>If there are several answers, print any of them. Uppercase and lowercase letters of the alphabet should be considered different. </p></div>

## Input

<p>The first line contains the positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>) — the number of pupils.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain the pupils' description. In the <span class="tex-span"><i>i</i></span>-th line there is pupil's name <span class="tex-span"><i>name</i><sub class="lower-index"><i>i</i></sub></span> (a non-empty string which consists of uppercase and lowercase Latin letters, the length does not exceed five) and pupil's height <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">130 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 215</span>). Some pupils can have the same name. Uppercase and lowercase letters of the alphabet should be considered different. </p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> lines — pupils' names in the non-decreasing order of their heights. Each line must contain exactly one name. </p><p>If there are several answers, print any of them. Uppercase and lowercase letters of the alphabet should be considered different. </p>





```input1
4
Ivan 150
Igor 215
Dasha 158
Katya 150

```




```input2
2
SASHA 180
SASHA 170

```




```output1
Ivan
Katya
Dasha
Igor

```




```output2
SASHA
SASHA

```


