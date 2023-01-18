## Description

<div><p>The Fire Lord attacked the Frost Kingdom. He has already got to the Ice Fortress, where the Snow Queen dwells. He arranged his army on a segment <span class="tex-span"><i>n</i></span> in length not far from the city walls. And only the frost magician Solomon can save the Frost Kingdom.</p><center> <img class="tex-graphics" src="file://FDM4L1Fr.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The <span class="tex-span"><i>n</i></span>-long segment is located at a distance equal exactly to <span class="tex-span">1</span> from the castle walls. It can be imaginarily divided into unit segments. On some of the unit segments <span class="tex-font-style-it">fire demons</span> are located — no more than one demon per position. Each demon is characterised by his <span class="tex-font-style-it">strength</span> - by some positive integer. We can regard the fire demons being idle.</p><p>Initially Solomon is positioned on the fortress wall. He can perform the following actions several times in a row: </p><ul><li> "<span class="tex-font-style-tt">L</span>" — Solomon shifts one unit to the left. This movement cannot be performed on the castle wall.</li><li> "<span class="tex-font-style-tt">R</span>" — Solomon shifts one unit to the left. This movement cannot be performed if there's no ice block to the right.</li><li> "<span class="tex-font-style-tt">A</span>" — If there's nothing to the right of Solomon, then Solomon creates an ice block that immediately freezes to the block that Solomon is currently standing on. If there already is an ice block, then Solomon destroys it. At that the ice blocks to the right of the destroyed one can remain but they are left unsupported. Those ice blocks fall down.</li></ul><p>Solomon spends exactly a second on each of these actions.</p><p>As the result of Solomon's actions, ice blocks' segments fall down. When an ice block falls on a fire demon, the block evaporates and the demon's strength is reduced by <span class="tex-span">1</span>. When the demons' strength is equal to <span class="tex-span">0</span>, the fire demon vanishes. The picture below shows how it happens. The ice block that falls on the position with no demon, breaks into lots of tiny pieces and vanishes without hurting anybody.</p><center> <img class="tex-graphics" src="file://XFNo3f1c.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Help Solomon destroy all the Fire Lord's army in minimum time.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>). The next line contains <span class="tex-span"><i>n</i></span> numbers, the <span class="tex-span"><i>i</i></span>-th of them represents the strength of the fire demon standing of the <span class="tex-span"><i>i</i></span>-th position, an integer from <span class="tex-span">1</span> to <span class="tex-span">100</span>. If there's no demon on the <span class="tex-span"><i>i</i></span>-th position, then the <span class="tex-span"><i>i</i></span>-th number equals to <span class="tex-span">0</span>. It is guaranteed that the input data have at least one fire demon.</p></div><div class="output-specification"><p>Print a string of minimum length, containing characters "<span class="tex-font-style-tt">L</span>", "<span class="tex-font-style-tt">R</span>" and "<span class="tex-font-style-tt">A</span>" — the succession of actions leading to the required result.</p><p>If there are several possible answers, print any of them.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>). The next line contains <span class="tex-span"><i>n</i></span> numbers, the <span class="tex-span"><i>i</i></span>-th of them represents the strength of the fire demon standing of the <span class="tex-span"><i>i</i></span>-th position, an integer from <span class="tex-span">1</span> to <span class="tex-span">100</span>. If there's no demon on the <span class="tex-span"><i>i</i></span>-th position, then the <span class="tex-span"><i>i</i></span>-th number equals to <span class="tex-span">0</span>. It is guaranteed that the input data have at least one fire demon.</p>

## Output

<p>Print a string of minimum length, containing characters "<span class="tex-font-style-tt">L</span>", "<span class="tex-font-style-tt">R</span>" and "<span class="tex-font-style-tt">A</span>" — the succession of actions leading to the required result.</p><p>If there are several possible answers, print any of them.</p>





```input1
3
1 0 1

```




```input2
3
0 2 0

```




```output1
ARARARALLLA
```




```output2
ARARALAARALA
```


