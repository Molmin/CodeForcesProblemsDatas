## Description

<div><p>Pushok the dog has been chasing Imp for a few hours already.</p><center> <img class="tex-graphics" src="file://vxUvKkqv.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Fortunately, Imp knows that Pushok is afraid of a robot vacuum cleaner. </p><p>While moving, the robot generates a string <span class="tex-span"><i>t</i></span> consisting of letters '<span class="tex-font-style-tt">s</span>' and '<span class="tex-font-style-tt">h</span>', that produces a lot of noise. We define <span class="tex-font-style-it">noise</span> of string <span class="tex-span"><i>t</i></span> as the number of occurrences of string "<span class="tex-font-style-tt">sh</span>" as a <span class="tex-font-style-bf">subsequence</span> in it, in other words, the number of such pairs <span class="tex-span">(<i>i</i>, <i>j</i>)</span>, that <span class="tex-span"><i>i</i> &lt; <i>j</i></span> and <img align="middle" class="tex-formula" src="file://zlFP7wlJ.png" style="max-width: 100.0%;max-height: 100.0%;"> and <img align="middle" class="tex-formula" src="file://7Y2YXp6E.png" style="max-width: 100.0%;max-height: 100.0%;">. </p><p>The robot is off at the moment. Imp knows that it has a sequence of strings <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> in its memory, and he can arbitrary change their order. When the robot is started, it generates the string <span class="tex-span"><i>t</i></span> as a concatenation of these strings in the given order. The noise of the resulting string equals the noise of this concatenation.</p><p>Help Imp to find the maximum noise he can achieve by changing the order of the strings.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of strings in robot's memory.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain the strings <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span>, one per line. It is guaranteed that the strings are non-empty, contain only English letters '<span class="tex-font-style-tt">s</span>' and '<span class="tex-font-style-tt">h</span>' and their total length does not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the maxumum possible <span class="tex-font-style-it">noise</span> Imp can achieve by changing the order of the strings.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of strings in robot's memory.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain the strings <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span>, one per line. It is guaranteed that the strings are non-empty, contain only English letters '<span class="tex-font-style-tt">s</span>' and '<span class="tex-font-style-tt">h</span>' and their total length does not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p>

## Output

<p>Print a single integer&nbsp;— the maxumum possible <span class="tex-font-style-it">noise</span> Imp can achieve by changing the order of the strings.</p>





```input1
4
ssh
hs
s
hhhs

```




```input2
2
h
s

```




```output1
18

```




```output2
1

```



## Note

<p>The optimal concatenation in the first sample is <span class="tex-span"><i>ssshhshhhs</i></span>.</p>
