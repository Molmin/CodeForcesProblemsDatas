## Description

<div><p>Arkady wants to have a dinner. He has just returned from a shop where he has bought a semifinished cutlet. He only needs to fry it. The cutlet should be fried for <span class="tex-span">2<i>n</i></span> seconds, in particular, it should be fried for <span class="tex-span"><i>n</i></span> seconds on one side and <span class="tex-span"><i>n</i></span> seconds on the other side. Arkady has already got a frying pan and turn on fire, but understood that maybe he won't be able to flip the cutlet exactly after <span class="tex-span"><i>n</i></span> seconds after the beginning of cooking.</p><p>Arkady is too busy with sorting sticker packs in his favorite messenger and can flip the cutlet only in some periods of time. Namely, there are <span class="tex-span"><i>k</i></span> periods of time in which he can do it, the <span class="tex-span"><i>i</i></span>-th of them is an interval of time from <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> seconds after he starts cooking till <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> seconds, inclusive. Arkady decided that it's not required to flip the cutlet exactly in the middle of cooking, instead, he will flip it several times in such a way that the cutlet will be fried exactly <span class="tex-span"><i>n</i></span> seconds on one side and <span class="tex-span"><i>n</i></span> seconds on the other side in total.</p><p>Help Arkady and find out if it's possible for him to cook the cutlet, if he is able to flip the cutlet only in given periods of time; and if yes, find the minimum number of flips he needs to cook the cutlet.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 100</span>)&nbsp;— the number of seconds the cutlet should be cooked on each side and number of periods of time in which Arkady can flip it.</p><p>The next <span class="tex-span"><i>k</i></span> lines contain descriptions of these intervals. Each line contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 2·<i>n</i></span>), meaning that Arkady can flip the cutlet in any moment starting from <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> seconds after the beginning of cooking and finishing at <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> seconds after beginning of cooking. In particular, if <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub> = <i>r</i><sub class="lower-index"><i>i</i></sub></span> then Arkady can flip the cutlet only in the moment <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub> = <i>r</i><sub class="lower-index"><i>i</i></sub></span>. It's guaranteed that <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub> &gt; <i>r</i><sub class="lower-index"><i>i</i> - 1</sub></span> for all <span class="tex-span">2 ≤ <i>i</i> ≤ <i>k</i></span>.</p></div><div class="output-specification"><p>Output "<span class="tex-font-style-tt">Hungry</span>" if Arkady won't be able to fry the cutlet for exactly <span class="tex-span"><i>n</i></span> seconds on one side and exactly <span class="tex-span"><i>n</i></span> seconds on the other side.</p><p>Otherwise, output "<span class="tex-font-style-tt">Full</span>" in the first line, and the minimum number of times he should flip the cutlet in the second line.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 100</span>)&nbsp;— the number of seconds the cutlet should be cooked on each side and number of periods of time in which Arkady can flip it.</p><p>The next <span class="tex-span"><i>k</i></span> lines contain descriptions of these intervals. Each line contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 2·<i>n</i></span>), meaning that Arkady can flip the cutlet in any moment starting from <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> seconds after the beginning of cooking and finishing at <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> seconds after beginning of cooking. In particular, if <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub> = <i>r</i><sub class="lower-index"><i>i</i></sub></span> then Arkady can flip the cutlet only in the moment <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub> = <i>r</i><sub class="lower-index"><i>i</i></sub></span>. It's guaranteed that <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub> &gt; <i>r</i><sub class="lower-index"><i>i</i> - 1</sub></span> for all <span class="tex-span">2 ≤ <i>i</i> ≤ <i>k</i></span>.</p>

## Output

<p>Output "<span class="tex-font-style-tt">Hungry</span>" if Arkady won't be able to fry the cutlet for exactly <span class="tex-span"><i>n</i></span> seconds on one side and exactly <span class="tex-span"><i>n</i></span> seconds on the other side.</p><p>Otherwise, output "<span class="tex-font-style-tt">Full</span>" in the first line, and the minimum number of times he should flip the cutlet in the second line.</p>





```input1
10 2
3 5
11 13

```




```input2
10 3
3 5
9 10
11 13

```




```input3
20 1
3 19

```




```output1
Full
2

```




```output2
Full
1

```




```output3
Hungry

```



## Note

<p>In the first example Arkady should flip the cutlet in time moment <span class="tex-span">3</span> seconds after he starts cooking and in time moment <span class="tex-span">13</span> seconds after he starts cooking.</p><p>In the second example, Arkady can flip the cutlet at <span class="tex-span">10</span> seconds after he starts cooking.</p>
