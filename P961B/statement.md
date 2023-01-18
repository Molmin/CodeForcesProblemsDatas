## Description

<div><p>Your friend Mishka and you attend a calculus lecture. Lecture lasts <span class="tex-span"><i>n</i></span> minutes. Lecturer tells <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> theorems during the <span class="tex-span"><i>i</i></span>-th minute.</p><p>Mishka is really interested in calculus, though it is so hard to stay awake for all the time of lecture. You are given an array <span class="tex-span"><i>t</i></span> of Mishka's behavior. If Mishka is asleep during the <span class="tex-span"><i>i</i></span>-th minute of the lecture then <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> will be equal to <span class="tex-span">0</span>, otherwise it will be equal to <span class="tex-span">1</span>. When Mishka is awake he writes down all the theorems he is being told — <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> during the <span class="tex-span"><i>i</i></span>-th minute. Otherwise he writes nothing.</p><p>You know some secret technique to keep Mishka awake for <span class="tex-span"><i>k</i></span> minutes straight. However you can use it <span class="tex-font-style-bf">only once</span>. You can start using it at the beginning of any minute between <span class="tex-span">1</span> and <span class="tex-span"><i>n</i> - <i>k</i> + 1</span>. If you use it on some minute <span class="tex-span"><i>i</i></span> then Mishka will be awake during minutes <span class="tex-span"><i>j</i></span> such that <img align="middle" class="tex-formula" src="file://0TUg0tnX.png" style="max-width: 100.0%;max-height: 100.0%;"> and will write down all the theorems lecturer tells.</p><p>You task is to calculate the maximum number of theorems Mishka will be able to write down if you use your technique <span class="tex-font-style-bf">only once</span> to wake him up.</p></div><div class="input-specification"><p>The first line of the input contains two integer numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the duration of the lecture in minutes and the number of minutes you can keep Mishka awake.</p><p>The second line of the input contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>) — the number of theorems lecturer tells during the <span class="tex-span"><i>i</i></span>-th minute.</p><p>The third line of the input contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ... <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 1</span>) — type of Mishka's behavior at the <span class="tex-span"><i>i</i></span>-th minute of the lecture.</p></div><div class="output-specification"><p>Print only one integer — the maximum number of theorems Mishka will be able to write down if you use your technique <span class="tex-font-style-bf">only once</span> to wake him up.</p></div>

## Input

<p>The first line of the input contains two integer numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the duration of the lecture in minutes and the number of minutes you can keep Mishka awake.</p><p>The second line of the input contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>) — the number of theorems lecturer tells during the <span class="tex-span"><i>i</i></span>-th minute.</p><p>The third line of the input contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ... <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 1</span>) — type of Mishka's behavior at the <span class="tex-span"><i>i</i></span>-th minute of the lecture.</p>

## Output

<p>Print only one integer — the maximum number of theorems Mishka will be able to write down if you use your technique <span class="tex-font-style-bf">only once</span> to wake him up.</p>





```input1
6 3
1 3 5 2 5 4
1 1 0 1 0 0

```




```output1
16

```



## Note

<p>In the sample case the better way is to use the secret technique at the beginning of the third minute. Then the number of theorems Mishka will be able to write down will be equal to <span class="tex-span">16</span>.</p>
