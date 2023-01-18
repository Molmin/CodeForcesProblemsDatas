## Description

<div><p>Lord Tirek is a centaur and the main antagonist in the season four finale episodes in the series "My Little Pony: Friendship Is Magic". In "Twilight's Kingdom" (Part 1), Tirek escapes from Tartarus and drains magic from ponies to grow stronger.</p><center> <img class="tex-graphics" src="file://kOlGiJrk.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The core skill of Tirek is called Absorb Mana. It takes all mana from a magic creature and gives them to the caster.</p><p>Now to simplify the problem, assume you have <span class="tex-span"><i>n</i></span> ponies (numbered from 1 to <span class="tex-span"><i>n</i></span>). Each pony has three attributes:</p><ul> <li> <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> : amount of mana that the pony has at time 0; </li><li> <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> : maximum mana that the pony can have; </li><li> <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> : mana regeneration per unit time. </li></ul><p>Lord Tirek will do <span class="tex-span"><i>m</i></span> instructions, each of them can be described with three integers: <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub>, <i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span>. The instruction means that at time <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, Tirek will use Absorb Mana on ponies with numbers from <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (both borders inclusive). We'll give you all the <span class="tex-span"><i>m</i></span> instructions in order, count how much mana Tirek absorbs for each instruction.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of ponies. Each of the next <span class="tex-span"><i>n</i></span> lines contains three integers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub>, <i>m</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>;&nbsp;0 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span>, describing a pony. </p><p>The next line contains an integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of instructions. Each of the next <span class="tex-span"><i>m</i></span> lines contains three integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub>, <i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>;&nbsp;1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>, describing an instruction of Lord Tirek. The instructions are given in strictly increasing order of <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (all <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> are distinct).</p></div><div class="output-specification"><p>For each instruction, output a single line which contains a single integer, the total mana absorbed in this instruction.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of ponies. Each of the next <span class="tex-span"><i>n</i></span> lines contains three integers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub>, <i>m</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>;&nbsp;0 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span>, describing a pony. </p><p>The next line contains an integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of instructions. Each of the next <span class="tex-span"><i>m</i></span> lines contains three integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub>, <i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>;&nbsp;1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>, describing an instruction of Lord Tirek. The instructions are given in strictly increasing order of <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (all <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> are distinct).</p>

## Output

<p>For each instruction, output a single line which contains a single integer, the total mana absorbed in this instruction.</p>





```input1
5
0 10 1
0 12 1
0 20 1
0 12 1
0 10 1
2
5 1 5
19 1 5

```




```output1
25
58

```



## Note

<p>Every pony starts with zero mana. For the first instruction, each pony has 5 mana, so you get 25 mana in total and each pony has 0 mana after the first instruction.</p><p>For the second instruction, pony 3 has 14 mana and other ponies have mana equal to their <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span>.</p>
