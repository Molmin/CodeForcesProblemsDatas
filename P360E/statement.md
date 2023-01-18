## Description

<div><p>Levko loves sports pathfinding competitions in his city very much. In order to boost his performance, Levko spends his spare time practicing. The practice is a game.</p><p>The city consists of <span class="tex-span"><i>n</i></span> intersections connected by <span class="tex-span"><i>m</i> + <i>k</i></span> directed roads. Two or more roads can connect the same pair of intersections. Besides, there can be roads leading from an intersection to itself. </p><p>Levko and Zenyk are playing a game. First Levko stands on intersection <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span>, and Zenyk stands on intersection <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span>. They both want to get to intersection <span class="tex-span"><i>f</i></span>. The person who does it quicker wins. If they get there at the same time, the game ends with a draw. By agreement both players start simultaneously and move with the same speed.</p><p>Levko wants to win very much. He knows the lengths of all the roads in the city. Also he knows that he can change the lengths of some roads (there are <span class="tex-span"><i>k</i></span> such roads at all) if he pays the government. So, the government can change the length of the <span class="tex-span"><i>i</i></span>-th road to any integer value in the segment [<span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>] (both borders inclusive). Levko wondered if he can reconstruct the roads so as to win the game and whether he can hope for the draw if he cannot win.</p><p>You should consider that both players play optimally well. It is guaranteed that we can get from intersections <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> to intersection <span class="tex-span"><i>f</i></span>. </p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">4</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 100</span>). The second line contains three integers <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>f</i></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, <i>f</i> ≤ <i>n</i></span>).</p><p>The next <span class="tex-span"><i>m</i></span> lines contains the descriptions of the roads that cannot be changed by Levko. Each line contains three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), representing a road from intersection <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to intersection <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> of length <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>The next <span class="tex-span"><i>k</i></span> lines contains the descriptions of the roads that can be changed by Levko. Each line contains four integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), representing a road from intersection <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to intersection <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, Levko can set the road's length within limits <span class="tex-span">[<i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>]</span>.</p><p>Consider all intersections numbered from 1 to <span class="tex-span"><i>n</i></span>. It is guaranteed that you can get from intersections <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> to intersection <span class="tex-span"><i>f</i></span>.</p></div><div class="output-specification"><p>In the first line print string "<span class="tex-font-style-tt">WIN</span>" (without the quotes) if Levko can win this game, string "<span class="tex-font-style-tt">DRAW</span>" (without the quotes) if Levko can end the game with a draw and "<span class="tex-font-style-tt">LOSE</span>" (without the quotes) if he loses for sure.</p><p>If the answer is "<span class="tex-font-style-tt">WIN</span>" or "<span class="tex-font-style-tt">DRAW</span>", then print on the second line <span class="tex-span"><i>k</i></span> space-separated integers — the length of the roads Levko sets in the order they occur in the input.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">4</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 100</span>). The second line contains three integers <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>f</i></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, <i>f</i> ≤ <i>n</i></span>).</p><p>The next <span class="tex-span"><i>m</i></span> lines contains the descriptions of the roads that cannot be changed by Levko. Each line contains three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), representing a road from intersection <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to intersection <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> of length <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>The next <span class="tex-span"><i>k</i></span> lines contains the descriptions of the roads that can be changed by Levko. Each line contains four integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), representing a road from intersection <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to intersection <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, Levko can set the road's length within limits <span class="tex-span">[<i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>]</span>.</p><p>Consider all intersections numbered from 1 to <span class="tex-span"><i>n</i></span>. It is guaranteed that you can get from intersections <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> to intersection <span class="tex-span"><i>f</i></span>.</p>

## Output

<p>In the first line print string "<span class="tex-font-style-tt">WIN</span>" (without the quotes) if Levko can win this game, string "<span class="tex-font-style-tt">DRAW</span>" (without the quotes) if Levko can end the game with a draw and "<span class="tex-font-style-tt">LOSE</span>" (without the quotes) if he loses for sure.</p><p>If the answer is "<span class="tex-font-style-tt">WIN</span>" or "<span class="tex-font-style-tt">DRAW</span>", then print on the second line <span class="tex-span"><i>k</i></span> space-separated integers — the length of the roads Levko sets in the order they occur in the input.</p>





```input1
4 1 3
1 3 4
3 2 2
1 2 1 3
2 4 1 3
3 4 1 3

```




```input2
4 1 3
1 3 4
3 2 2
1 2 1 3
2 4 1 3
3 4 1 2

```




```input3
5 4 2
1 2 5
1 3 3
1 4 4
2 3 2
2 4 3
3 5 1 5
4 5 4 7

```




```output1
WIN
1 1 3
```




```output2
DRAW
1 1 2
```




```output3
LOSE

```


