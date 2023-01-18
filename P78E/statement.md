## Description

<div><p>They've screwed something up yet again... In one nuclear reactor of a research station an uncontrolled reaction is in progress and explosion which will destroy the whole station will happen soon.</p><p>The station is represented by a square <span class="tex-span"><i>n</i> × <i>n</i></span> divided into <span class="tex-span">1 × 1</span> blocks. Each block is either a reactor or a laboratory. There can be several reactors and exactly one of them will explode soon. The reactors can be considered impassable blocks, but one can move through laboratories. Between any two laboratories, which are in adjacent blocks, there is a corridor. Blocks are considered adjacent if they have a common edge.</p><p>In each laboratory there is some number of scientists and some number of rescue capsules. Once the scientist climbs into a capsule, he is considered to be saved. Each capsule has room for not more than one scientist.</p><p>The reactor, which is about to explode, is damaged and a toxic coolant trickles from it into the neighboring blocks. The block, which contains the reactor, is considered infected. Every minute the coolant spreads over the laboratories through corridors. If at some moment one of the blocks is infected, then the next minute all the neighboring laboratories also become infected. Once a lab is infected, all the scientists there that are not in rescue capsules die. The coolant does not spread through reactor blocks.</p><p>There are exactly <span class="tex-span"><i>t</i></span> minutes to the explosion. Any scientist in a minute can move down the corridor to the next lab, if it is not infected. On any corridor an unlimited number of scientists can simultaneously move in both directions. It is believed that the scientists inside a lab moves without consuming time. Moreover, any scientist could get into the rescue capsule instantly. It is also believed that any scientist at any given moment always has the time to perform their actions (move from the given laboratory into the next one, or climb into the rescue capsule) before the laboratory will be infected.</p><p>Find the maximum number of scientists who will be able to escape.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10</span>, <span class="tex-span">1 ≤ <i>t</i> ≤ 60</span>). Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>n</i></span> characters. These lines describe the scientists' locations. Then exactly one empty line follows. Each of the next <span class="tex-span"><i>n</i></span> more lines contains <span class="tex-span"><i>n</i></span> characters. These lines describe the rescue capsules' locations.</p><p>In the description of the scientists' and the rescue capsules' locations the character "<span class="tex-font-style-tt">Y</span>" stands for a properly functioning reactor, "<span class="tex-font-style-tt">Z</span>" stands for the malfunctioning reactor. The reactors' positions in both descriptions coincide. There is exactly one malfunctioning reactor on the station. The digits "<span class="tex-font-style-tt">0</span>" - "<span class="tex-font-style-tt">9</span>" stand for the laboratories. In the description of the scientists' locations those numbers stand for the number of scientists in the corresponding laboratories. In the rescue capsules' descriptions they stand for the number of such capsules in each laboratory.</p></div><div class="output-specification"><p>Print a single number — the maximum number of scientists who will manage to save themselves.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10</span>, <span class="tex-span">1 ≤ <i>t</i> ≤ 60</span>). Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>n</i></span> characters. These lines describe the scientists' locations. Then exactly one empty line follows. Each of the next <span class="tex-span"><i>n</i></span> more lines contains <span class="tex-span"><i>n</i></span> characters. These lines describe the rescue capsules' locations.</p><p>In the description of the scientists' and the rescue capsules' locations the character "<span class="tex-font-style-tt">Y</span>" stands for a properly functioning reactor, "<span class="tex-font-style-tt">Z</span>" stands for the malfunctioning reactor. The reactors' positions in both descriptions coincide. There is exactly one malfunctioning reactor on the station. The digits "<span class="tex-font-style-tt">0</span>" - "<span class="tex-font-style-tt">9</span>" stand for the laboratories. In the description of the scientists' locations those numbers stand for the number of scientists in the corresponding laboratories. In the rescue capsules' descriptions they stand for the number of such capsules in each laboratory.</p>

## Output

<p>Print a single number — the maximum number of scientists who will manage to save themselves.</p>





```input1
3 3
1YZ
1YY
100

0YZ
0YY
003

```




```input2
4 4
Y110
1Y1Z
1Y0Y
0100

Y001
0Y0Z
0Y0Y
0005

```




```output1
2
```




```output2
3
```



## Note

<p>In the second sample the events could take place as follows: </p><center> <img class="tex-graphics" src="file://UtMbgZJl.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
