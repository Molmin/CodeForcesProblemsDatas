## Description

<div><p>Cucumber boy is fan of Kyubeat, a famous music game.</p><p>Kyubeat has <span class="tex-span">16</span> panels for playing arranged in <span class="tex-span">4 × 4</span> table. When a panel lights up, he has to press that panel.</p><p>Each panel has a <span class="tex-font-style-bf">timing</span> to press (the preffered time when a player should press it), and Cucumber boy is able to press at most <span class="tex-span"><i>k</i></span> panels in a time with his one hand. Cucumber boy is trying to press all panels in perfect timing, that is he wants to press each panel exactly in its preffered time. If he cannot press the panels with his <span class="tex-font-style-bf">two hands</span> in perfect timing, his challenge to press all the panels in perfect timing will fail.</p><p>You are given one scene of Kyubeat's panel from the music Cucumber boy is trying. Tell him is he able to press all the panels in perfect timing.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 5</span>) — the number of panels Cucumber boy can press with his one hand.</p><p>Next 4 lines contain 4 characters each (digits from 1 to 9, or period) — table of panels. If a digit <span class="tex-span"><i>i</i></span> was written on the panel, it means the boy has to press that panel in time <span class="tex-span"><i>i</i></span>. If period was written on the panel, he doesn't have to press that panel.</p></div><div class="output-specification"><p>Output "<span class="tex-font-style-tt">YES</span>" (without quotes), if he is able to press all the panels in perfect timing. If not, output "<span class="tex-font-style-tt">NO</span>" (without quotes).</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 5</span>) — the number of panels Cucumber boy can press with his one hand.</p><p>Next 4 lines contain 4 characters each (digits from 1 to 9, or period) — table of panels. If a digit <span class="tex-span"><i>i</i></span> was written on the panel, it means the boy has to press that panel in time <span class="tex-span"><i>i</i></span>. If period was written on the panel, he doesn't have to press that panel.</p>

## Output

<p>Output "<span class="tex-font-style-tt">YES</span>" (without quotes), if he is able to press all the panels in perfect timing. If not, output "<span class="tex-font-style-tt">NO</span>" (without quotes).</p>





```input1
1
.135
1247
3468
5789

```




```input2
5
..1.
1111
..1.
..1.

```




```input3
1
....
12.1
.2..
.2..

```




```output1
YES

```




```output2
YES

```




```output3
NO

```



## Note

<p>In the third sample boy cannot press all panels in perfect timing. He can press all the panels in timing in time 1, but he cannot press the panels in time 2 in timing with his two hands.</p>
