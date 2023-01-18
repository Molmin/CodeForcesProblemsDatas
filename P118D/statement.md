## Description

<div><p>Gaius Julius Caesar, a famous general, loved to line up his soldiers. Overall the army had <span class="tex-span"><i>n</i><sub class="lower-index">1</sub></span> footmen and <span class="tex-span"><i>n</i><sub class="lower-index">2</sub></span> horsemen. Caesar thought that an arrangement is <span class="tex-font-style-bf">not</span> beautiful if somewhere in the line there are strictly more that <span class="tex-span"><i>k</i><sub class="lower-index">1</sub></span> footmen standing successively one after another, or there are strictly more than <span class="tex-span"><i>k</i><sub class="lower-index">2</sub></span> horsemen standing successively one after another. Find the number of <span class="tex-font-style-underline">beautiful</span> arrangements of the soldiers. </p><p>Note that all <span class="tex-span"><i>n</i><sub class="lower-index">1</sub> + <i>n</i><sub class="lower-index">2</sub></span> warriors should be present at each arrangement. All footmen are considered indistinguishable among themselves. Similarly, all horsemen are considered indistinguishable among themselves.</p></div><div class="input-specification"><p>The only line contains four space-separated integers <span class="tex-span"><i>n</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>n</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>k</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>k</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>n</i><sub class="lower-index">1</sub>, <i>n</i><sub class="lower-index">2</sub> ≤ 100, 1 ≤ <i>k</i><sub class="lower-index">1</sub>, <i>k</i><sub class="lower-index">2</sub> ≤ 10</span>) which represent how many footmen and horsemen there are and the largest acceptable number of footmen and horsemen standing in succession, correspondingly.</p></div><div class="output-specification"><p>Print the number of beautiful arrangements of the army modulo <span class="tex-span">100000000</span> <span class="tex-span">(10<sup class="upper-index">8</sup>)</span>. That is, print the number of such ways to line up the soldiers, that no more than <span class="tex-span"><i>k</i><sub class="lower-index">1</sub></span> footmen stand successively, and no more than <span class="tex-span"><i>k</i><sub class="lower-index">2</sub></span> horsemen stand successively.</p></div>

## Input

<p>The only line contains four space-separated integers <span class="tex-span"><i>n</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>n</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>k</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>k</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>n</i><sub class="lower-index">1</sub>, <i>n</i><sub class="lower-index">2</sub> ≤ 100, 1 ≤ <i>k</i><sub class="lower-index">1</sub>, <i>k</i><sub class="lower-index">2</sub> ≤ 10</span>) which represent how many footmen and horsemen there are and the largest acceptable number of footmen and horsemen standing in succession, correspondingly.</p>

## Output

<p>Print the number of beautiful arrangements of the army modulo <span class="tex-span">100000000</span> <span class="tex-span">(10<sup class="upper-index">8</sup>)</span>. That is, print the number of such ways to line up the soldiers, that no more than <span class="tex-span"><i>k</i><sub class="lower-index">1</sub></span> footmen stand successively, and no more than <span class="tex-span"><i>k</i><sub class="lower-index">2</sub></span> horsemen stand successively.</p>





```input1
2 1 1 10

```




```input2
2 3 1 2

```




```input3
2 4 1 1

```




```output1
1

```




```output2
5

```




```output3
0

```



## Note

<p>Let's mark a footman as <span class="tex-font-style-tt">1</span>, and a horseman as <span class="tex-font-style-tt">2</span>.</p><p>In the first sample the only beautiful line-up is: <span class="tex-font-style-tt">121</span></p><p>In the second sample 5 beautiful line-ups exist: <span class="tex-font-style-tt">12122</span>, <span class="tex-font-style-tt">12212</span>, <span class="tex-font-style-tt">21212</span>, <span class="tex-font-style-tt">21221</span>, <span class="tex-font-style-tt">22121</span></p>
